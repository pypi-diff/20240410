# Comparing `tmp/xindex-0.3.0.tar.gz` & `tmp/xindex-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xindex-0.3.0.tar", last modified: Wed Apr 10 17:25:30 2024, max compression
+gzip compressed data, was "xindex-0.4.0.tar", last modified: Wed Apr 10 17:51:47 2024, max compression
```

## Comparing `xindex-0.3.0.tar` & `xindex-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      954 2024-04-10 17:25:30.497096 xindex-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1410 2024-04-10 17:25:16.569078 xindex-0.3.0/src/xindex/__init__.py
--rw-r--r--   0        0        0       18 2024-04-10 17:25:16.569078 xindex-0.3.0/src/xindex/__version__.py
--rw-r--r--   0        0        0        0 2024-04-10 17:25:16.569078 xindex-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5394 2024-04-10 17:25:16.569078 xindex-0.3.0/tests/test_xindex.py
--rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2024-04-10 17:51:47.704763 xindex-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1826 2024-04-10 17:51:33.168745 xindex-0.4.0/src/xindex/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 17:51:33.168745 xindex-0.4.0/src/xindex/__version__.py
+-rw-r--r--   0        0        0       68 2024-04-10 17:51:33.168745 xindex-0.4.0/src/xindex/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:51:33.168745 xindex-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     5394 2024-04-10 17:51:33.168745 xindex-0.4.0/tests/test_xindex.py
+-rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.4.0/PKG-INFO
```

### Comparing `xindex-0.3.0/pyproject.toml` & `xindex-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xindex"
-version = "0.3.0"
+version = "0.4.0"
 requires-python = ">=3.10"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `xindex-0.3.0/src/xindex/__init__.py` & `xindex-0.4.0/src/xindex/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 from collections import UserList
 import typing as t
 
-
-T = t.TypeVar('T')
+from .typealiases import IndexOrSlice
 
 
-NOTHING = object()
+T = t.TypeVar('T')
 
 
 class XIndex(UserList, t.Generic[T]):
+    data: list[T]
+
     def __init__(self, initlist: t.Optional[t.Iterable[T]] = None, i: int = 0):
         assert i >= 0
         super().__init__(initlist)
         self.i = i
 
     def shift_int(self, i: int):
         shift = self.i
         if 0 <= i < shift:
             raise IndexError(f'list index {i} out of range')
         if shift <= i:
             i -= shift
         return i
 
-    def shift(self, i: t.Union[slice, int]):
+    # @t.overload
+    # def shift(self, i: t.SupportsIndex) -> int: ...
+    # @t.overload
+    # def shift(self, i: slice) -> slice: ...
+    def shift(self, i: IndexOrSlice):
         if isinstance(i, slice):
             i = slice(
                 None if i.start is None else self.shift_int(i.start),
                 None if i.stop is None else self.shift_int(i.stop),
                 i.step,
             )
         else:
-            i = self.shift_int(i)
+            i = self.shift_int(t.cast(int, i))
         return i
 
-    def __getitem__(self, i):
+    @t.overload
+    def __getitem__(self, i: t.SupportsIndex, /) -> T: ...
+    @t.overload
+    def __getitem__(self, i: slice, /) -> 'XIndex[T]': ...
+    def __getitem__(self, i: IndexOrSlice):
         i = self.shift(i)
         return super().__getitem__(i)
 
     def __setitem__(self, i, item):
         i = self.shift(i)
         return super().__setitem__(i, item)
 
@@ -51,7 +60,13 @@
 
     def pop(self, i=-1):
         i = self.shift_int(i)
         return super().pop(i)
 
     def enumerate(self):
         return enumerate(iterable=self.data, start=self.i)
+
+
+if 0:
+    xi = XIndex([1])
+    ssss = xi[slice(0, 2)]
+    eeee = xi[0]
```

### Comparing `xindex-0.3.0/tests/test_xindex.py` & `xindex-0.4.0/tests/test_xindex.py`

 * *Files identical despite different names*

