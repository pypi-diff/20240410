# Comparing `tmp/notification_py-0.0.9.tar.gz` & `tmp/notification_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.9.tar", max compression
+gzip compressed data, was "notification_py-1.0.1.tar", max compression
```

## Comparing `notification_py-0.0.9.tar` & `notification_py-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.9/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.9/README.md
--rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.9/notification_py/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.9/notification_py/custom_types.py
--rw-r--r--   0        0        0     1865 2024-04-10 01:31:34.794458 notification_py-0.0.9/notification_py/main.py
--rw-r--r--   0        0        0        0 2024-03-30 07:36:24.198672 notification_py-0.0.9/notification_py/services/__init__.py
--rw-r--r--   0        0        0     4614 2024-04-10 01:31:17.218473 notification_py-0.0.9/notification_py/services/discord.py
--rw-r--r--   0        0        0     2368 2024-04-10 01:31:22.262468 notification_py-0.0.9/notification_py/services/email.py
--rw-r--r--   0        0        0     3726 2024-04-10 01:31:27.349464 notification_py-0.0.9/notification_py/services/slack.py
--rw-r--r--   0        0        0      779 2024-04-10 01:42:56.917605 notification_py-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 notification_py-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5810 2024-04-10 04:13:10.312440 notification_py-1.0.1/README.md
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-1.0.1/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-10 03:19:23.410798 notification_py-1.0.1/notification_py/custom_types.py
+-rw-r--r--   0        0        0     2409 2024-04-10 04:04:06.737194 notification_py-1.0.1/notification_py/main.py
+-rw-r--r--   0        0        0        0 2024-03-30 07:36:24.198672 notification_py-1.0.1/notification_py/services/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-10 03:57:16.042206 notification_py-1.0.1/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2300 2024-04-10 03:57:04.290177 notification_py-1.0.1/notification_py/services/email.py
+-rw-r--r--   0        0        0     3666 2024-04-10 03:57:23.424224 notification_py-1.0.1/notification_py/services/slack.py
+-rw-r--r--   0        0        0      774 2024-04-10 04:13:58.066233 notification_py-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 notification_py-1.0.1/PKG-INFO
```

### Comparing `notification_py-0.0.9/LICENSE` & `notification_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.9/notification_py/custom_types.py` & `notification_py-1.0.1/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.9/notification_py/main.py` & `notification_py-1.0.1/notification_py/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,64 @@
-from notification_py.custom_types import Message, NotificationResponse
+import asyncio
+from notification_py.custom_types import (
+    Message,
+    NotificationResponse,
+    BasicAPIResponse,
+)
 
 from notification_py.services.slack import send_message_to_slack
 from notification_py.services.discord import send_message_to_discord
 from notification_py.services.email import send_email
 
 
 async def send_notification(message: Message) -> NotificationResponse:
     try:
-        result_slack = None
-        result_discord = None
-        result_email = None
+        tasks = []
 
         if message.creds.slack:
-
-            result_slack = await send_message_to_slack(message)
-            if not result_slack.success:
-                raise ValueError(result_slack.error)
+            slack_message = message.model_copy(deep=True)
+            tasks.append(send_message_to_slack(slack_message))
 
         if message.creds.discord:
-
-            result_discord = await send_message_to_discord(message)
-            if not result_discord.success:
-                raise ValueError(result_discord.error)
+            discord_message = message.model_copy(deep=True)
+            tasks.append(send_message_to_discord(discord_message))
 
         if message.creds.email:
+            email_message = message.model_copy(deep=True)
+            tasks.append(send_email(email_message))
 
-            result_email = await send_email(message)
-            if not result_email.success:
-                raise ValueError(result_email.error)
-
-        if not result_slack and not result_discord and not result_email:
+        if not tasks:
             return NotificationResponse(
                 success=False,
                 message="No message sent!",
                 error="No creds provided!",
                 slack=None,
                 discord=None,
                 email=None,
             )
 
+        results = await asyncio.gather(*tasks, return_exceptions=True)
+
+        result_slack = None
+        result_discord = None
+        result_email = None
+
+        for index, result in enumerate(results):
+            if isinstance(result, BasicAPIResponse):
+                if not result.success:
+                    raise ValueError(result.error)
+                if index == 0 and message.creds.slack:
+                    result_slack = result
+                elif index == 1 and message.creds.discord:
+                    result_discord = result
+                elif index == 2 and message.creds.email:
+                    result_email = result
+            elif isinstance(result, Exception):
+                raise result
+
         # Send the response
         return NotificationResponse(
             success=True,
             message="Message sent successfully!",
             error=None,
             slack=result_slack,
             discord=result_discord,
```

### Comparing `notification_py-0.0.9/notification_py/services/discord.py` & `notification_py-1.0.1/notification_py/services/discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
                 headers = {
                     "Authorization": f"Bot {message.creds.discord.token}"
                 }
                 data = {
                     "embeds": [
                         {
                             "title": message.message_details.title,
-                            "description": message.message_details.text,
+                            "description": (
+                                f"<@&{message.creds.discord.team_id}>,"
+                                f"\n{message.message_details.text}"
+                            ),
                             "color": _get_color_for_severity(
                                 message.message_details.severity
                             ),
                             "fields": [
                                 {
                                     "name": "Error Source",
                                     "value": message.message_details.source,
@@ -97,21 +100,18 @@
     )
 
 
 def _update_message(message: Message) -> Message:
     message.message_details.title = (
         f"{message.message_details.title} - "
         f"{message.message_details.source} | "
-        f"Severity: {message.message_details.severity}"
+        f"Severity: {message.message_details.severity+1}"
     )
     if not message.creds.discord:
         raise ValueError("Discord credentials not provided.")
-    message.message_details.text = (
-        f"<@&{message.creds.discord.team_id}>,\n{message.message_details.text}"
-    )
 
     return message
 
 
 def _get_color_for_severity(severity: SeverityLiteral) -> int:
     if severity == 0:
         return 5763719
```

### Comparing `notification_py-0.0.9/notification_py/services/email.py` & `notification_py-1.0.1/notification_py/services/email.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,18 @@
     email_message["Subject"] = message.message_details.title
 
     # Create the body of the email
     body = f"Severity: {message.message_details.severity}\n"
     body += f"Source: {message.message_details.source}\n"
     body += f"Filename: {message.message_details.filename}\n"
     body += f"Line Number: {message.message_details.line_number}\n"
+    body += f"Description: {message.message_details.text}\n"
     body += f"Time: {message.message_details.time}\n\n"
-    body += message.message_details.text
 
+    body += "------------"
     # Attach the body to the email message
     email_message.attach(MIMEText(body, "plain"))
 
     try:
         # Create a connection to the SMTP server
         server = aiosmtplib.SMTP(
             hostname=email_creds.smtp_server,
@@ -51,13 +52,12 @@
         return BasicAPIResponse(success=False, message=None, error=str(e))
 
 
 def _update_message(message: Message) -> Message:
     message.message_details.title = (
         f"{message.message_details.title} - "
         f"{message.message_details.source} | "
-        f"Severity: {message.message_details.severity}"
+        f"Severity: {message.message_details.severity+1}"
     )
     if not message.creds.email:
         raise ValueError("Email credentials not provided.")
-    message.message_details.text = f"To: {message.creds.email.target_email}\n{message.message_details.text}"  # noqa
     return message
```

### Comparing `notification_py-0.0.9/notification_py/services/slack.py` & `notification_py-1.0.1/notification_py/services/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                     {
                         "fallback": message.message_details.title,
                         "color": _get_color_for_severity(
                             message.message_details.severity
                         ),
                         "pretext": message.message_details.title,
                         "title": message.message_details.source,
-                        "text": message.message_details.text,
+                        "text": f"<!channel>,\n{message.message_details.text}",
                         "fields": [
                             {
                                 "title": "Filename",
                                 "value": message.message_details.filename,
                                 "short": True,
                             },
                             {
@@ -76,17 +76,16 @@
             )
     except Exception as e:
         return BasicAPIResponse(success=False, message=None, error=str(e))
 
 
 def _update_message_for_slack(message: Message) -> Message:
     message.message_details.title = (
-        f"New Alert - Severity: {message.message_details.severity}"
+        f"New Alert - Severity: {message.message_details.severity+1}"
     )
-    message.message_details.text = f"<!channel> {message.message_details.text}"
     return message
 
 
 def _get_color_for_severity(severity: SeverityLiteral) -> str:
     severity_colors = {
         0: "#00FF00",  # Green
         1: "#00FFFF",  # Cyan
```

### Comparing `notification_py-0.0.9/pyproject.toml` & `notification_py-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "notification_py"
-version = "0.0.9"
+version = "1.0.1"
 description = "A simple package to send notifications on Discord, Slack and Email."
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
-repository = "https://github.com/ps428/notification_service/"
+repository = "https://github.com/ps428/notification-py/"
 packages = [{include = "notification_py"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.6.4"
 aiohttp = "^3.9.3"
```

