# Comparing `tmp/stringx-0.7.1.tar.gz` & `tmp/stringx-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringx-0.7.1.tar", last modified: Tue Apr  9 23:07:10 2024, max compression
+gzip compressed data, was "stringx-0.7.3.tar", last modified: Tue Apr  9 23:29:47 2024, max compression
```

## Comparing `stringx-0.7.1.tar` & `stringx-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-04-09 23:06:57.853015 stringx-0.7.1/LICENSE
--rw-r--r--   0        0        0     3218 2024-04-09 23:06:57.853015 stringx-0.7.1/README.md
--rw-r--r--   0        0        0     2102 2024-04-09 23:07:10.000943 stringx-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2564 2024-04-09 23:06:57.853015 stringx-0.7.1/src/stringx/__init__.py
--rw-r--r--   0        0        0     4253 2024-04-09 23:06:57.853015 stringx-0.7.1/src/stringx/client.py
--rw-r--r--   0        0        0        0 2024-04-09 23:06:57.853015 stringx-0.7.1/src/stringx/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0      163 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     7334 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/test_client.py
--rw-r--r--   0        0        0     1535 2024-04-09 23:06:57.853015 stringx-0.7.1/tests/test_stringx.py
--rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-09 23:29:35.148434 stringx-0.7.3/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-09 23:29:35.148434 stringx-0.7.3/README.md
+-rw-r--r--   0        0        0     2102 2024-04-09 23:29:47.840355 stringx-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2564 2024-04-09 23:29:35.148434 stringx-0.7.3/src/stringx/__init__.py
+-rw-r--r--   0        0        0     4253 2024-04-09 23:29:35.152434 stringx-0.7.3/src/stringx/client.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:29:35.152434 stringx-0.7.3/src/stringx/py.typed
+-rw-r--r--   0        0        0        0 2024-04-09 23:29:35.152434 stringx-0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-09 23:29:35.152434 stringx-0.7.3/tests/conftest.py
+-rw-r--r--   0        0        0     7334 2024-04-09 23:29:35.152434 stringx-0.7.3/tests/test_client.py
+-rw-r--r--   0        0        0     1535 2024-04-09 23:29:35.152434 stringx-0.7.3/tests/test_stringx.py
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.7.3/PKG-INFO
```

### Comparing `stringx-0.7.1/LICENSE` & `stringx-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stringx-0.7.1/README.md` & `stringx-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `stringx-0.7.1/pyproject.toml` & `stringx-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.7.1"
+version = "0.7.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pypi.org/project/stringx"
 Repository = "https://github.com/cachitas/stringx"
```

### Comparing `stringx-0.7.1/src/stringx/__init__.py` & `stringx-0.7.3/src/stringx/__init__.py`

 * *Files identical despite different names*

### Comparing `stringx-0.7.1/src/stringx/client.py` & `stringx-0.7.3/src/stringx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations  # required in Python 3.9
 
 import logging
 
 import httpx
 
-__version__ = "0.7.1"
+__version__ = "0.7.3"
 
 logger = logging.getLogger("stringx")
 
 
 class Client(httpx.Client):
     def __init__(self, identity: str, base_url: str = "https://string-db.org") -> None:
         if not identity:
```

### Comparing `stringx-0.7.1/tests/test_client.py` & `stringx-0.7.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stringx-0.7.1/tests/test_stringx.py` & `stringx-0.7.3/tests/test_stringx.py`

 * *Files identical despite different names*

### Comparing `stringx-0.7.1/PKG-INFO` & `stringx-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringx
-Version: 0.7.1
+Version: 0.7.3
 Summary: STRING DB API Client
 Keywords: string api client httpx sib cpr embl biodata elixir protein gene interaction
 Author-Email: Hugo Cachitas <hcachitas@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

