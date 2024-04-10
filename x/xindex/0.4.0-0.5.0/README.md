# Comparing `tmp/xindex-0.4.0.tar.gz` & `tmp/xindex-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xindex-0.4.0.tar", last modified: Wed Apr 10 17:51:47 2024, max compression
+gzip compressed data, was "xindex-0.5.0.tar", last modified: Wed Apr 10 18:50:01 2024, max compression
```

## Comparing `xindex-0.4.0.tar` & `xindex-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      954 2024-04-10 17:51:47.704763 xindex-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1826 2024-04-10 17:51:33.168745 xindex-0.4.0/src/xindex/__init__.py
--rw-r--r--   0        0        0       18 2024-04-10 17:51:33.168745 xindex-0.4.0/src/xindex/__version__.py
--rw-r--r--   0        0        0       68 2024-04-10 17:51:33.168745 xindex-0.4.0/src/xindex/typealiases.py
--rw-r--r--   0        0        0        0 2024-04-10 17:51:33.168745 xindex-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     5394 2024-04-10 17:51:33.168745 xindex-0.4.0/tests/test_xindex.py
--rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2024-04-10 18:50:01.017464 xindex-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1907 2024-04-10 18:49:40.189660 xindex-0.5.0/src/xindex/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 18:49:40.189660 xindex-0.5.0/src/xindex/__version__.py
+-rw-r--r--   0        0        0       68 2024-04-10 18:49:40.189660 xindex-0.5.0/src/xindex/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-10 18:49:40.189660 xindex-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     5394 2024-04-10 18:49:40.189660 xindex-0.5.0/tests/test_xindex.py
+-rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.5.0/PKG-INFO
```

### Comparing `xindex-0.4.0/pyproject.toml` & `xindex-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xindex"
-version = "0.4.0"
+version = "0.5.0"
 requires-python = ">=3.10"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `xindex-0.4.0/src/xindex/__init__.py` & `xindex-0.5.0/src/xindex/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .typealiases import IndexOrSlice
 
 
 T = t.TypeVar('T')
 
 
-class XIndex(UserList, t.Generic[T]):
+class XIndex(UserList[T]):
     data: list[T]
 
     def __init__(self, initlist: t.Optional[t.Iterable[T]] = None, i: int = 0):
         assert i >= 0
         super().__init__(initlist)
         self.i = i
 
@@ -40,15 +40,17 @@
 
     @t.overload
     def __getitem__(self, i: t.SupportsIndex, /) -> T: ...
     @t.overload
     def __getitem__(self, i: slice, /) -> 'XIndex[T]': ...
     def __getitem__(self, i: IndexOrSlice):
         i = self.shift(i)
-        return super().__getitem__(i)
+        if isinstance(i, slice):
+            return XIndex(self.data[i], self.i)
+        return self.data[i]
 
     def __setitem__(self, i, item):
         i = self.shift(i)
         return super().__setitem__(i, item)
 
     def __delitem__(self, i):
         i = self.shift(i)
@@ -66,7 +68,9 @@
         return enumerate(iterable=self.data, start=self.i)
 
 
 if 0:
     xi = XIndex([1])
     ssss = xi[slice(0, 2)]
     eeee = xi[0]
+
+    llll = list(xi)
```

### Comparing `xindex-0.4.0/tests/test_xindex.py` & `xindex-0.5.0/tests/test_xindex.py`

 * *Files identical despite different names*

