# Comparing `tmp/notification_py-0.0.2.tar.gz` & `tmp/notification_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.2.tar", max compression
+gzip compressed data, was "notification_py-0.0.3.tar", max compression
```

## Comparing `notification_py-0.0.2.tar` & `notification_py-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.2/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.2/README.md
--rw-r--r--   0        0        0      769 2024-04-10 00:42:54.327949 notification_py-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      450 2024-04-10 00:31:19.219378 notification_py-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.2/src/custom_types.py
--rw-r--r--   0        0        0     1817 2024-04-10 00:26:14.147485 notification_py-0.0.2/src/main.py
--rw-r--r--   0        0        0     4602 2024-04-10 00:26:20.796709 notification_py-0.0.2/src/services/discord.py
--rw-r--r--   0        0        0     2356 2024-04-10 00:26:27.225926 notification_py-0.0.2/src/services/email.py
--rw-r--r--   0        0        0     3697 2024-04-10 00:26:34.277164 notification_py-0.0.2/src/services/slack.py
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 notification_py-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.3/LICENSE
+-rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.3/README.md
+-rw-r--r--   0        0        0      769 2024-04-10 00:48:23.571255 notification_py-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      450 2024-04-10 00:31:19.219378 notification_py-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.3/src/custom_types.py
+-rw-r--r--   0        0        0     1817 2024-04-10 00:26:14.147485 notification_py-0.0.3/src/main.py
+-rw-r--r--   0        0        0     4602 2024-04-10 00:26:20.796709 notification_py-0.0.3/src/services/discord.py
+-rw-r--r--   0        0        0     2356 2024-04-10 00:26:27.225926 notification_py-0.0.3/src/services/email.py
+-rw-r--r--   0        0        0     3697 2024-04-10 00:26:34.277164 notification_py-0.0.3/src/services/slack.py
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 notification_py-0.0.3/PKG-INFO
```

### Comparing `notification_py-0.0.2/LICENSE` & `notification_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.2/pyproject.toml` & `notification_py-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "notification-py"
-version = "0.0.2"
+name = "notification_py"
+version = "0.0.3"
 description = ""
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 packages = [
 {include = "src"},
 ]
```

### Comparing `notification_py-0.0.2/src/custom_types.py` & `notification_py-0.0.3/src/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.2/src/main.py` & `notification_py-0.0.3/src/main.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.2/src/services/discord.py` & `notification_py-0.0.3/src/services/discord.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.2/src/services/email.py` & `notification_py-0.0.3/src/services/email.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.2/src/services/slack.py` & `notification_py-0.0.3/src/services/slack.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.2/PKG-INFO` & `notification_py-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: notification-py
-Version: 0.0.2
+Name: notification_py
+Version: 0.0.3
 Summary: 
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

