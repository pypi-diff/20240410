# Comparing `tmp/ros-cdk-vod-1.0.23.tar.gz` & `tmp/ros-cdk-vod-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-vod-1.0.23.tar", last modified: Mon Mar  4 06:18:40 2024, max compression
+gzip compressed data, was "dist/ros-cdk-vod-1.0.24.tar", last modified: Wed Apr 10 04:11:19 2024, max compression
```

## Comparing `ros-cdk-vod-1.0.23.tar` & `ros-cdk-vod-1.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1292 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1910 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/
--rw-r--r--   0 root         (0) root         (0)    96805 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50135 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/_jsii/ros-cdk-vod@1.0.23.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/datasource/
--rw-r--r--   0 root         (0) root         (0)    16450 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:18:39.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1292 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-04 06:18:40.000000 ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1292 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/
+-rw-r--r--   0 root         (0) root         (0)    97117 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50722 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/_jsii/ros-cdk-vod@1.0.24.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/datasource/
+-rw-r--r--   0 root         (0) root         (0)    16602 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1292 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-10 04:11:19.000000 ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/top_level.txt
```

### Comparing `ros-cdk-vod-1.0.23/LICENSE` & `ros-cdk-vod-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-vod-1.0.23/PKG-INFO` & `ros-cdk-vod-1.0.24/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-vod
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS VOD Construct Library
```

### Comparing `ros-cdk-vod-1.0.23/setup.py` & `ros-cdk-vod-1.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-vod",
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
         "ros_cdk_vod",
         "ros_cdk_vod._jsii",
         "ros_cdk_vod.datasource"
     ],
     "package_data": {
         "ros_cdk_vod._jsii": [
-            "ros-cdk-vod@1.0.23.jsii.tgz"
+            "ros-cdk-vod@1.0.24.jsii.tgz"
         ],
         "ros_cdk_vod": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-vod-1.0.23/src/ros_cdk_vod/__init__.py` & `ros-cdk-vod-1.0.24/src/ros_cdk_vod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class EditingProject(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-vod.EditingProject",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::VOD::EditingProject``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::VOD::EditingProject``, which is used to create an online editing project.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosEditingProject``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-vod-editingproject
     '''
 
@@ -227,15 +227,15 @@
 
 
 class MessageCallback(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-vod.MessageCallback",
 ):
-    '''This class encapsulates and extends the ROS resource type ``ALIYUN::VOD::MessageCallback``.
+    '''This class encapsulates and extends the ROS resource type ``ALIYUN::VOD::MessageCallback``, which is used to configure the callback method, callback URL, and event types for an event notification.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosMessageCallback``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-vod-messagecallback
     '''
 
@@ -529,15 +529,15 @@
 
 
 class RosEditingProject(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-vod.RosEditingProject",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::VOD::EditingProject``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::VOD::EditingProject``, which is used to create an online editing project.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``EditingProject`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-vod-editingproject
     '''
 
@@ -797,15 +797,15 @@
 
 
 class RosMessageCallback(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-vod.RosMessageCallback",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::VOD::MessageCallback``.
+    '''This class is a base encapsulation around the ROS resource type ``ALIYUN::VOD::MessageCallback``, which is used to configure the callback method, callback URL, and event types for an event notification.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``MessageCallback`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-vod-messagecallback
     '''
```

### Comparing `ros-cdk-vod-1.0.23/src/ros_cdk_vod/datasource/__init__.py` & `ros-cdk-vod-1.0.24/src/ros_cdk_vod/datasource/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class EditingProjects(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-vod.datasource.EditingProjects",
 ):
-    '''This class encapsulates and extends the ROS resource type ``DATASOURCE::VOD::EditingProjects``.
+    '''This class encapsulates and extends the ROS resource type ``DATASOURCE::VOD::EditingProjects``, which is used to query the basic information about online editing projects.
 
     :Note:
 
     This class may have some new functions to facilitate development, so it is recommended to use this class instead of ``RosEditingProjects``for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/datasource-vod-editingprojects
     '''
 
@@ -156,15 +156,15 @@
 
 
 class RosEditingProjects(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-vod.datasource.RosEditingProjects",
 ):
-    '''This class is a base encapsulation around the ROS resource type ``DATASOURCE::VOD::EditingProjects``.
+    '''This class is a base encapsulation around the ROS resource type ``DATASOURCE::VOD::EditingProjects``, which is used to query the basic information about online editing projects.
 
     :Note:
 
     This class does not contain additional functions, so it is recommended to use the ``EditingProjects`` class instead of this class for a more convenient development experience.
     See https://www.alibabacloud.com/help/ros/developer-reference/datasource-vod-editingprojects
     '''
```

### Comparing `ros-cdk-vod-1.0.23/src/ros_cdk_vod.egg-info/PKG-INFO` & `ros-cdk-vod-1.0.24/src/ros_cdk_vod.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-vod
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS VOD Construct Library
```

