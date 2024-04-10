# Comparing `tmp/xindex-0.2.0.tar.gz` & `tmp/xindex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xindex-0.2.0.tar", last modified: Wed Apr 10 17:10:51 2024, max compression
+gzip compressed data, was "xindex-0.3.0.tar", last modified: Wed Apr 10 17:25:30 2024, max compression
```

## Comparing `xindex-0.2.0.tar` & `xindex-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      954 2024-04-10 17:10:51.951829 xindex-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1396 2024-04-10 17:10:37.403854 xindex-0.2.0/src/xindex/__init__.py
--rw-r--r--   0        0        0       18 2024-04-10 17:10:37.403854 xindex-0.2.0/src/xindex/__version__.py
--rw-r--r--   0        0        0        0 2024-04-10 17:10:37.403854 xindex-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5394 2024-04-10 17:10:37.403854 xindex-0.2.0/tests/test_xindex.py
--rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2024-04-10 17:25:30.497096 xindex-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1410 2024-04-10 17:25:16.569078 xindex-0.3.0/src/xindex/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 17:25:16.569078 xindex-0.3.0/src/xindex/__version__.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:25:16.569078 xindex-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5394 2024-04-10 17:25:16.569078 xindex-0.3.0/tests/test_xindex.py
+-rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.3.0/PKG-INFO
```

### Comparing `xindex-0.2.0/pyproject.toml` & `xindex-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xindex"
-version = "0.2.0"
+version = "0.3.0"
 requires-python = ">=3.10"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `xindex-0.2.0/src/xindex/__init__.py` & `xindex-0.3.0/src/xindex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 T = t.TypeVar('T')
 
 
 NOTHING = object()
 
 
-class XIndex(UserList):
+class XIndex(UserList, t.Generic[T]):
     def __init__(self, initlist: t.Optional[t.Iterable[T]] = None, i: int = 0):
         assert i >= 0
         super().__init__(initlist)
         self.i = i
 
     def shift_int(self, i: int):
         shift = self.i
```

### Comparing `xindex-0.2.0/tests/test_xindex.py` & `xindex-0.3.0/tests/test_xindex.py`

 * *Files identical despite different names*

