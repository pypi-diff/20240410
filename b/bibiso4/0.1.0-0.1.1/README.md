# Comparing `tmp/bibiso4-0.1.0.tar.gz` & `tmp/bibiso4-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibiso4-0.1.0.tar", last modified: Fri Mar 29 07:30:27 2024, max compression
+gzip compressed data, was "bibiso4-0.1.1.tar", last modified: Wed Apr 10 03:45:05 2024, max compression
```

## Comparing `bibiso4-0.1.0.tar` & `bibiso4-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-29 07:30:27.279503 bibiso4-0.1.0/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1070 2024-03-29 05:09:41.000000 bibiso4-0.1.0/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)      504 2024-03-29 07:30:27.279503 bibiso4-0.1.0/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      165 2024-03-29 05:26:04.000000 bibiso4-0.1.0/README.md
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      565 2024-03-29 05:28:44.000000 bibiso4-0.1.0/pyproject.toml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-03-29 07:30:27.279503 bibiso4-0.1.0/setup.cfg
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-29 07:30:27.275503 bibiso4-0.1.0/src/
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-29 07:30:27.279503 bibiso4-0.1.0/src/bibiso4/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3136 2024-03-29 05:38:24.000000 bibiso4-0.1.0/src/bibiso4/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)   413939 2024-03-21 05:21:01.000000 bibiso4-0.1.0/src/bibiso4/exact.json
--rw-rw-r--   0 andrew    (1000) andrew    (1000)   413939 2024-03-21 05:21:01.000000 bibiso4-0.1.0/src/bibiso4/prefix.json
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3923 2024-03-21 05:21:01.000000 bibiso4-0.1.0/src/bibiso4/suffix.json
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-29 07:30:27.279503 bibiso4-0.1.0/src/bibiso4.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      504 2024-03-29 07:30:27.000000 bibiso4-0.1.0/src/bibiso4.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      305 2024-03-29 07:30:27.000000 bibiso4-0.1.0/src/bibiso4.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-03-29 07:30:27.000000 bibiso4-0.1.0/src/bibiso4.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       55 2024-03-29 07:30:27.000000 bibiso4-0.1.0/src/bibiso4.egg-info/entry_points.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2024-03-29 07:30:27.000000 bibiso4-0.1.0/src/bibiso4.egg-info/top_level.txt
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-10 03:45:05.321403 bibiso4-0.1.1/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1070 2024-04-10 03:13:45.000000 bibiso4-0.1.1/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      796 2024-04-10 03:45:05.321403 bibiso4-0.1.1/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      457 2024-04-10 03:13:45.000000 bibiso4-0.1.1/README.md
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      565 2024-04-10 03:43:40.000000 bibiso4-0.1.1/pyproject.toml
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-04-10 03:45:05.321403 bibiso4-0.1.1/setup.cfg
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-10 03:45:05.321403 bibiso4-0.1.1/src/
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-10 03:45:05.321403 bibiso4-0.1.1/src/bibiso4/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3136 2024-04-10 03:43:00.000000 bibiso4-0.1.1/src/bibiso4/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   863649 2024-04-10 03:40:34.000000 bibiso4-0.1.1/src/bibiso4/exact.json
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   413939 2024-04-10 03:13:45.000000 bibiso4-0.1.1/src/bibiso4/prefix.json
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3923 2024-04-10 03:13:45.000000 bibiso4-0.1.1/src/bibiso4/suffix.json
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-10 03:45:05.321403 bibiso4-0.1.1/src/bibiso4.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      796 2024-04-10 03:45:05.000000 bibiso4-0.1.1/src/bibiso4.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      305 2024-04-10 03:45:05.000000 bibiso4-0.1.1/src/bibiso4.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-04-10 03:45:05.000000 bibiso4-0.1.1/src/bibiso4.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       55 2024-04-10 03:45:05.000000 bibiso4-0.1.1/src/bibiso4.egg-info/entry_points.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2024-04-10 03:45:05.000000 bibiso4-0.1.1/src/bibiso4.egg-info/top_level.txt
```

### Comparing `bibiso4-0.1.0/LICENSE` & `bibiso4-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bibiso4-0.1.0/pyproject.toml` & `bibiso4-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "bibiso4"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Andrew Fowlie", email = "andrew.j.fowlie@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `bibiso4-0.1.0/src/bibiso4/__init__.py` & `bibiso4-0.1.1/src/bibiso4/__init__.py`

 * *Files identical despite different names*

### Comparing `bibiso4-0.1.0/src/bibiso4/exact.json` & `bibiso4-0.1.1/src/bibiso4/prefix.json`

 * *Files identical despite different names*

### Comparing `bibiso4-0.1.0/src/bibiso4/suffix.json` & `bibiso4-0.1.1/src/bibiso4/suffix.json`

 * *Files identical despite different names*

