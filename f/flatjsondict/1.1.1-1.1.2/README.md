# Comparing `tmp/flatjsondict-1.1.1.tar.gz` & `tmp/flatjsondict-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.1.1.tar", max compression
+gzip compressed data, was "flatjsondict-1.1.2.tar", max compression
```

## Comparing `flatjsondict-1.1.1.tar` & `flatjsondict-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-10 04:59:35.497487 flatjsondict-1.1.1/LICENSE
--rw-r--r--   0        0        0     3346 2024-04-10 04:59:35.497487 flatjsondict-1.1.1/README.md
--rw-r--r--   0        0        0       58 2024-04-10 04:59:35.498487 flatjsondict-1.1.1/flatjsondict/__init__.py
--rw-r--r--   0        0        0    18574 2024-04-10 04:59:35.498487 flatjsondict-1.1.1/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2024-04-10 04:59:35.498487 flatjsondict-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 flatjsondict-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3346 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/README.md
+-rw-r--r--   0        0        0       58 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    19090 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 flatjsondict-1.1.2/PKG-INFO
```

### Comparing `flatjsondict-1.1.1/LICENSE` & `flatjsondict-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.1/README.md` & `flatjsondict-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.1/flatjsondict/flatjsondict.py` & `flatjsondict-1.1.2/flatjsondict/flatjsondict.py`

 * *Files 4% similar despite different names*

```diff
@@ -483,20 +483,60 @@
         """Return a list of `FlatJson` labels as path-like keys."""
         return [
             self._keypath_separator.join(map(str, item)) 
             if isinstance(item, list) 
             else item for item in self._listkeys()
         ]
 
-    def to_dict(self) -> dict:
+    def slice(self, *args: tuple) -> Union[None, Self]:
         """
-        Convert `FlatJson` to {(key, subkey,) -> value} dict object.
-        Return a dictionary of `FlatJson` data parent key tuples.
+        Return a slice of `FlatJson`.
+
+        Parameters
+        ----------
+        *args : tuple
+            Provide slice keys.
+
+        Returns
+        -------
+        FlatJson
         """
-        return dict(self.items())
+        keys_intersection = self.keys() & dict.fromkeys(args).keys()
+        return self.__class__(
+                (
+                    (k, self.__getitem__(k))
+                    for k in self.keys()
+                    if k in keys_intersection
+                ),
+                self._keypath_separator,
+                self._keyfill_value
+            )
+
+    def to_dict(self, join_key_tuples: bool = False) -> dict:
+        """
+        Convert `FlatJson` to flat dict object with  parent keys as
+        a tuple {(key, subkey,) -> value} or optionally parent keys
+        as a string path separated with the key separator value
+        {'key/subkey' -> value}.
+        
+        Return a dictionary of `FlatJson` data with flat parent keys.
+
+        Parameters
+        ----------
+        join_key_tuples : bool, default False
+            If ``True``, joins parent keys using key separator value.
+
+        Returns
+        -------
+        dict
+        """
+        if not join_key_tuples:
+            return dict(self.items())
+        else:
+            return dict(zip(self.paths(),self.values()))
 
     def to_series(self) -> dict:
         """
         Convert `FlatJson` to {(key, subkey, '') -> value} dict object.
         Return a dictionary of `FlatJson` data with padded label key tuples.
         """
         from itertools import zip_longest
@@ -511,32 +551,8 @@
         ))
 
     def to_json(self) -> Union[dict, list]:
         """Return nested json-like data from `FlatJson`."""
         if self.original_type in self._ARRAYS:
             return self._as_list()
         else:
-            return self._as_dict()
-
-    def slice(self, *args: tuple) -> Union[None, Self]:
-        """
-        Return a slice of `FlatJson`.
-
-        Parameters
-        ----------
-        *args : tuple
-            Provide slice keys.
-
-        Returns
-        -------
-        FlatJson
-        """
-        keys_intersection = self.keys() & dict.fromkeys(args).keys()
-        return self.__class__(
-                (
-                    (k, self.__getitem__(k))
-                    for k in self.keys()
-                    if k in keys_intersection
-                ),
-                self._keypath_separator,
-                self._keyfill_value
-            )
+            return self._as_dict()
```

### Comparing `flatjsondict-1.1.1/pyproject.toml` & `flatjsondict-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.1.1"
+version = "1.1.2"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.1.1/PKG-INFO` & `flatjsondict-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.1.1
+Version: 1.1.2
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

