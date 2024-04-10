# Comparing `tmp/mlscat-0.0.3.tar.gz` & `tmp/mlscat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlscat-0.0.3.tar", last modified: Mon Apr  8 13:28:43 2024, max compression
+gzip compressed data, was "mlscat-0.0.4.tar", last modified: Wed Apr 10 06:56:34 2024, max compression
```

## Comparing `mlscat-0.0.3.tar` & `mlscat-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 13:28:43.788320 mlscat-0.0.3/
--rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-08 13:28:43.788099 mlscat-0.0.3/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      481 2024-04-08 13:21:38.000000 mlscat-0.0.3/README.md
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 13:28:43.786797 mlscat-0.0.3/mlscat/
--rw-r--r--   0 wink       (501) staff       (20)       41 2024-04-08 13:28:38.000000 mlscat-0.0.3/mlscat/__init__.py
--rw-r--r--   0 wink       (501) staff       (20)     1397 2024-04-08 12:56:27.000000 mlscat-0.0.3/mlscat/utils.py
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-08 13:28:43.787873 mlscat-0.0.3/mlscat.egg-info/
--rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-08 13:28:43.000000 mlscat-0.0.3/mlscat.egg-info/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      202 2024-04-08 13:28:43.000000 mlscat-0.0.3/mlscat.egg-info/SOURCES.txt
--rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-08 13:28:43.000000 mlscat-0.0.3/mlscat.egg-info/dependency_links.txt
--rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-08 13:28:43.000000 mlscat-0.0.3/mlscat.egg-info/requires.txt
--rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-08 13:28:43.000000 mlscat-0.0.3/mlscat.egg-info/top_level.txt
--rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-08 13:28:43.788360 mlscat-0.0.3/setup.cfg
--rw-r--r--   0 wink       (501) staff       (20)      608 2024-04-08 13:19:29.000000 mlscat-0.0.3/setup.py
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.523596 mlscat-0.0.4/
+-rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-10 06:56:34.523291 mlscat-0.0.4/PKG-INFO
+-rw-r--r--   0 wink       (501) staff       (20)      481 2024-04-09 04:32:51.000000 mlscat-0.0.4/README.md
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.519654 mlscat-0.0.4/mlscat/
+-rw-r--r--   0 wink       (501) staff       (20)      131 2024-04-10 06:56:27.000000 mlscat-0.0.4/mlscat/__init__.py
+-rw-r--r--   0 wink       (501) staff       (20)      172 2024-04-08 14:31:16.000000 mlscat-0.0.4/mlscat/api.py
+-rw-r--r--   0 wink       (501) staff       (20)     2110 2024-04-10 06:42:52.000000 mlscat-0.0.4/mlscat/attacks.py
+-rw-r--r--   0 wink       (501) staff       (20)     1420 2024-04-09 07:28:32.000000 mlscat-0.0.4/mlscat/ranks.py
+-rw-r--r--   0 wink       (501) staff       (20)     1700 2024-04-10 06:37:33.000000 mlscat-0.0.4/mlscat/utils.py
+drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.522991 mlscat-0.0.4/mlscat.egg-info/
+-rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/PKG-INFO
+-rw-r--r--   0 wink       (501) staff       (20)      250 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/SOURCES.txt
+-rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/dependency_links.txt
+-rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/requires.txt
+-rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/top_level.txt
+-rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-10 06:56:34.523657 mlscat-0.0.4/setup.cfg
+-rw-r--r--   0 wink       (501) staff       (20)      608 2024-04-08 13:19:29.000000 mlscat-0.0.4/setup.py
```

### Comparing `mlscat-0.0.3/PKG-INFO` & `mlscat-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
```

### Comparing `mlscat-0.0.3/mlscat.egg-info/PKG-INFO` & `mlscat-0.0.4/mlscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
```

### Comparing `mlscat-0.0.3/setup.py` & `mlscat-0.0.4/setup.py`

 * *Files identical despite different names*

