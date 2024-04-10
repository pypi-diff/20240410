# Comparing `tmp/pprint_tools-0.0.1.tar.gz` & `tmp/pprint_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pprint_tools-0.0.1.tar", max compression
+gzip compressed data, was "pprint_tools-0.0.2.tar", max compression
```

## Comparing `pprint_tools-0.0.1.tar` & `pprint_tools-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      477 2023-10-17 15:24:26.797844 pprint_tools-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-10-17 15:02:26.416321 pprint_tools-0.0.1/pprint_tools/__init__.py
--rw-r--r--   0        0        0     4409 2023-10-17 15:11:52.698258 pprint_tools-0.0.1/pprint_tools/app.py
--rw-r--r--   0        0        0     1084 2023-10-17 15:35:01.666585 pprint_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 pprint_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      477 2023-10-17 15:24:26.797844 pprint_tools-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-10-17 15:02:26.416321 pprint_tools-0.0.2/pprint_tools/__init__.py
+-rw-r--r--   0        0        0     4409 2023-10-17 15:11:52.698258 pprint_tools-0.0.2/pprint_tools/app.py
+-rw-r--r--   0        0        0     1084 2024-03-28 04:25:15.448886 pprint_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 pprint_tools-0.0.2/PKG-INFO
```

### Comparing `pprint_tools-0.0.1/pprint_tools/app.py` & `pprint_tools-0.0.2/pprint_tools/app.py`

 * *Files identical despite different names*

### Comparing `pprint_tools-0.0.1/pyproject.toml` & `pprint_tools-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pprint-tools"
-version = "0.0.1"
+version = "0.0.2"
 description = "decorators cli tools"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "logrich", "rich"]
 
 [project.urls]
 "Homepage" = "https://github.com/MavlinD/pprint-tools"
 "Bug Tracker" = "https://github.com/MavlinD/pprint-tools/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 logrich = "^1.0.3"
-anyio = "^4.0.0"
+anyio = "^3.6.1"
 pre-commit = "^3.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "6.2.4"
 pytest-picked = "0.4.6"
 pytest-testmon = "1.1.1"
 pytest-watch = "4.2.0"
```

### Comparing `pprint_tools-0.0.1/PKG-INFO` & `pprint_tools-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pprint-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: decorators cli tools
 License: GPL
 Keywords: logger,logrich,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anyio (>=4.0.0,<5.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anyio (>=3.6.1,<4.0.0)
 Requires-Dist: logrich (>=1.0.3,<2.0.0)
 Requires-Dist: pre-commit (>=3.5.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 ### Фабрика декораторов
 включает два декоратора, один для вывода времени выполнения, второй для вывода аргументов в консоль
```

