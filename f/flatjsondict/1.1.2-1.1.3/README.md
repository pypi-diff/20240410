# Comparing `tmp/flatjsondict-1.1.2.tar.gz` & `tmp/flatjsondict-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.1.2.tar", max compression
+gzip compressed data, was "flatjsondict-1.1.3.tar", max compression
```

## Comparing `flatjsondict-1.1.2.tar` & `flatjsondict-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/LICENSE
--rw-r--r--   0        0        0     3346 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/README.md
--rw-r--r--   0        0        0       58 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/flatjsondict/__init__.py
--rw-r--r--   0        0        0    19090 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2024-04-10 12:46:06.825647 flatjsondict-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 flatjsondict-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3502 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/README.md
+-rw-r--r--   0        0        0       58 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    19267 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2024-04-10 13:14:27.102817 flatjsondict-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 flatjsondict-1.1.3/PKG-INFO
```

### Comparing `flatjsondict-1.1.2/LICENSE` & `flatjsondict-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.1.2/README.md` & `flatjsondict-1.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 
 ## Examples
 Constructing `FlatJson` from a nested dictionary.
 ```python
 >>> import flatjsondict as fj
 >>> d = {'a': 1, 'b': {'c': 3}}
 >>> d_fj = fj.FlatJson(data=d)
->>> d_fj
+>>> d_fj.to_dict()
 {('a',): 1, ('b', 'c'): 3}
 ```
 
 Note that the nested objects are dictionaries hence all label keys are 
 string values.
 
 ```python
 >>> d = {'a': 1, 'b': ['c', 3]}
 >>> d_fj = fj.FlatJson(data=d)
->>> d_fj
+>>> d_fj.to_dict()
 {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 ```
 
 Note that the labels keys for nested lists are integer values.
 
 ```python
 >>> d = {'a': 1, 'b': ['c', 3]}
@@ -59,21 +59,23 @@
 transform deeply nested JSON object data to Pandas `Series`.
 
 Constructing nested json-like data from `FlatJson`-like dictioaries.
 ```python
 >>> import flatjsondict as fj
 >>> d = {('a', ''): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> d_fj = fj.FlatJson(data=d)
+>>> d_fj.to_dict()
+{('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> d_fj.to_json()
 {'a': 1, 'b': ['c', 3]}
 
 >>> d_fj.paths()
 ['a', 'b/0', 'b/1']
-```
-
+>>> d_fj.to_dict(join_key_tuples = True)
+{'a': 1, 'b/0': 'c', 'b/1': 3}
 Constructing `FlatJson` from Pandas `Series.to_dict()`.
 ```python
 >>> import pandas as pd
 >>> import flatjsondict as fj
 >>> d = {('a', ''): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> ds = pd.Series(d)
 >>> ds.to_dict(fj.FlatJson)
@@ -88,12 +90,12 @@
 `FlatJson.to_json()` to return nested JSON-like data.
 
 Slicing `FlatJson` using multiple keys.
 ```python
 >>> import flatjsondict as fj
 >>> d = {'a': 1, 'b': ['c', 3]}
 >>> d_fj = fj.FlatJson(data=d)
->>> d_fj
+>>> d_fj.to_dict()
 {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> d_fj.slice(('a',), ('b', 1)).to_json()
 {'a': 1, 'b': [3]}
 ```
```

### Comparing `flatjsondict-1.1.2/flatjsondict/flatjsondict.py` & `flatjsondict-1.1.3/flatjsondict/flatjsondict.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,23 +50,23 @@
 
     Examples
     --------
     Constructing `FlatJson` from a nested dictionary.
     >>> import flatjsondict as fj
     >>> d = {'a': 1, 'b': {'c': 3}}
     >>> d_fj = fj.FlatJson(data=d)
-    >>> d_fj
+    >>> d_fj.to_dict()
     {('a',): 1, ('b', 'c'): 3}
 
     Note that the nested objects are dictionaries hence all label keys are 
     string values.
 
     >>> d = {'a': 1, 'b': ['c', 3]}
     >>> d_fj = fj.FlatJson(data=d)
-    >>> d_fj
+    >>> d_fj.to_dict()
     {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 
     Note that the labels keys for nested lists are integer values.
 
     >>> d = {'a': 1, 'b': ['c', 3]}
     >>> d_fj = fj.FlatJson(data=d)
     >>> d_fj.to_series()
@@ -78,18 +78,22 @@
     creation of Pandas `Series` objects with MultiIndex index allowing to 
     transform deeply nested JSON object data to Pandas `Series`.
 
     Constructing nested json-like data from `FlatJson`-like dictioaries.
     >>> import flatjsondict as fj
     >>> d = {('a', ''): 1, ('b', 0): 'c', ('b', 1): 3}
     >>> d_fj = fj.FlatJson(data=d)
+    >>> d_fj.to_dict()
+    {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
     >>> d_fj.to_json()
     {'a': 1, 'b': ['c', 3]}
     >>> d_fj.paths()
     ['a', 'b/0', 'b/1']
+    >>> d_fj.to_dict(join_key_tuples = True)
+    {'a': 1, 'b/0': 'c', 'b/1': 3}
 
     Constructing `FlatJson` from Pandas `Series.to_dict()`.
     >>> import pandas as pd
     >>> import flatjsondict as fj
     >>> d = {('a', ''): 1, ('b', 0): 'c', ('b', 1): 3}
     >>> ds = pd.Series(d)
     >>> ds.to_dict(fj.FlatJson)
@@ -103,15 +107,15 @@
     `FlatJson.to_json()` to return nested JSON-like data.
 
     Slicing `FlatJson` using multiple keys.
     ```python
     >>> import flatjsondict as fj
     >>> d = {'a': 1, 'b': ['c', 3]}
     >>> d_fj = fj.FlatJson(data=d)
-    >>> d_fj
+    >>> d_fj.to_dict()
     {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
     >>> d_fj.slice(('a',), ('b', 1)).to_json()
     {'a': 1, 'b': [3]}
     ```
     """
 
     _COERCE = list, set, tuple, dict
```

### Comparing `flatjsondict-1.1.2/pyproject.toml` & `flatjsondict-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.1.2"
+version = "1.1.3"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.1.2/PKG-INFO` & `flatjsondict-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.1.2
+Version: 1.1.3
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -44,25 +44,25 @@
 
 ## Examples
 Constructing `FlatJson` from a nested dictionary.
 ```python
 >>> import flatjsondict as fj
 >>> d = {'a': 1, 'b': {'c': 3}}
 >>> d_fj = fj.FlatJson(data=d)
->>> d_fj
+>>> d_fj.to_dict()
 {('a',): 1, ('b', 'c'): 3}
 ```
 
 Note that the nested objects are dictionaries hence all label keys are 
 string values.
 
 ```python
 >>> d = {'a': 1, 'b': ['c', 3]}
 >>> d_fj = fj.FlatJson(data=d)
->>> d_fj
+>>> d_fj.to_dict()
 {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 ```
 
 Note that the labels keys for nested lists are integer values.
 
 ```python
 >>> d = {'a': 1, 'b': ['c', 3]}
@@ -78,21 +78,23 @@
 transform deeply nested JSON object data to Pandas `Series`.
 
 Constructing nested json-like data from `FlatJson`-like dictioaries.
 ```python
 >>> import flatjsondict as fj
 >>> d = {('a', ''): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> d_fj = fj.FlatJson(data=d)
+>>> d_fj.to_dict()
+{('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> d_fj.to_json()
 {'a': 1, 'b': ['c', 3]}
 
 >>> d_fj.paths()
 ['a', 'b/0', 'b/1']
-```
-
+>>> d_fj.to_dict(join_key_tuples = True)
+{'a': 1, 'b/0': 'c', 'b/1': 3}
 Constructing `FlatJson` from Pandas `Series.to_dict()`.
 ```python
 >>> import pandas as pd
 >>> import flatjsondict as fj
 >>> d = {('a', ''): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> ds = pd.Series(d)
 >>> ds.to_dict(fj.FlatJson)
@@ -107,12 +109,12 @@
 `FlatJson.to_json()` to return nested JSON-like data.
 
 Slicing `FlatJson` using multiple keys.
 ```python
 >>> import flatjsondict as fj
 >>> d = {'a': 1, 'b': ['c', 3]}
 >>> d_fj = fj.FlatJson(data=d)
->>> d_fj
+>>> d_fj.to_dict()
 {('a',): 1, ('b', 0): 'c', ('b', 1): 3}
 >>> d_fj.slice(('a',), ('b', 1)).to_json()
 {'a': 1, 'b': [3]}
 ```
```

