# Comparing `tmp/cdk-events-notify-2.2.91.tar.gz` & `tmp/cdk-events-notify-2.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-events-notify-2.2.91.tar", last modified: Sat Apr  6 00:11:38 2024, max compression
+gzip compressed data, was "cdk-events-notify-2.2.92.tar", last modified: Tue Apr  9 00:13:09 2024, max compression
```

## Comparing `cdk-events-notify-2.2.91.tar` & `cdk-events-notify-2.2.92.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/cdk_events_notify/
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/cdk_events_notify/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24937 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.91.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:26.000000 cdk-events-notify-2.2.91/src/cdk_events_notify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:38.481758 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 00:11:38.000000 cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.727883 cdk-events-notify-2.2.92/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.727883 cdk-events-notify-2.2.92/src/cdk_events_notify/
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.92.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.727883 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/top_level.txt
```

### Comparing `cdk-events-notify-2.2.91/LICENSE` & `cdk-events-notify-2.2.92/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.91/PKG-INFO` & `cdk-events-notify-2.2.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.91
+Version: 2.2.92
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-events-notify-2.2.91/README.md` & `cdk-events-notify-2.2.92/README.md`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.91/setup.py` & `cdk-events-notify-2.2.92/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-events-notify",
-    "version": "2.2.91",
+    "version": "2.2.92",
     "description": "The Events Notify AWS Construct lib for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-events-notify.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_events_notify",
         "cdk_events_notify._jsii"
     ],
     "package_data": {
         "cdk_events_notify._jsii": [
-            "cdk-events-notify@2.2.91.jsii.tgz"
+            "cdk-events-notify@2.2.92.jsii.tgz"
         ],
         "cdk_events_notify": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.126.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-events-notify-2.2.91/src/cdk_events_notify/__init__.py` & `cdk-events-notify-2.2.92/src/cdk_events_notify/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.91/src/cdk_events_notify.egg-info/PKG-INFO` & `cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.91
+Version: 2.2.92
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

