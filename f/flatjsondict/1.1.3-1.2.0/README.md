# Comparing `tmp/flatjsondict-1.1.3.tar.gz` & `tmp/flatjsondict-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.1.3.tar", max compression
+gzip compressed data, was "flatjsondict-1.2.0.tar", max compression
```

## Comparing `flatjsondict-1.1.3.tar` & `flatjsondict-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/LICENSE
--rw-r--r--   0        0        0     3502 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/README.md
--rw-r--r--   0        0        0       58 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/flatjsondict/__init__.py
--rw-r--r--   0        0        0    19267 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 flatjsondict-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-10 17:07:45.823115 flatjsondict-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3502 2024-04-10 17:07:45.823115 flatjsondict-1.2.0/README.md
+-rw-r--r--   0        0        0       58 2024-04-10 17:07:45.824115 flatjsondict-1.2.0/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    19558 2024-04-10 17:07:45.824115 flatjsondict-1.2.0/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2024-04-10 17:07:45.824115 flatjsondict-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 flatjsondict-1.2.0/PKG-INFO
```

### Comparing `flatjsondict-1.1.3/LICENSE` & `flatjsondict-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.3/README.md` & `flatjsondict-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.3/flatjsondict/flatjsondict.py` & `flatjsondict-1.2.0/flatjsondict/flatjsondict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from collections.abc import MutableMapping
 from typing import (
     Optional, Union, Generator
 )
-from typing import TypeVar
+from typing import TypeVar, Type, Iterable
 try:
     from typing import Self
 except ImportError:
     from typing import TypeVar
     Self = TypeVar("Self", bound="FlatJson")
 from itertools import zip_longest
 
@@ -511,15 +511,15 @@
                     for k in self.keys()
                     if k in keys_intersection
                 ),
                 self._keypath_separator,
                 self._keyfill_value
             )
 
-    def to_dict(self, join_key_tuples: bool = False) -> dict:
+    def to_dict(self, join_key_tuples: bool = False, into: Iterable = dict) -> dict:
         """
         Convert `FlatJson` to flat dict object with  parent keys as
         a tuple {(key, subkey,) -> value} or optionally parent keys
         as a string path separated with the key separator value
         {'key/subkey' -> value}.
         
         Return a dictionary of `FlatJson` data with flat parent keys.
@@ -534,29 +534,37 @@
         dict
         """
         if not join_key_tuples:
             return dict(self.items())
         else:
             return dict(zip(self.paths(),self.values()))
 
-    def to_series(self) -> dict:
+    def to_series(self, into: Type[Iterable] = dict) -> Iterable:
         """
-        Convert `FlatJson` to {(key, subkey, '') -> value} dict object.
-        Return a dictionary of `FlatJson` data with padded label key tuples.
+        Convert `FlatJson` to {(key, subkey, '') -> value} iterable object.
+        Return an iterable object (default dictionary) of `FlatJson` data 
+        with padded label key tuples.
+
+        into : Type[Iterable], default dict
+            Iterable type to convert to the returned iterable object.
+
+        Returns
+        -------
+        Iterable
         """
         from itertools import zip_longest
-        return dict(zip(
+        return into(dict(zip(
             zip_longest(
                 *zip_longest(
                     *map(tuple, self._listkeys()),
                     fillvalue = self._keyfill_value
                 )
             ),
             self.values()
-        ))
+        )).items())
 
     def to_json(self) -> Union[dict, list]:
         """Return nested json-like data from `FlatJson`."""
         if self.original_type in self._ARRAYS:
             return self._as_list()
         else:
             return self._as_dict()
```

### Comparing `flatjsondict-1.1.3/pyproject.toml` & `flatjsondict-1.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.1.3"
+version = "1.2.0"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.1.3/PKG-INFO` & `flatjsondict-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.1.3
+Version: 1.2.0
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

