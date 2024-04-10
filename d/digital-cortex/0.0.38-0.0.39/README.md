# Comparing `tmp/digital_cortex-0.0.38.tar.gz` & `tmp/digital_cortex-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_cortex-0.0.38.tar", max compression
+gzip compressed data, was "digital_cortex-0.0.39.tar", max compression
```

## Comparing `digital_cortex-0.0.38.tar` & `digital_cortex-0.0.39.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       58 2023-08-11 11:23:30.471834 digital_cortex-0.0.38/LICENSE.md
--rw-r--r--   0        0        0      485 2023-08-22 06:05:46.698541 digital_cortex-0.0.38/README.md
--rw-r--r--   0        0        0     9511 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/Statement-Semantic-Sort-v2.py
--rw-r--r--   0        0        0       41 2024-02-26 07:43:45.437169 digital_cortex-0.0.38/digital_cortex/__init__.py
--rw-r--r--   0        0        0      705 2024-02-26 07:40:29.709771 digital_cortex-0.0.38/digital_cortex/client.py
--rw-r--r--   0        0        0      142 2024-02-26 10:25:33.119484 digital_cortex-0.0.38/digital_cortex/config.py
--rw-r--r--   0        0        0     6634 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/datasets.py
--rw-r--r--   0        0        0     2020 2023-09-08 11:41:22.746460 digital_cortex-0.0.38/digital_cortex/function_creator.py
--rw-r--r--   0        0        0      512 2024-02-26 07:40:41.497735 digital_cortex-0.0.38/digital_cortex/function_runner.py
--rw-r--r--   0        0        0     6945 2024-02-26 10:22:53.597290 digital_cortex-0.0.38/digital_cortex/functions.py
--rw-r--r--   0        0        0     5858 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/models.py
--rw-r--r--   0        0        0     3782 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/pipelines.py
--rw-r--r--   0        0        0        0 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/schema/__init__.py
--rw-r--r--   0        0        0     2767 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/schema/datasets.py
--rw-r--r--   0        0        0      886 2023-09-08 06:47:07.943346 digital_cortex-0.0.38/digital_cortex/schema/functions.py
--rw-r--r--   0        0        0     1531 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/schema/models.py
--rw-r--r--   0        0        0      546 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/schema/pipelines.py
--rw-r--r--   0        0        0       98 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/schema/scoring.py
--rw-r--r--   0        0        0      118 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/schema/tags.py
--rw-r--r--   0        0        0      479 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/scoring.py
--rw-r--r--   0        0        0      872 2023-08-22 05:52:45.619133 digital_cortex-0.0.38/digital_cortex/tags.py
--rw-r--r--   0        0        0      968 2024-02-26 10:29:47.824809 digital_cortex-0.0.38/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 digital_cortex-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-08-11 11:23:30.471834 digital_cortex-0.0.39/LICENSE.md
+-rw-r--r--   0        0        0      485 2023-08-22 06:05:46.698541 digital_cortex-0.0.39/README.md
+-rw-r--r--   0        0        0     9511 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/Statement-Semantic-Sort-v2.py
+-rw-r--r--   0        0        0       41 2024-02-26 07:43:45.437169 digital_cortex-0.0.39/digital_cortex/__init__.py
+-rw-r--r--   0        0        0      705 2024-02-26 07:40:29.709771 digital_cortex-0.0.39/digital_cortex/client.py
+-rw-r--r--   0        0        0      112 2024-04-10 11:01:21.586948 digital_cortex-0.0.39/digital_cortex/config.py
+-rw-r--r--   0        0        0     6634 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/datasets.py
+-rw-r--r--   0        0        0     2024 2024-04-10 10:45:38.480952 digital_cortex-0.0.39/digital_cortex/function_creator.py
+-rw-r--r--   0        0        0      512 2024-02-26 07:40:41.497735 digital_cortex-0.0.39/digital_cortex/function_runner.py
+-rw-r--r--   0        0        0     6900 2024-04-10 10:50:58.415709 digital_cortex-0.0.39/digital_cortex/functions.py
+-rw-r--r--   0        0        0     5858 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/models.py
+-rw-r--r--   0        0        0     3782 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/pipelines.py
+-rw-r--r--   0        0        0        0 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/schema/__init__.py
+-rw-r--r--   0        0        0     2767 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/schema/datasets.py
+-rw-r--r--   0        0        0      886 2023-09-08 06:47:07.943346 digital_cortex-0.0.39/digital_cortex/schema/functions.py
+-rw-r--r--   0        0        0     1531 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/schema/models.py
+-rw-r--r--   0        0        0      546 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/schema/pipelines.py
+-rw-r--r--   0        0        0       98 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/schema/scoring.py
+-rw-r--r--   0        0        0      118 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/schema/tags.py
+-rw-r--r--   0        0        0      479 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/scoring.py
+-rw-r--r--   0        0        0      872 2023-08-22 05:52:45.619133 digital_cortex-0.0.39/digital_cortex/tags.py
+-rw-r--r--   0        0        0      968 2024-04-10 11:02:39.688134 digital_cortex-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 digital_cortex-0.0.39/PKG-INFO
```

### Comparing `digital_cortex-0.0.38/digital_cortex/Statement-Semantic-Sort-v2.py` & `digital_cortex-0.0.39/digital_cortex/Statement-Semantic-Sort-v2.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/client.py` & `digital_cortex-0.0.39/digital_cortex/client.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/datasets.py` & `digital_cortex-0.0.39/digital_cortex/datasets.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/function_creator.py` & `digital_cortex-0.0.39/digital_cortex/function_creator.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,14 @@
             }
 
     def execute(self, *args, **kwargs):
         if self.create_or_update:
             payload = {"params": {"args": args, "kwargs": kwargs}}
             url = self.host_url + BASE_PATH + f'/sdk/run/{self.function_id}'
             response = requests.post(url, headers=self.headers, json=payload)
-            return response.text
+            return response.json()
         else:
             url = self.host_url + BASE_PATH + '/sdk/evaluate'
             params = {"params": {"args": args, "kwargs": kwargs}}
             payload = {**self.payload, **params}
             response = requests.post(url, headers=self.headers, json=payload)
-            return response.text
+            return response.json()
```

### Comparing `digital_cortex-0.0.38/digital_cortex/function_runner.py` & `digital_cortex-0.0.39/digital_cortex/function_runner.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/functions.py` & `digital_cortex-0.0.39/digital_cortex/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import re
 
 import requests
 
 from digital_cortex.function_creator import FunctionCreator
 from digital_cortex.function_runner import FunctionRunner
 from digital_cortex.schema.functions import *
-from digital_cortex.schema.tags import TagForm
 
 BASE_PATH = "/api/v1/functions"
 
 
 class Functions:
     def __init__(self, host_url, headers):
         self.host_url = host_url
@@ -139,15 +138,15 @@
                     payload = {"computeType": compute_type, "script": code,
                                "dependency": dependencies, "params": {"args": args, "kwargs": kwargs},
                                "functionName": inner_function_name,
                                "async": blocking, "createOrUpdate": create_or_update, "isPublished": is_published,
                                "geography": geography}
                     url = self.host_url + BASE_PATH + "/sdk/evaluate/script"
                     response = requests.post(url, headers=self.headers, json=payload)
-                    result = response.text
+                    result = response.json()
 
                 else:
                     result = None
 
                 return result
 
             return wrapper
```

### Comparing `digital_cortex-0.0.38/digital_cortex/models.py` & `digital_cortex-0.0.39/digital_cortex/models.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/pipelines.py` & `digital_cortex-0.0.39/digital_cortex/pipelines.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/schema/datasets.py` & `digital_cortex-0.0.39/digital_cortex/schema/datasets.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/schema/functions.py` & `digital_cortex-0.0.39/digital_cortex/schema/functions.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/schema/models.py` & `digital_cortex-0.0.39/digital_cortex/schema/models.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/schema/pipelines.py` & `digital_cortex-0.0.39/digital_cortex/schema/pipelines.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/digital_cortex/tags.py` & `digital_cortex-0.0.39/digital_cortex/tags.py`

 * *Files identical despite different names*

### Comparing `digital_cortex-0.0.38/pyproject.toml` & `digital_cortex-0.0.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=65.0', 'pandas>=1.5', 'numpy>=1.23.5', 'requests>=2.28.1', 'python-dotenv>=1.0.0', "pydantic>=2.1.1"]
 build-backend = 'setuptools.build_meta'
 
 [tool.poetry]
 name = 'digital_cortex'
-version = '0.0.38'
+version = '0.0.39'
 authors = [
     "Charlie Wardell <charlie@digital-cortex.io>",
     "Chris Esworthy <chris@digital-cortex.io>",
     "Satendra Kumar <satendra.kumar@thirdnormal.com>",
     "Prachi Soni <prachi.soni@thirdnormal.com>",
     "Mohd Sabir <sabir@thirdnormal.com>",
 ]
```

### Comparing `digital_cortex-0.0.38/PKG-INFO` & `digital_cortex-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-cortex
-Version: 0.0.38
+Version: 0.0.39
 Summary: Python Client for Digital Cortex
 Author: Charlie Wardell
 Author-email: charlie@digital-cortex.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

