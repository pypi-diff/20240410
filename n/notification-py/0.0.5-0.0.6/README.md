# Comparing `tmp/notification_py-0.0.5.tar.gz` & `tmp/notification_py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.5.tar", max compression
+gzip compressed data, was "notification_py-0.0.6.tar", max compression
```

## Comparing `notification_py-0.0.5.tar` & `notification_py-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.5/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.5/README.md
--rw-r--r--   0        0        0      771 2024-04-10 01:08:20.193075 notification_py-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.5/src/notification_py/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.5/src/notification_py/custom_types.py
--rw-r--r--   0        0        0     1881 2024-04-10 01:05:27.105985 notification_py-0.0.5/src/notification_py/main.py
--rw-r--r--   0        0        0     4618 2024-04-10 01:05:27.239986 notification_py-0.0.5/src/notification_py/services/discord.py
--rw-r--r--   0        0        0     2372 2024-04-10 01:05:27.319987 notification_py-0.0.5/src/notification_py/services/email.py
--rw-r--r--   0        0        0     3730 2024-04-10 01:05:27.536988 notification_py-0.0.5/src/notification_py/services/slack.py
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 notification_py-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.6/LICENSE
+-rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.6/README.md
+-rw-r--r--   0        0        0      772 2024-04-10 01:17:19.097715 notification_py-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.6/src/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.6/src/notification_py/custom_types.py
+-rw-r--r--   0        0        0     1881 2024-04-10 01:05:27.105985 notification_py-0.0.6/src/notification_py/main.py
+-rw-r--r--   0        0        0     4618 2024-04-10 01:05:27.239986 notification_py-0.0.6/src/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2372 2024-04-10 01:05:27.319987 notification_py-0.0.6/src/notification_py/services/email.py
+-rw-r--r--   0        0        0     3730 2024-04-10 01:05:27.536988 notification_py-0.0.6/src/notification_py/services/slack.py
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 notification_py-0.0.6/PKG-INFO
```

### Comparing `notification_py-0.0.5/LICENSE` & `notification_py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.5/src/notification_py/custom_types.py` & `notification_py-0.0.6/src/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.5/src/notification_py/main.py` & `notification_py-0.0.6/src/notification_py/main.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.5/src/notification_py/services/discord.py` & `notification_py-0.0.6/src/notification_py/services/discord.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.5/src/notification_py/services/email.py` & `notification_py-0.0.6/src/notification_py/services/email.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.5/src/notification_py/services/slack.py` & `notification_py-0.0.6/src/notification_py/services/slack.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.5/PKG-INFO` & `notification_py-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: notification-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: aiosmtplib (>=3.0.1,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: print-position (>=2.0.1,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
```

