# Comparing `tmp/fastapi_cruddy_framework-1.4.4.tar.gz` & `tmp/fastapi_cruddy_framework-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.4.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.4.5.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.4.tar` & `fastapi_cruddy_framework-1.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.4/LICENSE
--rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.4/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    41190 2024-04-03 20:42:10.151471 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    31212 2024-04-04 01:35:09.196680 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     7939 2024-04-04 00:54:23.318752 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2252 2024-04-04 01:37:33.723638 fastapi_cruddy_framework-1.4.4/pyproject.toml
--rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.5/LICENSE
+-rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.5/README.md
+-rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    41190 2024-04-03 20:42:10.151471 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    31242 2024-04-10 15:35:08.516897 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-04-10 15:42:15.748054 fastapi_cruddy_framework-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.5/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.4/LICENSE` & `fastapi_cruddy_framework-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/README.md` & `fastapi_cruddy_framework-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/graphql.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .repository import AbstractRepository
 from .adapters import BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter
 from .util import (
     possible_id_types,
     possible_id_values,
     lifecycle_types,
     estimate_simple_example,
+    squash_type,
 )
 
 
 class SchemaDict(TypedDict):
     single: Type[CruddyGenericModel]
     many: Type[CruddyGenericModel]
     create: Type[CruddyGenericModel]
@@ -330,15 +331,15 @@
                     default_example = possible_example
             elif v.default is not None:
                 default_example = v.default
             elif v.default_factory is not None:
                 default_example = v.default_factory()
             if default_example is None:
                 default_example = estimate_simple_example(v.annotation)
-            view_example_dict[k] = default_example
+            view_example_dict[k] = squash_type(default_example)
         view_example_dict["links"] = {}
         for k, v in self._relations.items():
             ex_link = self._single_link(id=str(example_id), relationship=k)
             link_object[k] = (
                 str,
                 Field(schema_extra={"json_schema_extra": {"example": ex_link}}),
             )
```

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,14 +215,26 @@
     return getattr(connection.state, key, default)
 
 
 def set_state(connection: Request | WebSocket, key: str, value: Any) -> None:
     setattr(connection.state, key, value)
 
 
+def squash_type(value: Any):
+    if value is None:
+        return None
+    if isinstance(value, (datetime, date)):
+        return value.isoformat()
+    if isinstance(value, (bool, str, int, float)):
+        return value
+    if isinstance(value, (dict, list)):
+        return to_json_object(value)
+    return f"{value}"
+
+
 def estimate_example_for_type(type_annotation: type[Any] | None):
     if type_annotation is None or not inspect.isclass(type_annotation):
         return None
     if issubclass(type_annotation, UUID):
         return f"{uuid7()}"
     if issubclass(type_annotation, bool):
         return True
```

### Comparing `fastapi_cruddy_framework-1.4.4/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.4.5/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.4/pyproject.toml` & `fastapi_cruddy_framework-1.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.4"
+version = "1.4.5"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-1.4.4/PKG-INFO` & `fastapi_cruddy_framework-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.4
+Version: 1.4.5
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.4 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.5 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

