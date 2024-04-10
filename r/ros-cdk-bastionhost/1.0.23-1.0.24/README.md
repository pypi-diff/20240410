# Comparing `tmp/ros-cdk-bastionhost-1.0.23.tar.gz` & `tmp/ros-cdk-bastionhost-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-bastionhost-1.0.23.tar", last modified: Mon Mar  4 07:39:40 2024, max compression
+gzip compressed data, was "dist/ros-cdk-bastionhost-1.0.24.tar", last modified: Wed Apr 10 03:03:08 2024, max compression
```

## Comparing `ros-cdk-bastionhost-1.0.23.tar` & `ros-cdk-bastionhost-1.0.24.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1324 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1924 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/
--rw-r--r--   0 root         (0) root         (0)   100924 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/_jsii/
--rw-r--r--   0 root         (0) root         (0)      435 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50162 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/_jsii/ros-cdk-bastionhost@1.0.23.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1324 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      481 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-04 07:39:40.000000 ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/
+-rw-r--r--   0 root         (0) root         (0)   100924 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50161 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/_jsii/ros-cdk-bastionhost@1.0.24.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      481 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 03:03:08.000000 ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/top_level.txt
```

### Comparing `ros-cdk-bastionhost-1.0.23/LICENSE` & `ros-cdk-bastionhost-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-bastionhost-1.0.23/PKG-INFO` & `ros-cdk-bastionhost-1.0.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bastionhost
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BASTIONHOST Construct Library
```

### Comparing `ros-cdk-bastionhost-1.0.23/setup.py` & `ros-cdk-bastionhost-1.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-bastionhost",
-    "version": "1.0.23",
+    "version": "1.0.24",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ros_cdk_bastionhost",
         "ros_cdk_bastionhost._jsii"
     ],
     "package_data": {
         "ros_cdk_bastionhost._jsii": [
-            "ros-cdk-bastionhost@1.0.23.jsii.tgz"
+            "ros-cdk-bastionhost@1.0.24.jsii.tgz"
         ],
         "ros_cdk_bastionhost": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost/__init__.py` & `ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-bastionhost-1.0.23/src/ros_cdk_bastionhost.egg-info/PKG-INFO` & `ros-cdk-bastionhost-1.0.24/src/ros_cdk_bastionhost.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bastionhost
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BASTIONHOST Construct Library
```

