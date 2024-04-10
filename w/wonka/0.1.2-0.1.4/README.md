# Comparing `tmp/wonka-0.1.2.tar.gz` & `tmp/wonka-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonka-0.1.2.tar", last modified: Fri Nov  3 04:22:50 2023, max compression
+gzip compressed data, was "wonka-0.1.4.tar", last modified: Wed Apr 10 06:53:11 2024, max compression
```

## Comparing `wonka-0.1.2.tar` & `wonka-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      591 2023-11-03 04:22:34.167249 wonka-0.1.2/LICENSE
--rwxr-xr-x   0        0        0    11631 2023-11-03 04:22:34.167249 wonka-0.1.2/README.md
--rw-r--r--   0        0        0     3900 2023-11-03 04:22:50.091479 wonka-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1066 2023-11-03 04:22:34.171249 wonka-0.1.2/src/wonka/__init__.py
--rw-r--r--   0        0        0     5938 2023-11-03 04:22:34.171249 wonka-0.1.2/src/wonka/base.py
--rw-r--r--   0        0        0     4454 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/configuration.py
--rw-r--r--   0        0        0     6653 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/dispatchers.py
--rw-r--r--   0        0        0     6589 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/managers.py
--rw-r--r--   0        0        0     4071 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/producers.py
--rw-r--r--   0        0        0     1298 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/prototypers.py
--rw-r--r--   0        0        0     4522 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/registries.py
--rw-r--r--   0        0        0     3418 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/shared.py
--rw-r--r--   0        0        0     7512 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/storage.py
--rw-r--r--   0        0        0     2389 2023-11-03 04:22:34.175249 wonka-0.1.2/src/wonka/utilities.py
--rw-r--r--   0        0        0     1506 2023-11-03 04:22:34.175249 wonka-0.1.2/tests/test_dispatchers.py
--rw-r--r--   0        0        0     1179 2023-11-03 04:22:34.175249 wonka-0.1.2/tests/test_managers.py
--rw-r--r--   0        0        0     1709 2023-11-03 04:22:34.175249 wonka-0.1.2/tests/test_producers.py
--rw-r--r--   0        0        0      726 2023-11-03 04:22:34.175249 wonka-0.1.2/tests/test_prototypers.py
--rw-r--r--   0        0        0     1323 2023-11-03 04:22:34.175249 wonka-0.1.2/tests/test_registries.py
--rw-r--r--   0        0        0     1430 2023-11-03 04:22:34.175249 wonka-0.1.2/tests/test_storage.py
--rw-r--r--   0        0        0    12689 1970-01-01 00:00:00.000000 wonka-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-10 06:52:55.102756 wonka-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0    11631 2024-04-10 06:52:55.102756 wonka-0.1.4/README.md
+-rw-r--r--   0        0        0     3878 2024-04-10 06:53:11.086894 wonka-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1066 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/__init__.py
+-rw-r--r--   0        0        0     5938 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/base.py
+-rw-r--r--   0        0        0     4454 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/configuration.py
+-rw-r--r--   0        0        0     6653 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/dispatchers.py
+-rw-r--r--   0        0        0     6589 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/managers.py
+-rw-r--r--   0        0        0     4071 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/producers.py
+-rw-r--r--   0        0        0     1298 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/prototypers.py
+-rw-r--r--   0        0        0     4522 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/registries.py
+-rw-r--r--   0        0        0     3418 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/shared.py
+-rw-r--r--   0        0        0     7512 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/storage.py
+-rw-r--r--   0        0        0     2389 2024-04-10 06:52:55.106756 wonka-0.1.4/src/wonka/utilities.py
+-rw-r--r--   0        0        0     1506 2024-04-10 06:52:55.110756 wonka-0.1.4/tests/test_dispatchers.py
+-rw-r--r--   0        0        0     1179 2024-04-10 06:52:55.110756 wonka-0.1.4/tests/test_managers.py
+-rw-r--r--   0        0        0     1709 2024-04-10 06:52:55.110756 wonka-0.1.4/tests/test_producers.py
+-rw-r--r--   0        0        0      726 2024-04-10 06:52:55.110756 wonka-0.1.4/tests/test_prototypers.py
+-rw-r--r--   0        0        0     1323 2024-04-10 06:52:55.110756 wonka-0.1.4/tests/test_registries.py
+-rw-r--r--   0        0        0     1430 2024-04-10 06:52:55.110756 wonka-0.1.4/tests/test_storage.py
+-rw-r--r--   0        0        0    12689 1970-01-01 00:00:00.000000 wonka-0.1.4/PKG-INFO
```

### Comparing `wonka-0.1.2/LICENSE` & `wonka-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/README.md` & `wonka-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/pyproject.toml` & `wonka-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keywords = [
     "factory",
     "construction",
     "constructor",
     "design pattern",
 ]
 dependencies = []
-version = "0.1.2"
+version = "0.1.4"
 
 [project.license]
 text = "Apache Software License 2.0"
 
 [project.urls]
 Documentation = "https://WithPrecedent.github.io/wonka"
 Repository = "https://github.com/WithPrecedent/wonka"
@@ -81,15 +81,14 @@
 
 [tool.pdm.version]
 source = "file"
 path = "src/wonka/__init__.py"
 
 [tool.pytest.ini_options]
 addopts = "--showlocals"
-asyncio_mode = "auto"
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
 pythonpath = [
     "src",
 ]
```

### Comparing `wonka-0.1.2/src/wonka/__init__.py` & `wonka-0.1.4/src/wonka/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Flexible, accessible, extensible Python factories"""
 
 from __future__ import annotations
 
-__version__ = '0.1.2'
+__version__ = '0.1.4'
 
 __author__: str = 'Corey Rayburn Yung'
 
 __all__: list[str] = [
     'Assembler',
     'Classer',
     'Delegate',
```

### Comparing `wonka-0.1.2/src/wonka/base.py` & `wonka-0.1.4/src/wonka/base.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/configuration.py` & `wonka-0.1.4/src/wonka/configuration.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/dispatchers.py` & `wonka-0.1.4/src/wonka/dispatchers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/managers.py` & `wonka-0.1.4/src/wonka/managers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/producers.py` & `wonka-0.1.4/src/wonka/producers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/prototypers.py` & `wonka-0.1.4/src/wonka/prototypers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/registries.py` & `wonka-0.1.4/src/wonka/registries.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/shared.py` & `wonka-0.1.4/src/wonka/shared.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/storage.py` & `wonka-0.1.4/src/wonka/storage.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/src/wonka/utilities.py` & `wonka-0.1.4/src/wonka/utilities.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/tests/test_dispatchers.py` & `wonka-0.1.4/tests/test_dispatchers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/tests/test_managers.py` & `wonka-0.1.4/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/tests/test_producers.py` & `wonka-0.1.4/tests/test_producers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/tests/test_prototypers.py` & `wonka-0.1.4/tests/test_prototypers.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/tests/test_registries.py` & `wonka-0.1.4/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/tests/test_storage.py` & `wonka-0.1.4/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `wonka-0.1.2/PKG-INFO` & `wonka-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wonka
-Version: 0.1.2
+Version: 0.1.4
 Summary: Flexible, accessible, extensible Python factories
 Keywords: factory construction constructor design pattern
 Author-Email: Corey Rayburn Yung <coreyrayburnyung@gmail.com>
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

