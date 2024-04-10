# Comparing `tmp/ros-cdk-graphdatabase-1.0.23.tar.gz` & `tmp/ros-cdk-graphdatabase-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-graphdatabase-1.0.23.tar", last modified: Mon Mar  4 06:25:01 2024, max compression
+gzip compressed data, was "dist/ros-cdk-graphdatabase-1.0.24.tar", last modified: Wed Apr 10 03:24:06 2024, max compression
```

## Comparing `ros-cdk-graphdatabase-1.0.23.tar` & `ros-cdk-graphdatabase-1.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1332 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      209 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1980 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/
--rw-r--r--   0 root         (0) root         (0)   135281 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/_jsii/
--rw-r--r--   0 root         (0) root         (0)      439 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65338 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/_jsii/ros-cdk-graphdatabase@1.0.23.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/datasource/
--rw-r--r--   0 root         (0) root         (0)    42148 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1332 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      550 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-04 06:25:01.000000 ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      209 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/
+-rw-r--r--   0 root         (0) root         (0)   135281 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      439 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65336 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/_jsii/ros-cdk-graphdatabase@1.0.24.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/datasource/
+-rw-r--r--   0 root         (0) root         (0)    42148 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:24:05.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      550 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-10 03:24:06.000000 ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/top_level.txt
```

### Comparing `ros-cdk-graphdatabase-1.0.23/LICENSE` & `ros-cdk-graphdatabase-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-graphdatabase-1.0.23/PKG-INFO` & `ros-cdk-graphdatabase-1.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-graphdatabase
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS GRAPHDATABASE Construct Library
```

### Comparing `ros-cdk-graphdatabase-1.0.23/setup.py` & `ros-cdk-graphdatabase-1.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-graphdatabase",
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
         "ros_cdk_graphdatabase",
         "ros_cdk_graphdatabase._jsii",
         "ros_cdk_graphdatabase.datasource"
     ],
     "package_data": {
         "ros_cdk_graphdatabase._jsii": [
-            "ros-cdk-graphdatabase@1.0.23.jsii.tgz"
+            "ros-cdk-graphdatabase@1.0.24.jsii.tgz"
         ],
         "ros_cdk_graphdatabase": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/__init__.py` & `ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/_jsii/ros-cdk-graphdatabase@1.0.23.jsii.tgz` & `ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/_jsii/ros-cdk-graphdatabase@1.0.24.jsii.tgz`

 * *Files 22% similar despite different names*

#### Comparing `ros-cdk-graphdatabase@1.0.23.jsii.tgz-content` & `ros-cdk-graphdatabase@1.0.24.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'fingerprint'": "'yksA3ToerHkc/X6ZNhGeXq2+VRg9UZ1VIAbThLTATYE='", "'version'": "'1.0.24'"}*

```diff
@@ -108,15 +108,15 @@
                     "distName": "constructs",
                     "module": "constructs"
                 }
             }
         }
     },
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
-    "fingerprint": "6PPbKBji+4Cd9IFNvWejCFYkjTxFhoGjPDHPdSFgtGg=",
+    "fingerprint": "yksA3ToerHkc/X6ZNhGeXq2+VRg9UZ1VIAbThLTATYE=",
     "homepage": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "jsiiVersion": "1.85.0 (build 08ee592)",
     "license": "Apache-2.0",
     "metadata": {
         "jsii": {
             "pacmak": {
                 "hasDefaultInterfaces": true
@@ -4996,9 +4996,9 @@
                         }
                     }
                 }
             ],
             "symbolId": "lib/datasource/graphdatabase.generated:RosDbInstancesProps"
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

 * *Similarity: 0.9999854651162791%*

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

### Comparing `ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase/datasource/__init__.py` & `ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/PKG-INFO` & `ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-graphdatabase
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS GRAPHDATABASE Construct Library
```

### Comparing `ros-cdk-graphdatabase-1.0.23/src/ros_cdk_graphdatabase.egg-info/SOURCES.txt` & `ros-cdk-graphdatabase-1.0.24/src/ros_cdk_graphdatabase.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 src/ros_cdk_graphdatabase/py.typed
 src/ros_cdk_graphdatabase.egg-info/PKG-INFO
 src/ros_cdk_graphdatabase.egg-info/SOURCES.txt
 src/ros_cdk_graphdatabase.egg-info/dependency_links.txt
 src/ros_cdk_graphdatabase.egg-info/requires.txt
 src/ros_cdk_graphdatabase.egg-info/top_level.txt
 src/ros_cdk_graphdatabase/_jsii/__init__.py
-src/ros_cdk_graphdatabase/_jsii/ros-cdk-graphdatabase@1.0.23.jsii.tgz
+src/ros_cdk_graphdatabase/_jsii/ros-cdk-graphdatabase@1.0.24.jsii.tgz
 src/ros_cdk_graphdatabase/datasource/__init__.py
```

