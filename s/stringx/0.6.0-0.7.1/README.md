# Comparing `tmp/stringx-0.6.0.tar.gz` & `tmp/stringx-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringx-0.6.0.tar", last modified: Tue Apr  9 00:06:50 2024, max compression
+gzip compressed data, was "stringx-0.7.1.tar", last modified: Tue Apr  9 23:07:10 2024, max compression
```

## Comparing `stringx-0.6.0.tar` & `stringx-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-03-18 00:39:05.484210 stringx-0.6.0/LICENSE
--rw-r--r--   0        0        0     3218 2024-04-05 12:51:19.529957 stringx-0.6.0/README.md
--rw-r--r--   0        0        0     2080 2024-04-09 00:06:50.593190 stringx-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2564 2024-04-09 00:05:02.653192 stringx-0.6.0/src/stringx/__init__.py
--rw-r--r--   0        0        0     4253 2024-04-09 00:06:25.103189 stringx-0.6.0/src/stringx/client.py
--rw-r--r--   0        0        0        0 2024-04-03 22:27:23.943070 stringx-0.6.0/src/stringx/py.typed
--rw-r--r--   0        0        0        0 2024-03-18 00:39:05.504210 stringx-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      163 2024-04-04 00:02:15.343066 stringx-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     7334 2024-04-09 00:00:22.273194 stringx-0.6.0/tests/test_client.py
--rw-r--r--   0        0        0     1535 2024-04-08 18:05:17.473191 stringx-0.6.0/tests/test_stringx.py
--rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-09 23:06:57.853015 stringx-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-09 23:06:57.853015 stringx-0.7.1/README.md
+-rw-r--r--   0        0        0     2102 2024-04-09 23:07:10.000943 stringx-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2564 2024-04-09 23:06:57.853015 stringx-0.7.1/src/stringx/__init__.py
+-rw-r--r--   0        0        0     4253 2024-04-09 23:06:57.853015 stringx-0.7.1/src/stringx/client.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:06:57.853015 stringx-0.7.1/src/stringx/py.typed
+-rw-r--r--   0        0        0        0 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     7334 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/test_client.py
+-rw-r--r--   0        0        0     1535 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/test_stringx.py
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.7.1/PKG-INFO
```

### Comparing `stringx-0.6.0/LICENSE` & `stringx-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stringx-0.6.0/README.md` & `stringx-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `stringx-0.6.0/pyproject.toml` & `stringx-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,31 +43,35 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.6.0"
+version = "0.7.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pypi.org/project/stringx"
 Repository = "https://github.com/cachitas/stringx"
 Issues = "https://github.com/cachitas/stringx/issues"
 
 [tool.pdm.dev-dependencies]
 dev = [
+    "tox-pdm>=0.7.2",
+]
+test = [
     "pytest>=8.1.1",
     "pytest-httpx>=0.30.0",
+]
+lint = [
     "ruff>=0.3.5",
     "mypy>=1.9.0",
-    "tox-pdm>=0.7.2",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "src/stringx/client.py"
 
 [tool.pdm.scripts]
```

### Comparing `stringx-0.6.0/src/stringx/__init__.py` & `stringx-0.7.1/src/stringx/__init__.py`

 * *Files identical despite different names*

### Comparing `stringx-0.6.0/src/stringx/client.py` & `stringx-0.7.1/src/stringx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations  # required in Python 3.9
 
 import logging
 
 import httpx
 
-__version__ = "0.6.0"
+__version__ = "0.7.1"
 
 logger = logging.getLogger("stringx")
 
 
 class Client(httpx.Client):
     def __init__(self, identity: str, base_url: str = "https://string-db.org") -> None:
         if not identity:
```

### Comparing `stringx-0.6.0/tests/test_client.py` & `stringx-0.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stringx-0.6.0/tests/test_stringx.py` & `stringx-0.7.1/tests/test_stringx.py`

 * *Files identical despite different names*

### Comparing `stringx-0.6.0/PKG-INFO` & `stringx-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringx
-Version: 0.6.0
+Version: 0.7.1
 Summary: STRING DB API Client
 Keywords: string api client httpx sib cpr embl biodata elixir protein gene interaction
 Author-Email: Hugo Cachitas <hcachitas@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

