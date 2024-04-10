# Comparing `tmp/nhmail-1.0.2.tar.gz` & `tmp/nhmail-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhmail-1.0.2.tar", last modified: Tue Apr  9 01:23:38 2024, max compression
+gzip compressed data, was "nhmail-1.0.3.tar", last modified: Wed Apr 10 01:50:30 2024, max compression
```

## Comparing `nhmail-1.0.2.tar` & `nhmail-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 01:23:38.906709 nhmail-1.0.2/
--rw-r--r--   0 phamchuong   (501) staff       (20)     1062 2024-04-08 06:19:52.000000 nhmail-1.0.2/LICENSE
--rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-09 01:23:38.906480 nhmail-1.0.2/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1086 2024-04-08 08:02:58.000000 nhmail-1.0.2/README.md
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 01:23:38.905423 nhmail-1.0.2/nhmail/
--rw-r--r--   0 phamchuong   (501) staff       (20)     1658 2024-04-09 01:16:26.000000 nhmail-1.0.2/nhmail/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-04-08 07:26:40.000000 nhmail-1.0.2/nhmail/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      350 2024-04-08 07:54:41.000000 nhmail-1.0.2/nhmail/constants.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      553 2024-04-08 07:26:40.000000 nhmail-1.0.2/nhmail/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 01:23:38.906234 nhmail-1.0.2/nhmail.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-09 01:23:38.000000 nhmail-1.0.2/nhmail.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      252 2024-04-09 01:23:38.000000 nhmail-1.0.2/nhmail.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-09 01:23:38.000000 nhmail-1.0.2/nhmail.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-09 01:23:38.000000 nhmail-1.0.2/nhmail.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)        7 2024-04-09 01:23:38.000000 nhmail-1.0.2/nhmail.egg-info/top_level.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-09 01:23:38.906767 nhmail-1.0.2/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      757 2024-04-09 01:22:40.000000 nhmail-1.0.2/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-10 01:50:30.633634 nhmail-1.0.3/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1062 2024-04-08 06:19:52.000000 nhmail-1.0.3/LICENSE
+-rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-10 01:50:30.633408 nhmail-1.0.3/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1086 2024-04-08 08:02:58.000000 nhmail-1.0.3/README.md
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-10 01:50:30.632453 nhmail-1.0.3/nhmail/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1658 2024-04-09 01:16:26.000000 nhmail-1.0.3/nhmail/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-04-08 07:26:40.000000 nhmail-1.0.3/nhmail/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      350 2024-04-08 07:54:41.000000 nhmail-1.0.3/nhmail/constants.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      492 2024-04-10 01:49:36.000000 nhmail-1.0.3/nhmail/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-10 01:50:30.633171 nhmail-1.0.3/nhmail.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      252 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)        7 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/top_level.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-10 01:50:30.633683 nhmail-1.0.3/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      757 2024-04-10 01:50:25.000000 nhmail-1.0.3/setup.py
```

### Comparing `nhmail-1.0.2/LICENSE` & `nhmail-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.2/PKG-INFO` & `nhmail-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhmail
-Version: 1.0.2
+Version: 1.0.3
 Summary: email of nandh SDK for Python
 Home-page: https://github.com/ITNHL/nh-mail-sdk
 Author: it@nandhlogistics.vn
 Author-email: it@nandhlogistics.vn
 License: Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `nhmail-1.0.2/README.md` & `nhmail-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.2/nhmail/__init__.py` & `nhmail-1.0.3/nhmail/__init__.py`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.2/nhmail/client.py` & `nhmail-1.0.3/nhmail/client.py`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.2/nhmail.egg-info/PKG-INFO` & `nhmail-1.0.3/nhmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhmail
-Version: 1.0.2
+Version: 1.0.3
 Summary: email of nandh SDK for Python
 Home-page: https://github.com/ITNHL/nh-mail-sdk
 Author: it@nandhlogistics.vn
 Author-email: it@nandhlogistics.vn
 License: Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `nhmail-1.0.2/setup.py` & `nhmail-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "nhmail"
-version = "1.0.2"
+version = "1.0.3"
 long_desc = (
     """This SDK is a programatic inteface into the mail APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

