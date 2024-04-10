# Comparing `tmp/afas_connector-0.1.1.tar.gz` & `tmp/afas_connector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afas_connector-0.1.1.tar", last modified: Tue Apr  9 07:48:00 2024, max compression
+gzip compressed data, was "afas_connector-0.1.2.tar", last modified: Tue Apr  9 08:25:27 2024, max compression
```

## Comparing `afas_connector-0.1.1.tar` & `afas_connector-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:48:00.070103 afas_connector-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 07:47:51.000000 afas_connector-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 07:48:00.070103 afas_connector-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-09 07:47:51.000000 afas_connector-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:48:00.070103 afas_connector-0.1.1/afas_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 07:47:51.000000 afas_connector-0.1.1/afas_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-09 07:47:51.000000 afas_connector-0.1.1/afas_connector/afas_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-09 07:47:51.000000 afas_connector-0.1.1/afas_connector/afas_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 07:47:51.000000 afas_connector-0.1.1/afas_connector/afas_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:48:00.070103 afas_connector-0.1.1/afas_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 07:48:00.000000 afas_connector-0.1.1/afas_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 07:48:00.000000 afas_connector-0.1.1/afas_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:48:00.000000 afas_connector-0.1.1/afas_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:48:00.000000 afas_connector-0.1.1/afas_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 07:48:00.000000 afas_connector-0.1.1/afas_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:48:00.070103 afas_connector-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 07:47:57.000000 afas_connector-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:27.120999 afas_connector-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 08:25:18.000000 afas_connector-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 08:25:27.120999 afas_connector-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-09 08:25:18.000000 afas_connector-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:27.120999 afas_connector-0.1.2/afas_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 08:25:18.000000 afas_connector-0.1.2/afas_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-09 08:25:18.000000 afas_connector-0.1.2/afas_connector/afas_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-09 08:25:18.000000 afas_connector-0.1.2/afas_connector/afas_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 08:25:18.000000 afas_connector-0.1.2/afas_connector/afas_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:27.120999 afas_connector-0.1.2/afas_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-09 08:25:27.000000 afas_connector-0.1.2/afas_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 08:25:27.000000 afas_connector-0.1.2/afas_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:25:27.000000 afas_connector-0.1.2/afas_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:25:27.000000 afas_connector-0.1.2/afas_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 08:25:27.000000 afas_connector-0.1.2/afas_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:25:27.120999 afas_connector-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 08:25:24.000000 afas_connector-0.1.2/setup.py
```

### Comparing `afas_connector-0.1.1/LICENSE` & `afas_connector-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.1/PKG-INFO` & `afas_connector-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afas_connector
-Version: 0.1.1
+Version: 0.1.2
 Summary: AfasConnector is a Python package that simplifies interacting with AFAS Connectors via HTTP requests. It provides classes for making GET, POST, and PUT requests to AFAS Connectors and handling their responses.
 Home-page: https://github.com/bakeable/afas-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -84,15 +84,15 @@
 
 
 ### AfasObject
 The `AfasObject` is a wrapper for updating an item in Afas. The object has an `update` method that uses the `AfasConnector` class to update an item in a single line.
 
 #### Usage
 
-Here's an exampke of how to use the `AfasFilter` class:
+Here's an exampke of how to use the `AfasObject` class:
 
 ```python
 from afas.afas_object import AfasObject
 
 # Create an instance of AfasObject
 obj = AfasObject('FbItemArticle', {'Field1': 'Value1', 'Field2': 'Value2'})
```

### Comparing `afas_connector-0.1.1/README.md` & `afas_connector-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 ### AfasObject
 The `AfasObject` is a wrapper for updating an item in Afas. The object has an `update` method that uses the `AfasConnector` class to update an item in a single line.
 
 #### Usage
 
-Here's an exampke of how to use the `AfasFilter` class:
+Here's an exampke of how to use the `AfasObject` class:
 
 ```python
 from afas.afas_object import AfasObject
 
 # Create an instance of AfasObject
 obj = AfasObject('FbItemArticle', {'Field1': 'Value1', 'Field2': 'Value2'})
```

### Comparing `afas_connector-0.1.1/afas_connector/afas_connector.py` & `afas_connector-0.1.2/afas_connector/afas_connector.py`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.1/afas_connector/afas_filter.py` & `afas_connector-0.1.2/afas_connector/afas_filter.py`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.1/afas_connector/afas_object.py` & `afas_connector-0.1.2/afas_connector/afas_object.py`

 * *Files identical despite different names*

### Comparing `afas_connector-0.1.1/afas_connector.egg-info/PKG-INFO` & `afas_connector-0.1.2/afas_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afas_connector
-Version: 0.1.1
+Version: 0.1.2
 Summary: AfasConnector is a Python package that simplifies interacting with AFAS Connectors via HTTP requests. It provides classes for making GET, POST, and PUT requests to AFAS Connectors and handling their responses.
 Home-page: https://github.com/bakeable/afas-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -84,15 +84,15 @@
 
 
 ### AfasObject
 The `AfasObject` is a wrapper for updating an item in Afas. The object has an `update` method that uses the `AfasConnector` class to update an item in a single line.
 
 #### Usage
 
-Here's an exampke of how to use the `AfasFilter` class:
+Here's an exampke of how to use the `AfasObject` class:
 
 ```python
 from afas.afas_object import AfasObject
 
 # Create an instance of AfasObject
 obj = AfasObject('FbItemArticle', {'Field1': 'Value1', 'Field2': 'Value2'})
```

### Comparing `afas_connector-0.1.1/setup.py` & `afas_connector-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="afas_connector",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

