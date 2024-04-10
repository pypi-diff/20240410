# Comparing `tmp/classic-operations-0.2.0.tar.gz` & `tmp/classic-operations-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classic-operations-0.2.0.tar", last modified: Thu Jan 25 07:17:45 2024, max compression
+gzip compressed data, was "classic-operations-0.2.1.tar", last modified: Wed Apr 10 12:29:03 2024, max compression
```

## Comparing `classic-operations-0.2.0.tar` & `classic-operations-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-01-25 07:17:45.697875 classic-operations-0.2.0/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     1071 2023-12-11 13:09:36.000000 classic-operations-0.2.0/LICENSE
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11897 2024-01-25 07:17:45.691865 classic-operations-0.2.0/PKG-INFO
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11059 2024-01-23 11:52:49.000000 classic-operations-0.2.0/README.md
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      110 2023-12-11 13:09:36.000000 classic-operations-0.2.0/pyproject.toml
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      869 2024-01-25 07:17:45.705813 classic-operations-0.2.0/setup.cfg
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)       38 2023-12-11 13:09:36.000000 classic-operations-0.2.0/setup.py
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-01-25 07:17:45.178005 classic-operations-0.2.0/sources/
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-01-25 07:17:45.171205 classic-operations-0.2.0/sources/classic/
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-01-25 07:17:45.417003 classic-operations-0.2.0/sources/classic/operations/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)       66 2024-01-23 11:52:49.000000 classic-operations-0.2.0/sources/classic/operations/__init__.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      490 2024-01-23 11:52:49.000000 classic-operations-0.2.0/sources/classic/operations/callbacks.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      814 2024-01-25 07:15:19.000000 classic-operations-0.2.0/sources/classic/operations/decorator.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     9233 2024-01-23 11:52:49.000000 classic-operations-0.2.0/sources/classic/operations/operation.py
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-01-25 07:17:45.676071 classic-operations-0.2.0/sources/classic_operations.egg-info/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11897 2024-01-25 07:17:44.000000 classic-operations-0.2.0/sources/classic_operations.egg-info/PKG-INFO
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      507 2024-01-25 07:17:44.000000 classic-operations-0.2.0/sources/classic_operations.egg-info/SOURCES.txt
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)        1 2024-01-25 07:17:44.000000 classic-operations-0.2.0/sources/classic_operations.egg-info/dependency_links.txt
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)       85 2024-01-25 07:17:44.000000 classic-operations-0.2.0/sources/classic_operations.egg-info/requires.txt
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)        8 2024-01-25 07:17:44.000000 classic-operations-0.2.0/sources/classic_operations.egg-info/top_level.txt
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-01-25 07:17:45.637633 classic-operations-0.2.0/tests/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      777 2024-01-23 11:52:49.000000 classic-operations-0.2.0/tests/test_decorator.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11843 2024-01-23 11:52:49.000000 classic-operations-0.2.0/tests/test_operation.py
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 12:29:03.929991 classic-operations-0.2.1/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     1071 2023-12-11 13:09:36.000000 classic-operations-0.2.1/LICENSE
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11897 2024-04-10 12:29:03.927992 classic-operations-0.2.1/PKG-INFO
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11059 2024-01-23 11:52:49.000000 classic-operations-0.2.1/README.md
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      110 2023-12-11 13:09:36.000000 classic-operations-0.2.1/pyproject.toml
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      869 2024-04-10 12:29:03.935099 classic-operations-0.2.1/setup.cfg
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)       38 2023-12-11 13:09:36.000000 classic-operations-0.2.1/setup.py
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 12:29:03.670842 classic-operations-0.2.1/sources/
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 12:29:03.668763 classic-operations-0.2.1/sources/classic/
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 12:29:03.788380 classic-operations-0.2.1/sources/classic/operations/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)       66 2024-01-23 11:52:49.000000 classic-operations-0.2.1/sources/classic/operations/__init__.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      490 2024-01-23 11:52:49.000000 classic-operations-0.2.1/sources/classic/operations/callbacks.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      840 2024-04-10 12:28:45.000000 classic-operations-0.2.1/sources/classic/operations/decorator.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     9233 2024-01-23 11:52:49.000000 classic-operations-0.2.1/sources/classic/operations/operation.py
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 12:29:03.917856 classic-operations-0.2.1/sources/classic_operations.egg-info/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11897 2024-04-10 12:29:03.000000 classic-operations-0.2.1/sources/classic_operations.egg-info/PKG-INFO
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      507 2024-04-10 12:29:03.000000 classic-operations-0.2.1/sources/classic_operations.egg-info/SOURCES.txt
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)        1 2024-04-10 12:29:03.000000 classic-operations-0.2.1/sources/classic_operations.egg-info/dependency_links.txt
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)       85 2024-04-10 12:29:03.000000 classic-operations-0.2.1/sources/classic_operations.egg-info/requires.txt
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)        8 2024-04-10 12:29:03.000000 classic-operations-0.2.1/sources/classic_operations.egg-info/top_level.txt
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 12:29:03.897574 classic-operations-0.2.1/tests/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      777 2024-01-23 11:52:49.000000 classic-operations-0.2.1/tests/test_decorator.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    11843 2024-01-23 11:52:49.000000 classic-operations-0.2.1/tests/test_operation.py
```

### Comparing `classic-operations-0.2.0/LICENSE` & `classic-operations-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `classic-operations-0.2.0/PKG-INFO` & `classic-operations-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classic-operations
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides primitives for transactional application logic
 Home-page: https://github.com/variasov/classic-operations
 Author: Sergei Variasov
 Author-email: variasov@gmail.com
 Project-URL: Bug Tracker, https://github.com/variasov/classic-operations/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `classic-operations-0.2.0/README.md` & `classic-operations-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `classic-operations-0.2.0/setup.cfg` & `classic-operations-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = classic-operations
-version = 0.2.0
+version = 0.2.1
 description = Provides primitives for transactional application logic
 author = Sergei Variasov
 author_email = variasov@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/variasov/classic-operations
 project_urls =
```

### Comparing `classic-operations-0.2.0/sources/classic/operations/decorator.py` & `classic-operations-0.2.1/sources/classic/operations/decorator.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from classic.components import add_extra_annotation, doublewrap
 
 from .operation import Operation
 
 
 @doublewrap
-def operation(method, prop: str = 'operation_'):
+def operation(method, prop: str = 'operation_', type_: Operation = Operation):
     """Сахар для облегчения применения операций.
     По сути просто оборачивает функцию в блок with c указанным полем из self.
 
     Если установлена библиотека classic.components, то добавляет операцию в
     дополнительные аннотации.
     """
 
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         with getattr(self, prop):
             result = method(self, *args, **kwargs)
 
         return result
 
-    return add_extra_annotation(wrapper, prop, Operation)
+    return add_extra_annotation(wrapper, prop, type_)
```

### Comparing `classic-operations-0.2.0/sources/classic/operations/operation.py` & `classic-operations-0.2.1/sources/classic/operations/operation.py`

 * *Files identical despite different names*

### Comparing `classic-operations-0.2.0/sources/classic_operations.egg-info/PKG-INFO` & `classic-operations-0.2.1/sources/classic_operations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classic-operations
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides primitives for transactional application logic
 Home-page: https://github.com/variasov/classic-operations
 Author: Sergei Variasov
 Author-email: variasov@gmail.com
 Project-URL: Bug Tracker, https://github.com/variasov/classic-operations/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `classic-operations-0.2.0/tests/test_decorator.py` & `classic-operations-0.2.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `classic-operations-0.2.0/tests/test_operation.py` & `classic-operations-0.2.1/tests/test_operation.py`

 * *Files identical despite different names*

