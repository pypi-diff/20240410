# Comparing `tmp/autogluon-1.0.1b20240408.tar.gz` & `tmp/autogluon-1.1.0b20240409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.0.1b20240408.tar", last modified: Mon Apr  8 09:05:52 2024, max compression
+gzip compressed data, was "autogluon-1.1.0b20240409.tar", last modified: Tue Apr  9 09:06:18 2024, max compression
```

## Comparing `autogluon-1.0.1b20240408.tar` & `autogluon-1.1.0b20240409.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:52.258606 autogluon-1.0.1b20240408/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-08 09:05:52.258606 autogluon-1.0.1b20240408/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:05:52.258606 autogluon-1.0.1b20240408/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-08 09:04:26.000000 autogluon-1.0.1b20240408/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:52.254606 autogluon-1.0.1b20240408/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:52.254606 autogluon-1.0.1b20240408/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:52.258606 autogluon-1.0.1b20240408/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:04:26.000000 autogluon-1.0.1b20240408/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:52.258606 autogluon-1.0.1b20240408/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:05:52.000000 autogluon-1.0.1b20240408/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-09 09:04:42.000000 autogluon-1.1.0b20240409/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.897552 autogluon-1.1.0b20240409/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.897552 autogluon-1.1.0b20240409/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:04:42.000000 autogluon-1.1.0b20240409/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.0.1b20240408/PKG-INFO` & `autogluon-1.1.0b20240409/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.0.1b20240408
+Version: 1.1.0b20240409
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.0.1b20240408/setup.py` & `autogluon-1.1.0b20240409/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.0.1b20240408/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.0b20240409/src/autogluon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.0.1b20240408
+Version: 1.1.0b20240409
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

