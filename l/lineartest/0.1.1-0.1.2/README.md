# Comparing `tmp/lineartest-0.1.1.tar.gz` & `tmp/lineartest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.1.1.tar", max compression
+gzip compressed data, was "lineartest-0.1.2.tar", max compression
```

## Comparing `lineartest-0.1.1.tar` & `lineartest-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.1.1/LICENSE
--rw-r--r--   0        0        0     2245 2024-04-09 02:39:05.544332 lineartest-0.1.1/README.md
--rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.1.1/lineartest/__init__.py
--rw-r--r--   0        0        0     1436 2024-04-08 09:41:54.891450 lineartest-0.1.1/lineartest/_log.py
--rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.1.1/lineartest/_type.py
--rw-r--r--   0        0        0     7602 2024-04-08 09:41:54.892075 lineartest-0.1.1/lineartest/client.py
--rw-r--r--   0        0        0     6291 2024-04-08 09:41:54.892408 lineartest-0.1.1/lineartest/schedule.py
--rw-r--r--   0        0        0     1178 2024-04-09 02:37:23.118278 lineartest-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 lineartest-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2245 2024-04-09 02:47:37.099907 lineartest-0.1.2/README.md
+-rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.1.2/lineartest/__init__.py
+-rw-r--r--   0        0        0     1436 2024-04-08 09:41:54.891450 lineartest-0.1.2/lineartest/_log.py
+-rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.1.2/lineartest/_type.py
+-rw-r--r--   0        0        0     7650 2024-04-09 03:36:09.904701 lineartest-0.1.2/lineartest/client.py
+-rw-r--r--   0        0        0     6291 2024-04-08 09:41:54.892408 lineartest-0.1.2/lineartest/schedule.py
+-rw-r--r--   0        0        0     1178 2024-04-09 03:36:09.905046 lineartest-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 lineartest-0.1.2/PKG-INFO
```

### Comparing `lineartest-0.1.1/LICENSE` & `lineartest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.1/README.md` & `lineartest-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.1/lineartest/_log.py` & `lineartest-0.1.2/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.1/lineartest/client.py` & `lineartest-0.1.2/lineartest/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,17 @@
         if data:
             self.info('>>> Request data:')
             self._log(self.info, prefix, data)
 
         # log files
         if files:
             self.info('>>> Request files:')
-            self._log(self.info, prefix, {file.name for file in files})
+            self._log(
+                self.info, prefix, {key: file.name for key, file in files.items()}
+            )
 
         # log json
         if json:
             self.info('>>> Request JSON:')
             self._log(self.info, prefix, json)
 
         # log headers
```

### Comparing `lineartest-0.1.1/lineartest/schedule.py` & `lineartest-0.1.2/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.1/pyproject.toml` & `lineartest-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.1.1"
+version = "0.1.2"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `lineartest-0.1.1/PKG-INFO` & `lineartest-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.1.1
+Version: 0.1.2
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

