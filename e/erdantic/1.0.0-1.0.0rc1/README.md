# Comparing `tmp/erdantic-1.0.0.tar.gz` & `tmp/erdantic-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdantic-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "erdantic-1.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `erdantic-1.0.0.tar` & `erdantic-1.0.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4154 2024-04-10 02:10:10.934654 erdantic-1.0.0/README.md
--rw-r--r--   0        0        0      426 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/__init__.py
--rw-r--r--   0        0        0       66 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/__main__.py
--rw-r--r--   0        0        0      112 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/_logging.py
--rw-r--r--   0        0        0     2656 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/_repr_utils.py
--rw-r--r--   0        0        0       80 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/_version.py
--rw-r--r--   0        0        0     7502 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/cli.py
--rw-r--r--   0        0        0     8420 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/convenience.py
--rw-r--r--   0        0        0    28058 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/core.py
--rw-r--r--   0        0        0      189 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/examples/__init__.py
--rw-r--r--   0        0        0     2302 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/examples/attrs.py
--rw-r--r--   0        0        0     2330 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/examples/dataclasses.py
--rw-r--r--   0        0        0     2251 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/examples/pydantic.py
--rw-r--r--   0        0        0     2307 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/examples/pydantic_v1.py
--rw-r--r--   0        0        0     5000 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/exceptions.py
--rw-r--r--   0        0        0     3446 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/plugins/__init__.py
--rw-r--r--   0        0        0     2184 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/plugins/attrs.py
--rw-r--r--   0        0        0     3847 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/plugins/dataclasses.py
--rw-r--r--   0        0        0     4797 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/plugins/pydantic.py
--rw-r--r--   0        0        0        0 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/py.typed
--rw-r--r--   0        0        0     3526 2024-04-10 02:10:10.942654 erdantic-1.0.0/erdantic/typing_utils.py
--rw-r--r--   0        0        0     2120 2024-04-10 02:10:10.942654 erdantic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5572 1970-01-01 00:00:00.000000 erdantic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4154 2024-03-31 00:41:27.886743 erdantic-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      426 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/__init__.py
+-rw-r--r--   0        0        0       66 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/__main__.py
+-rw-r--r--   0        0        0      112 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_logging.py
+-rw-r--r--   0        0        0     2656 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_repr_utils.py
+-rw-r--r--   0        0        0       80 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_version.py
+-rw-r--r--   0        0        0     7502 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/cli.py
+-rw-r--r--   0        0        0     8420 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/convenience.py
+-rw-r--r--   0        0        0    28058 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/core.py
+-rw-r--r--   0        0        0      189 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/__init__.py
+-rw-r--r--   0        0        0     2302 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/attrs.py
+-rw-r--r--   0        0        0     2330 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/dataclasses.py
+-rw-r--r--   0        0        0     2251 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/pydantic.py
+-rw-r--r--   0        0        0     2307 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/pydantic_v1.py
+-rw-r--r--   0        0        0     5000 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/exceptions.py
+-rw-r--r--   0        0        0     3446 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/__init__.py
+-rw-r--r--   0        0        0     2184 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/attrs.py
+-rw-r--r--   0        0        0     3847 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/dataclasses.py
+-rw-r--r--   0        0        0     4797 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/pydantic.py
+-rw-r--r--   0        0        0        0 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/py.typed
+-rw-r--r--   0        0        0     3526 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/typing_utils.py
+-rw-r--r--   0        0        0     2123 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 erdantic-1.0.0rc1/PKG-INFO
```

### Comparing `erdantic-1.0.0/README.md` & `erdantic-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/_repr_utils.py` & `erdantic-1.0.0rc1/erdantic/_repr_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/cli.py` & `erdantic-1.0.0rc1/erdantic/cli.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/convenience.py` & `erdantic-1.0.0rc1/erdantic/convenience.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/core.py` & `erdantic-1.0.0rc1/erdantic/core.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/examples/attrs.py` & `erdantic-1.0.0rc1/erdantic/examples/attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/examples/dataclasses.py` & `erdantic-1.0.0rc1/erdantic/examples/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/examples/pydantic.py` & `erdantic-1.0.0rc1/erdantic/examples/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/examples/pydantic_v1.py` & `erdantic-1.0.0rc1/erdantic/examples/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/exceptions.py` & `erdantic-1.0.0rc1/erdantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/plugins/__init__.py` & `erdantic-1.0.0rc1/erdantic/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/plugins/attrs.py` & `erdantic-1.0.0rc1/erdantic/plugins/attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/plugins/dataclasses.py` & `erdantic-1.0.0rc1/erdantic/plugins/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/plugins/pydantic.py` & `erdantic-1.0.0rc1/erdantic/plugins/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/erdantic/typing_utils.py` & `erdantic-1.0.0rc1/erdantic/typing_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0/pyproject.toml` & `erdantic-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "erdantic"
-version = "1.0.0"
+version = "1.0.0rc1"
 description = "Entity relationship diagrams for Python data model classes like Pydantic."
 readme = "README.md"
 authors = [{ name = "DrivenData", email = "info@drivendata.org" }, { name = "Jay Qi" }]
 license = { text = "MIT License" }
 keywords = ["erd", "entity relationship diagram", "dataclasses", "pydantic", "attrs"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `erdantic-1.0.0/PKG-INFO` & `erdantic-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdantic
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Entity relationship diagrams for Python data model classes like Pydantic.
 Keywords: erd,entity relationship diagram,dataclasses,pydantic,attrs
 Author: Jay Qi
 Author-email: DrivenData <info@drivendata.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
```

