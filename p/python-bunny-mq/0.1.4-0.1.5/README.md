# Comparing `tmp/python_bunny_mq-0.1.4.tar.gz` & `tmp/python_bunny_mq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bunny_mq-0.1.4.tar", max compression
+gzip compressed data, was "python_bunny_mq-0.1.5.tar", max compression
```

## Comparing `python_bunny_mq-0.1.4.tar` & `python_bunny_mq-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1687 2024-04-08 22:10:31.538782 python_bunny_mq-0.1.4/README.md
--rw-r--r--   0        0        0      830 2024-04-09 19:34:13.733563 python_bunny_mq-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       34 2024-03-29 22:39:24.413846 python_bunny_mq-0.1.4/python_bunny_mq/__init__.py
--rw-r--r--   0        0        0     4968 2024-04-09 19:34:41.473020 python_bunny_mq-0.1.4/python_bunny_mq/bunny_mq.py
--rw-r--r--   0        0        0     1315 2024-04-09 19:34:41.459255 python_bunny_mq-0.1.4/python_bunny_mq/test_bunny_queue.py
--rw-r--r--   0        0        0     2326 1970-01-01 00:00:00.000000 python_bunny_mq-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1687 2024-04-08 22:10:31.538782 python_bunny_mq-0.1.5/README.md
+-rw-r--r--   0        0        0      830 2024-04-09 19:36:57.214043 python_bunny_mq-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-29 22:39:24.413846 python_bunny_mq-0.1.5/python_bunny_mq/__init__.py
+-rw-r--r--   0        0        0     4968 2024-04-09 19:34:41.473020 python_bunny_mq-0.1.5/python_bunny_mq/bunny_mq.py
+-rw-r--r--   0        0        0     1315 2024-04-09 19:34:41.459255 python_bunny_mq-0.1.5/python_bunny_mq/test_bunny_queue.py
+-rw-r--r--   0        0        0     2326 1970-01-01 00:00:00.000000 python_bunny_mq-0.1.5/PKG-INFO
```

### Comparing `python_bunny_mq-0.1.4/README.md` & `python_bunny_mq-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python_bunny_mq-0.1.4/pyproject.toml` & `python_bunny_mq-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-bunny-mq"
-version = "0.1.4"
+version = "0.1.5"
 description = "Ultra-lightweight (no-dependency) message queue for intra-process pub-sub communication."
 authors = ["Steven Miers <steven.miers@gmail.com>"]
 license = "THE UNLICENSE"
 readme = "README.md"
 homepage = "https://pypi.org/project/python-bunny-mq/"
 repository = "https://github.com/tangledpath/python-bunny-mq"
 documentation = "https://tangledpath.github.io/python-bunny-mq"
```

### Comparing `python_bunny_mq-0.1.4/python_bunny_mq/bunny_mq.py` & `python_bunny_mq-0.1.5/python_bunny_mq/bunny_mq.py`

 * *Files identical despite different names*

### Comparing `python_bunny_mq-0.1.4/python_bunny_mq/test_bunny_queue.py` & `python_bunny_mq-0.1.5/python_bunny_mq/test_bunny_queue.py`

 * *Files identical despite different names*

### Comparing `python_bunny_mq-0.1.4/PKG-INFO` & `python_bunny_mq-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bunny-mq
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ultra-lightweight (no-dependency) message queue for intra-process pub-sub communication.
 Home-page: https://pypi.org/project/python-bunny-mq/
 License: Unlicense
 Author: Steven Miers
 Author-email: steven.miers@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved
```

