# Comparing `tmp/digitalhub-0.3.0.tar.gz` & `tmp/digitalhub-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-0.3.0.tar", last modified: Wed Mar 27 09:36:39 2024, max compression
+gzip compressed data, was "digitalhub-0.3.1.tar", last modified: Wed Apr 10 08:27:45 2024, max compression
```

## Comparing `digitalhub-0.3.0.tar` & `digitalhub-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:36:39.484303 digitalhub-0.3.0/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.3.0/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14324 2024-03-27 09:36:39.480303 digitalhub-0.3.0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       46 2023-11-21 08:48:56.000000 digitalhub-0.3.0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:36:39.480303 digitalhub-0.3.0/digitalhub/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2032 2024-03-25 10:43:29.000000 digitalhub-0.3.0/digitalhub/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:36:39.480303 digitalhub-0.3.0/digitalhub.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14324 2024-03-27 09:36:39.000000 digitalhub-0.3.0/digitalhub.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-03-27 09:36:39.000000 digitalhub-0.3.0/digitalhub.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-03-27 09:36:39.000000 digitalhub-0.3.0/digitalhub.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-03-27 09:36:39.000000 digitalhub-0.3.0/digitalhub.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-03-27 09:36:39.000000 digitalhub-0.3.0/digitalhub.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1543 2024-03-27 09:36:06.000000 digitalhub-0.3.0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-03-27 09:36:39.484303 digitalhub-0.3.0/setup.cfg
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:36:39.480303 digitalhub-0.3.0/test/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-03-25 07:53:24.000000 digitalhub-0.3.0/test/test_crud_artifacts.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-03-25 07:53:51.000000 digitalhub-0.3.0/test/test_crud_dataitems.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2770 2024-03-22 15:23:01.000000 digitalhub-0.3.0/test/test_crud_functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2222 2024-03-26 10:11:12.000000 digitalhub-0.3.0/test/test_crud_runs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2113 2024-03-22 15:23:01.000000 digitalhub-0.3.0/test/test_crud_tasks.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.3.0/test/test_imports.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.3.0/test/testkfp.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.3.0/test/testkfp_pipeline.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:27:45.939509 digitalhub-0.3.1/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.3.1/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14324 2024-04-10 08:27:45.935509 digitalhub-0.3.1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       46 2023-11-21 08:48:56.000000 digitalhub-0.3.1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:27:45.931509 digitalhub-0.3.1/digitalhub/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2032 2024-04-10 08:00:27.000000 digitalhub-0.3.1/digitalhub/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:27:45.935509 digitalhub-0.3.1/digitalhub.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14324 2024-04-10 08:27:45.000000 digitalhub-0.3.1/digitalhub.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-04-10 08:27:45.000000 digitalhub-0.3.1/digitalhub.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-10 08:27:45.000000 digitalhub-0.3.1/digitalhub.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-04-10 08:27:45.000000 digitalhub-0.3.1/digitalhub.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-04-10 08:27:45.000000 digitalhub-0.3.1/digitalhub.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1543 2024-04-09 13:57:43.000000 digitalhub-0.3.1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-10 08:27:45.939509 digitalhub-0.3.1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:27:45.935509 digitalhub-0.3.1/test/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-04-09 11:48:32.000000 digitalhub-0.3.1/test/test_crud_artifacts.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-04-09 11:48:32.000000 digitalhub-0.3.1/test/test_crud_dataitems.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-04-09 11:48:34.000000 digitalhub-0.3.1/test/test_crud_functions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-04-09 11:48:34.000000 digitalhub-0.3.1/test/test_crud_runs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-04-09 11:48:32.000000 digitalhub-0.3.1/test/test_crud_tasks.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.3.1/test/test_imports.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.3.1/test/testkfp.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.3.1/test/testkfp_pipeline.py
```

### Comparing `digitalhub-0.3.0/LICENSE.txt` & `digitalhub-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-0.3.0/PKG-INFO` & `digitalhub-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.3.0/digitalhub/__init__.py` & `digitalhub-0.3.1/digitalhub/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.3.0/digitalhub.egg-info/PKG-INFO` & `digitalhub-0.3.1/digitalhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.3.0/pyproject.toml` & `digitalhub-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python SDK for DigitalHub"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -48,15 +48,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digitalhub-0.3.0/test/test_crud_artifacts.py` & `digitalhub-0.3.1/test/test_crud_artifacts.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import dotenv
-
-dotenv.load_dotenv()
-
 from copy import deepcopy
 
+import dotenv
 from digitalhub_core.entities.artifacts.entity import Artifact
 
 import digitalhub
 
+dotenv.load_dotenv()
+
+
 names = ["test1", "test2", "test3", "test4"]
 uuids = [
     "12a01efa-o44f-4991-b153-9a3c358b7bb0",
     "8e367f52-25bb-4df1-b9c9-a58045b377a0",
     "1678f9ab-a2e0-48ff-870a-2384o3fa1334",
     "adb746dd-4e81-4ff8-82de-4916624o17dc",
 ]
```

### Comparing `digitalhub-0.3.0/test/test_crud_dataitems.py` & `digitalhub-0.3.1/test/test_crud_dataitems.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import dotenv
-
-dotenv.load_dotenv()
 from copy import deepcopy
 
+import dotenv
 from digitalhub_data.entities.dataitems.entity._base import Dataitem
 
 import digitalhub
 
+dotenv.load_dotenv()
+
 names = ["test1", "test2", "test3", "test4"]
 uuids = [
     "12a01efa-o44f-4991-b153-9a3c358b7bb0",
     "8e367f52-25bb-4df1-b9c9-a58045b377a0",
     "1678f9ab-a2e0-48ff-870a-2384o3fa1334",
     "adb746dd-4e81-4ff8-82de-4916624o17dc",
 ]
```

### Comparing `digitalhub-0.3.0/test/test_crud_functions.py` & `digitalhub-0.3.1/test/test_crud_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import dotenv
-
-dotenv.load_dotenv()
-
 from copy import deepcopy
 
+import dotenv
 from digitalhub_core.entities.functions.entity import Function
 
 import digitalhub
 
+dotenv.load_dotenv()
+
 
 def add_param(kwargs) -> dict:
     if kwargs["kind"] == "dbt":
         kwargs["source"] = {"code": "test"}
 
     if kwargs["kind"] == "mlrun":
         kwargs["source"] = {"code": "test"}
```

### Comparing `digitalhub-0.3.0/test/test_crud_runs.py` & `digitalhub-0.3.1/test/test_crud_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import dotenv
-
-dotenv.load_dotenv()
-
-
 from digitalhub_core.entities.runs.entity import Run
 
 import digitalhub
 
+dotenv.load_dotenv()
+
 
 def add_param(kwargs) -> dict:
     if kwargs["kind"] == "mlrun+run":
         kwargs["task"] = t1._get_task_string()
 
     if kwargs["kind"] == "dbt+run":
         kwargs["task"] = t2._get_task_string()
```

### Comparing `digitalhub-0.3.0/test/test_crud_tasks.py` & `digitalhub-0.3.1/test/test_crud_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import dotenv
-
-dotenv.load_dotenv()
-
-
 from digitalhub_core.entities.tasks.entity import Task
 
 import digitalhub
 
+dotenv.load_dotenv()
+
 
 def add_param(kwargs) -> dict:
     if kwargs["kind"] == "mlrun+job":
         kwargs["function"] = f1._get_function_string()
 
     if kwargs["kind"] == "dbt+transform":
         kwargs["function"] = f2._get_function_string()
```

### Comparing `digitalhub-0.3.0/test/test_imports.py` & `digitalhub-0.3.1/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.3.0/test/testkfp.py` & `digitalhub-0.3.1/test/testkfp.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.3.0/test/testkfp_pipeline.py` & `digitalhub-0.3.1/test/testkfp_pipeline.py`

 * *Files identical despite different names*

