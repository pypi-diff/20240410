# Comparing `tmp/xindex-0.6.0.tar.gz` & `tmp/xindex-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xindex-0.6.0.tar", last modified: Wed Apr 10 19:33:20 2024, max compression
+gzip compressed data, was "xindex-0.7.0.tar", last modified: Wed Apr 10 19:53:43 2024, max compression
```

## Comparing `xindex-0.6.0.tar` & `xindex-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      954 2024-04-10 19:33:20.526103 xindex-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1907 2024-04-10 19:32:55.942158 xindex-0.6.0/src/xindex/__init__.py
--rw-r--r--   0        0        0       18 2024-04-10 19:32:55.942158 xindex-0.6.0/src/xindex/__version__.py
--rw-r--r--   0        0        0       68 2024-04-10 19:32:55.942158 xindex-0.6.0/src/xindex/typealiases.py
--rw-r--r--   0        0        0        0 2024-04-10 19:32:55.942158 xindex-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     5394 2024-04-10 19:32:55.942158 xindex-0.6.0/tests/test_xindex.py
--rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2024-04-10 19:53:43.081124 xindex-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1963 2024-04-10 19:53:28.913138 xindex-0.7.0/src/xindex/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 19:53:28.913138 xindex-0.7.0/src/xindex/__version__.py
+-rw-r--r--   0        0        0       68 2024-04-10 19:53:28.913138 xindex-0.7.0/src/xindex/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:53:28.913138 xindex-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     5813 2024-04-10 19:53:28.913138 xindex-0.7.0/tests/test_xindex.py
+-rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.7.0/PKG-INFO
```

### Comparing `xindex-0.6.0/pyproject.toml` & `xindex-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xindex"
-version = "0.6.0"
+version = "0.7.0"
 requires-python = ">=3.10"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `xindex-0.6.0/src/xindex/__init__.py` & `xindex-0.7.0/src/xindex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     data: list[T]
 
     def __init__(self, initlist: t.Optional[t.Iterable[T]] = None, i: int = 0):
         assert i >= 0
         super().__init__(initlist)
         self.i = i
 
+    def __iter__(self):
+        return iter(self.data)
+
     def shift_int(self, i: int):
         shift = self.i
         if 0 <= i < shift:
             raise IndexError(f'list index {i} out of range')
         if shift <= i:
             i -= shift
         return i
```

### Comparing `xindex-0.6.0/tests/test_xindex.py` & `xindex-0.7.0/tests/test_xindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,29 @@
 
 
 @pytest.fixture
 def xindex():
     return XIndex([2, 3, 4, 5], i=2)
 
 
+def test_iter(
+    xlist,
+    xindex,
+):
+    assert list(xlist) == [2, 3, 4, 5]
+    for x in xlist:
+        break
+    assert x == 2
+
+    assert list(xindex) == [2, 3, 4, 5]
+    for x in xindex:
+        break
+    assert x == 2
+
+
 def test_lt(
     xlist,
     xindex,
 ):
     assert xlist < [3, 3, 4, 5]
     assert xindex < [3, 3, 4, 5]
 
@@ -290,7 +305,15 @@
     xlist.pop(1)
     assert xlist == [2, 4]
 
     xindex.pop()
     assert xindex == [2, 3, 4]
     xindex.pop(3)
     assert xindex == [2, 4]
+
+
+def test_enumerate(
+    xlist,
+    xindex,
+):
+    assert list(xlist.enumerate()) == [(0, 2), (1, 3), (2, 4), (3, 5)]
+    assert list(xindex.enumerate()) == [(2, 2), (3, 3), (4, 4), (5, 5)]
```

