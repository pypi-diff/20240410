# Comparing `tmp/resamp-1.6.5.tar.gz` & `tmp/resamp-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.5.tar", last modified: Tue Apr  9 22:28:41 2024, max compression
+gzip compressed data, was "resamp-1.6.7.tar", last modified: Wed Apr 10 05:18:07 2024, max compression
```

## Comparing `resamp-1.6.5.tar` & `resamp-1.6.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:28:41.291058 resamp-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 22:28:37.000000 resamp-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-09 22:28:41.291058 resamp-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-09 22:28:37.000000 resamp-1.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:28:41.287058 resamp-1.6.5/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 22:28:37.000000 resamp-1.6.5/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-04-09 22:28:37.000000 resamp-1.6.5/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:28:41.291058 resamp-1.6.5/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:28:41.291058 resamp-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 22:28:37.000000 resamp-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:18:07.493957 resamp-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 05:18:03.000000 resamp-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-10 05:18:07.493957 resamp-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-10 05:18:03.000000 resamp-1.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:18:07.493957 resamp-1.6.7/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-10 05:18:03.000000 resamp-1.6.7/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-04-10 05:18:03.000000 resamp-1.6.7/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:18:07.493957 resamp-1.6.7/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-10 05:18:07.000000 resamp-1.6.7/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 05:18:07.000000 resamp-1.6.7/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:18:07.000000 resamp-1.6.7/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 05:18:07.000000 resamp-1.6.7/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 05:18:07.000000 resamp-1.6.7/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:18:07.493957 resamp-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-10 05:18:03.000000 resamp-1.6.7/setup.py
```

### Comparing `resamp-1.6.5/LICENSE` & `resamp-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.5/PKG-INFO` & `resamp-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.5
+Version: 1.6.7
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.5/README.md` & `resamp-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `resamp-1.6.5/resamp/__init__.py` & `resamp-1.6.7/resamp/__init__.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.5/resamp/resamp.py` & `resamp-1.6.7/resamp/resamp.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.5/resamp.egg-info/PKG-INFO` & `resamp-1.6.7/resamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.5
+Version: 1.6.7
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.5/setup.py` & `resamp-1.6.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.5',
+    version='1.6.7',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
     description='A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
```

