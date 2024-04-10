# Comparing `tmp/define-oc-1.0.0.tar.gz` & `tmp/define-oc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "define-oc-1.0.0.tar", last modified: Wed Jan 24 00:23:57 2024, max compression
+gzip compressed data, was "define-oc-1.0.1.tar", last modified: Wed Apr 10 21:24:01 2024, max compression
```

## Comparing `define-oc-1.0.0.tar` & `define-oc-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-01-24 00:23:57.242526 define-oc-1.0.0/
--rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-03-18 13:46:48.000000 define-oc-1.0.0/LICENSE
--rw-rw-r--   0 bast      (1000) bast      (1000)      722 2024-01-24 00:23:57.242526 define-oc-1.0.0/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)       83 2023-03-18 13:46:48.000000 define-oc-1.0.0/README.md
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-01-24 00:23:57.238526 define-oc-1.0.0/define/
--rw-rw-r--   0 bast      (1000) bast      (1000)      562 2023-08-26 21:15:56.000000 define-oc-1.0.0/define/__init__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)       48 2023-03-19 23:23:20.000000 define-oc-1.0.0/define/__main__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     9648 2023-09-10 16:55:07.000000 define-oc-1.0.0/define/array.py
--rw-rw-r--   0 bast      (1000) bast      (1000)    10011 2023-10-22 17:09:46.000000 define-oc-1.0.0/define/base.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     1840 2023-08-26 20:16:25.000000 define-oc-1.0.0/define/constants.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     5015 2023-09-10 16:55:27.000000 define-oc-1.0.0/define/hash.py
--rw-rw-r--   0 bast      (1000) bast      (1000)    28743 2023-10-22 17:16:44.000000 define-oc-1.0.0/define/node.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     5866 2023-10-22 17:16:43.000000 define-oc-1.0.0/define/options.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     8398 2023-10-22 17:09:36.000000 define-oc-1.0.0/define/parent.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     2420 2023-09-10 16:54:19.000000 define-oc-1.0.0/define/tree.py
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-01-24 00:23:57.242526 define-oc-1.0.0/define_oc.egg-info/
--rw-rw-r--   0 bast      (1000) bast      (1000)      722 2024-01-24 00:23:57.000000 define-oc-1.0.0/define_oc.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)      397 2024-01-24 00:23:57.000000 define-oc-1.0.0/define_oc.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-01-24 00:23:57.000000 define-oc-1.0.0/define_oc.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)       84 2024-01-24 00:23:57.000000 define-oc-1.0.0/define_oc.egg-info/requires.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        7 2024-01-24 00:23:57.000000 define-oc-1.0.0/define_oc.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-03-19 23:26:46.000000 define-oc-1.0.0/define_oc.egg-info/zip-safe
--rw-rw-r--   0 bast      (1000) bast      (1000)       79 2024-01-24 00:23:57.242526 define-oc-1.0.0/setup.cfg
--rw-rw-r--   0 bast      (1000) bast      (1000)      943 2024-01-24 00:23:17.000000 define-oc-1.0.0/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-04-10 21:24:01.889660 define-oc-1.0.1/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-03-18 13:46:48.000000 define-oc-1.0.1/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)     4505 2024-04-10 21:24:01.889660 define-oc-1.0.1/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)     3866 2024-04-10 21:17:06.000000 define-oc-1.0.1/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-04-10 21:24:01.889660 define-oc-1.0.1/define/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      562 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)       48 2023-03-19 23:23:20.000000 define-oc-1.0.1/define/__main__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     9648 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/array.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    10012 2024-04-10 20:13:03.000000 define-oc-1.0.1/define/base.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1840 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/constants.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5015 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/hash.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    28743 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/node.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5866 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/options.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     8398 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/parent.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2420 2024-01-24 00:25:01.000000 define-oc-1.0.1/define/tree.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-04-10 21:24:01.889660 define-oc-1.0.1/define_oc.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     4505 2024-04-10 21:24:01.000000 define-oc-1.0.1/define_oc.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      397 2024-04-10 21:24:01.000000 define-oc-1.0.1/define_oc.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-04-10 21:24:01.000000 define-oc-1.0.1/define_oc.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       84 2024-04-10 21:24:01.000000 define-oc-1.0.1/define_oc.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        7 2024-04-10 21:24:01.000000 define-oc-1.0.1/define_oc.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-03-19 23:26:46.000000 define-oc-1.0.1/define_oc.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1000) bast      (1000)       79 2024-04-10 21:24:01.889660 define-oc-1.0.1/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)      943 2024-04-10 19:22:37.000000 define-oc-1.0.1/setup.py
```

### Comparing `define-oc-1.0.0/LICENSE` & `define-oc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/__init__.py` & `define-oc-1.0.1/define/__init__.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/array.py` & `define-oc-1.0.1/define/array.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/base.py` & `define-oc-1.0.1/define/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 				self.__class__.__name__,
 				sys._getframe().f_code.co_name
 			))
 
 		# Store the class name for the child
 		self.__class = self.__class__.__name__
 
-		# Init the list of the last falures generated in valid
+		# Init the list of the last failures generated in valid
 		self._validation_failures = None
 
 		# Init the optional flag, assume all nodes are necessary
 		self._optional = False
 
 		# If the details contains an optional flag
 		if '__optional__' in details:
```

### Comparing `define-oc-1.0.0/define/constants.py` & `define-oc-1.0.1/define/constants.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/hash.py` & `define-oc-1.0.1/define/hash.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/node.py` & `define-oc-1.0.1/define/node.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/options.py` & `define-oc-1.0.1/define/options.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/parent.py` & `define-oc-1.0.1/define/parent.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/define/tree.py` & `define-oc-1.0.1/define/tree.py`

 * *Files identical despite different names*

### Comparing `define-oc-1.0.0/setup.py` & `define-oc-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='define-oc',
-	version='1.0.0',
+	version='1.0.1',
 	description='A system for defining and validating data regardless of data store',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/format-oc',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/format-oc',
 		'Source': 'https://github.com/ouroboroscoding/define-python',
```

