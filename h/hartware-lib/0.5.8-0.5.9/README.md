# Comparing `tmp/hartware_lib-0.5.8.tar.gz` & `tmp/hartware_lib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hartware_lib-0.5.8.tar", max compression
+gzip compressed data, was "hartware_lib-0.5.9.tar", max compression
```

## Comparing `hartware_lib-0.5.8.tar` & `hartware_lib-0.5.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-12-25 16:42:43.686739 hartware_lib-0.5.8/LICENSE
--rw-r--r--   0        0        0       15 2023-12-25 16:42:43.687431 hartware_lib-0.5.8/README.md
--rw-r--r--   0        0        0        0 2023-12-25 16:42:43.688094 hartware_lib-0.5.8/hartware_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-12-25 16:42:43.688386 hartware_lib-0.5.8/hartware_lib/adapters/__init__.py
--rw-r--r--   0        0        0     1093 2024-01-11 21:30:18.536843 hartware_lib-0.5.8/hartware_lib/adapters/async_http.py
--rw-r--r--   0        0        0     3078 2024-01-11 21:30:18.537333 hartware_lib-0.5.8/hartware_lib/adapters/filesystem.py
--rw-r--r--   0        0        0     2387 2024-01-11 21:30:18.537883 hartware_lib-0.5.8/hartware_lib/adapters/hartware.py
--rw-r--r--   0        0        0     8726 2024-01-26 22:20:27.909394 hartware_lib-0.5.8/hartware_lib/adapters/rabbitmq.py
--rw-r--r--   0        0        0      800 2024-01-11 21:30:18.539079 hartware_lib-0.5.8/hartware_lib/adapters/slack.py
--rw-r--r--   0        0        0        0 2023-12-25 16:42:43.689513 hartware_lib-0.5.8/hartware_lib/commands/__init__.py
--rw-r--r--   0        0        0      681 2024-01-11 21:30:18.539533 hartware_lib-0.5.8/hartware_lib/commands/slack.py
--rw-r--r--   0        0        0        0 2024-01-11 21:30:18.539746 hartware_lib-0.5.8/hartware_lib/controllers/__init__.py
--rw-r--r--   0        0        0     4505 2024-01-26 22:20:27.686589 hartware_lib-0.5.8/hartware_lib/controllers/http_rpc.py
--rw-r--r--   0        0        0     5126 2024-01-26 22:20:28.414578 hartware_lib-0.5.8/hartware_lib/controllers/rmq_rpc.py
--rw-r--r--   0        0        0        0 2023-12-25 16:42:43.689763 hartware_lib-0.5.8/hartware_lib/py.typed
--rw-r--r--   0        0        0      297 2024-01-26 22:20:27.938493 hartware_lib-0.5.8/hartware_lib/serializers/__init__.py
--rw-r--r--   0        0        0     1855 2024-01-26 22:20:28.089974 hartware_lib-0.5.8/hartware_lib/serializers/builders.py
--rw-r--r--   0        0        0      895 2024-01-26 22:15:01.581679 hartware_lib-0.5.8/hartware_lib/serializers/dataclasses.py
--rw-r--r--   0        0        0     2455 2024-01-26 21:56:39.120329 hartware_lib-0.5.8/hartware_lib/serializers/main.py
--rw-r--r--   0        0        0     1132 2024-01-26 21:56:35.269565 hartware_lib-0.5.8/hartware_lib/serializers/pandas.py
--rw-r--r--   0        0        0     4832 2024-01-26 12:40:35.150194 hartware_lib-0.5.8/hartware_lib/settings.py
--rw-r--r--   0        0        0      337 2024-01-26 22:15:05.779614 hartware_lib-0.5.8/hartware_lib/types.py
--rw-r--r--   0        0        0        0 2023-12-25 16:42:43.690677 hartware_lib-0.5.8/hartware_lib/utils/__init__.py
--rw-r--r--   0        0        0      124 2024-01-11 21:30:18.542447 hartware_lib-0.5.8/hartware_lib/utils/casing.py
--rw-r--r--   0        0        0      360 2023-12-25 16:42:43.691288 hartware_lib-0.5.8/hartware_lib/utils/datetime.py
--rw-r--r--   0        0        0     1690 2024-01-26 22:23:58.910209 hartware_lib-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 hartware_lib-0.5.8/setup.py
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 hartware_lib-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-12-25 16:42:43.686739 hartware_lib-0.5.9/LICENSE
+-rw-r--r--   0        0        0       15 2023-12-25 16:42:43.687431 hartware_lib-0.5.9/README.md
+-rw-r--r--   0        0        0        0 2023-12-25 16:42:43.688094 hartware_lib-0.5.9/hartware_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-25 16:42:43.688386 hartware_lib-0.5.9/hartware_lib/adapters/__init__.py
+-rw-r--r--   0        0        0     1093 2024-01-11 21:30:18.536843 hartware_lib-0.5.9/hartware_lib/adapters/async_http.py
+-rw-r--r--   0        0        0     3078 2024-01-11 21:30:18.537333 hartware_lib-0.5.9/hartware_lib/adapters/filesystem.py
+-rw-r--r--   0        0        0     2387 2024-01-11 21:30:18.537883 hartware_lib-0.5.9/hartware_lib/adapters/hartware.py
+-rw-r--r--   0        0        0     8726 2024-01-26 23:10:15.122256 hartware_lib-0.5.9/hartware_lib/adapters/rabbitmq.py
+-rw-r--r--   0        0        0      800 2024-01-11 21:30:18.539079 hartware_lib-0.5.9/hartware_lib/adapters/slack.py
+-rw-r--r--   0        0        0        0 2023-12-25 16:42:43.689513 hartware_lib-0.5.9/hartware_lib/commands/__init__.py
+-rw-r--r--   0        0        0      681 2024-01-11 21:30:18.539533 hartware_lib-0.5.9/hartware_lib/commands/slack.py
+-rw-r--r--   0        0        0        0 2024-01-11 21:30:18.539746 hartware_lib-0.5.9/hartware_lib/controllers/__init__.py
+-rw-r--r--   0        0        0     4505 2024-01-26 23:10:14.980404 hartware_lib-0.5.9/hartware_lib/controllers/http_rpc.py
+-rw-r--r--   0        0        0     5126 2024-01-26 23:10:15.415621 hartware_lib-0.5.9/hartware_lib/controllers/rmq_rpc.py
+-rw-r--r--   0        0        0        0 2023-12-25 16:42:43.689763 hartware_lib-0.5.9/hartware_lib/py.typed
+-rw-r--r--   0        0        0      297 2024-01-26 23:10:15.151197 hartware_lib-0.5.9/hartware_lib/serializers/__init__.py
+-rw-r--r--   0        0        0     1855 2024-01-26 23:10:15.289508 hartware_lib-0.5.9/hartware_lib/serializers/builders.py
+-rw-r--r--   0        0        0      895 2024-01-26 22:15:01.581679 hartware_lib-0.5.9/hartware_lib/serializers/dataclasses.py
+-rw-r--r--   0        0        0     2636 2024-01-26 23:04:14.047245 hartware_lib-0.5.9/hartware_lib/serializers/main.py
+-rw-r--r--   0        0        0     1132 2024-01-26 21:56:35.269565 hartware_lib-0.5.9/hartware_lib/serializers/pandas.py
+-rw-r--r--   0        0        0     4832 2024-01-26 12:40:35.150194 hartware_lib-0.5.9/hartware_lib/settings.py
+-rw-r--r--   0        0        0      337 2024-01-26 22:15:05.779614 hartware_lib-0.5.9/hartware_lib/types.py
+-rw-r--r--   0        0        0        0 2023-12-25 16:42:43.690677 hartware_lib-0.5.9/hartware_lib/utils/__init__.py
+-rw-r--r--   0        0        0      124 2024-01-11 21:30:18.542447 hartware_lib-0.5.9/hartware_lib/utils/casing.py
+-rw-r--r--   0        0        0      360 2023-12-25 16:42:43.691288 hartware_lib-0.5.9/hartware_lib/utils/datetime.py
+-rw-r--r--   0        0        0     1690 2024-01-26 23:11:26.215697 hartware_lib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 hartware_lib-0.5.9/setup.py
+-rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 hartware_lib-0.5.9/PKG-INFO
```

### Comparing `hartware_lib-0.5.8/LICENSE` & `hartware_lib-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/adapters/async_http.py` & `hartware_lib-0.5.9/hartware_lib/adapters/async_http.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/adapters/filesystem.py` & `hartware_lib-0.5.9/hartware_lib/adapters/filesystem.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/adapters/hartware.py` & `hartware_lib-0.5.9/hartware_lib/adapters/hartware.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/adapters/rabbitmq.py` & `hartware_lib-0.5.9/hartware_lib/adapters/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/adapters/slack.py` & `hartware_lib-0.5.9/hartware_lib/adapters/slack.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/commands/slack.py` & `hartware_lib-0.5.9/hartware_lib/commands/slack.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/controllers/http_rpc.py` & `hartware_lib-0.5.9/hartware_lib/controllers/http_rpc.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/controllers/rmq_rpc.py` & `hartware_lib-0.5.9/hartware_lib/controllers/rmq_rpc.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/serializers/builders.py` & `hartware_lib-0.5.9/hartware_lib/serializers/builders.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/serializers/dataclasses.py` & `hartware_lib-0.5.9/hartware_lib/serializers/dataclasses.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/serializers/main.py` & `hartware_lib-0.5.9/hartware_lib/serializers/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from datetime import datetime
 from decimal import Decimal
 from functools import partial
+from pathlib import Path
 from typing import Any, Optional, Sequence, Union
 
 from hartware_lib.types import AnyDict, ExtraDeserializer, ExtraSerializer
 
 
 class NoSerializerMatch(Exception):
     pass
@@ -25,14 +26,16 @@
     def default(self, o: Any) -> AnyDict:
         if isinstance(o, datetime):
             return {"_type": o.__class__.__name__, "value": o.isoformat()}
         elif isinstance(o, set):
             return {"_type": o.__class__.__name__, "value": list(o)}
         elif isinstance(o, Decimal):
             return {"_type": o.__class__.__name__, "value": str(o)}
+        elif isinstance(o, Path):
+            return {"_type": "Path", "value": str(o)}
         elif self.extra_serializers:
             for extra_serializer in self.extra_serializers:
                 try:
                     return extra_serializer(o)
                 except NoSerializerMatch:
                     pass
 
@@ -53,20 +56,22 @@
 
 def _global_decoder(
     obj: AnyDict, extra_deserializers: Sequence[ExtraSerializer]
 ) -> Any:
     if obj_type := obj.get("_type"):
         obj_value = obj["value"]
 
-        if obj_type == "set":
-            return set(obj_value)
-        elif obj_type == "datetime":
+        if obj_type == "datetime":
             return datetime.fromisoformat(obj_value)
+        elif obj_type == "set":
+            return set(obj_value)
         elif obj_type == "Decimal":
             return Decimal(obj_value)
+        elif obj_type == "Path":
+            return Path(obj_value)
         elif extra_deserializers:
             for extra_deserializer in extra_deserializers:
                 try:
                     return extra_deserializer(obj)
                 except NoSerializerMatch:
                     pass
```

### Comparing `hartware_lib-0.5.8/hartware_lib/serializers/pandas.py` & `hartware_lib-0.5.9/hartware_lib/serializers/pandas.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/hartware_lib/settings.py` & `hartware_lib-0.5.9/hartware_lib/settings.py`

 * *Files identical despite different names*

### Comparing `hartware_lib-0.5.8/pyproject.toml` & `hartware_lib-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hartware-lib"
-version = "0.5.8"
+version = "0.5.9"
 description = "Core helper lib for Hartware codes."
 authors = ["Laurent Arthur <laurent.arthur75@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://gitlab.com/ludwig778/python-lib"
 repository = "https://gitlab.com/ludwig778/python-lib"
 classifiers = [
```

### Comparing `hartware_lib-0.5.8/setup.py` & `hartware_lib-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'slack': ['slack-sdk>=3.11.2,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['slack_send = hartware_lib.commands.slack:slack_send']}
 
 setup_kwargs = {
     'name': 'hartware-lib',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Core helper lib for Hartware codes.',
     'long_description': '# Hartware Lib\n',
     'author': 'Laurent Arthur',
     'author_email': 'laurent.arthur75@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ludwig778/python-lib',
```

### Comparing `hartware_lib-0.5.8/PKG-INFO` & `hartware_lib-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hartware-lib
-Version: 0.5.8
+Version: 0.5.9
 Summary: Core helper lib for Hartware codes.
 Home-page: https://gitlab.com/ludwig778/python-lib
 License: GPLv3
 Author: Laurent Arthur
 Author-email: laurent.arthur75@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

