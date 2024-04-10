# Comparing `tmp/concurrent_tasks-1.7.1.tar.gz` & `tmp/concurrent_tasks-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concurrent_tasks-1.7.1.tar", max compression
+gzip compressed data, was "concurrent_tasks-1.7.2.tar", max compression
```

## Comparing `concurrent_tasks-1.7.1.tar` & `concurrent_tasks-1.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/LICENSE
--rw-r--r--   0        0        0     6078 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/README.md
--rw-r--r--   0        0        0      518 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/__init__.py
--rw-r--r--   0        0        0     1458 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/background.py
--rw-r--r--   0        0        0     3551 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/exception_handler.py
--rw-r--r--   0        0        0     1081 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/periodic.py
--rw-r--r--   0        0        0        0 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/py.typed
--rw-r--r--   0        0        0     3097 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/restartable.py
--rw-r--r--   0        0        0     4208 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/thread_safe_pool.py
--rw-r--r--   0        0        0      228 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/__init__.py
--rw-r--r--   0        0        0     1696 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/aio.py
--rw-r--r--   0        0        0     4655 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/base.py
--rw-r--r--   0        0        0     1638 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/blocking.py
--rw-r--r--   0        0        0      932 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     6852 1970-01-01 00:00:00.000000 concurrent_tasks-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-10 08:22:34.551578 concurrent_tasks-1.7.2/LICENSE
+-rw-r--r--   0        0        0     6078 2024-04-10 08:22:34.551578 concurrent_tasks-1.7.2/README.md
+-rw-r--r--   0        0        0      518 2024-04-10 08:22:34.551578 concurrent_tasks-1.7.2/concurrent_tasks/__init__.py
+-rw-r--r--   0        0        0     1458 2024-04-10 08:22:34.551578 concurrent_tasks-1.7.2/concurrent_tasks/background.py
+-rw-r--r--   0        0        0     3551 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/exception_handler.py
+-rw-r--r--   0        0        0     1087 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/periodic.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/py.typed
+-rw-r--r--   0        0        0     3097 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/restartable.py
+-rw-r--r--   0        0        0     4208 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/thread_safe_pool.py
+-rw-r--r--   0        0        0      228 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/__init__.py
+-rw-r--r--   0        0        0     1696 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/aio.py
+-rw-r--r--   0        0        0     4655 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/base.py
+-rw-r--r--   0        0        0     1638 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/blocking.py
+-rw-r--r--   0        0        0      932 2024-04-10 08:22:34.555578 concurrent_tasks-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6852 1970-01-01 00:00:00.000000 concurrent_tasks-1.7.2/PKG-INFO
```

### Comparing `concurrent_tasks-1.7.1/LICENSE` & `concurrent_tasks-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/README.md` & `concurrent_tasks-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/__init__.py` & `concurrent_tasks-1.7.2/concurrent_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/background.py` & `concurrent_tasks-1.7.2/concurrent_tasks/background.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/exception_handler.py` & `concurrent_tasks-1.7.2/concurrent_tasks/exception_handler.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/periodic.py` & `concurrent_tasks-1.7.2/concurrent_tasks/periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
         super().__init__(self._run, interval, *args, **kwargs)
         self._initial_func = func
 
     async def _run(self, interval: float, *args: P.args, **kwargs: P.kwargs):
         while True:
             start = monotonic()
             await self._initial_func(*args, **kwargs)
-            if remaining := interval - (monotonic() - start):
+            if (remaining := interval - (monotonic() - start)) > 0:
                 await asyncio.sleep(remaining)
```

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/restartable.py` & `concurrent_tasks-1.7.2/concurrent_tasks/restartable.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/thread_safe_pool.py` & `concurrent_tasks-1.7.2/concurrent_tasks/thread_safe_pool.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/aio.py` & `concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/aio.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/base.py` & `concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/base.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/blocking.py` & `concurrent_tasks-1.7.2/concurrent_tasks/threaded_pool/blocking.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.1/pyproject.toml` & `concurrent_tasks-1.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "concurrent_tasks"
-version = "1.7.1"
+version = "1.7.2"
 description = "Tools to run asyncio tasks concurrently."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/asyncio-concurrent-tasks"
 include = ["concurrent_tasks/py.typed"]
 
@@ -12,15 +12,15 @@
 python = ">=3.8"
 typing-extensions = ">=4.10"
 
 [tool.poetry.group.test.dependencies]
 pytest = "==8.1.1"
 pytest-asyncio = "==0.21.1"
 pytest-mock = "==3.14.0"
-ruff = "==0.3.4"
+ruff = "==0.3.5"
 mypy = "==1.9.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `concurrent_tasks-1.7.1/PKG-INFO` & `concurrent_tasks-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concurrent_tasks
-Version: 1.7.1
+Version: 1.7.2
 Summary: Tools to run asyncio tasks concurrently.
 Home-page: https://github.com/gpajot/asyncio-concurrent-tasks
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

