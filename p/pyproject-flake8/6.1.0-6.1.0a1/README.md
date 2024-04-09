# Comparing `tmp/pyproject_flake8-6.1.0.tar.gz` & `tmp/pyproject_flake8-6.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_flake8-6.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyproject_flake8-6.1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyproject_flake8-6.1.0.tar` & `pyproject_flake8-6.1.0a1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-09-23 10:46:02.629613 pyproject_flake8-6.1.0/LICENSE
--rw-r--r--   0        0        0     3189 2023-09-23 10:46:02.629613 pyproject_flake8-6.1.0/README.md
--rw-r--r--   0        0        0     3935 2023-09-23 10:46:02.629613 pyproject_flake8-6.1.0/pflake8/__init__.py
--rw-r--r--   0        0        0       76 2023-09-23 10:46:02.629613 pyproject_flake8-6.1.0/pflake8/__main__.py
--rw-r--r--   0        0        0      766 2023-09-23 10:46:02.629613 pyproject_flake8-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 pyproject_flake8-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/LICENSE
+-rw-r--r--   0        0        0     3189 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/README.md
+-rw-r--r--   0        0        0     3937 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/pflake8/__init__.py
+-rw-r--r--   0        0        0       76 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/pflake8/__main__.py
+-rw-r--r--   0        0        0      766 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 pyproject_flake8-6.1.0a1/PKG-INFO
```

### Comparing `pyproject_flake8-6.1.0/LICENSE` & `pyproject_flake8-6.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_flake8-6.1.0/README.md` & `pyproject_flake8-6.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_flake8-6.1.0/pflake8/__init__.py` & `pyproject_flake8-6.1.0a1/pflake8/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ pyproject-flake8 (`pflake8`), a monkey patching wrapper to connect flake8 with pyproject.toml configuration """  # noqa
 
-__version__ = '6.1.0'
+__version__ = '6.1.0a1'
 
 import ast
 import configparser
 import multiprocessing.pool
 import sys
 from pathlib import Path
 from types import ModuleType
```

### Comparing `pyproject_flake8-6.1.0/pyproject.toml` & `pyproject_flake8-6.1.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [{name = "Christian Sachs", email = "sachs.christian@gmail.com"}]
 readme = "README.md"
 license = { file = "LICENSE" } 
 classifiers = []
 requires-python = ">=3.8.1"
 dependencies = [
     "tomli; python_version < '3.11'",
-    "flake8 == 6.1.0"
+    "flake8 >= 6.1.0"
 ]
 
 [project.urls]
 Home = "https://github.com/csachs/pyproject-flake8"
 
 [project.scripts]
 pflake8 = "pflake8.__main__:main"
```

### Comparing `pyproject_flake8-6.1.0/PKG-INFO` & `pyproject_flake8-6.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyproject-flake8
-Version: 6.1.0
+Version: 6.1.0a1
 Summary: pyproject-flake8 (`pflake8`), a monkey patching wrapper to connect flake8 with pyproject.toml configuration 
 Author-email: Christian Sachs <sachs.christian@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Requires-Dist: tomli; python_version < '3.11'
-Requires-Dist: flake8 == 6.1.0
+Requires-Dist: flake8 >= 6.1.0
 Project-URL: Home, https://github.com/csachs/pyproject-flake8
 
 # pyproject-flake8 (`pflake8`)
 
 A monkey patching wrapper to connect flake8 with `pyproject.toml` configuration.
 
 ## Update concerning versioning:
```

