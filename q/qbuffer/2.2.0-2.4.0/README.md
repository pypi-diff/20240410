# Comparing `tmp/qbuffer-2.2.0.tar.gz` & `tmp/qbuffer-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbuffer-2.2.0.tar", last modified: Fri Mar  8 15:23:43 2024, max compression
+gzip compressed data, was "qbuffer-2.4.0.tar", last modified: Wed Apr 10 14:25:46 2024, max compression
```

## Comparing `qbuffer-2.2.0.tar` & `qbuffer-2.4.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      885 2024-03-08 15:23:43.552617 qbuffer-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1089 2024-03-08 15:23:27.532371 qbuffer-2.2.0/src/qbuffer/__init__.py
--rw-r--r--   0        0        0       18 2024-03-08 15:23:27.532371 qbuffer-2.2.0/src/qbuffer/__version__.py
--rw-r--r--   0        0        0        0 2024-03-08 15:23:27.532371 qbuffer-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0      556 2024-03-08 15:23:27.532371 qbuffer-2.2.0/tests/test_buffer.py
--rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 qbuffer-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      928 2024-04-10 14:25:46.765519 qbuffer-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1091 2024-04-10 14:25:34.497490 qbuffer-2.4.0/src/qbuffer/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 14:25:34.497490 qbuffer-2.4.0/src/qbuffer/__version__.py
+-rw-r--r--   0        0        0      864 2024-04-10 14:25:34.497490 qbuffer-2.4.0/src/qbuffer/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:25:34.497490 qbuffer-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      556 2024-04-10 14:25:34.497490 qbuffer-2.4.0/tests/test_buffer.py
+-rw-r--r--   0        0        0       74 1970-01-01 00:00:00.000000 qbuffer-2.4.0/PKG-INFO
```

### Comparing `qbuffer-2.2.0/pyproject.toml` & `qbuffer-2.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qbuffer"
-version = "2.2.0"
+version = "2.4.0"
 requires-python = ">=3.8"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
@@ -31,14 +31,17 @@
 
 [tool.ruff]
 line-length = 100
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.format]
+quote-style = "single"
+
 [tool.ruff.lint]
 extend-select = [
     "W",
     "I",
     "N",
     "S",
     "PTH",
```

### Comparing `qbuffer-2.2.0/src/qbuffer/__init__.py` & `qbuffer-2.4.0/src/qbuffer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 
 class Qbuffer(t.Generic[T]):
     def __init__(
         self,
         *,
         maxlen: int,
-        callback: t.Callable[[T], None],
-        flush_callback: t.Callable[[], None] = lambda: None,
+        callback: t.Callable[[T], t.Any],
+        flush_callback: t.Callable[[], t.Any] = lambda: None,
     ):
         self.maxlen = maxlen
         self.callback = callback
         self.flush_callback = flush_callback
         self.data: deque[T] = deque()
 
     def append(self, item: T, *, flush=False):
```

### Comparing `qbuffer-2.2.0/tests/test_buffer.py` & `qbuffer-2.4.0/tests/test_buffer.py`

 * *Files identical despite different names*

