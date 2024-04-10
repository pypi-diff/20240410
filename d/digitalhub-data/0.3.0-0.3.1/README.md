# Comparing `tmp/digitalhub-data-0.3.0.tar.gz` & `tmp/digitalhub-data-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-data-0.3.0.tar", last modified: Wed Mar 27 09:38:01 2024, max compression
+gzip compressed data, was "digitalhub-data-0.3.1.tar", last modified: Wed Apr 10 08:28:35 2024, max compression
```

## Comparing `digitalhub-data-0.3.0.tar` & `digitalhub-data-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       81 2023-11-20 10:01:24.000000 digitalhub-data-0.3.0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.412671 digitalhub-data-0.3.0/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-03-25 10:43:29.000000 digitalhub-data-0.3.0/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.412671 digitalhub-data-0.3.0/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub-data-0.3.0/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.412671 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3446 2024-03-25 10:43:29.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-03-25 10:43:29.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.412671 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6405 2024-03-12 14:22:03.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1464 2024-03-15 12:04:30.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1344 2024-03-15 13:53:09.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub-data-0.3.0/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-03-25 10:43:29.000000 digitalhub-data-0.3.0/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6167 2024-03-25 10:43:29.000000 digitalhub-data-0.3.0/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub-data-0.3.0/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      816 2024-03-07 13:44:22.000000 digitalhub-data-0.3.0/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub-data-0.3.0/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub-data-0.3.0/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub-data-0.3.0/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub-data-0.3.0/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub-data-0.3.0/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub-data-0.3.0/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-03-27 09:38:01.000000 digitalhub-data-0.3.0/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1260 2024-03-27 09:38:01.000000 digitalhub-data-0.3.0/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-03-27 09:38:01.000000 digitalhub-data-0.3.0/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-03-27 09:38:01.000000 digitalhub-data-0.3.0/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-03-27 09:38:01.000000 digitalhub-data-0.3.0/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1052 2024-03-27 09:36:06.000000 digitalhub-data-0.3.0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-03-27 09:38:01.416671 digitalhub-data-0.3.0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       81 2023-11-20 10:01:24.000000 digitalhub-data-0.3.1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.147824 digitalhub-data-0.3.1/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.147824 digitalhub-data-0.3.1/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub-data-0.3.1/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.147824 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3446 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6512 2024-04-10 08:26:04.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1464 2024-03-15 12:04:30.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6167 2024-04-10 08:26:04.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      816 2024-03-07 13:44:22.000000 digitalhub-data-0.3.1/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub-data-0.3.1/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub-data-0.3.1/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1052 2024-04-09 13:57:43.000000 digitalhub-data-0.3.1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/setup.cfg
```

### Comparing `digitalhub-data-0.3.0/PKG-INFO` & `digitalhub-data-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
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

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/builder.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/crud.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,37 +72,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Dataitem:
         """
-        Save dataitem into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         uuid : str
             Specify uuid for the dataitem to update
 
         Returns
         -------
-        dict
-            Mapping representation of Dataitem from backend.
+        Dataitem
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "dataitems")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "dataitems", self.id)
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

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/spec.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Dataitem specification module.
 """
 from __future__ import annotations
 
 from digitalhub_core.entities._base.spec import Spec, SpecParams
+from digitalhub_data.entities.dataitems.models import TableSchema
 from pydantic import Field
 
 
 class DataitemSpec(Spec):
     """
     Dataitem specifications.
     """
@@ -41,28 +42,28 @@
 
 
 class DataitemSpecTable(DataitemSpec):
     """
     Dataitem table specifications.
     """
 
-    def __init__(self, path: str, schema: str | None = None) -> None:
+    def __init__(self, path: str, schema: dict | None = None) -> None:
         """
         Constructor.
         """
         super().__init__(path)
         self.schema = schema
 
 
 class DataitemParamsTable(DataitemParams):
     """
     Dataitem table parameters.
     """
 
-    schema_: dict = Field(default=None, alias="schema")
+    schema_: TableSchema = Field(default=None, alias="schema")
     """The schema of the dataitem in table schema format."""
 
 
 class DataitemSpecIceberg(DataitemSpec):
     """
     Dataitem iceberg specifications.
     """
```

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/dataitems/status.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/projects/crud.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/projects/entity.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/projects/spec.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/entities/registries.py` & `digitalhub-data-0.3.1/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data/utils/data_utils.py` & `digitalhub-data-0.3.1/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.0/digitalhub_data.egg-info/PKG-INFO` & `digitalhub-data-0.3.1/digitalhub_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
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

### Comparing `digitalhub-data-0.3.0/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub-data-0.3.1/digitalhub_data.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 digitalhub_data.egg-info/top_level.txt
 digitalhub_data/entities/__init__.py
 digitalhub_data/entities/registries.py
 digitalhub_data/entities/dataitems/__init__.py
 digitalhub_data/entities/dataitems/builder.py
 digitalhub_data/entities/dataitems/crud.py
 digitalhub_data/entities/dataitems/metadata.py
+digitalhub_data/entities/dataitems/models.py
 digitalhub_data/entities/dataitems/spec.py
 digitalhub_data/entities/dataitems/status.py
 digitalhub_data/entities/dataitems/entity/__init__.py
 digitalhub_data/entities/dataitems/entity/_base.py
 digitalhub_data/entities/dataitems/entity/dataitem.py
 digitalhub_data/entities/dataitems/entity/iceberg.py
 digitalhub_data/entities/dataitems/entity/table.py
```

### Comparing `digitalhub-data-0.3.0/pyproject.toml` & `digitalhub-data-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
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
     "digitalhub-core~=0.3",
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

