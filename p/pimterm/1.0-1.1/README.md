# Comparing `tmp/pimterm-1.0.tar.gz` & `tmp/pimterm-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimterm-1.0.tar", last modified: Tue Apr  9 11:51:01 2024, max compression
+gzip compressed data, was "pimterm-1.1.tar", last modified: Wed Apr 10 20:40:32 2024, max compression
```

## Comparing `pimterm-1.0.tar` & `pimterm-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 pim       (1000) pim       (1000)        0 2024-04-09 11:51:01.909286 pimterm-1.0/
--rw-rw-r--   0 pim       (1000) pim       (1000)     1067 2024-04-08 19:38:24.000000 pimterm-1.0/LICENSE
--rw-r--r--   0 pim       (1000) pim       (1000)     1311 2024-04-09 11:51:01.905286 pimterm-1.0/PKG-INFO
--rw-rw-r--   0 pim       (1000) pim       (1000)      912 2024-04-09 11:47:01.000000 pimterm-1.0/README.md
-drwxrwxr-x   0 pim       (1000) pim       (1000)        0 2024-04-09 11:51:01.905286 pimterm-1.0/pimterm.egg-info/
--rw-r--r--   0 pim       (1000) pim       (1000)     1311 2024-04-09 11:51:01.000000 pimterm-1.0/pimterm.egg-info/PKG-INFO
--rw-rw-r--   0 pim       (1000) pim       (1000)      214 2024-04-09 11:51:01.000000 pimterm-1.0/pimterm.egg-info/SOURCES.txt
--rw-rw-r--   0 pim       (1000) pim       (1000)        1 2024-04-09 11:51:01.000000 pimterm-1.0/pimterm.egg-info/dependency_links.txt
--rw-rw-r--   0 pim       (1000) pim       (1000)       46 2024-04-09 11:51:01.000000 pimterm-1.0/pimterm.egg-info/entry_points.txt
--rw-rw-r--   0 pim       (1000) pim       (1000)        7 2024-04-09 11:51:01.000000 pimterm-1.0/pimterm.egg-info/requires.txt
--rw-rw-r--   0 pim       (1000) pim       (1000)        1 2024-04-09 11:51:01.000000 pimterm-1.0/pimterm.egg-info/top_level.txt
--rw-rw-r--   0 pim       (1000) pim       (1000)       38 2024-04-09 11:51:01.909286 pimterm-1.0/setup.cfg
--rw-rw-r--   0 pim       (1000) pim       (1000)      697 2024-04-09 11:47:01.000000 pimterm-1.0/setup.py
+drwxrwxr-x   0 pim       (1000) pim       (1000)        0 2024-04-10 20:40:32.292571 pimterm-1.1/
+-rw-rw-r--   0 pim       (1000) pim       (1000)     1067 2024-04-08 19:38:24.000000 pimterm-1.1/LICENSE
+-rw-r--r--   0 pim       (1000) pim       (1000)     1311 2024-04-10 20:40:32.292571 pimterm-1.1/PKG-INFO
+-rw-rw-r--   0 pim       (1000) pim       (1000)      912 2024-04-09 11:47:01.000000 pimterm-1.1/README.md
+drwxrwxr-x   0 pim       (1000) pim       (1000)        0 2024-04-10 20:40:32.292571 pimterm-1.1/pimterm.egg-info/
+-rw-r--r--   0 pim       (1000) pim       (1000)     1311 2024-04-10 20:40:32.000000 pimterm-1.1/pimterm.egg-info/PKG-INFO
+-rw-rw-r--   0 pim       (1000) pim       (1000)      214 2024-04-10 20:40:32.000000 pimterm-1.1/pimterm.egg-info/SOURCES.txt
+-rw-rw-r--   0 pim       (1000) pim       (1000)        1 2024-04-10 20:40:32.000000 pimterm-1.1/pimterm.egg-info/dependency_links.txt
+-rw-rw-r--   0 pim       (1000) pim       (1000)       46 2024-04-10 20:40:32.000000 pimterm-1.1/pimterm.egg-info/entry_points.txt
+-rw-rw-r--   0 pim       (1000) pim       (1000)        7 2024-04-10 20:40:32.000000 pimterm-1.1/pimterm.egg-info/requires.txt
+-rw-rw-r--   0 pim       (1000) pim       (1000)        1 2024-04-10 20:40:32.000000 pimterm-1.1/pimterm.egg-info/top_level.txt
+-rw-rw-r--   0 pim       (1000) pim       (1000)       38 2024-04-10 20:40:32.292571 pimterm-1.1/setup.cfg
+-rw-rw-r--   0 pim       (1000) pim       (1000)      697 2024-04-10 20:33:57.000000 pimterm-1.1/setup.py
```

### Comparing `pimterm-1.0/LICENSE` & `pimterm-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pimterm-1.0/PKG-INFO` & `pimterm-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimterm
-Version: 1.0
+Version: 1.1
 Summary: A simple Python package that helps you find the command you need.
 Author: Pim Verleg
 Author-email: pim_iets@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `pimterm-1.0/README.md` & `pimterm-1.1/README.md`

 * *Files identical despite different names*

### Comparing `pimterm-1.0/pimterm.egg-info/PKG-INFO` & `pimterm-1.1/pimterm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimterm
-Version: 1.0
+Version: 1.1
 Summary: A simple Python package that helps you find the command you need.
 Author: Pim Verleg
 Author-email: pim_iets@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `pimterm-1.0/setup.py` & `pimterm-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pimterm",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'pimterm=pimterm.main:main',
         ],
     },
     description="A simple Python package that helps you find the command you need.",
```

