# Comparing `tmp/easyaddition_quicklyfix-0.0.7.tar.gz` & `tmp/easyaddition_quicklyfix-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyaddition_quicklyfix-0.0.7.tar", last modified: Wed Apr 10 11:24:45 2024, max compression
+gzip compressed data, was "easyaddition_quicklyfix-0.0.8.tar", last modified: Wed Apr 10 11:45:48 2024, max compression
```

## Comparing `easyaddition_quicklyfix-0.0.7.tar` & `easyaddition_quicklyfix-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:24:45.156967 easyaddition_quicklyfix-0.0.7/
--rw-r--r--   0 agatsa     (501) staff       (20)      580 2024-04-10 11:24:45.155846 easyaddition_quicklyfix-0.0.7/PKG-INFO
--rw-r--r--   0 agatsa     (501) staff       (20)        0 2024-04-10 07:22:16.000000 easyaddition_quicklyfix-0.0.7/README.md
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:24:45.148974 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix/
--rw-r--r--   0 agatsa     (501) staff       (20)       31 2024-04-10 10:40:21.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix/__init__.py
--rw-r--r--   0 agatsa     (501) staff       (20)       64 2024-04-10 10:52:23.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix/module.py
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:24:45.154976 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/
--rw-r--r--   0 agatsa     (501) staff       (20)      580 2024-04-10 11:24:44.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/PKG-INFO
--rw-r--r--   0 agatsa     (501) staff       (20)      322 2024-04-10 11:24:45.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/SOURCES.txt
--rw-r--r--   0 agatsa     (501) staff       (20)        1 2024-04-10 11:24:44.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/dependency_links.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       13 2024-04-10 11:24:44.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/requires.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       24 2024-04-10 11:24:44.000000 easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/top_level.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       38 2024-04-10 11:24:45.157221 easyaddition_quicklyfix-0.0.7/setup.cfg
--rw-r--r--   0 agatsa     (501) staff       (20)     1048 2024-04-10 11:24:34.000000 easyaddition_quicklyfix-0.0.7/setup.py
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:45:48.133341 easyaddition_quicklyfix-0.0.8/
+-rw-r--r--   0 agatsa     (501) staff       (20)      580 2024-04-10 11:45:48.132169 easyaddition_quicklyfix-0.0.8/PKG-INFO
+-rw-r--r--   0 agatsa     (501) staff       (20)        0 2024-04-10 07:22:16.000000 easyaddition_quicklyfix-0.0.8/README.md
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:45:48.124608 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix/
+-rw-r--r--   0 agatsa     (501) staff       (20)       31 2024-04-10 10:40:21.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix/__init__.py
+-rw-r--r--   0 agatsa     (501) staff       (20)       64 2024-04-10 10:52:23.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix/module.py
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:45:48.131034 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/
+-rw-r--r--   0 agatsa     (501) staff       (20)      580 2024-04-10 11:45:47.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/PKG-INFO
+-rw-r--r--   0 agatsa     (501) staff       (20)      322 2024-04-10 11:45:48.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/SOURCES.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)        1 2024-04-10 11:45:47.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/dependency_links.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       13 2024-04-10 11:45:47.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/requires.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       24 2024-04-10 11:45:47.000000 easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/top_level.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       38 2024-04-10 11:45:48.133796 easyaddition_quicklyfix-0.0.8/setup.cfg
+-rw-r--r--   0 agatsa     (501) staff       (20)     1048 2024-04-10 11:45:35.000000 easyaddition_quicklyfix-0.0.8/setup.py
```

### Comparing `easyaddition_quicklyfix-0.0.7/PKG-INFO` & `easyaddition_quicklyfix-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaddition_quicklyfix
-Version: 0.0.7
+Version: 0.0.8
 Summary: My first Python package
 Author: Saurabh Kumar
 Author-email: saurabh.kumar@agatsa.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `easyaddition_quicklyfix-0.0.7/easyaddition_quicklyfix.egg-info/PKG-INFO` & `easyaddition_quicklyfix-0.0.8/easyaddition_quicklyfix.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaddition-quicklyfix
-Version: 0.0.7
+Version: 0.0.8
 Summary: My first Python package
 Author: Saurabh Kumar
 Author-email: saurabh.kumar@agatsa.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `easyaddition_quicklyfix-0.0.7/setup.py` & `easyaddition_quicklyfix-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="easyaddition_quicklyfix",
```

