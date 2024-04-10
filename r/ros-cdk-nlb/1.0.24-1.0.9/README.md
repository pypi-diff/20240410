# Comparing `tmp/ros-cdk-nlb-1.0.24.tar.gz` & `tmp/ros-cdk-nlb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-nlb-1.0.24.tar", last modified: Wed Apr 10 04:00:31 2024, max compression
+gzip compressed data, was "dist/ros-cdk-nlb-1.0.9.tar", last modified: Fri Sep 23 12:25:10 2022, max compression
```

## Comparing `ros-cdk-nlb-1.0.24.tar` & `ros-cdk-nlb-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1292 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1910 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/
--rw-r--r--   0 root         (0) root         (0)   306062 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98080 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/_jsii/ros-cdk-nlb@1.0.24.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/datasource/
--rw-r--r--   0 root         (0) root         (0)    52430 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1292 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-10 04:00:31.000000 ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb/
+-rw-r--r--   0 root         (0) root         (0)   163110 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63787 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb/_jsii/ros-cdk-nlb@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:25:10.000000 ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/top_level.txt
```

### Comparing `ros-cdk-nlb-1.0.24/LICENSE` & `ros-cdk-nlb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-nlb-1.0.24/PKG-INFO` & `ros-cdk-nlb-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nlb
-Version: 1.0.24
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NLB Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ros-cdk-nlb-1.0.24/setup.py` & `ros-cdk-nlb-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-nlb",
-    "version": "1.0.24",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -18,43 +18,41 @@
         "Source": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "ros_cdk_nlb",
-        "ros_cdk_nlb._jsii",
-        "ros_cdk_nlb.datasource"
+        "ros_cdk_nlb._jsii"
     ],
     "package_data": {
         "ros_cdk_nlb._jsii": [
-            "ros-cdk-nlb@1.0.24.jsii.tgz"
+            "ros-cdk-nlb@1.0.9.jsii.tgz"
         ],
         "ros_cdk_nlb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>1.12.0, <=1.85.0",
+        "jsii>=1.68.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3"
     ],
     "scripts": []
 }
 """
```

### Comparing `ros-cdk-nlb-1.0.24/src/ros_cdk_nlb.egg-info/PKG-INFO` & `ros-cdk-nlb-1.0.9/src/ros_cdk_nlb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nlb
-Version: 1.0.24
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NLB Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```
