# Comparing `tmp/srinadhch07-0.21.tar.gz` & `tmp/srinadhch07-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srinadhch07-0.21.tar", last modified: Tue Apr  9 18:15:40 2024, max compression
+gzip compressed data, was "srinadhch07-0.23.tar", last modified: Tue Apr  9 18:02:45 2024, max compression
```

## Comparing `srinadhch07-0.21.tar` & `srinadhch07-0.23.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:40.534579 srinadhch07-0.21/
--rw-rw-rw-   0        0        0      549 2024-04-09 18:15:40.533583 srinadhch07-0.21/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-09 18:15:40.535582 srinadhch07-0.21/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-04-09 18:14:50.000000 srinadhch07-0.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:40.526202 srinadhch07-0.21/srinadhch07/
--rw-rw-rw-   0        0        0       39 2024-04-09 18:14:35.000000 srinadhch07-0.21/srinadhch07/__init__.py
--rw-rw-rw-   0        0        0       63 2024-04-09 17:28:52.000000 srinadhch07-0.21/srinadhch07/hello.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:40.533583 srinadhch07-0.21/srinadhch07.egg-info/
--rw-rw-rw-   0        0        0      549 2024-04-09 18:15:40.000000 srinadhch07-0.21/srinadhch07.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-09 18:15:40.000000 srinadhch07-0.21/srinadhch07.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:15:40.000000 srinadhch07-0.21/srinadhch07.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 18:15:40.000000 srinadhch07-0.21/srinadhch07.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 18:02:45.585675 srinadhch07-0.23/
+-rw-rw-rw-   0        0        0      549 2024-04-09 18:02:45.584677 srinadhch07-0.23/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:02:45.585675 srinadhch07-0.23/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-04-09 18:02:35.000000 srinadhch07-0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:02:45.577674 srinadhch07-0.23/srinadhch07/
+-rw-rw-rw-   0        0        0       27 2024-04-09 17:29:17.000000 srinadhch07-0.23/srinadhch07/__init__.py
+-rw-rw-rw-   0        0        0       63 2024-04-09 17:28:52.000000 srinadhch07-0.23/srinadhch07/hello.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:02:45.583676 srinadhch07-0.23/srinadhch07.egg-info/
+-rw-rw-rw-   0        0        0      549 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/top_level.txt
```

### Comparing `srinadhch07-0.21/PKG-INFO` & `srinadhch07-0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srinadhch07
-Version: 0.21
+Version: 0.23
 Summary: Hello package
 Author: srinadhch07
 Author-email: <srinadhc07@gmail.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `srinadhch07-0.21/setup.py` & `srinadhch07-0.23/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.21'
+VERSION = '0.23'
 DESCRIPTION = 'Hello package'
 long_description = 'First package.'
 
 # Setting up
 setup(
     name="srinadhch07",
     version=VERSION,
```

### Comparing `srinadhch07-0.21/srinadhch07.egg-info/PKG-INFO` & `srinadhch07-0.23/srinadhch07.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srinadhch07
-Version: 0.21
+Version: 0.23
 Summary: Hello package
 Author: srinadhch07
 Author-email: <srinadhc07@gmail.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

