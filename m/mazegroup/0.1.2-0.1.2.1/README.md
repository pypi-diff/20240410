# Comparing `tmp/mazegroup-0.1.2.tar.gz` & `tmp/mazegroup-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.2.tar", last modified: Wed Apr 10 07:19:15 2024, max compression
+gzip compressed data, was "mazegroup-0.1.2.1.tar", last modified: Wed Apr 10 07:30:03 2024, max compression
```

## Comparing `mazegroup-0.1.2.tar` & `mazegroup-0.1.2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:15.525224 mazegroup-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 07:19:15.525224 mazegroup-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 07:19:11.000000 mazegroup-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:15.525224 mazegroup-0.1.2/mazegroup/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:19:11.000000 mazegroup-0.1.2/mazegroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:15.525224 mazegroup-0.1.2/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 07:19:15.000000 mazegroup-0.1.2/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-10 07:19:15.000000 mazegroup-0.1.2/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:19:15.000000 mazegroup-0.1.2/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 07:19:15.000000 mazegroup-0.1.2/mazegroup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 07:19:15.000000 mazegroup-0.1.2/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:19:15.525224 mazegroup-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-10 07:19:11.000000 mazegroup-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:30:03.766442 mazegroup-0.1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 07:30:03.766442 mazegroup-0.1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 07:29:57.000000 mazegroup-0.1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:30:03.762442 mazegroup-0.1.2.1/mazegroup/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:29:57.000000 mazegroup-0.1.2.1/mazegroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:30:03.766442 mazegroup-0.1.2.1/mazegroup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:29:57.000000 mazegroup-0.1.2.1/mazegroup/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:30:03.766442 mazegroup-0.1.2.1/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 07:30:03.000000 mazegroup-0.1.2.1/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 07:30:03.000000 mazegroup-0.1.2.1/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:30:03.000000 mazegroup-0.1.2.1/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 07:30:03.000000 mazegroup-0.1.2.1/mazegroup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 07:30:03.000000 mazegroup-0.1.2.1/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:30:03.766442 mazegroup-0.1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 07:29:57.000000 mazegroup-0.1.2.1/setup.py
```

### Comparing `mazegroup-0.1.2/PKG-INFO` & `mazegroup-0.1.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um & Rayanis55
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.2/mazegroup.egg-info/PKG-INFO` & `mazegroup-0.1.2.1/mazegroup.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um & Rayanis55
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.2/setup.py` & `mazegroup-0.1.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mazegroup",
-    version="0.1.2",
+    version="0.1.2.1",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Genius_um & Rayanis55",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
-    packages=find_packages(),
+    packages=["mazegroup", "mazegroup/cli"], # find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
```

