# Comparing `tmp/ros-cdk-directmail-1.0.23.tar.gz` & `tmp/ros-cdk-directmail-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-directmail-1.0.23.tar", last modified: Mon Mar  4 06:50:57 2024, max compression
+gzip compressed data, was "dist/ros-cdk-directmail-1.0.24.tar", last modified: Wed Apr 10 03:20:30 2024, max compression
```

## Comparing `ros-cdk-directmail-1.0.23.tar` & `ros-cdk-directmail-1.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1320 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1959 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/
--rw-r--r--   0 root         (0) root         (0)    42411 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/_jsii/
--rw-r--r--   0 root         (0) root         (0)      433 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39747 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/_jsii/ros-cdk-directmail@1.0.23.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/datasource/
--rw-r--r--   0 root         (0) root         (0)    25267 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1320 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-04 06:50:57.000000 ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/
+-rw-r--r--   0 root         (0) root         (0)    42411 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39743 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/_jsii/ros-cdk-directmail@1.0.24.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/datasource/
+-rw-r--r--   0 root         (0) root         (0)    25267 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:20:29.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 03:20:30.000000 ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/top_level.txt
```

### Comparing `ros-cdk-directmail-1.0.23/LICENSE` & `ros-cdk-directmail-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-directmail-1.0.23/PKG-INFO` & `ros-cdk-directmail-1.0.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-directmail
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DIRECTMAIL Construct Library
```

### Comparing `ros-cdk-directmail-1.0.23/setup.py` & `ros-cdk-directmail-1.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-directmail",
-    "version": "1.0.23",
+    "version": "1.0.24",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "ros_cdk_directmail",
         "ros_cdk_directmail._jsii",
         "ros_cdk_directmail.datasource"
     ],
     "package_data": {
         "ros_cdk_directmail._jsii": [
-            "ros-cdk-directmail@1.0.23.jsii.tgz"
+            "ros-cdk-directmail@1.0.24.jsii.tgz"
         ],
         "ros_cdk_directmail": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/__init__.py` & `ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-directmail-1.0.23/src/ros_cdk_directmail/datasource/__init__.py` & `ros-cdk-directmail-1.0.24/src/ros_cdk_directmail/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/PKG-INFO` & `ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-directmail
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DIRECTMAIL Construct Library
```

### Comparing `ros-cdk-directmail-1.0.23/src/ros_cdk_directmail.egg-info/SOURCES.txt` & `ros-cdk-directmail-1.0.24/src/ros_cdk_directmail.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 src/ros_cdk_directmail/py.typed
 src/ros_cdk_directmail.egg-info/PKG-INFO
 src/ros_cdk_directmail.egg-info/SOURCES.txt
 src/ros_cdk_directmail.egg-info/dependency_links.txt
 src/ros_cdk_directmail.egg-info/requires.txt
 src/ros_cdk_directmail.egg-info/top_level.txt
 src/ros_cdk_directmail/_jsii/__init__.py
-src/ros_cdk_directmail/_jsii/ros-cdk-directmail@1.0.23.jsii.tgz
+src/ros_cdk_directmail/_jsii/ros-cdk-directmail@1.0.24.jsii.tgz
 src/ros_cdk_directmail/datasource/__init__.py
```

