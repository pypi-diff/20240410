# Comparing `tmp/mazegroup-0.1.0.tar.gz` & `tmp/mazegroup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.0.tar", last modified: Wed Apr 10 06:43:54 2024, max compression
+gzip compressed data, was "mazegroup-0.1.1.tar", last modified: Wed Apr 10 06:50:34 2024, max compression
```

## Comparing `mazegroup-0.1.0.tar` & `mazegroup-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:43:54.440965 mazegroup-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 06:43:54.440965 mazegroup-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 06:43:49.000000 mazegroup-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:43:54.440965 mazegroup-0.1.0/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 06:43:54.000000 mazegroup-0.1.0/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-10 06:43:54.000000 mazegroup-0.1.0/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:43:54.000000 mazegroup-0.1.0/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 06:43:54.000000 mazegroup-0.1.0/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:43:54.440965 mazegroup-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-10 06:43:49.000000 mazegroup-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:50:34.106891 mazegroup-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 06:50:34.106891 mazegroup-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 06:50:28.000000 mazegroup-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:50:34.106891 mazegroup-0.1.1/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 06:50:34.000000 mazegroup-0.1.1/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 06:50:34.000000 mazegroup-0.1.1/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:50:34.000000 mazegroup-0.1.1/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 06:50:34.000000 mazegroup-0.1.1/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:50:34.106891 mazegroup-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 06:50:28.000000 mazegroup-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:50:34.106891 mazegroup-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 06:50:28.000000 mazegroup-0.1.1/src/__init__.py
```

### Comparing `mazegroup-0.1.0/PKG-INFO` & `mazegroup-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.0
+Version: 0.1.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um & Rayanis55
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.0/mazegroup.egg-info/PKG-INFO` & `mazegroup-0.1.1/mazegroup.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.0
+Version: 0.1.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um & Rayanis55
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.0/setup.py` & `mazegroup-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mazegroup",
-    version="0.1.0",
+    version="0.1.1",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Genius_um & Rayanis55",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
-    packages=["mazegroup"], #find_packages(),
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

