# Comparing `tmp/ros-cdk-nlpautoml-1.0.23.tar.gz` & `tmp/ros-cdk-nlpautoml-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-nlpautoml-1.0.23.tar", last modified: Mon Mar  4 06:21:21 2024, max compression
+gzip compressed data, was "dist/ros-cdk-nlpautoml-1.0.24.tar", last modified: Wed Apr 10 02:37:35 2024, max compression
```

## Comparing `ros-cdk-nlpautoml-1.0.23.tar` & `ros-cdk-nlpautoml-1.0.24.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1316 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1912 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/
--rw-r--r--   0 root         (0) root         (0)    80929 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/_jsii/
--rw-r--r--   0 root         (0) root         (0)      431 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44371 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/_jsii/ros-cdk-nlpautoml@1.0.23.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:21:21.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-04 06:21:20.000000 ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/
+-rw-r--r--   0 root         (0) root         (0)    80999 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44059 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/_jsii/ros-cdk-nlpautoml@1.0.24.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 02:37:35.000000 ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/top_level.txt
```

### Comparing `ros-cdk-nlpautoml-1.0.23/LICENSE` & `ros-cdk-nlpautoml-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-nlpautoml-1.0.23/PKG-INFO` & `ros-cdk-nlpautoml-1.0.24/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nlpautoml
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NLPAUTOML Construct Library
```

### Comparing `ros-cdk-nlpautoml-1.0.23/setup.py` & `ros-cdk-nlpautoml-1.0.24/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-nlpautoml",
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
         "ros_cdk_nlpautoml",
         "ros_cdk_nlpautoml._jsii"
     ],
     "package_data": {
         "ros_cdk_nlpautoml._jsii": [
-            "ros-cdk-nlpautoml@1.0.23.jsii.tgz"
+            "ros-cdk-nlpautoml@1.0.24.jsii.tgz"
         ],
         "ros_cdk_nlpautoml": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml/__init__.py` & `ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class Dataset(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-nlpautoml.Dataset",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::NLPAUTOML::Dataset``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::NLPAUTOML::Dataset``, which is used to create a dataset.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosDataset``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-nlpautoml-dataset
     '''
 
@@ -601,15 +601,15 @@
 
 
 class RosDataset(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-nlpautoml.RosDataset",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::NLPAUTOML::Dataset``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::NLPAUTOML::Dataset``, which is used to create a dataset.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Dataset`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-nlpautoml-dataset
     '''
```

### Comparing `ros-cdk-nlpautoml-1.0.23/src/ros_cdk_nlpautoml.egg-info/PKG-INFO` & `ros-cdk-nlpautoml-1.0.24/src/ros_cdk_nlpautoml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nlpautoml
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NLPAUTOML Construct Library
```

