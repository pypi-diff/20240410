# Comparing `tmp/flatjsondict-1.1.0.tar.gz` & `tmp/flatjsondict-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.1.0.tar", max compression
+gzip compressed data, was "flatjsondict-1.1.1.tar", max compression
```

## Comparing `flatjsondict-1.1.0.tar` & `flatjsondict-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/LICENSE
--rw-r--r--   0        0        0     3346 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/README.md
--rw-r--r--   0        0        0       58 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/flatjsondict/__init__.py
--rw-r--r--   0        0        0    18462 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 flatjsondict-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-10 04:59:35.497487 flatjsondict-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3346 2024-04-10 04:59:35.497487 flatjsondict-1.1.1/README.md
+-rw-r--r--   0        0        0       58 2024-04-10 04:59:35.498487 flatjsondict-1.1.1/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    18574 2024-04-10 04:59:35.498487 flatjsondict-1.1.1/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2024-04-10 04:59:35.498487 flatjsondict-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 flatjsondict-1.1.1/PKG-INFO
```

### Comparing `flatjsondict-1.1.0/LICENSE` & `flatjsondict-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.0/README.md` & `flatjsondict-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.0/flatjsondict/flatjsondict.py` & `flatjsondict-1.1.1/flatjsondict/flatjsondict.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,16 +472,16 @@
         return [(k, self.__getitem__(k)) for k in self.keys()]
 
     def values(self) -> list:
         """Return a list of `FlatJson` values."""
         return [self.__getitem__(k) for k in self.keys()]
 
     def keys(self) -> list:
-        """Return a list of `FlatJson` labels as tuple keys."""
-        return list(map(tuple, self._listkeys()))
+        """Return a list of `FlatJson` labels as dict keys."""
+        return dict.fromkeys(map(tuple, self._listkeys())).keys()
 
     def paths(self) -> list:
         """Return a list of `FlatJson` labels as path-like keys."""
         return [
             self._keypath_separator.join(map(str, item)) 
             if isinstance(item, list) 
             else item for item in self._listkeys()
@@ -513,28 +513,30 @@
     def to_json(self) -> Union[dict, list]:
         """Return nested json-like data from `FlatJson`."""
         if self.original_type in self._ARRAYS:
             return self._as_list()
         else:
             return self._as_dict()
 
-    def slice(self, *args) -> Union[None, Self]:
+    def slice(self, *args: tuple) -> Union[None, Self]:
         """
         Return a slice of `FlatJson`.
 
         Parameters
         ----------
         *args : tuple
             Provide slice keys.
 
         Returns
         -------
         FlatJson
         """
+        keys_intersection = self.keys() & dict.fromkeys(args).keys()
         return self.__class__(
                 (
-                    (k, self.__getitem__(k)) 
-                    for k in set(self.keys()).intersection(args)
+                    (k, self.__getitem__(k))
+                    for k in self.keys()
+                    if k in keys_intersection
                 ),
                 self._keypath_separator,
                 self._keyfill_value
             )
```

### Comparing `flatjsondict-1.1.0/pyproject.toml` & `flatjsondict-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.1.0"
+version = "1.1.1"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.1.0/PKG-INFO` & `flatjsondict-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.1.0
+Version: 1.1.1
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

