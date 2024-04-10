# Comparing `tmp/eaf_base_api-1.5.tar.gz` & `tmp/eaf_base_api-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eaf_base_api-1.5.tar", last modified: Mon Apr  1 23:41:06 2024, max compression
+gzip compressed data, was "eaf_base_api-1.6.tar", last modified: Wed Apr 10 18:25:28 2024, max compression
```

## Comparing `eaf_base_api-1.5.tar` & `eaf_base_api-1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.810887 eaf_base_api-1.5/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-04-01 23:41:06.810887 eaf_base_api-1.5/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1134 2024-02-25 13:36:08.000000 eaf_base_api-1.5/README.md
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.807554 eaf_base_api-1.5/base_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 20:06:14.000000 eaf_base_api-1.5/base_api/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     5695 2024-03-29 12:15:28.000000 eaf_base_api-1.5/base_api/base.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.810887 eaf_base_api-1.5/base_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 23:21:34.000000 eaf_base_api-1.5/base_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-03-29 13:01:59.000000 eaf_base_api-1.5/base_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     5868 2024-03-29 13:09:26.000000 eaf_base_api-1.5/base_api/modules/download.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1559 2024-02-17 21:49:48.000000 eaf_base_api-1.5/base_api/modules/progress_bars.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      101 2024-02-17 21:30:46.000000 eaf_base_api-1.5/base_api/modules/quality.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:41:06.810887 eaf_base_api-1.5/eaf_base_api.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      382 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        9 2024-04-01 23:41:06.000000 eaf_base_api-1.5/eaf_base_api.egg-info/top_level.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-01 23:41:06.810887 eaf_base_api-1.5/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      846 2024-04-01 23:40:24.000000 eaf_base_api-1.5/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-10 18:25:28.245301 eaf_base_api-1.6/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-04-10 18:25:28.245301 eaf_base_api-1.6/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1134 2024-02-25 13:36:08.000000 eaf_base_api-1.6/README.md
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-10 18:25:28.245301 eaf_base_api-1.6/base_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 20:06:14.000000 eaf_base_api-1.6/base_api/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     6004 2024-04-10 18:24:29.000000 eaf_base_api-1.6/base_api/base.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-10 18:25:28.245301 eaf_base_api-1.6/base_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-17 23:21:34.000000 eaf_base_api-1.6/base_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-03-29 13:01:59.000000 eaf_base_api-1.6/base_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     5868 2024-03-29 13:09:26.000000 eaf_base_api-1.6/base_api/modules/download.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1559 2024-02-17 21:49:48.000000 eaf_base_api-1.6/base_api/modules/progress_bars.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      101 2024-02-17 21:30:46.000000 eaf_base_api-1.6/base_api/modules/quality.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-10 18:25:28.245301 eaf_base_api-1.6/eaf_base_api.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1603 2024-04-10 18:25:28.000000 eaf_base_api-1.6/eaf_base_api.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      382 2024-04-10 18:25:28.000000 eaf_base_api-1.6/eaf_base_api.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-10 18:25:28.000000 eaf_base_api-1.6/eaf_base_api.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       31 2024-04-10 18:25:28.000000 eaf_base_api-1.6/eaf_base_api.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        9 2024-04-10 18:25:28.000000 eaf_base_api-1.6/eaf_base_api.egg-info/top_level.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-10 18:25:28.248634 eaf_base_api-1.6/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      846 2024-04-10 18:24:55.000000 eaf_base_api-1.6/setup.py
```

### Comparing `eaf_base_api-1.5/PKG-INFO` & `eaf_base_api-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaf_base_api
-Version: 1.5
+Version: 1.6
 Summary: A base API for EchterAlsFake's Porn APIs
 Home-page: https://github.com/EchterAlsFake/eaf_base_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `eaf_base_api-1.5/README.md` & `eaf_base_api-1.6/README.md`

 * *Files identical despite different names*

### Comparing `eaf_base_api-1.5/base_api/base.py` & `eaf_base_api-1.6/base_api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import logging
 import time
 import string
+import os
 
 from base_api.modules.quality import Quality
 from base_api.modules.progress_bars import Callback
 from base_api.modules.download import default, threaded, FFMPEG
 from base_api.modules.consts import MAX_RETRIES
 from pathlib import Path
 
@@ -147,8 +148,22 @@
     def strip_title(cls, title: str) -> str:
         """
         :param title:
         :return: str: strips out non UTF-8 chars of the title
         """
         illegal_chars = '<>:"/\\|?*'
         cleaned_title = ''.join([char for char in title if char in string.printable and char not in illegal_chars])
-        return cleaned_title
+        return cleaned_title
+
+    @classmethod
+    def return_path(cls, video, args):
+        path = args.output
+        if args.use_title:
+            if not str(path).endswith(os.sep):
+                path += os.sep
+
+            path += video.title + ".mp4"
+
+        else:
+            path = args.output
+
+        return path
```

### Comparing `eaf_base_api-1.5/base_api/modules/download.py` & `eaf_base_api-1.6/base_api/modules/download.py`

 * *Files identical despite different names*

### Comparing `eaf_base_api-1.5/base_api/modules/progress_bars.py` & `eaf_base_api-1.6/base_api/modules/progress_bars.py`

 * *Files identical despite different names*

### Comparing `eaf_base_api-1.5/eaf_base_api.egg-info/PKG-INFO` & `eaf_base_api-1.6/eaf_base_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaf_base_api
-Version: 1.5
+Version: 1.6
 Summary: A base API for EchterAlsFake's Porn APIs
 Home-page: https://github.com/EchterAlsFake/eaf_base_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `eaf_base_api-1.5/setup.py` & `eaf_base_api-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eaf_base_api",
-    version="1.5",
+    version="1.6",
     packages=find_packages(),
     install_requires=[
         "requests", "ffmpeg-progress-yield"
     ],
     entry_points={
         'console_scripts': [
             # If you want to create any executable scripts
```

