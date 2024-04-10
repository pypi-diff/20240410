# Comparing `tmp/momodeltool-0.0.8.tar.gz` & `tmp/momodeltool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momodeltool-0.0.8.tar", last modified: Thu Nov  2 04:39:10 2023, max compression
+gzip compressed data, was "momodeltool-0.0.9.tar", last modified: Thu Nov  2 06:05:13 2023, max compression
```

## Comparing `momodeltool-0.0.8.tar` & `momodeltool-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 zichuana  (1000) zichuana  (1000)        0 2023-11-02 04:39:10.299625 momodeltool-0.0.8/
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)     1072 2023-10-27 10:31:13.000000 momodeltool-0.0.8/LICENSE
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      574 2023-11-02 04:39:10.299625 momodeltool-0.0.8/PKG-INFO
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       23 2023-10-26 05:36:21.000000 momodeltool-0.0.8/README.md
-drwxrwxr-x   0 zichuana  (1000) zichuana  (1000)        0 2023-11-02 04:39:10.299625 momodeltool-0.0.8/momodeltool/
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       86 2023-10-27 10:29:10.000000 momodeltool-0.0.8/momodeltool/__init__.py
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)    26721 2023-11-02 04:37:55.000000 momodeltool-0.0.8/momodeltool/momodeltool.py
-drwxrwxr-x   0 zichuana  (1000) zichuana  (1000)        0 2023-11-02 04:39:10.299625 momodeltool-0.0.8/momodeltool.egg-info/
--rw-r--r--   0 zichuana  (1000) zichuana  (1000)      574 2023-11-02 04:39:10.000000 momodeltool-0.0.8/momodeltool.egg-info/PKG-INFO
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      266 2023-11-02 04:39:10.000000 momodeltool-0.0.8/momodeltool.egg-info/SOURCES.txt
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)        1 2023-11-02 04:39:10.000000 momodeltool-0.0.8/momodeltool.egg-info/dependency_links.txt
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       26 2023-11-02 04:39:10.000000 momodeltool-0.0.8/momodeltool.egg-info/requires.txt
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       12 2023-11-02 04:39:10.000000 momodeltool-0.0.8/momodeltool.egg-info/top_level.txt
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      486 2023-11-02 04:38:44.000000 momodeltool-0.0.8/pyproject.toml
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       38 2023-11-02 04:39:10.299625 momodeltool-0.0.8/setup.cfg
--rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      741 2023-11-02 04:38:40.000000 momodeltool-0.0.8/setup.py
+drwxrwxr-x   0 zichuana  (1000) zichuana  (1000)        0 2023-11-02 06:05:13.819605 momodeltool-0.0.9/
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)     1072 2023-10-27 10:31:13.000000 momodeltool-0.0.9/LICENSE
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      574 2023-11-02 06:05:13.819605 momodeltool-0.0.9/PKG-INFO
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       23 2023-10-26 05:36:21.000000 momodeltool-0.0.9/README.md
+drwxrwxr-x   0 zichuana  (1000) zichuana  (1000)        0 2023-11-02 06:05:13.819605 momodeltool-0.0.9/momodeltool/
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      118 2023-11-02 06:03:54.000000 momodeltool-0.0.9/momodeltool/__init__.py
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)     1516 2023-11-02 06:00:17.000000 momodeltool-0.0.9/momodeltool/model_process.py
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)    26720 2023-11-02 06:04:07.000000 momodeltool-0.0.9/momodeltool/visualization.py
+drwxrwxr-x   0 zichuana  (1000) zichuana  (1000)        0 2023-11-02 06:05:13.819605 momodeltool-0.0.9/momodeltool.egg-info/
+-rw-r--r--   0 zichuana  (1000) zichuana  (1000)      574 2023-11-02 06:05:13.000000 momodeltool-0.0.9/momodeltool.egg-info/PKG-INFO
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      297 2023-11-02 06:05:13.000000 momodeltool-0.0.9/momodeltool.egg-info/SOURCES.txt
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)        1 2023-11-02 06:05:13.000000 momodeltool-0.0.9/momodeltool.egg-info/dependency_links.txt
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       26 2023-11-02 06:05:13.000000 momodeltool-0.0.9/momodeltool.egg-info/requires.txt
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       12 2023-11-02 06:05:13.000000 momodeltool-0.0.9/momodeltool.egg-info/top_level.txt
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      486 2023-11-02 06:04:31.000000 momodeltool-0.0.9/pyproject.toml
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)       38 2023-11-02 06:05:13.819605 momodeltool-0.0.9/setup.cfg
+-rw-rw-r--   0 zichuana  (1000) zichuana  (1000)      741 2023-11-02 06:04:36.000000 momodeltool-0.0.9/setup.py
```

### Comparing `momodeltool-0.0.8/LICENSE` & `momodeltool-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `momodeltool-0.0.8/PKG-INFO` & `momodeltool-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momodeltool
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/
 Author: momodeltool
 Author-email: JekkeySun <jianqi.sun@metoak.net>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `momodeltool-0.0.8/momodeltool/momodeltool.py` & `momodeltool-0.0.9/momodeltool/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import cv2
 import numpy as np
 import torch
 import os
 from math import *
 
-
 class Visualization(object):
     def __init__(self) -> None:
         self.window_num = 0
         self.switch = False
 
     def destroyAllWindows(self):
         cv2.waitKey(0)
```

### Comparing `momodeltool-0.0.8/momodeltool.egg-info/PKG-INFO` & `momodeltool-0.0.9/momodeltool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momodeltool
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/
 Author: momodeltool
 Author-email: JekkeySun <jianqi.sun@metoak.net>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `momodeltool-0.0.8/setup.py` & `momodeltool-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md",'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "momodeltool",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "momodeltool",
     author_email = "jianqi.sun@metoak.net",
     description = "This is a demo.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

