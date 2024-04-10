# Comparing `tmp/mazegroup-0.1.2.2.tar.gz` & `tmp/mazegroup-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.2.2.tar", last modified: Wed Apr 10 07:36:45 2024, max compression
+gzip compressed data, was "mazegroup-0.1.3.tar", last modified: Wed Apr 10 19:25:17 2024, max compression
```

## Comparing `mazegroup-0.1.2.2.tar` & `mazegroup-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:36:45.681665 mazegroup-0.1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 07:36:45.681665 mazegroup-0.1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 07:36:41.000000 mazegroup-0.1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:36:45.681665 mazegroup-0.1.2.2/mazegroup/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:36:41.000000 mazegroup-0.1.2.2/mazegroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:36:45.681665 mazegroup-0.1.2.2/mazegroup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:36:41.000000 mazegroup-0.1.2.2/mazegroup/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:36:45.681665 mazegroup-0.1.2.2/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 07:36:45.000000 mazegroup-0.1.2.2/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 07:36:45.000000 mazegroup-0.1.2.2/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:36:45.000000 mazegroup-0.1.2.2/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 07:36:45.000000 mazegroup-0.1.2.2/mazegroup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 07:36:45.000000 mazegroup-0.1.2.2/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:36:45.681665 mazegroup-0.1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 07:36:41.000000 mazegroup-0.1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:25:17.037829 mazegroup-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-10 19:25:17.033829 mazegroup-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-10 19:25:02.000000 mazegroup-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:25:17.033829 mazegroup-0.1.3/mazegroup/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 19:25:02.000000 mazegroup-0.1.3/mazegroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:25:17.033829 mazegroup-0.1.3/mazegroup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 19:25:02.000000 mazegroup-0.1.3/mazegroup/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-10 19:25:02.000000 mazegroup-0.1.3/mazegroup/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 19:25:02.000000 mazegroup-0.1.3/mazegroup/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 19:25:02.000000 mazegroup-0.1.3/mazegroup/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:25:17.033829 mazegroup-0.1.3/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-10 19:25:16.000000 mazegroup-0.1.3/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-10 19:25:16.000000 mazegroup-0.1.3/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:25:16.000000 mazegroup-0.1.3/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 19:25:16.000000 mazegroup-0.1.3/mazegroup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 19:25:16.000000 mazegroup-0.1.3/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:25:17.037829 mazegroup-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-10 19:25:02.000000 mazegroup-0.1.3/setup.py
```

### Comparing `mazegroup-0.1.2.2/setup.py` & `mazegroup-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 
+#
+
 setup(
     name="mazegroup",
-    version="0.1.2.2",
+    version="0.1.3",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    author="Genius_um & Rayanis55",
+    author="Genius_um",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
     packages=["mazegroup", "mazegroup/cli"], # find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

