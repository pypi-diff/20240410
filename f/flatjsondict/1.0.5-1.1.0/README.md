# Comparing `tmp/flatjsondict-1.0.5.tar.gz` & `tmp/flatjsondict-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.0.5.tar", max compression
+gzip compressed data, was "flatjsondict-1.1.0.tar", max compression
```

## Comparing `flatjsondict-1.0.5.tar` & `flatjsondict-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2023-07-01 04:54:47.135752 flatjsondict-1.0.5/LICENSE
--rw-r--r--   0        0        0     3087 2023-07-01 04:54:47.135752 flatjsondict-1.0.5/README.md
--rw-r--r--   0        0        0       58 2023-07-01 04:54:47.135752 flatjsondict-1.0.5/flatjsondict/__init__.py
--rw-r--r--   0        0        0    17414 2023-07-01 04:54:47.136752 flatjsondict-1.0.5/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2023-07-01 04:54:47.136752 flatjsondict-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3346 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/README.md
+-rw-r--r--   0        0        0       58 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    18462 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2024-04-10 03:46:25.556372 flatjsondict-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 flatjsondict-1.1.0/PKG-INFO
```

### Comparing `flatjsondict-1.0.5/LICENSE` & `flatjsondict-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.5/README.md` & `flatjsondict-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,8 +81,19 @@
 
 >>> ds.to_dict(fj.FlatJson).to_json()
 {'a': 1, 'b': ['c', 3]}
 ```
 
 Note that you can pass `FlatJson` to Pandas `Series.to_dict(FlatJson)` 
 to directly derive `FlatJson` from Pandas `Series` data. Then use
-`FlatJson.to_json()` to return nested JSON-like data.
+`FlatJson.to_json()` to return nested JSON-like data.
+
+Slicing `FlatJson` using multiple keys.
+```python
+>>> import flatjsondict as fj
+>>> d = {'a': 1, 'b': ['c', 3]}
+>>> d_fj = fj.FlatJson(data=d)
+>>> d_fj
+{('a',): 1, ('b', 0): 'c', ('b', 1): 3}
+>>> d_fj.slice(('a',), ('b', 1)).to_json()
+{'a': 1, 'b': [3]}
+```
```

### Comparing `flatjsondict-1.0.5/flatjsondict/flatjsondict.py` & `flatjsondict-1.1.0/flatjsondict/flatjsondict.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,25 @@
 
     >>> ds.to_dict(fj.FlatJson).to_json()
     {'a': 1, 'b': ['c', 3]}
 
     Note that you can pass `FlatJson` to Pandas `Series.to_dict(FlatJson)` 
     to directly derive `FlatJson` from Pandas `Series` data. Then use
     `FlatJson.to_json()` to return nested JSON-like data.
+
+    Slicing `FlatJson` using multiple keys.
+    ```python
+    >>> import flatjsondict as fj
+    >>> d = {'a': 1, 'b': ['c', 3]}
+    >>> d_fj = fj.FlatJson(data=d)
+    >>> d_fj
+    {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
+    >>> d_fj.slice(('a',), ('b', 1)).to_json()
+    {'a': 1, 'b': [3]}
+    ```
     """
 
     _COERCE = list, set, tuple, dict
     _ARRAYS = list, set, tuple
 
     # -------------------------------------------------------------------------
     # Constructors
@@ -472,14 +483,21 @@
         """Return a list of `FlatJson` labels as path-like keys."""
         return [
             self._keypath_separator.join(map(str, item)) 
             if isinstance(item, list) 
             else item for item in self._listkeys()
         ]
 
+    def to_dict(self) -> dict:
+        """
+        Convert `FlatJson` to {(key, subkey,) -> value} dict object.
+        Return a dictionary of `FlatJson` data parent key tuples.
+        """
+        return dict(self.items())
+
     def to_series(self) -> dict:
         """
         Convert `FlatJson` to {(key, subkey, '') -> value} dict object.
         Return a dictionary of `FlatJson` data with padded label key tuples.
         """
         from itertools import zip_longest
         return dict(zip(
@@ -494,7 +512,29 @@
 
     def to_json(self) -> Union[dict, list]:
         """Return nested json-like data from `FlatJson`."""
         if self.original_type in self._ARRAYS:
             return self._as_list()
         else:
             return self._as_dict()
+
+    def slice(self, *args) -> Union[None, Self]:
+        """
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
+        """
+        return self.__class__(
+                (
+                    (k, self.__getitem__(k)) 
+                    for k in set(self.keys()).intersection(args)
+                ),
+                self._keypath_separator,
+                self._keyfill_value
+            )
```

### Comparing `flatjsondict-1.0.5/pyproject.toml` & `flatjsondict-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.0.5"
+version = "1.1.0"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.0.5/PKG-INFO` & `flatjsondict-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.0.5
+Version: 1.1.0
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md
 Project-URL: Repository, https://gitlab.com/martins-bruvelis/flatjsondict
 Description-Content-Type: text/markdown
 
 # flatjsondict: efficient JSON-like data transformation tool
 
 ## What is it?
@@ -100,7 +101,18 @@
 >>> ds.to_dict(fj.FlatJson).to_json()
 {'a': 1, 'b': ['c', 3]}
 ```
 
 Note that you can pass `FlatJson` to Pandas `Series.to_dict(FlatJson)` 
 to directly derive `FlatJson` from Pandas `Series` data. Then use
 `FlatJson.to_json()` to return nested JSON-like data.
+
+Slicing `FlatJson` using multiple keys.
+```python
+>>> import flatjsondict as fj
+>>> d = {'a': 1, 'b': ['c', 3]}
+>>> d_fj = fj.FlatJson(data=d)
+>>> d_fj
+{('a',): 1, ('b', 0): 'c', ('b', 1): 3}
+>>> d_fj.slice(('a',), ('b', 1)).to_json()
+{'a': 1, 'b': [3]}
+```
```

