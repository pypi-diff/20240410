# Comparing `tmp/akeneo_connector-0.1.6.tar.gz` & `tmp/akeneo_connector-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo_connector-0.1.6.tar", last modified: Tue Apr  9 10:17:07 2024, max compression
+gzip compressed data, was "akeneo_connector-0.1.7.tar", last modified: Wed Apr 10 13:06:11 2024, max compression
```

## Comparing `akeneo_connector-0.1.6.tar` & `akeneo_connector-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:17:07.060224 akeneo_connector-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 10:17:01.000000 akeneo_connector-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 10:17:07.060224 akeneo_connector-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 10:17:01.000000 akeneo_connector-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:17:07.060224 akeneo_connector-0.1.6/akeneo_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 10:17:01.000000 akeneo_connector-0.1.6/akeneo_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-09 10:17:01.000000 akeneo_connector-0.1.6/akeneo_connector/akeneo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-09 10:17:01.000000 akeneo_connector-0.1.6/akeneo_connector/akeneo_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-09 10:17:01.000000 akeneo_connector-0.1.6/akeneo_connector/akeneo_product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:17:07.060224 akeneo_connector-0.1.6/akeneo_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 10:17:07.000000 akeneo_connector-0.1.6/akeneo_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 10:17:07.000000 akeneo_connector-0.1.6/akeneo_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:17:07.000000 akeneo_connector-0.1.6/akeneo_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:17:07.000000 akeneo_connector-0.1.6/akeneo_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 10:17:07.000000 akeneo_connector-0.1.6/akeneo_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:17:07.060224 akeneo_connector-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 10:17:04.000000 akeneo_connector-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:06:11.419987 akeneo_connector-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-10 13:06:00.000000 akeneo_connector-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-10 13:06:11.419987 akeneo_connector-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-10 13:06:00.000000 akeneo_connector-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:06:11.419987 akeneo_connector-0.1.7/akeneo_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 13:06:00.000000 akeneo_connector-0.1.7/akeneo_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-10 13:06:00.000000 akeneo_connector-0.1.7/akeneo_connector/akeneo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-10 13:06:00.000000 akeneo_connector-0.1.7/akeneo_connector/akeneo_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-10 13:06:00.000000 akeneo_connector-0.1.7/akeneo_connector/akeneo_product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:06:11.419987 akeneo_connector-0.1.7/akeneo_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-10 13:06:11.000000 akeneo_connector-0.1.7/akeneo_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 13:06:11.000000 akeneo_connector-0.1.7/akeneo_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:06:11.000000 akeneo_connector-0.1.7/akeneo_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:06:11.000000 akeneo_connector-0.1.7/akeneo_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 13:06:11.000000 akeneo_connector-0.1.7/akeneo_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:06:11.419987 akeneo_connector-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-10 13:06:07.000000 akeneo_connector-0.1.7/setup.py
```

### Comparing `akeneo_connector-0.1.6/LICENSE` & `akeneo_connector-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.6/PKG-INFO` & `akeneo_connector-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.6
+Version: 0.1.7
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.6/README.md` & `akeneo_connector-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.6/akeneo_connector/akeneo_connector.py` & `akeneo_connector-0.1.7/akeneo_connector/akeneo_connector.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.6/akeneo_connector/akeneo_paginator.py` & `akeneo_connector-0.1.7/akeneo_connector/akeneo_paginator.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.6/akeneo_connector/akeneo_product.py` & `akeneo_connector-0.1.7/akeneo_connector/akeneo_product.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,8 +229,19 @@
         url = self.connector.product_url.format(identifier=self.identifier)
 
         # Update the product
         self.connector.update(url, self.payload())
 
         return True
 
+    def create(self):
+        """
+        Creates the product.
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        #  Update is same
+        self.update()
+
+        return True
```

### Comparing `akeneo_connector-0.1.6/akeneo_connector.egg-info/PKG-INFO` & `akeneo_connector-0.1.7/akeneo_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.6
+Version: 0.1.7
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.6/setup.py` & `akeneo_connector-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="akeneo_connector",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```
