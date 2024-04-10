# Comparing `tmp/slim_helper-2.0.1.tar.gz` & `tmp/slim_helper-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim_helper-2.0.1.tar", last modified: Fri Dec  8 03:35:29 2023, max compression
+gzip compressed data, was "slim_helper-2.0.4.tar", last modified: Thu Dec 21 09:14:53 2023, max compression
```

## Comparing `slim_helper-2.0.1.tar` & `slim_helper-2.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3237 2023-12-08 03:35:18.406072 slim_helper-2.0.1/README.md
--rw-r--r--   0        0        0      635 2023-12-08 03:35:29.874215 slim_helper-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-26 03:55:24.295135 slim_helper-2.0.1/src/slim_helper/__init__.py
--rw-r--r--   0        0        0     1394 2023-12-08 03:13:02.969645 slim_helper-2.0.1/src/slim_helper/common.py
--rw-r--r--   0        0        0     7265 2023-12-08 02:56:50.471431 slim_helper-2.0.1/src/slim_helper/database.py
--rw-r--r--   0        0        0     2087 2023-12-08 03:03:08.716755 slim_helper-2.0.1/src/slim_helper/display.py
--rw-r--r--   0        0        0     5838 2023-12-08 03:34:42.785625 slim_helper-2.0.1/src/slim_helper/io.py
--rw-r--r--   0        0        0      924 2023-12-08 02:34:23.394826 slim_helper-2.0.1/src/slim_helper/process.py
--rw-r--r--   0        0        0      851 2023-12-08 02:35:26.575032 slim_helper-2.0.1/src/slim_helper/security.py
--rw-r--r--   0        0        0     2807 2023-12-08 03:03:36.132852 slim_helper-2.0.1/src/slim_helper/task.py
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 slim_helper-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3237 2023-12-08 03:35:18.000000 slim_helper-2.0.4/README.md
+-rw-r--r--   0        0        0      635 2023-12-21 09:14:53.389654 slim_helper-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-26 03:55:24.000000 slim_helper-2.0.4/src/slim_helper/__init__.py
+-rw-r--r--   0        0        0     1394 2023-12-08 03:13:02.000000 slim_helper-2.0.4/src/slim_helper/common.py
+-rw-r--r--   0        0        0     7265 2023-12-08 02:56:50.000000 slim_helper-2.0.4/src/slim_helper/database.py
+-rw-r--r--   0        0        0     2087 2023-12-08 03:03:08.000000 slim_helper-2.0.4/src/slim_helper/display.py
+-rw-r--r--   0        0        0     5838 2023-12-08 03:34:42.000000 slim_helper-2.0.4/src/slim_helper/io.py
+-rw-r--r--   0        0        0      924 2023-12-08 02:34:23.000000 slim_helper-2.0.4/src/slim_helper/process.py
+-rw-r--r--   0        0        0      851 2023-12-08 02:35:26.000000 slim_helper-2.0.4/src/slim_helper/security.py
+-rw-r--r--   0        0        0     3679 2023-12-21 09:14:14.449440 slim_helper-2.0.4/src/slim_helper/task.py
+-rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 slim_helper-2.0.4/PKG-INFO
```

### Comparing `slim_helper-2.0.1/README.md` & `slim_helper-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/pyproject.toml` & `slim_helper-2.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "slim-helper"
-version = "2.0.1"
+version = "2.0.4"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = []
 requires-python = ">=3.11"
 readme = "README.md"
```

### Comparing `slim_helper-2.0.1/src/slim_helper/common.py` & `slim_helper-2.0.4/src/slim_helper/common.py`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/src/slim_helper/database.py` & `slim_helper-2.0.4/src/slim_helper/database.py`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/src/slim_helper/display.py` & `slim_helper-2.0.4/src/slim_helper/display.py`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/src/slim_helper/io.py` & `slim_helper-2.0.4/src/slim_helper/io.py`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/src/slim_helper/process.py` & `slim_helper-2.0.4/src/slim_helper/process.py`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/src/slim_helper/security.py` & `slim_helper-2.0.4/src/slim_helper/security.py`

 * *Files identical despite different names*

### Comparing `slim_helper-2.0.1/src/slim_helper/task.py` & `slim_helper-2.0.4/src/slim_helper/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,46 +14,67 @@
 
     def __init__(
         self,
         callback: Callable,
         parallel: int = 1,
         max_input: int = 0,
         max_output: int = 0,
+        context_maker: Callable = None,
+        context_cleaner : Callable = None
     ):
         """
         Args:
             callback (Callable): callback function
             parallel (int, optional): parallel number. Defaults to 1.
             max_input (int, optional): input queue capacity. Defaults to 0.
             max_output (int, optional): output queue capacity. Defaults to 0.
+            context_maker ( Callable, optional): get context values, used as the first argument
+            context_cleaner ( Callable, optional): close context
         """
         self.__parallel = parallel
         self.__callback = callback
         self.__input = mp.Queue(maxsize=max_input)
         self.__output = mp.Queue(maxsize=max_output)
         self.__processes: Sequence[mp.Process] = []
+        self.__context_maker = context_maker
+        self.__context_cleaner = context_cleaner
         self.reset()
 
     def reset(self):
         """reset"""
         self.kill()
         self.clear()
         self.__processes = []
         for _ in range(self.__parallel):
             p = mp.Process(target=self.__work, daemon=True)
             self.__processes.append(p)
             p.start()
 
     def __work(self):
+        context_error = None
+        context = None
+        if self.__context_maker:
+            try:
+                context = self.__context_maker()
+            except Exception as e:
+                context_error = e
+        else:
+            context = None
+            
         for arg in iter(self.__input.get, None):
+            if context_error is not None:
+                self.__output.put((arg, context_error))
+                continue
             try:
-                r = self.__callback(*arg)
+                r = self.__callback(context,*arg) if self.__context_maker else self.__callback(*arg)
                 self.__output.put((arg, r))
             except Exception as e:
                 self.__output.put((arg, e))
+        if self.__context_cleaner:
+            self.__context_cleaner(context)
 
     def stop(self):
         """stop processes"""
         for _ in self.__processes:
             self.__input.put(None)
 
     def kill(self):
```

### Comparing `slim_helper-2.0.1/PKG-INFO` & `slim_helper-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-helper
-Version: 2.0.1
+Version: 2.0.4
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: postgres
 Provides-Extra: oracle
 Provides-Extra: all
 Requires-Dist: psycopg>=3.1.14; extra == "postgres"
 Requires-Dist: oracledb>=1.4.2; extra == "oracle"
```

