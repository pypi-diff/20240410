# Comparing `tmp/easyaddition_quicklyfix-0.0.4.tar.gz` & `tmp/easyaddition_quicklyfix-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyaddition_quicklyfix-0.0.4.tar", last modified: Wed Apr 10 11:05:58 2024, max compression
+gzip compressed data, was "easyaddition_quicklyfix-0.0.5.tar", last modified: Wed Apr 10 11:10:34 2024, max compression
```

## Comparing `easyaddition_quicklyfix-0.0.4.tar` & `easyaddition_quicklyfix-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:05:58.619699 easyaddition_quicklyfix-0.0.4/
--rw-r--r--   0 agatsa     (501) staff       (20)      537 2024-04-10 11:05:58.619017 easyaddition_quicklyfix-0.0.4/PKG-INFO
--rw-r--r--   0 agatsa     (501) staff       (20)        0 2024-04-10 07:22:16.000000 easyaddition_quicklyfix-0.0.4/README.md
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:05:58.613635 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix/
--rw-r--r--   0 agatsa     (501) staff       (20)       31 2024-04-10 10:40:21.000000 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix/__init__.py
--rw-r--r--   0 agatsa     (501) staff       (20)       64 2024-04-10 10:52:23.000000 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix/module.py
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:05:58.618249 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix.egg-info/
--rw-r--r--   0 agatsa     (501) staff       (20)      537 2024-04-10 11:05:58.000000 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix.egg-info/PKG-INFO
--rw-r--r--   0 agatsa     (501) staff       (20)      276 2024-04-10 11:05:58.000000 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix.egg-info/SOURCES.txt
--rw-r--r--   0 agatsa     (501) staff       (20)        1 2024-04-10 11:05:58.000000 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix.egg-info/dependency_links.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       24 2024-04-10 11:05:58.000000 easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix.egg-info/top_level.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       38 2024-04-10 11:05:58.619877 easyaddition_quicklyfix-0.0.4/setup.cfg
--rw-r--r--   0 agatsa     (501) staff       (20)     1054 2024-04-10 11:05:42.000000 easyaddition_quicklyfix-0.0.4/setup.py
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:10:34.055285 easyaddition_quicklyfix-0.0.5/
+-rw-r--r--   0 agatsa     (501) staff       (20)      537 2024-04-10 11:10:34.054565 easyaddition_quicklyfix-0.0.5/PKG-INFO
+-rw-r--r--   0 agatsa     (501) staff       (20)        0 2024-04-10 07:22:16.000000 easyaddition_quicklyfix-0.0.5/README.md
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:10:34.049054 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix/
+-rw-r--r--   0 agatsa     (501) staff       (20)       31 2024-04-10 10:40:21.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix/__init__.py
+-rw-r--r--   0 agatsa     (501) staff       (20)       64 2024-04-10 10:52:23.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix/module.py
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:10:34.053858 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/
+-rw-r--r--   0 agatsa     (501) staff       (20)      537 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/PKG-INFO
+-rw-r--r--   0 agatsa     (501) staff       (20)      276 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/SOURCES.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)        1 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/dependency_links.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       24 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/top_level.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       38 2024-04-10 11:10:34.055509 easyaddition_quicklyfix-0.0.5/setup.cfg
+-rw-r--r--   0 agatsa     (501) staff       (20)     1054 2024-04-10 11:09:58.000000 easyaddition_quicklyfix-0.0.5/setup.py
```

### Comparing `easyaddition_quicklyfix-0.0.4/PKG-INFO` & `easyaddition_quicklyfix-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaddition_quicklyfix
-Version: 0.0.4
+Version: 0.0.5
 Summary: My first Python package
 Author: Saurabh Kumar
 Author-email: saurabh.kumar@agatsa.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `easyaddition_quicklyfix-0.0.4/easyaddition_quicklyfix.egg-info/PKG-INFO` & `easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaddition-quicklyfix
-Version: 0.0.4
+Version: 0.0.5
 Summary: My first Python package
 Author: Saurabh Kumar
 Author-email: saurabh.kumar@agatsa.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `easyaddition_quicklyfix-0.0.4/setup.py` & `easyaddition_quicklyfix-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="easyaddition_quicklyfix",
```
