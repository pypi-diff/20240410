# Comparing `tmp/alma-cdk.project-1.0.0b5.tar.gz` & `tmp/alma-cdk.project-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alma-cdk.project-1.0.0b5.tar", last modified: Thu Mar 21 14:43:23 2024, max compression
+gzip compressed data, was "alma-cdk.project-1.0.0b6.tar", last modified: Wed Apr 10 13:31:07 2024, max compression
```

## Comparing `alma-cdk.project-1.0.0b5.tar` & `alma-cdk.project-1.0.0b6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:43:23.676597 alma-cdk.project-1.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-03-21 14:43:23.676597 alma-cdk.project-1.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 14:43:23.676597 alma-cdk.project-1.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:43:23.672598 alma-cdk.project-1.0.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:43:23.672598 alma-cdk.project-1.0.0b5/src/alma_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:43:23.676597 alma-cdk.project-1.0.0b5/src/alma_cdk/project/
--rw-r--r--   0 runner    (1001) docker     (127)   124020 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/src/alma_cdk/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:43:23.676597 alma-cdk.project-1.0.0b5/src/alma_cdk/project/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/src/alma_cdk/project/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   317141 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/src/alma_cdk/project/_jsii/project@1.0.0-beta.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 14:43:11.000000 alma-cdk.project-1.0.0b5/src/alma_cdk/project/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:43:23.672598 alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-03-21 14:43:23.000000 alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-21 14:43:23.000000 alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 14:43:23.000000 alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-21 14:43:23.000000 alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 14:43:23.000000 alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:31:07.002326 alma-cdk.project-1.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-10 13:31:07.002326 alma-cdk.project-1.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:31:07.002326 alma-cdk.project-1.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:31:06.998326 alma-cdk.project-1.0.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:31:06.998326 alma-cdk.project-1.0.0b6/src/alma_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:31:07.002326 alma-cdk.project-1.0.0b6/src/alma_cdk/project/
+-rw-r--r--   0 runner    (1001) docker     (127)   124019 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/src/alma_cdk/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:31:07.002326 alma-cdk.project-1.0.0b6/src/alma_cdk/project/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/src/alma_cdk/project/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   317131 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/src/alma_cdk/project/_jsii/project@1.0.0-beta.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:30:55.000000 alma-cdk.project-1.0.0b6/src/alma_cdk/project/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:31:07.002326 alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-10 13:31:06.000000 alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 13:31:06.000000 alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:31:06.000000 alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 13:31:06.000000 alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 13:31:06.000000 alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/top_level.txt
```

### Comparing `alma-cdk.project-1.0.0b5/LICENSE` & `alma-cdk.project-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `alma-cdk.project-1.0.0b5/PKG-INFO` & `alma-cdk.project-1.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alma-cdk.project
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: Opinionated CDK Project “Framework”
 Home-page: https://github.com/alma-cdk/project.git
 Author: Alma Media<opensource@almamedia.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/alma-cdk/project.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -126,15 +126,15 @@
    ```python
    // lib/my-stack.ts
    import { Construct } from 'constructs';
    import { StackProps, RemovalPolicy } from 'aws-cdk-lib';
    import { SmartStack, Name, UrlName, PathName, EC } from '@alma-cdk/project';
 
    export class MyStack extends SmartStack {
-     constructor(scope: Construct, id: string, props?: StackProps) {
+     constructor(scope: Construct, id: string, props: StackProps) {
        super(scope, id, props);
 
        new dynamodb.Table(this, 'Table', {
          removalPolicy: EC.isStable(this) ? RemovalPolicy.RETAIN : RemovalPolicy.DESTROY,
 
          tableName: Name.it(this, 'MyTable'),
          partitionKey: {
```

### Comparing `alma-cdk.project-1.0.0b5/README.md` & `alma-cdk.project-1.0.0b6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
    ```python
    // lib/my-stack.ts
    import { Construct } from 'constructs';
    import { StackProps, RemovalPolicy } from 'aws-cdk-lib';
    import { SmartStack, Name, UrlName, PathName, EC } from '@alma-cdk/project';
 
    export class MyStack extends SmartStack {
-     constructor(scope: Construct, id: string, props?: StackProps) {
+     constructor(scope: Construct, id: string, props: StackProps) {
        super(scope, id, props);
 
        new dynamodb.Table(this, 'Table', {
          removalPolicy: EC.isStable(this) ? RemovalPolicy.RETAIN : RemovalPolicy.DESTROY,
 
          tableName: Name.it(this, 'MyTable'),
          partitionKey: {
```

### Comparing `alma-cdk.project-1.0.0b5/setup.py` & `alma-cdk.project-1.0.0b6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "alma-cdk.project",
-    "version": "1.0.0.b5",
+    "version": "1.0.0.b6",
     "description": "Opinionated CDK Project “Framework”",
     "license": "Apache-2.0",
     "url": "https://github.com/alma-cdk/project.git",
     "long_description_content_type": "text/markdown",
     "author": "Alma Media<opensource@almamedia.dev>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "alma_cdk.project",
         "alma_cdk.project._jsii"
     ],
     "package_data": {
         "alma_cdk.project._jsii": [
-            "project@1.0.0-beta.5.jsii.tgz"
+            "project@1.0.0-beta.6.jsii.tgz"
         ],
         "alma_cdk.project": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `alma-cdk.project-1.0.0b5/src/alma_cdk/project/__init__.py` & `alma-cdk.project-1.0.0b6/src/alma_cdk/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
    ```python
    // lib/my-stack.ts
    import { Construct } from 'constructs';
    import { StackProps, RemovalPolicy } from 'aws-cdk-lib';
    import { SmartStack, Name, UrlName, PathName, EC } from '@alma-cdk/project';
 
    export class MyStack extends SmartStack {
-     constructor(scope: Construct, id: string, props?: StackProps) {
+     constructor(scope: Construct, id: string, props: StackProps) {
        super(scope, id, props);
 
        new dynamodb.Table(this, 'Table', {
          removalPolicy: EC.isStable(this) ? RemovalPolicy.RETAIN : RemovalPolicy.DESTROY,
 
          tableName: Name.it(this, 'MyTable'),
          partitionKey: {
```

### Comparing `alma-cdk.project-1.0.0b5/src/alma_cdk.project.egg-info/PKG-INFO` & `alma-cdk.project-1.0.0b6/src/alma_cdk.project.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alma-cdk.project
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: Opinionated CDK Project “Framework”
 Home-page: https://github.com/alma-cdk/project.git
 Author: Alma Media<opensource@almamedia.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/alma-cdk/project.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -126,15 +126,15 @@
    ```python
    // lib/my-stack.ts
    import { Construct } from 'constructs';
    import { StackProps, RemovalPolicy } from 'aws-cdk-lib';
    import { SmartStack, Name, UrlName, PathName, EC } from '@alma-cdk/project';
 
    export class MyStack extends SmartStack {
-     constructor(scope: Construct, id: string, props?: StackProps) {
+     constructor(scope: Construct, id: string, props: StackProps) {
        super(scope, id, props);
 
        new dynamodb.Table(this, 'Table', {
          removalPolicy: EC.isStable(this) ? RemovalPolicy.RETAIN : RemovalPolicy.DESTROY,
 
          tableName: Name.it(this, 'MyTable'),
          partitionKey: {
```

