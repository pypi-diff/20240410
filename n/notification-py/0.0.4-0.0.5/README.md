# Comparing `tmp/notification_py-0.0.4.tar.gz` & `tmp/notification_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.4.tar", max compression
+gzip compressed data, was "notification_py-0.0.5.tar", max compression
```

## Comparing `notification_py-0.0.4.tar` & `notification_py-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.4/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.4/README.md
--rw-r--r--   0        0        0      771 2024-04-10 00:55:04.389842 notification_py-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      450 2024-04-10 00:31:19.219378 notification_py-0.0.4/src/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.4/src/custom_types.py
--rw-r--r--   0        0        0     1817 2024-04-10 00:26:14.147485 notification_py-0.0.4/src/main.py
--rw-r--r--   0        0        0     4602 2024-04-10 00:26:20.796709 notification_py-0.0.4/src/services/discord.py
--rw-r--r--   0        0        0     2356 2024-04-10 00:26:27.225926 notification_py-0.0.4/src/services/email.py
--rw-r--r--   0        0        0     3697 2024-04-10 00:26:34.277164 notification_py-0.0.4/src/services/slack.py
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 notification_py-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.5/LICENSE
+-rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.5/README.md
+-rw-r--r--   0        0        0      771 2024-04-10 01:08:20.193075 notification_py-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.5/src/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.5/src/notification_py/custom_types.py
+-rw-r--r--   0        0        0     1881 2024-04-10 01:05:27.105985 notification_py-0.0.5/src/notification_py/main.py
+-rw-r--r--   0        0        0     4618 2024-04-10 01:05:27.239986 notification_py-0.0.5/src/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2372 2024-04-10 01:05:27.319987 notification_py-0.0.5/src/notification_py/services/email.py
+-rw-r--r--   0        0        0     3730 2024-04-10 01:05:27.536988 notification_py-0.0.5/src/notification_py/services/slack.py
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 notification_py-0.0.5/PKG-INFO
```

### Comparing `notification_py-0.0.4/LICENSE` & `notification_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.4/pyproject.toml` & `notification_py-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notification_py"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 packages = [
 {include = "src"},
 ]
 
@@ -39,11 +39,11 @@
 flake8 = "^6.1.0"
 ruff = "^0.1.11"
 mypy = "^1.8.0"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
 
+[build-system]
+requires = ['setuptools>=42']
+build-backend = 'setuptools.build_meta'
```

### Comparing `notification_py-0.0.4/src/custom_types.py` & `notification_py-0.0.5/src/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.4/src/main.py` & `notification_py-0.0.5/src/notification_py/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from src.custom_types import Message, NotificationResponse
+from src.notification_py.custom_types import Message, NotificationResponse
 
-from src.services.slack import send_message_to_slack
-from src.services.discord import send_message_to_discord
-from src.services.email import send_email
+from src.notification_py.services.slack import send_message_to_slack
+from src.notification_py.services.discord import send_message_to_discord
+from src.notification_py.services.email import send_email
 
 
 async def send_notification(message: Message) -> NotificationResponse:
     try:
         result_slack = None
         result_discord = None
         result_email = None
```

### Comparing `notification_py-0.0.4/src/services/discord.py` & `notification_py-0.0.5/src/notification_py/services/discord.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import aiohttp
-from src.custom_types import (
+from src.notification_py.custom_types import (
     DiscordCreds,
     Message,
     BasicAPIResponse,
     SeverityLiteral,
 )
```

### Comparing `notification_py-0.0.4/src/services/email.py` & `notification_py-0.0.5/src/notification_py/services/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import aiosmtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
-from src.custom_types import BasicAPIResponse, Message
+from src.notification_py.custom_types import BasicAPIResponse, Message
 
 
 async def send_email(message: Message) -> BasicAPIResponse:
     if message.creds is None or message.creds.email is None:
         raise ValueError("Email credentials are missing.")
 
     message = _update_message(message)
```

### Comparing `notification_py-0.0.4/src/services/slack.py` & `notification_py-0.0.5/src/notification_py/services/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import aiohttp
-from src.custom_types import BasicAPIResponse, Message, SeverityLiteral
+from src.notification_py.custom_types import (
+    BasicAPIResponse,
+    Message,
+    SeverityLiteral,
+)
 
 
 async def send_message_to_slack(message: Message) -> BasicAPIResponse:
     try:
         if message.creds and message.creds.slack:
             message = _update_message_for_slack(message)
```

### Comparing `notification_py-0.0.4/PKG-INFO` & `notification_py-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notification-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
```

