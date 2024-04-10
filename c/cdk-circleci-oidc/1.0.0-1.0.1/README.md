# Comparing `tmp/cdk-circleci-oidc-1.0.0.tar.gz` & `tmp/cdk-circleci-oidc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-circleci-oidc-1.0.0.tar", last modified: Fri Apr  5 23:41:15 2024, max compression
+gzip compressed data, was "cdk-circleci-oidc-1.0.1.tar", last modified: Wed Apr 10 21:54:29 2024, max compression
```

## Comparing `cdk-circleci-oidc-1.0.0.tar` & `cdk-circleci-oidc-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    52357 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/_jsii/cdk-circleci-oidc@1.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:41:05.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:41:15.935001 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-05 23:41:15.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 23:41:15.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:41:15.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 23:41:15.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 23:41:15.000000 cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    52357 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42102 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/_jsii/cdk-circleci-oidc@1.0.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:54:18.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:54:29.694025 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-10 21:54:29.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-10 21:54:29.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:54:29.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 21:54:29.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 21:54:29.000000 cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/top_level.txt
```

### Comparing `cdk-circleci-oidc-1.0.0/LICENSE` & `cdk-circleci-oidc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-circleci-oidc-1.0.0/PKG-INFO` & `cdk-circleci-oidc-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cdk-circleci-oidc
-Version: 1.0.0
-Summary: @blimmer/cdk-circleci-oidc
+Version: 1.0.1
+Summary: AWS CDK construct to create OIDC roles for CircleCI jobs
 Home-page: https://github.com/blimmer/cdk-circleci-oidc.git
 Author: Ben Limmer<hello@benlimmer.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-circleci-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `cdk-circleci-oidc-1.0.0/README.md` & `cdk-circleci-oidc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-circleci-oidc-1.0.0/setup.py` & `cdk-circleci-oidc-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-circleci-oidc",
-    "version": "1.0.0",
-    "description": "@blimmer/cdk-circleci-oidc",
+    "version": "1.0.1",
+    "description": "AWS CDK construct to create OIDC roles for CircleCI jobs",
     "license": "Apache-2.0",
     "url": "https://github.com/blimmer/cdk-circleci-oidc.git",
     "long_description_content_type": "text/markdown",
     "author": "Ben Limmer<hello@benlimmer.com>",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_circleci_oidc",
         "cdk_circleci_oidc._jsii"
     ],
     "package_data": {
         "cdk_circleci_oidc._jsii": [
-            "cdk-circleci-oidc@1.0.0.jsii.tgz"
+            "cdk-circleci-oidc@1.0.1.jsii.tgz"
         ],
         "cdk_circleci_oidc": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc/__init__.py` & `cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-circleci-oidc-1.0.0/src/cdk_circleci_oidc.egg-info/PKG-INFO` & `cdk-circleci-oidc-1.0.1/src/cdk_circleci_oidc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cdk-circleci-oidc
-Version: 1.0.0
-Summary: @blimmer/cdk-circleci-oidc
+Version: 1.0.1
+Summary: AWS CDK construct to create OIDC roles for CircleCI jobs
 Home-page: https://github.com/blimmer/cdk-circleci-oidc.git
 Author: Ben Limmer<hello@benlimmer.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-circleci-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

