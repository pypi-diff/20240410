# Comparing `tmp/recflows-0.0.1.tar.gz` & `tmp/recflows-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recflows-0.0.1.tar", last modified: Wed Apr 10 07:20:41 2024, max compression
+gzip compressed data, was "recflows-0.0.2.tar", last modified: Wed Apr 10 16:57:42 2024, max compression
```

## Comparing `recflows-0.0.1.tar` & `recflows-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 07:20:41.194749 recflows-0.0.1/
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)     1065 2024-04-10 07:18:06.000000 recflows-0.0.1/LICENSE
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)      574 2024-04-10 07:20:41.185753 recflows-0.0.1/PKG-INFO
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)      186 2024-04-10 07:03:18.000000 recflows-0.0.1/README.md
-drwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 07:20:40.982682 recflows-0.0.1/recflows/
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-09 18:00:48.000000 recflows-0.0.1/recflows/__init__.py
-drwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 07:20:41.075203 recflows-0.0.1/recflows/decorators/
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 06:37:16.000000 recflows-0.0.1/recflows/decorators/__init__.py
-drwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 07:20:41.127202 recflows-0.0.1/recflows/resources/
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 06:37:47.000000 recflows-0.0.1/recflows/resources/__init__.py
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)      132 2024-04-10 06:57:06.000000 recflows-0.0.1/recflows/resources/app.py
-drwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 07:20:41.173753 recflows-0.0.1/recflows.egg-info/
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)      574 2024-04-10 07:20:40.000000 recflows-0.0.1/recflows.egg-info/PKG-INFO
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)      313 2024-04-10 07:20:40.000000 recflows-0.0.1/recflows.egg-info/SOURCES.txt
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        1 2024-04-10 07:20:40.000000 recflows-0.0.1/recflows.egg-info/dependency_links.txt
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)       14 2024-04-10 07:20:40.000000 recflows-0.0.1/recflows.egg-info/requires.txt
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        9 2024-04-10 07:20:40.000000 recflows-0.0.1/recflows.egg-info/top_level.txt
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)       38 2024-04-10 07:20:41.196753 recflows-0.0.1/setup.cfg
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)      701 2024-04-10 07:01:42.000000 recflows-0.0.1/setup.py
-drwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)        0 2024-04-10 07:20:41.155757 recflows-0.0.1/tests/
--rwxrwxrwx   0 cogdiver  (1000) cogdiver  (1000)       96 2024-04-10 07:05:40.000000 recflows-0.0.1/tests/test_app.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 16:57:42.467565 recflows-0.0.2/
+-rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.2/LICENSE
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 16:57:42.459563 recflows-0.0.2/PKG-INFO
+-rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.2/README.md
+drwxrwxrwx   0     1000     1000        0 2024-04-10 16:57:42.295565 recflows-0.0.2/recflows/
+-rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.2/recflows/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 16:57:42.381564 recflows-0.0.2/recflows/decorators/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.2/recflows/decorators/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 16:57:42.415562 recflows-0.0.2/recflows/resources/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.2/recflows/resources/__init__.py
+-rwxrwxrwx   0     1000     1000      424 2024-04-10 16:39:15.000000 recflows-0.0.2/recflows/resources/app.py
+-rwxrwxrwx   0     1000     1000      216 2024-04-10 16:37:04.000000 recflows-0.0.2/recflows/vars.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 16:57:42.451568 recflows-0.0.2/recflows.egg-info/
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 16:57:42.000000 recflows-0.0.2/recflows.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      330 2024-04-10 16:57:42.000000 recflows-0.0.2/recflows.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2024-04-10 16:57:42.000000 recflows-0.0.2/recflows.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       14 2024-04-10 16:57:42.000000 recflows-0.0.2/recflows.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        9 2024-04-10 16:57:42.000000 recflows-0.0.2/recflows.egg-info/top_level.txt
+-rwxrwxrwx   0     1000     1000       38 2024-04-10 16:57:42.468567 recflows-0.0.2/setup.cfg
+-rwxrwxrwx   0     1000     1000      701 2024-04-10 16:55:52.000000 recflows-0.0.2/setup.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 16:57:42.430564 recflows-0.0.2/tests/
+-rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.2/tests/test_app.py
```

### Comparing `recflows-0.0.1/LICENSE` & `recflows-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recflows-0.0.1/PKG-INFO` & `recflows-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.1
+Version: 0.0.2
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.1
 
-# RecsFlow
+# RecFlows
 
 Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 
 
 ## Usage
 ```bash
 docker run recflows
```

### Comparing `recflows-0.0.1/recflows.egg-info/PKG-INFO` & `recflows-0.0.2/recflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.1
+Version: 0.0.2
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.1
 
-# RecsFlow
+# RecFlows
 
 Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 
 
 ## Usage
 ```bash
 docker run recflows
```

### Comparing `recflows-0.0.1/setup.py` & `recflows-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def read_requirements():
     return read('requirements.txt').splitlines()
 
 
 setup(
     name="recflows",
-    version="0.0.1",
+    version="0.0.2",
     description="Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/cogdiver/recflows",
     license="MIT",
     packages=find_packages(),
     install_requires=read_requirements(),
```

