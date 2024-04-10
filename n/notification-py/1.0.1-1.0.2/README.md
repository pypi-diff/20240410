# Comparing `tmp/notification_py-1.0.1.tar.gz` & `tmp/notification_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-1.0.1.tar", max compression
+gzip compressed data, was "notification_py-1.0.2.tar", max compression
```

## Comparing `notification_py-1.0.1.tar` & `notification_py-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-1.0.1/LICENSE
--rw-r--r--   0        0        0     5810 2024-04-10 04:13:10.312440 notification_py-1.0.1/README.md
--rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-1.0.1/notification_py/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-10 03:19:23.410798 notification_py-1.0.1/notification_py/custom_types.py
--rw-r--r--   0        0        0     2409 2024-04-10 04:04:06.737194 notification_py-1.0.1/notification_py/main.py
--rw-r--r--   0        0        0        0 2024-03-30 07:36:24.198672 notification_py-1.0.1/notification_py/services/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-10 03:57:16.042206 notification_py-1.0.1/notification_py/services/discord.py
--rw-r--r--   0        0        0     2300 2024-04-10 03:57:04.290177 notification_py-1.0.1/notification_py/services/email.py
--rw-r--r--   0        0        0     3666 2024-04-10 03:57:23.424224 notification_py-1.0.1/notification_py/services/slack.py
--rw-r--r--   0        0        0      774 2024-04-10 04:13:58.066233 notification_py-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 notification_py-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5957 2024-04-10 04:16:54.650659 notification_py-1.0.2/README.md
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-1.0.2/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-10 03:19:23.410798 notification_py-1.0.2/notification_py/custom_types.py
+-rw-r--r--   0        0        0     2409 2024-04-10 04:04:06.737194 notification_py-1.0.2/notification_py/main.py
+-rw-r--r--   0        0        0        0 2024-03-30 07:36:24.198672 notification_py-1.0.2/notification_py/services/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-10 03:57:16.042206 notification_py-1.0.2/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2300 2024-04-10 03:57:04.290177 notification_py-1.0.2/notification_py/services/email.py
+-rw-r--r--   0        0        0     3666 2024-04-10 03:57:23.424224 notification_py-1.0.2/notification_py/services/slack.py
+-rw-r--r--   0        0        0      774 2024-04-10 04:17:27.013582 notification_py-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 notification_py-1.0.2/PKG-INFO
```

### Comparing `notification_py-1.0.1/LICENSE` & `notification_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.1/README.md` & `notification_py-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -127,19 +127,19 @@
 smtp_port = "587"
 target_email = "RECIPIENT_ID@gmail.com"
 
 ```
 
 ## Sample notifications
 ### 1. Discord
-![Sample Discord Notifications](./screenshots/discord.png)
+![Sample Discord Notifications](https://github.com/ps428/notification-py/blob/main/screenshots/discord.png)
 ### 2. Slack
-![Sample Slack Notifications](./screenshots/slack.png)
+![Sample Slack Notifications](https://github.com/ps428/notification-py/blob/main/screenshots/slack.png)
 ### 3. Email
-![Sample Email Notifications](./screenshots/email.png)
+![Sample Email Notifications](https://github.com/ps428/notification-py/blob/main/screenshots/email.png)
 
 
 # Contact me
 
 To raise any **issues/requests** you may refer the issue page [here](https://github.com/ps428/notification-py/issues).
 
 You may **mail me** here on my [mail id](mailto:pranav.bhawan@gmail.com).
```

### Comparing `notification_py-1.0.1/notification_py/custom_types.py` & `notification_py-1.0.2/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.1/notification_py/main.py` & `notification_py-1.0.2/notification_py/main.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.1/notification_py/services/discord.py` & `notification_py-1.0.2/notification_py/services/discord.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.1/notification_py/services/email.py` & `notification_py-1.0.2/notification_py/services/email.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.1/notification_py/services/slack.py` & `notification_py-1.0.2/notification_py/services/slack.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.1/pyproject.toml` & `notification_py-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notification_py"
-version = "1.0.1"
+version = "1.0.2"
 description = "A simple package to send notifications on Discord, Slack and Email."
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/ps428/notification-py/"
 packages = [{include = "notification_py"}]
```

### Comparing `notification_py-1.0.1/PKG-INFO` & `notification_py-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notification-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple package to send notifications on Discord, Slack and Email.
 Home-page: https://github.com/ps428/notification-py/
 License: Apache-2.0
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -150,19 +150,19 @@
 smtp_port = "587"
 target_email = "RECIPIENT_ID@gmail.com"
 
 ```
 
 ## Sample notifications
 ### 1. Discord
-![Sample Discord Notifications](./screenshots/discord.png)
+![Sample Discord Notifications](https://github.com/ps428/notification-py/blob/main/screenshots/discord.png)
 ### 2. Slack
-![Sample Slack Notifications](./screenshots/slack.png)
+![Sample Slack Notifications](https://github.com/ps428/notification-py/blob/main/screenshots/slack.png)
 ### 3. Email
-![Sample Email Notifications](./screenshots/email.png)
+![Sample Email Notifications](https://github.com/ps428/notification-py/blob/main/screenshots/email.png)
 
 
 # Contact me
 
 To raise any **issues/requests** you may refer the issue page [here](https://github.com/ps428/notification-py/issues).
 
 You may **mail me** here on my [mail id](mailto:pranav.bhawan@gmail.com).
```

