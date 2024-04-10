# Comparing `tmp/ros-cdk-rocketmq5-1.0.23.tar.gz` & `tmp/ros-cdk-rocketmq5-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-rocketmq5-1.0.23.tar", last modified: Mon Mar  4 07:13:19 2024, max compression
+gzip compressed data, was "dist/ros-cdk-rocketmq5-1.0.24.tar", last modified: Wed Apr 10 03:20:40 2024, max compression
```

## Comparing `ros-cdk-rocketmq5-1.0.23.tar` & `ros-cdk-rocketmq5-1.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1316 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1952 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/
--rw-r--r--   0 root         (0) root         (0)   127352 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/_jsii/
--rw-r--r--   0 root         (0) root         (0)      431 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60487 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/_jsii/ros-cdk-rocketmq5@1.0.23.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/datasource/
--rw-r--r--   0 root         (0) root         (0)    16489 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-04 07:13:19.000000 ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/
+-rw-r--r--   0 root         (0) root         (0)   127336 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60520 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/_jsii/ros-cdk-rocketmq5@1.0.24.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/datasource/
+-rw-r--r--   0 root         (0) root         (0)    16489 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:20:39.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 03:20:40.000000 ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/top_level.txt
```

### Comparing `ros-cdk-rocketmq5-1.0.23/LICENSE` & `ros-cdk-rocketmq5-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-rocketmq5-1.0.23/PKG-INFO` & `ros-cdk-rocketmq5-1.0.24/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rocketmq5
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROCKETMQ5 Construct Library
```

### Comparing `ros-cdk-rocketmq5-1.0.23/setup.py` & `ros-cdk-rocketmq5-1.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-rocketmq5",
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
         "ros_cdk_rocketmq5",
         "ros_cdk_rocketmq5._jsii",
         "ros_cdk_rocketmq5.datasource"
     ],
     "package_data": {
         "ros_cdk_rocketmq5._jsii": [
-            "ros-cdk-rocketmq5@1.0.23.jsii.tgz"
+            "ros-cdk-rocketmq5@1.0.24.jsii.tgz"
         ],
         "ros_cdk_rocketmq5": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/__init__.py` & `ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class ConsumerGroup(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rocketmq5.ConsumerGroup",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``, which is used to create a consumer group in ApsaraMQ for RocketMQ 5.0.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosConsumerGroup``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-rocketmq5-consumergroup
     '''
 
@@ -236,15 +236,15 @@
 
 
 class Instance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rocketmq5.Instance",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ROCKETMQ5::Instance``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ROCKETMQ5::Instance``, which is used to create an ApsaraMQ for RocketMQ 5.0 instance.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosInstance``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-rocketmq5-instance
     '''
 
@@ -570,15 +570,15 @@
 
 
 class RosConsumerGroup(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rocketmq5.RosConsumerGroup",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``, which is used to create a consumer group in ApsaraMQ for RocketMQ 5.0.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ROCKETMQ5::ConsumerGroup``.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``ConsumerGroup`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-rocketmq5-consumergroup
     '''
 
@@ -949,15 +949,15 @@
 
 
 class RosInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rocketmq5.RosInstance",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ROCKETMQ5::Instance``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ROCKETMQ5::Instance``, which is used to create an ApsaraMQ for RocketMQ 5.0 instance.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Instance`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-rocketmq5-instance
     '''
```

### Comparing `ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5/datasource/__init__.py` & `ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-rocketmq5-1.0.23/src/ros_cdk_rocketmq5.egg-info/PKG-INFO` & `ros-cdk-rocketmq5-1.0.24/src/ros_cdk_rocketmq5.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rocketmq5
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROCKETMQ5 Construct Library
```

