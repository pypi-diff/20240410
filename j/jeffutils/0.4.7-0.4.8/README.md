# Comparing `tmp/jeffutils-0.4.7.tar.gz` & `tmp/jeffutils-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.4.7.tar", last modified: Thu Mar 28 20:06:50 2024, max compression
+gzip compressed data, was "jeffutils-0.4.8.tar", last modified: Wed Apr 10 18:59:47 2024, max compression
```

## Comparing `jeffutils-0.4.7.tar` & `jeffutils-0.4.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-03-28 20:06:50.910650 jeffutils-0.4.7/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.4.7/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-03-28 20:06:50.910650 jeffutils-0.4.7/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.4.7/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.4.7/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-03-28 20:06:50.910650 jeffutils-0.4.7/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-03-28 20:06:45.000000 jeffutils-0.4.7/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-03-28 20:06:50.910650 jeffutils-0.4.7/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-03-28 20:06:50.910650 jeffutils-0.4.7/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.4.7/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    14441 2024-03-28 20:06:09.000000 jeffutils-0.4.7/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-03-28 20:06:50.910650 jeffutils-0.4.7/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-03-28 20:06:50.000000 jeffutils-0.4.7/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-03-28 20:06:50.000000 jeffutils-0.4.7/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-03-28 20:06:50.000000 jeffutils-0.4.7/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-03-28 20:06:50.000000 jeffutils-0.4.7/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.4.8/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-10 18:59:47.768322 jeffutils-0.4.8/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.4.8/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.4.8/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-10 18:59:47.768322 jeffutils-0.4.8/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-10 18:59:35.000000 jeffutils-0.4.8/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.4.8/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    14879 2024-04-10 18:59:25.000000 jeffutils-0.4.8/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.4.7/LICENSE.txt` & `jeffutils-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.4.7/setup.py` & `jeffutils-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.4.7',
+    version='0.4.8',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.4.7/src/jeffutils/utils.py` & `jeffutils-0.4.8/src/jeffutils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import io
 import os
 import pstats
 import cProfile
 import traceback
 from IPython.display import display
 from copy import deepcopy
+import ast
 
 MAX_ROWS = 50
 NP_FLOAT_PRECISION = 7
 NP_FLOAT_PRECISION_F = lambda x: "{0:0.7f}".format(x) # shows 7 decimal places
 PD_FLOAT_PRECISION = 7 
 PD_FLOAT_PRECISION_F = lambda x: "{0:0.7f}".format(x) # shows 7 decimal places
 PD_MAX_COLUMNS = None # show all of the columns
@@ -307,14 +308,26 @@
     return np.vectorize(map.__getitem__)(arr)
 
 
 ###########################
 # FUNCTIONALITY FUNCTIONS #
 ###########################
 
+def str_to_list_py(string):
+    try:
+        # Using ast.literal_eval to safely evaluate string as Python literal
+        parsed_list = ast.literal_eval(string)
+        if isinstance(parsed_list, list):
+            return parsed_list
+        else:
+            raise ValueError("Input is not a valid string representation of a list.")
+    except (SyntaxError, ValueError) as e:
+        print(f"Error: {e}")
+        return None
+
 def argmax_py(lst):
     return max(range(len(lst)), key=lambda x: lst[x])
 
 
 def dict_update(d:dict, d_:dict, inplace=False):
     """ takes in two dictionaries and adds the key-value pairs from the second 
     dictionary to the first dictionary. If inplace is False, then it will return
```

