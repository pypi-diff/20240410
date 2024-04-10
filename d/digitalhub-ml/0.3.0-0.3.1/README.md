# Comparing `tmp/digitalhub-ml-0.3.0.tar.gz` & `tmp/digitalhub-ml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-ml-0.3.0.tar", last modified: Wed Mar 27 09:37:09 2024, max compression
+gzip compressed data, was "digitalhub-ml-0.3.1.tar", last modified: Wed Apr 10 08:28:41 2024, max compression
```

## Comparing `digitalhub-ml-0.3.0.tar` & `digitalhub-ml-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      548 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       74 2023-11-20 10:00:49.000000 digitalhub-ml-0.3.0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.740580 digitalhub-ml-0.3.0/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-03-25 10:43:29.000000 digitalhub-ml-0.3.0/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.740580 digitalhub-ml-0.3.0/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-03-25 10:43:29.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6837 2024-03-12 16:39:31.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1100 2024-02-01 11:42:03.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      404 2024-02-15 10:15:41.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-03-25 10:43:29.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6019 2024-03-25 10:43:29.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      986 2024-03-25 10:43:29.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      756 2024-03-07 13:44:23.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-03-25 10:43:29.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub-ml-0.3.0/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      548 2024-03-27 09:37:09.000000 digitalhub-ml-0.3.0/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-03-27 09:37:09.000000 digitalhub-ml-0.3.0/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-03-27 09:37:09.000000 digitalhub-ml-0.3.0/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-03-27 09:37:09.000000 digitalhub-ml-0.3.0/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-03-27 09:37:09.000000 digitalhub-ml-0.3.0/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-03-27 09:36:06.000000 digitalhub-ml-0.3.0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-03-27 09:37:09.744580 digitalhub-ml-0.3.0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      548 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       74 2023-11-20 10:00:49.000000 digitalhub-ml-0.3.1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-04-10 08:00:27.000000 digitalhub-ml-0.3.1/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-04-10 08:00:27.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6944 2024-04-10 08:26:04.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1100 2024-02-01 11:42:03.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      404 2024-02-15 10:15:41.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-04-10 08:00:27.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6019 2024-04-10 08:26:04.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      986 2024-04-10 08:00:27.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      756 2024-03-07 13:44:23.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-04-10 08:00:27.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub-ml-0.3.1/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      548 2024-04-10 08:28:41.000000 digitalhub-ml-0.3.1/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-04-10 08:28:41.000000 digitalhub-ml-0.3.1/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-10 08:28:41.000000 digitalhub-ml-0.3.1/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:41.000000 digitalhub-ml-0.3.1/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-04-10 08:28:41.000000 digitalhub-ml-0.3.1/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-09 13:57:43.000000 digitalhub-ml-0.3.1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-10 08:28:41.267863 digitalhub-ml-0.3.1/setup.cfg
```

### Comparing `digitalhub-ml-0.3.0/PKG-INFO` & `digitalhub-ml-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/models/crud.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/models/entity.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/models/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,37 +70,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Model:
         """
-        Save model into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             Flag to indicate update.
 
         Returns
         -------
-        dict
-            Mapping representation of Model from backend.
+        Model
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "models")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "models", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
```

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/models/metadata.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/models/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/crud.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/entity.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/projects/spec.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml/entities/registries.py` & `digitalhub-ml-0.3.1/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub-ml-0.3.1/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub-ml-0.3.0/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub-ml-0.3.1/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-ml-0.3.0/pyproject.toml` & `digitalhub-ml-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-data~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
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

