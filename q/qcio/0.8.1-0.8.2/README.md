# Comparing `tmp/qcio-0.8.1.tar.gz` & `tmp/qcio-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.8.1.tar", max compression
+gzip compressed data, was "qcio-0.8.2.tar", max compression
```

## Comparing `qcio-0.8.1.tar` & `qcio-0.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-03-29 23:18:12.256286 qcio-0.8.1/LICENSE
--rw-r--r--   0        0        0     7503 2024-03-29 23:18:12.256286 qcio-0.8.1/README.md
--rw-r--r--   0        0        0     1226 2024-03-29 23:18:12.256286 qcio-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      614 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/__init__.py
--rw-r--r--   0        0        0       89 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/constants.py
--rw-r--r--   0        0        0      748 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/helper_types.py
--rw-r--r--   0        0        0      235 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/__init__.py
--rw-r--r--   0        0        0     8752 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/base_models.py
--rw-r--r--   0        0        0     3034 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/inputs.py
--rw-r--r--   0        0        0     2800 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     9122 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/molecule.py
--rw-r--r--   0        0        0    10301 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/outputs.py
--rw-r--r--   0        0        0     1936 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/models/outputs_base.py
--rw-r--r--   0        0        0        0 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/py.typed
--rw-r--r--   0        0        0     4892 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/qcel.py
--rw-r--r--   0        0        0     1142 2024-03-29 23:18:12.256286 qcio-0.8.1/qcio/utils.py
--rw-r--r--   0        0        0     8308 1970-01-01 00:00:00.000000 qcio-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-10 00:42:54.581444 qcio-0.8.2/LICENSE
+-rw-r--r--   0        0        0     7503 2024-04-10 00:42:54.581444 qcio-0.8.2/README.md
+-rw-r--r--   0        0        0     1226 2024-04-10 00:42:54.581444 qcio-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      614 2024-04-10 00:42:54.581444 qcio-0.8.2/qcio/__init__.py
+-rw-r--r--   0        0        0     1753 2024-04-10 00:42:54.581444 qcio-0.8.2/qcio/constants.py
+-rw-r--r--   0        0        0      748 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/helper_types.py
+-rw-r--r--   0        0        0      235 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/__init__.py
+-rw-r--r--   0        0        0     8752 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3034 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2800 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     9122 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/molecule.py
+-rw-r--r--   0        0        0    10301 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1936 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/py.typed
+-rw-r--r--   0        0        0     4892 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/qcel.py
+-rw-r--r--   0        0        0     1142 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/utils.py
+-rw-r--r--   0        0        0     8308 1970-01-01 00:00:00.000000 qcio-0.8.2/PKG-INFO
```

### Comparing `qcio-0.8.1/LICENSE` & `qcio-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/README.md` & `qcio-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/pyproject.toml` & `qcio-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.8.1"
+version = "0.8.2"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.8.1/qcio/__init__.py` & `qcio-0.8.2/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/helper_types.py` & `qcio-0.8.2/qcio/helper_types.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/models/base_models.py` & `qcio-0.8.2/qcio/models/base_models.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/models/inputs.py` & `qcio-0.8.2/qcio/models/inputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/models/inputs_base.py` & `qcio-0.8.2/qcio/models/inputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/models/molecule.py` & `qcio-0.8.2/qcio/models/molecule.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/models/outputs.py` & `qcio-0.8.2/qcio/models/outputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/models/outputs_base.py` & `qcio-0.8.2/qcio/models/outputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/qcel.py` & `qcio-0.8.2/qcio/qcel.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/qcio/utils.py` & `qcio-0.8.2/qcio/utils.py`

 * *Files identical despite different names*

### Comparing `qcio-0.8.1/PKG-INFO` & `qcio-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.8.1
+Version: 0.8.2
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

