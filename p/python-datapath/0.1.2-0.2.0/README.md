# Comparing `tmp/python-datapath-0.1.2.tar.gz` & `tmp/python-datapath-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-datapath-0.1.2.tar", last modified: Thu Dec  7 04:06:41 2023, max compression
+gzip compressed data, was "python-datapath-0.2.0.tar", last modified: Wed Apr 10 04:23:35 2024, max compression
```

## Comparing `python-datapath-0.1.2.tar` & `python-datapath-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 04:06:41.917862 python-datapath-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1049 2023-11-28 22:29:53.000000 python-datapath-0.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      531 2023-12-07 04:06:41.916525 python-datapath-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1662 2023-12-07 03:41:28.000000 python-datapath-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 04:06:41.891943 python-datapath-0.1.2/datapath/
--rw-r--r--   0 root         (0) root         (0)      764 2023-12-03 00:04:46.000000 python-datapath-0.1.2/datapath/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10872 2023-12-07 03:50:03.000000 python-datapath-0.1.2/datapath/_base.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-12-05 04:05:57.000000 python-datapath-0.1.2/datapath/collection.py
--rw-r--r--   0 root         (0) root         (0)     7655 2023-12-07 03:50:26.000000 python-datapath-0.1.2/datapath/folding.py
--rw-r--r--   0 root         (0) root         (0)     5132 2023-12-07 03:48:50.000000 python-datapath-0.1.2/datapath/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 04:06:41.906619 python-datapath-0.1.2/python_datapath.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2023-12-07 04:06:41.000000 python-datapath-0.1.2/python_datapath.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2023-12-07 04:06:41.000000 python-datapath-0.1.2/python_datapath.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-07 04:06:41.000000 python-datapath-0.1.2/python_datapath.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-07 04:06:41.000000 python-datapath-0.1.2/python_datapath.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-12-07 04:06:41.000000 python-datapath-0.1.2/python_datapath.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-07 04:06:41.919164 python-datapath-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      571 2023-12-07 03:52:04.000000 python-datapath-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-07 04:06:41.913148 python-datapath-0.1.2/test/
--rw-r--r--   0 root         (0) root         (0)    10690 2023-12-07 03:39:08.000000 python-datapath-0.1.2/test/test_datapath.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-12-03 05:07:50.000000 python-datapath-0.1.2/test/test_folding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:23:35.123757 python-datapath-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-11-28 22:29:53.000000 python-datapath-0.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-10 04:23:35.119418 python-datapath-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-12-07 03:41:28.000000 python-datapath-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:23:35.067151 python-datapath-0.2.0/datapath/
+-rw-r--r--   0 root         (0) root         (0)      843 2024-04-10 01:28:51.000000 python-datapath-0.2.0/datapath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2024-04-10 03:43:58.000000 python-datapath-0.2.0/datapath/_base.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-12-05 04:05:57.000000 python-datapath-0.2.0/datapath/collection.py
+-rw-r--r--   0 root         (0) root         (0)     7655 2023-12-07 03:50:26.000000 python-datapath-0.2.0/datapath/folding.py
+-rw-r--r--   0 root         (0) root         (0)     4706 2024-04-10 04:17:11.000000 python-datapath-0.2.0/datapath/format.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-12-07 03:48:50.000000 python-datapath-0.2.0/datapath/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:23:35.088510 python-datapath-0.2.0/python_datapath.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-10 04:23:34.000000 python-datapath-0.2.0/python_datapath.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-10 04:23:34.000000 python-datapath-0.2.0/python_datapath.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:23:34.000000 python-datapath-0.2.0/python_datapath.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 04:23:34.000000 python-datapath-0.2.0/python_datapath.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-10 04:23:34.000000 python-datapath-0.2.0/python_datapath.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:23:35.124933 python-datapath-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      571 2024-04-10 03:59:31.000000 python-datapath-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:23:35.109764 python-datapath-0.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)    10820 2024-04-10 03:43:34.000000 python-datapath-0.2.0/test/test_datapath.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-12-03 05:07:50.000000 python-datapath-0.2.0/test/test_folding.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-10 04:17:51.000000 python-datapath-0.2.0/test/test_format.py
```

### Comparing `python-datapath-0.1.2/LICENSE.txt` & `python-datapath-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-datapath-0.1.2/PKG-INFO` & `python-datapath-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-datapath
-Version: 0.1.2
+Version: 0.2.0
 Summary: Functions for working with dotted and square-bracketed paths against a recursive dict/list structure
 Home-page: https://github.com/ashafer01/python-datapath
 Author: Alex Shafer
 Author-email: ashafer@pm.me
 License: MIT
 Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
```

### Comparing `python-datapath-0.1.2/README.md` & `python-datapath-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-datapath-0.1.2/datapath/__init__.py` & `python-datapath-0.2.0/datapath/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,27 @@
 from .collection import collection
 from .folding import (
     unfold_path_dict,
     fold_path_dict,
     complete_collection,
     UnfoldProcessor,
 )
+from .format import format, format_iterate
 from .types import (
     DatapathError,
     ValidationError,
     InvalidIterationError,
     PathLookupError,
 )
 
 __all__ = [
     'get',
+    'format',
     'iterate',
+    'format_iterate',
     'put',
     'delete',
     'discard',
     'is_path',
     'validate_path',
     'split',
     'join',
```

### Comparing `python-datapath-0.1.2/datapath/_base.py` & `python-datapath-0.2.0/datapath/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     """inverse of split() -- combine an iterable of keys/indexes into a dotted-path format
 
     Example:
 
     ```
     >>> join(['a', 'b', 5])
     'a.b[5]'
+
     ```
     """
     path = ''
     for i, part in enumerate(_split_path_from_iterable(split_path, True)):
         path = part.append_path(path)
     return path
 
@@ -183,17 +184,21 @@
         return leaf_obj[leaf_key]
     except LookupError as e:
         if default is NO_DEFAULT:
             raise e from None
         return default
 
 
+class iterate_result(tuple):
+    pass
+
+
 def iterate(obj: Collection,
             path: str,
-            default: Any = NO_DEFAULT) -> Generator[tuple[str, Any], None, None]:
+            default: Any = NO_DEFAULT) -> Generator[iterate_result[str, Any], None, None]:
     """
     yield entries from a collection using an iterable path -- that is, one containing one or more
     sets of empty square brackets (`[]`) or a key with a `*` (`*`/`wild*cards*`/etc.)
 
     * the path part just before an iteration point must refer to a list for `[]` and a dict
       for `*`-keys
     * each yielded value is a tuple (path, value); paths will be resolved with specific indexes
@@ -218,15 +223,15 @@
     split_path = split(path, iterable=True)
     yield from _iterate(obj, split_path, (), default)
 
 
 def _iterate(obj: Collection,
              split_path: SplitPath,
              base_path: SplitPath,
-             default: Any) -> Generator[tuple[str, Any], None, None]:
+             default: Any) -> Generator[iterate_result[str, Any], None, None]:
     """recursive core of iterate()"""
     if not isinstance(obj, _collection_types):
         raise ValidationError(f'{join(base_path + split_path)}: must be list/dict')
 
     # find first iteration point
     iter_index = None
     iter_point = None
@@ -234,15 +239,15 @@
         if part.iterable:
             iter_index = index
             iter_point = part
             break
 
     if iter_index is None:
         # no iteration points found, just need to get()
-        yield join(base_path + split_path), _get(obj, split_path, default)
+        yield iterate_result((join(base_path + split_path), _get(obj, split_path, default)))
         return
 
     # find the collection referred to by the portion of the path before the first iteration point
     before_split_path = split_path[:iter_index]
     try:
         collection = _get(obj, before_split_path)
     except PathLookupError:
@@ -260,15 +265,15 @@
     for key, element in iter_point.iter(collection):
         key_split_path = base_path + before_split_path + (key,)
         if after_split_path:
             # if there is a path after the iteration point, element must be a Collection
             yield from _iterate(element, after_split_path, key_split_path, default)
         else:
             # if there is no path after, then this element is what we're after
-            yield join(key_split_path), element
+            yield iterate_result((join(key_split_path), element))
 
 
 def put(obj: Collection, path: str, value: Any) -> None:
     """set the value at the path
 
     * mutates the leaf collection object
     * if any non-leaf path parts are not found, a LookupError will always be
```

### Comparing `python-datapath-0.1.2/datapath/collection.py` & `python-datapath-0.2.0/datapath/collection.py`

 * *Files identical despite different names*

### Comparing `python-datapath-0.1.2/datapath/folding.py` & `python-datapath-0.2.0/datapath/folding.py`

 * *Files identical despite different names*

### Comparing `python-datapath-0.1.2/datapath/types.py` & `python-datapath-0.2.0/datapath/types.py`

 * *Files identical despite different names*

### Comparing `python-datapath-0.1.2/python_datapath.egg-info/PKG-INFO` & `python-datapath-0.2.0/python_datapath.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-datapath
-Version: 0.1.2
+Version: 0.2.0
 Summary: Functions for working with dotted and square-bracketed paths against a recursive dict/list structure
 Home-page: https://github.com/ashafer01/python-datapath
 Author: Alex Shafer
 Author-email: ashafer@pm.me
 License: MIT
 Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
```

### Comparing `python-datapath-0.1.2/setup.py` & `python-datapath-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 desc = 'Functions for working with dotted and square-bracketed paths against a recursive dict/list structure'
 url = 'https://github.com/ashafer01/python-datapath'
 
 setup(
     name='python-datapath',
-    version='0.1.2',
+    version='0.2.0',
 
     author='Alex Shafer',
     author_email='ashafer@pm.me',
     description=desc,
     long_description=f'{desc}\n\nDocs at {url}',
     long_description_content_type='text/x-rst',
     url=url,
```

### Comparing `python-datapath-0.1.2/test/test_datapath.py` & `python-datapath-0.2.0/test/test_datapath.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import doctest
 import unittest
 
 import datapath
 import datapath._base
 import datapath.folding
 import datapath.types
 
@@ -38,14 +39,19 @@
     '[1'
     'test[1',
     '[1[2]',
     '[,%$^%^!@#$%[1]',
 )
 
 
+def load_tests(loader, tests, ignore):
+    tests.addTests(doctest.DocTestSuite(datapath._base))
+    return tests
+
+
 class TestDatapath(unittest.TestCase):
     def test_validate_path_valid_cases_iterable_false(self):
         for valid_path in valid_paths:
             with self.subTest(msg=f'valid path `{valid_path}`'):
                 try:
                     datapath.validate_path(valid_path, iterable=False)
                 except datapath.ValidationError:
```

### Comparing `python-datapath-0.1.2/test/test_folding.py` & `python-datapath-0.2.0/test/test_folding.py`

 * *Files identical despite different names*

