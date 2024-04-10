# Comparing `tmp/srinadhch07-0.23.tar.gz` & `tmp/srinadhch07-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srinadhch07-0.23.tar", last modified: Tue Apr  9 18:02:45 2024, max compression
+gzip compressed data, was "srinadhch07-0.25.tar", last modified: Wed Apr 10 17:53:55 2024, max compression
```

## Comparing `srinadhch07-0.23.tar` & `srinadhch07-0.25.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:02:45.585675 srinadhch07-0.23/
--rw-rw-rw-   0        0        0      549 2024-04-09 18:02:45.584677 srinadhch07-0.23/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-09 18:02:45.585675 srinadhch07-0.23/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-04-09 18:02:35.000000 srinadhch07-0.23/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:02:45.577674 srinadhch07-0.23/srinadhch07/
--rw-rw-rw-   0        0        0       27 2024-04-09 17:29:17.000000 srinadhch07-0.23/srinadhch07/__init__.py
--rw-rw-rw-   0        0        0       63 2024-04-09 17:28:52.000000 srinadhch07-0.23/srinadhch07/hello.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:02:45.583676 srinadhch07-0.23/srinadhch07.egg-info/
--rw-rw-rw-   0        0        0      549 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 18:02:45.000000 srinadhch07-0.23/srinadhch07.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 17:53:55.606143 srinadhch07-0.25/
+-rw-rw-rw-   0        0        0      949 2024-04-10 17:53:55.604143 srinadhch07-0.25/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-10 17:53:55.607141 srinadhch07-0.25/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2024-04-10 17:53:15.000000 srinadhch07-0.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:53:55.598150 srinadhch07-0.25/srinadhch07/
+-rw-rw-rw-   0        0        0    15222 2024-04-10 17:53:11.000000 srinadhch07-0.25/srinadhch07/BAv2.py
+-rw-rw-rw-   0        0        0       79 2024-04-10 17:53:09.000000 srinadhch07-0.25/srinadhch07/__init__.py
+-rw-rw-rw-   0        0        0       63 2024-04-10 17:53:13.000000 srinadhch07-0.25/srinadhch07/hello.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:53:55.603145 srinadhch07-0.25/srinadhch07.egg-info/
+-rw-rw-rw-   0        0        0      949 2024-04-10 17:53:55.000000 srinadhch07-0.25/srinadhch07.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-10 17:53:55.000000 srinadhch07-0.25/srinadhch07.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 17:53:55.000000 srinadhch07-0.25/srinadhch07.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 17:53:55.000000 srinadhch07-0.25/srinadhch07.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 17:53:55.000000 srinadhch07-0.25/srinadhch07.egg-info/top_level.txt
```

### Comparing `srinadhch07-0.23/PKG-INFO` & `srinadhch07-0.25/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
 Name: srinadhch07
-Version: 0.23
-Summary: Hello package
+Version: 0.25
+Summary: BAv2
 Author: srinadhch07
 Author-email: <srinadhc07@gmail.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Requires-Dist: generativeai
 
-First package.
+The BAv2 is an personalised digital  desktop assistant made for Developers and users.
```

### Comparing `srinadhch07-0.23/setup.py` & `srinadhch07-0.25/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.23'
-DESCRIPTION = 'Hello package'
-long_description = 'First package.'
+VERSION = '0.25'
+DESCRIPTION = 'BAv2'
+long_description = 'The BAv2 is an personalised digital  desktop assistant made for Developers and users.'
 
 # Setting up
 setup(
     name="srinadhch07",
     version=VERSION,
     author="srinadhch07",
     author_email="<srinadhc07@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['generativeai'],
     keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ]
 )
```

### Comparing `srinadhch07-0.23/srinadhch07.egg-info/PKG-INFO` & `srinadhch07-0.25/srinadhch07.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
 Name: srinadhch07
-Version: 0.23
-Summary: Hello package
+Version: 0.25
+Summary: BAv2
 Author: srinadhch07
 Author-email: <srinadhc07@gmail.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Requires-Dist: generativeai
 
-First package.
+The BAv2 is an personalised digital  desktop assistant made for Developers and users.
```

