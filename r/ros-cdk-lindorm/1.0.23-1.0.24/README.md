# Comparing `tmp/ros-cdk-lindorm-1.0.23.tar.gz` & `tmp/ros-cdk-lindorm-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-lindorm-1.0.23.tar", last modified: Mon Mar  4 07:03:22 2024, max compression
+gzip compressed data, was "dist/ros-cdk-lindorm-1.0.24.tar", last modified: Wed Apr 10 04:20:55 2024, max compression
```

## Comparing `ros-cdk-lindorm-1.0.23.tar` & `ros-cdk-lindorm-1.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1938 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/
--rw-r--r--   0 root         (0) root         (0)   252931 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/_jsii/
--rw-r--r--   0 root         (0) root         (0)      427 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78536 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/_jsii/ros-cdk-lindorm@1.0.23.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/datasource/
--rw-r--r--   0 root         (0) root         (0)    36422 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-04 07:03:22.000000 ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/
+-rw-r--r--   0 root         (0) root         (0)   252931 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78536 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/_jsii/ros-cdk-lindorm@1.0.24.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/datasource/
+-rw-r--r--   0 root         (0) root         (0)    36422 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-10 04:20:55.000000 ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/top_level.txt
```

### Comparing `ros-cdk-lindorm-1.0.23/LICENSE` & `ros-cdk-lindorm-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-lindorm-1.0.23/PKG-INFO` & `ros-cdk-lindorm-1.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-lindorm
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS LINDORM Construct Library
```

### Comparing `ros-cdk-lindorm-1.0.23/setup.py` & `ros-cdk-lindorm-1.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-lindorm",
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
         "ros_cdk_lindorm",
         "ros_cdk_lindorm._jsii",
         "ros_cdk_lindorm.datasource"
     ],
     "package_data": {
         "ros_cdk_lindorm._jsii": [
-            "ros-cdk-lindorm@1.0.23.jsii.tgz"
+            "ros-cdk-lindorm@1.0.24.jsii.tgz"
         ],
         "ros_cdk_lindorm": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/__init__.py` & `ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/_jsii/ros-cdk-lindorm@1.0.23.jsii.tgz` & `ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/_jsii/ros-cdk-lindorm@1.0.24.jsii.tgz`

 * *Files 25% similar despite different names*

#### Comparing `ros-cdk-lindorm@1.0.23.jsii.tgz-content` & `ros-cdk-lindorm@1.0.24.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'fingerprint'": "'bszDOmAq0fz6sok2IRVxQsoirs/mlsupy2x0D8MHVyY='", "'version'": "'1.0.24'"}*

```diff
@@ -108,15 +108,15 @@
                     "distName": "constructs",
                     "module": "constructs"
                 }
             }
         }
     },
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
-    "fingerprint": "rZivk88oSv0Ec8KT/ldcgCC0nwXran1FBLcFziOQOZk=",
+    "fingerprint": "bszDOmAq0fz6sok2IRVxQsoirs/mlsupy2x0D8MHVyY=",
     "homepage": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "jsiiVersion": "1.85.0 (build 08ee592)",
     "license": "Apache-2.0",
     "metadata": {
         "jsii": {
             "pacmak": {
                 "hasDefaultInterfaces": true
@@ -6142,9 +6142,9 @@
                         }
                     }
                 }
             ],
             "symbolId": "lib/datasource/lindorm.generated:RosInstancesProps"
         }
     },
-    "version": "1.0.23"
+    "version": "1.0.24"
 }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'1.0.24'"}*

```diff
@@ -46,9 +46,9 @@
         "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git"
     },
     "scripts": {
         "build": "tsc",
         "pack": "npm pack"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.23"
+    "version": "1.0.24"
 }
```

##### package/tsconfig.tsbuildinfo

###### Pretty-printed

 * *Similarity: 0.9999853971962617%*

 * *Differences: {"'program'": "{'fileInfos': {'../../ros-cdk-core/lib/ros-fn.ts': {'version': "*

 * *              "'41d3375c87926e2ea29759c6c5c83ed496efb33f2fb778184b836c57c2513a19'}}}"}*

```diff
@@ -672,15 +672,15 @@
             },
             "../../ros-cdk-core/lib/ros-element.ts": {
                 "affectsGlobalScope": false,
                 "version": "c57c5f49d3cf0b6c86f5ec12045aa89e25576ee67f3c17b56a08486895e004f6"
             },
             "../../ros-cdk-core/lib/ros-fn.ts": {
                 "affectsGlobalScope": false,
-                "version": "a69455229d4fa9dd60868c79f189d3db3fe432ca274e4357838955ff443273df"
+                "version": "41d3375c87926e2ea29759c6c5c83ed496efb33f2fb778184b836c57c2513a19"
             },
             "../../ros-cdk-core/lib/ros-info.ts": {
                 "affectsGlobalScope": false,
                 "version": "3abf00c9c05f16a560a6e5fbb68bf2510945377ab97aad2d0de57fcd617d7772"
             },
             "../../ros-cdk-core/lib/ros-mapping.ts": {
                 "affectsGlobalScope": false,
```

### Comparing `ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm/datasource/__init__.py` & `ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-lindorm-1.0.23/src/ros_cdk_lindorm.egg-info/PKG-INFO` & `ros-cdk-lindorm-1.0.24/src/ros_cdk_lindorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-lindorm
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS LINDORM Construct Library
```

