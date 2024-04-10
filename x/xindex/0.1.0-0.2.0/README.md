# Comparing `tmp/xindex-0.1.0.tar.gz` & `tmp/xindex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xindex-0.1.0.tar", last modified: Wed Apr 10 17:04:53 2024, max compression
+gzip compressed data, was "xindex-0.2.0.tar", last modified: Wed Apr 10 17:10:51 2024, max compression
```

## Comparing `xindex-0.1.0.tar` & `xindex-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      954 2024-04-10 17:04:53.265048 xindex-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1311 2024-04-10 17:04:37.384988 xindex-0.1.0/src/xindex/__init__.py
--rw-r--r--   0        0        0       18 2024-04-10 17:04:37.384988 xindex-0.1.0/src/xindex/__version__.py
--rw-r--r--   0        0        0        0 2024-04-10 17:04:37.384988 xindex-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5394 2024-04-10 17:04:37.384988 xindex-0.1.0/tests/test_xindex.py
--rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2024-04-10 17:10:51.951829 xindex-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1396 2024-04-10 17:10:37.403854 xindex-0.2.0/src/xindex/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 17:10:37.403854 xindex-0.2.0/src/xindex/__version__.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:10:37.403854 xindex-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5394 2024-04-10 17:10:37.403854 xindex-0.2.0/tests/test_xindex.py
+-rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 xindex-0.2.0/PKG-INFO
```

### Comparing `xindex-0.1.0/pyproject.toml` & `xindex-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xindex"
-version = "0.1.0"
+version = "0.2.0"
 requires-python = ">=3.10"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `xindex-0.1.0/src/xindex/__init__.py` & `xindex-0.2.0/src/xindex/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,7 +48,10 @@
     def insert(self, i, item):
         i = self.shift_int(i)
         return super().insert(i, item)
 
     def pop(self, i=-1):
         i = self.shift_int(i)
         return super().pop(i)
+
+    def enumerate(self):
+        return enumerate(iterable=self.data, start=self.i)
```

### Comparing `xindex-0.1.0/tests/test_xindex.py` & `xindex-0.2.0/tests/test_xindex.py`

 * *Files identical despite different names*

