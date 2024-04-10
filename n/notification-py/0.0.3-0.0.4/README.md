# Comparing `tmp/notification_py-0.0.3.tar.gz` & `tmp/notification_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.3.tar", max compression
+gzip compressed data, was "notification_py-0.0.4.tar", max compression
```

## Comparing `notification_py-0.0.3.tar` & `notification_py-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.3/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.3/README.md
--rw-r--r--   0        0        0      769 2024-04-10 00:48:23.571255 notification_py-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      450 2024-04-10 00:31:19.219378 notification_py-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.3/src/custom_types.py
--rw-r--r--   0        0        0     1817 2024-04-10 00:26:14.147485 notification_py-0.0.3/src/main.py
--rw-r--r--   0        0        0     4602 2024-04-10 00:26:20.796709 notification_py-0.0.3/src/services/discord.py
--rw-r--r--   0        0        0     2356 2024-04-10 00:26:27.225926 notification_py-0.0.3/src/services/email.py
--rw-r--r--   0        0        0     3697 2024-04-10 00:26:34.277164 notification_py-0.0.3/src/services/slack.py
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 notification_py-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.4/LICENSE
+-rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.4/README.md
+-rw-r--r--   0        0        0      771 2024-04-10 00:55:04.389842 notification_py-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      450 2024-04-10 00:31:19.219378 notification_py-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.4/src/custom_types.py
+-rw-r--r--   0        0        0     1817 2024-04-10 00:26:14.147485 notification_py-0.0.4/src/main.py
+-rw-r--r--   0        0        0     4602 2024-04-10 00:26:20.796709 notification_py-0.0.4/src/services/discord.py
+-rw-r--r--   0        0        0     2356 2024-04-10 00:26:27.225926 notification_py-0.0.4/src/services/email.py
+-rw-r--r--   0        0        0     3697 2024-04-10 00:26:34.277164 notification_py-0.0.4/src/services/slack.py
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 notification_py-0.0.4/PKG-INFO
```

### Comparing `notification_py-0.0.3/LICENSE` & `notification_py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.3/pyproject.toml` & `notification_py-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "notification_py"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 packages = [
 {include = "src"},
 ]
 
 
+
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.black]
 line-length = 79
 
@@ -41,7 +42,8 @@
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `notification_py-0.0.3/src/custom_types.py` & `notification_py-0.0.4/src/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.3/src/main.py` & `notification_py-0.0.4/src/main.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.3/src/services/discord.py` & `notification_py-0.0.4/src/services/discord.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.3/src/services/email.py` & `notification_py-0.0.4/src/services/email.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.3/src/services/slack.py` & `notification_py-0.0.4/src/services/slack.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.3/PKG-INFO` & `notification_py-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: notification_py
-Version: 0.0.3
+Name: notification-py
+Version: 0.0.4
 Summary: 
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: aiosmtplib (>=3.0.1,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: print-position (>=2.0.1,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
```

