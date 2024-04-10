# Comparing `tmp/vomero-0.1.3.tar.gz` & `tmp/vomero-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vomero-0.1.3.tar", max compression
+gzip compressed data, was "vomero-0.1.4.tar", max compression
```

## Comparing `vomero-0.1.3.tar` & `vomero-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-06 15:38:16.257012 vomero-0.1.3/LICENSE
--rw-r--r--   0        0        0     2605 2024-04-06 15:38:16.261012 vomero-0.1.3/README.md
--rw-r--r--   0        0        0      537 2024-04-06 15:38:16.261012 vomero-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-06 15:38:16.261012 vomero-0.1.3/src/vomero/__init__.py
--rw-r--r--   0        0        0     5641 2024-04-06 15:38:16.261012 vomero-0.1.3/src/vomero/streams.py
--rw-r--r--   0        0        0      357 2024-04-06 15:38:16.261012 vomero-0.1.3/src/vomero/types.py
--rw-r--r--   0        0        0      996 2024-04-06 15:38:16.261012 vomero-0.1.3/src/vomero/worker.py
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 vomero-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-10 20:42:15.590693 vomero-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2605 2024-04-10 20:42:15.590693 vomero-0.1.4/README.md
+-rw-r--r--   0        0        0      537 2024-04-10 20:42:15.590693 vomero-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-10 20:42:15.590693 vomero-0.1.4/src/vomero/__init__.py
+-rw-r--r--   0        0        0     5641 2024-04-10 20:42:15.590693 vomero-0.1.4/src/vomero/streams.py
+-rw-r--r--   0        0        0      357 2024-04-10 20:42:15.590693 vomero-0.1.4/src/vomero/types.py
+-rw-r--r--   0        0        0      996 2024-04-10 20:42:15.590693 vomero-0.1.4/src/vomero/worker.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 vomero-0.1.4/PKG-INFO
```

### Comparing `vomero-0.1.3/LICENSE` & `vomero-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vomero-0.1.3/README.md` & `vomero-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vomero-0.1.3/pyproject.toml` & `vomero-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vomero"
-version = "0.1.3"
+version = "0.1.4"
 description = "Event processing library for Python based on Redis Streams"
 authors = ["Marcin Sawicki <marcin.z.sawicki@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mzsawicki/vomero"
 
 [tool.poetry.dependencies]
```

### Comparing `vomero-0.1.3/src/vomero/streams.py` & `vomero-0.1.4/src/vomero/streams.py`

 * *Files identical despite different names*

### Comparing `vomero-0.1.3/src/vomero/worker.py` & `vomero-0.1.4/src/vomero/worker.py`

 * *Files identical despite different names*

### Comparing `vomero-0.1.3/PKG-INFO` & `vomero-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vomero
-Version: 0.1.3
+Version: 0.1.4
 Summary: Event processing library for Python based on Redis Streams
 Home-page: https://github.com/mzsawicki/vomero
 License: MIT
 Author: Marcin Sawicki
 Author-email: marcin.z.sawicki@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

