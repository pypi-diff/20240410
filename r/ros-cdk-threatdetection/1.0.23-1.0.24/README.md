# Comparing `tmp/ros-cdk-threatdetection-1.0.23.tar.gz` & `tmp/ros-cdk-threatdetection-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-threatdetection-1.0.23.tar", last modified: Mon Mar  4 07:08:17 2024, max compression
+gzip compressed data, was "dist/ros-cdk-threatdetection-1.0.24.tar", last modified: Wed Apr 10 04:14:20 2024, max compression
```

## Comparing `ros-cdk-threatdetection-1.0.23.tar` & `ros-cdk-threatdetection-1.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1340 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      215 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1994 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/
--rw-r--r--   0 root         (0) root         (0)   164863 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/_jsii/
--rw-r--r--   0 root         (0) root         (0)      443 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69247 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/_jsii/ros-cdk-threatdetection@1.0.23.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/datasource/
--rw-r--r--   0 root         (0) root         (0)    29730 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:08:16.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1340 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      572 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-03-04 07:08:17.000000 ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/
+-rw-r--r--   0 root         (0) root         (0)   165097 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      443 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70420 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/_jsii/ros-cdk-threatdetection@1.0.24.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/datasource/
+-rw-r--r--   0 root         (0) root         (0)    29730 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      572 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-10 04:14:20.000000 ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/top_level.txt
```

### Comparing `ros-cdk-threatdetection-1.0.23/LICENSE` & `ros-cdk-threatdetection-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-threatdetection-1.0.23/PKG-INFO` & `ros-cdk-threatdetection-1.0.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-threatdetection
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS THREATDETECTION Construct Library
```

### Comparing `ros-cdk-threatdetection-1.0.23/setup.py` & `ros-cdk-threatdetection-1.0.24/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-threatdetection",
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
         "ros_cdk_threatdetection",
         "ros_cdk_threatdetection._jsii",
         "ros_cdk_threatdetection.datasource"
     ],
     "package_data": {
         "ros_cdk_threatdetection._jsii": [
-            "ros-cdk-threatdetection@1.0.23.jsii.tgz"
+            "ros-cdk-threatdetection@1.0.24.jsii.tgz"
         ],
         "ros_cdk_threatdetection": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/__init__.py` & `ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class AntiBruteForceRule(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-threatdetection.AntiBruteForceRule",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ThreatDetection::AntiBruteForceRule``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ThreatDetection::AntiBruteForceRule``, which is used to create a defense rule against brute-force attacks.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosAntiBruteForceRule``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-threatdetection-antibruteforcerule
     '''
 
@@ -310,15 +310,15 @@
 
 
 class Instance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-threatdetection.Instance",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ThreatDetection::Instance``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::ThreatDetection::Instance``, which is used to purchase Security Center (SAS).
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosInstance``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-threatdetection-instance
     '''
 
@@ -1140,15 +1140,15 @@
 
 
 class RosAntiBruteForceRule(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-threatdetection.RosAntiBruteForceRule",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ThreatDetection::AntiBruteForceRule``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ThreatDetection::AntiBruteForceRule``, which is used to create a defense rule against brute-force attacks.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``AntiBruteForceRule`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-threatdetection-antibruteforcerule
     '''
 
@@ -1582,15 +1582,15 @@
 
 
 class RosInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-threatdetection.RosInstance",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ThreatDetection::Instance``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::ThreatDetection::Instance``, which is used to purchase Security Center (SAS).
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``Instance`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-threatdetection-instance
     '''
```

### Comparing `ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection/datasource/__init__.py` & `ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/PKG-INFO` & `ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-threatdetection
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS THREATDETECTION Construct Library
```

### Comparing `ros-cdk-threatdetection-1.0.23/src/ros_cdk_threatdetection.egg-info/SOURCES.txt` & `ros-cdk-threatdetection-1.0.24/src/ros_cdk_threatdetection.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 src/ros_cdk_threatdetection/py.typed
 src/ros_cdk_threatdetection.egg-info/PKG-INFO
 src/ros_cdk_threatdetection.egg-info/SOURCES.txt
 src/ros_cdk_threatdetection.egg-info/dependency_links.txt
 src/ros_cdk_threatdetection.egg-info/requires.txt
 src/ros_cdk_threatdetection.egg-info/top_level.txt
 src/ros_cdk_threatdetection/_jsii/__init__.py
-src/ros_cdk_threatdetection/_jsii/ros-cdk-threatdetection@1.0.23.jsii.tgz
+src/ros_cdk_threatdetection/_jsii/ros-cdk-threatdetection@1.0.24.jsii.tgz
 src/ros_cdk_threatdetection/datasource/__init__.py
```

