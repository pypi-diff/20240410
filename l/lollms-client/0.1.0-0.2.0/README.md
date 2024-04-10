# Comparing `tmp/lollms_client-0.1.0.tar.gz` & `tmp/lollms_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.1.0.tar", last modified: Mon Apr  8 23:34:05 2024, max compression
+gzip compressed data, was "lollms_client-0.2.0.tar", last modified: Wed Apr 10 07:30:46 2024, max compression
```

## Comparing `lollms_client-0.1.0.tar` & `lollms_client-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 23:34:05.410728 lollms_client-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-08 23:34:05.409720 lollms_client-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 23:34:05.395691 lollms_client-0.1.0/lollms_client/
--rw-rw-rw-   0        0        0     6583 2024-04-08 23:32:07.000000 lollms_client-0.1.0/lollms_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 23:34:05.408212 lollms_client-0.1.0/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 23:34:05.410728 lollms_client-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-07 10:55:31.000000 lollms_client-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:30:46.115906 lollms_client-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-10 07:30:46.114905 lollms_client-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 07:30:46.089904 lollms_client-0.2.0/lollms_client/
+-rw-rw-rw-   0        0        0    12127 2024-04-10 07:06:13.000000 lollms_client-0.2.0/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0     2035 2024-04-10 07:00:43.000000 lollms_client-0.2.0/lollms_client/lollms_types.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:30:46.113905 lollms_client-0.2.0/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-10 07:30:45.000000 lollms_client-0.2.0/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-10 07:30:45.000000 lollms_client-0.2.0/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 07:30:45.000000 lollms_client-0.2.0/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 07:30:45.000000 lollms_client-0.2.0/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 07:30:45.000000 lollms_client-0.2.0/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 07:30:46.115906 lollms_client-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-04-10 06:48:11.000000 lollms_client-0.2.0/setup.py
```

### Comparing `lollms_client-0.1.0/LICENSE` & `lollms_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.1.0/PKG-INFO` & `lollms_client-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.1.0/README.md` & `lollms_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.1.0/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.2.0/lollms_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.1.0/setup.py` & `lollms_client-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lollms_client",
-    version="0.1.0",
+    version="0.2.0",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

