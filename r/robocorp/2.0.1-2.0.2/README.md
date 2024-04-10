# Comparing `tmp/robocorp-2.0.1.tar.gz` & `tmp/robocorp-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-2.0.1.tar", max compression
+gzip compressed data, was "robocorp-2.0.2.tar", max compression
```

## Comparing `robocorp-2.0.1.tar` & `robocorp-2.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2927 2024-04-08 13:37:07.401201 robocorp-2.0.1/README.md
--rw-r--r--   0        0        0      816 2024-04-08 13:37:07.405202 robocorp-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-08 13:37:07.405202 robocorp-2.0.1/src/robocorp/_meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:37:07.405202 robocorp-2.0.1/src/robocorp/_meta/py.typed
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 robocorp-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2927 2024-04-10 04:59:41.289342 robocorp-2.0.2/README.md
+-rw-r--r--   0        0        0      816 2024-04-10 04:59:41.289342 robocorp-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-10 04:59:41.289342 robocorp-2.0.2/src/robocorp/_meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:59:41.289342 robocorp-2.0.2/src/robocorp/_meta/py.typed
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 robocorp-2.0.2/PKG-INFO
```

### Comparing `robocorp-2.0.1/README.md` & `robocorp-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `robocorp-2.0.1/pyproject.toml` & `robocorp-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp"
-version = "2.0.1"
+version = "2.0.2"
 description = "Robocorp core libraries for Python automation"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-tasks = "^3.0.2"
+robocorp-tasks = "^3.0.3"
 robocorp-log = "^2.9.2"
 robocorp-workitems = "^1.4.5"
 robocorp-vault = "^1.3.5"
 robocorp-storage = "^1.0.4"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
```

### Comparing `robocorp-2.0.1/PKG-INFO` & `robocorp-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: robocorp
-Version: 2.0.1
+Version: 2.0.2
 Summary: Robocorp core libraries for Python automation
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: robocorp-log (>=2.9.2,<3.0.0)
 Requires-Dist: robocorp-storage (>=1.0.4,<2.0.0)
-Requires-Dist: robocorp-tasks (>=3.0.2,<4.0.0)
+Requires-Dist: robocorp-tasks (>=3.0.3,<4.0.0)
 Requires-Dist: robocorp-vault (>=1.3.5,<2.0.0)
 Requires-Dist: robocorp-workitems (>=1.4.5,<2.0.0)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp
```

