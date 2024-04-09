# Comparing `tmp/k2eg-0.2.6.tar.gz` & `tmp/k2eg-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k2eg-0.2.6.tar", last modified: Thu Apr  4 23:40:31 2024, max compression
+gzip compressed data, was "k2eg-0.2.7.tar", last modified: Tue Apr  9 23:44:18 2024, max compression
```

## Comparing `k2eg-0.2.6.tar` & `k2eg-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 23:40:31.723717 k2eg-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 23:40:07.000000 k2eg-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.719717 k2eg-0.2.6/k2eg/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/k2eg/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/put.py
--rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/dml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/k2eg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 23:40:16.000000 k2eg-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:40:31.723717 k2eg-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 23:40:07.000000 k2eg-0.2.6/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-04 23:40:07.000000 k2eg-0.2.6/tests/test_dml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:18.314978 k2eg-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 23:44:18.314978 k2eg-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-09 23:43:58.000000 k2eg-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:18.310979 k2eg-0.2.7/k2eg/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:18.310979 k2eg-0.2.7/k2eg/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/cli/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/cli/put.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-04-09 23:43:58.000000 k2eg-0.2.7/k2eg/dml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:18.310979 k2eg-0.2.7/k2eg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 23:44:18.000000 k2eg-0.2.7/k2eg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 23:44:18.000000 k2eg-0.2.7/k2eg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:18.000000 k2eg-0.2.7/k2eg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 23:44:18.000000 k2eg-0.2.7/k2eg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 23:44:18.000000 k2eg-0.2.7/k2eg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 23:44:18.000000 k2eg-0.2.7/k2eg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 23:44:02.000000 k2eg-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:44:18.314978 k2eg-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:18.310979 k2eg-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 23:43:58.000000 k2eg-0.2.7/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-09 23:43:58.000000 k2eg-0.2.7/tests/test_dml.py
```

### Comparing `k2eg-0.2.6/PKG-INFO` & `k2eg-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2eg
-Version: 0.2.6
+Version: 0.2.7
 Summary: A k2eg library
 Author-email: Claudio Bisegni <bisegni@slac.stanford.edu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `k2eg-0.2.6/README.md` & `k2eg-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.6/k2eg/broker.py` & `k2eg-0.2.7/k2eg/broker.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.6/k2eg/cli/__main__.py` & `k2eg-0.2.7/k2eg/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.6/k2eg/cli/get.py` & `k2eg-0.2.7/k2eg/cli/get.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.6/k2eg/cli/monitor.py` & `k2eg-0.2.7/k2eg/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.6/k2eg/cli/put.py` & `k2eg-0.2.7/k2eg/cli/put.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.6/k2eg/dml.py` & `k2eg-0.2.7/k2eg/dml.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,23 @@
         self.error = error
 
 class dml:
     """K2EG client"""
     def __init__(
             self, 
             environment_id: str, 
-            app_name: str):
+            app_name: str,
+            group_name: str = None):
         if app_name is None:
             raise ValueError(
                 "The app name is mandatory"
             )
         self.__broker = None
         self.__thread = None
-        self.__broker = Broker(environment_id, app_name)
+        self.__broker = Broker(environment_id, app_name, group_name)
         self.__lock = rwlock.RWLockFairD()
         self.__reply_partition_assigned = threading.Event()
         
         #reset to listen form now
         self.__consume_data = True
         self.__thread = threading.Thread(
             target=self.__consumer_handler
```

### Comparing `k2eg-0.2.6/k2eg.egg-info/PKG-INFO` & `k2eg-0.2.7/k2eg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2eg
-Version: 0.2.6
+Version: 0.2.7
 Summary: A k2eg library
 Author-email: Claudio Bisegni <bisegni@slac.stanford.edu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `k2eg-0.2.6/pyproject.toml` & `k2eg-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "k2eg"
-version = "0.2.6"
+version = "0.2.7"
 description = "A k2eg library"
 readme = "README.md"
 authors = [{name = "Claudio Bisegni", email = "bisegni@slac.stanford.edu"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `k2eg-0.2.6/tests/test_dml.py` & `k2eg-0.2.7/tests/test_dml.py`

 * *Files identical despite different names*

