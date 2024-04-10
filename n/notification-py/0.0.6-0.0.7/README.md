# Comparing `tmp/notification_py-0.0.6.tar.gz` & `tmp/notification_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.6.tar", max compression
+gzip compressed data, was "notification_py-0.0.7.tar", max compression
```

## Comparing `notification_py-0.0.6.tar` & `notification_py-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.6/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.6/README.md
--rw-r--r--   0        0        0      772 2024-04-10 01:17:19.097715 notification_py-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.6/src/notification_py/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.6/src/notification_py/custom_types.py
--rw-r--r--   0        0        0     1881 2024-04-10 01:05:27.105985 notification_py-0.0.6/src/notification_py/main.py
--rw-r--r--   0        0        0     4618 2024-04-10 01:05:27.239986 notification_py-0.0.6/src/notification_py/services/discord.py
--rw-r--r--   0        0        0     2372 2024-04-10 01:05:27.319987 notification_py-0.0.6/src/notification_py/services/email.py
--rw-r--r--   0        0        0     3730 2024-04-10 01:05:27.536988 notification_py-0.0.6/src/notification_py/services/slack.py
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 notification_py-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.7/LICENSE
+-rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.7/README.md
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.7/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.7/notification_py/custom_types.py
+-rw-r--r--   0        0        0     1865 2024-04-10 01:31:34.794458 notification_py-0.0.7/notification_py/main.py
+-rw-r--r--   0        0        0     4614 2024-04-10 01:31:17.218473 notification_py-0.0.7/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2368 2024-04-10 01:31:22.262468 notification_py-0.0.7/notification_py/services/email.py
+-rw-r--r--   0        0        0     3726 2024-04-10 01:31:27.349464 notification_py-0.0.7/notification_py/services/slack.py
+-rw-r--r--   0        0        0      629 2024-04-10 01:33:09.143431 notification_py-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 notification_py-0.0.7/PKG-INFO
```

### Comparing `notification_py-0.0.6/LICENSE` & `notification_py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.6/pyproject.toml` & `notification_py-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,17 @@
 [tool.poetry]
 name = "notification_py"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 packages = [
-{include = "src"},
+{include = "notification_py"},
 ]
 
-
-
-[tool.isort]
-profile = "black"
-line_length = 79
-
-[tool.black]
-line-length = 79
-
-[tool.ruff]
-line-length = 79
-
-[tool.mypy]
-ignore_missing_imports = true
-
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.6.4"
 aiohttp = "^3.9.3"
 asyncio = "^3.4.3"
 python-dotenv = "^1.0.1"
 aiosmtplib = "^3.0.1"
```

### Comparing `notification_py-0.0.6/src/notification_py/custom_types.py` & `notification_py-0.0.7/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.6/src/notification_py/main.py` & `notification_py-0.0.7/notification_py/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from src.notification_py.custom_types import Message, NotificationResponse
+from notification_py.custom_types import Message, NotificationResponse
 
-from src.notification_py.services.slack import send_message_to_slack
-from src.notification_py.services.discord import send_message_to_discord
-from src.notification_py.services.email import send_email
+from notification_py.services.slack import send_message_to_slack
+from notification_py.services.discord import send_message_to_discord
+from notification_py.services.email import send_email
 
 
 async def send_notification(message: Message) -> NotificationResponse:
     try:
         result_slack = None
         result_discord = None
         result_email = None
```

### Comparing `notification_py-0.0.6/src/notification_py/services/discord.py` & `notification_py-0.0.7/notification_py/services/discord.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import aiohttp
-from src.notification_py.custom_types import (
+from notification_py.custom_types import (
     DiscordCreds,
     Message,
     BasicAPIResponse,
     SeverityLiteral,
 )
```

### Comparing `notification_py-0.0.6/src/notification_py/services/email.py` & `notification_py-0.0.7/notification_py/services/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import aiosmtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
-from src.notification_py.custom_types import BasicAPIResponse, Message
+from notification_py.custom_types import BasicAPIResponse, Message
 
 
 async def send_email(message: Message) -> BasicAPIResponse:
     if message.creds is None or message.creds.email is None:
         raise ValueError("Email credentials are missing.")
 
     message = _update_message(message)
```

### Comparing `notification_py-0.0.6/src/notification_py/services/slack.py` & `notification_py-0.0.7/notification_py/services/slack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import aiohttp
-from src.notification_py.custom_types import (
+from notification_py.custom_types import (
     BasicAPIResponse,
     Message,
     SeverityLiteral,
 )
 
 
 async def send_message_to_slack(message: Message) -> BasicAPIResponse:
```

### Comparing `notification_py-0.0.6/PKG-INFO` & `notification_py-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notification-py
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

