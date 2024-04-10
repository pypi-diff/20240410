# Comparing `tmp/botocore-a-la-carte-apigateway-1.34.80.tar.gz` & `tmp/botocore-a-la-carte-apigateway-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-apigateway-1.34.80.tar", last modified: Tue Apr  9 01:00:33 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-apigateway-1.34.9.tar", last modified: Thu Dec 28 01:06:36 2023, max compression
```

## Comparing `botocore-a-la-carte-apigateway-1.34.80.tar` & `botocore-a-la-carte-apigateway-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:33.024026 botocore-a-la-carte-apigateway-1.34.80/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 01:00:32.000000 botocore-a-la-carte-apigateway-1.34.80/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 01:00:33.020026 botocore-a-la-carte-apigateway-1.34.80/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:33.020026 botocore-a-la-carte-apigateway-1.34.80/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:33.020026 botocore-a-la-carte-apigateway-1.34.80/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:33.020026 botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:33.020026 botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/
--rw-r--r--   0 runner    (1001) docker     (127)    13742 2024-04-09 01:00:23.000000 botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 01:00:23.000000 botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-09 01:00:23.000000 botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   308833 2024-04-09 01:00:23.000000 botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:33.020026 botocore-a-la-carte-apigateway-1.34.80/botocore_a_la_carte_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 01:00:32.000000 botocore-a-la-carte-apigateway-1.34.80/botocore_a_la_carte_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 01:00:32.000000 botocore-a-la-carte-apigateway-1.34.80/botocore_a_la_carte_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:00:32.000000 botocore-a-la-carte-apigateway-1.34.80/botocore_a_la_carte_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:00:32.000000 botocore-a-la-carte-apigateway-1.34.80/botocore_a_la_carte_apigateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:00:33.024026 botocore-a-la-carte-apigateway-1.34.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-09 01:00:32.000000 botocore-a-la-carte-apigateway-1.34.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigateway-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/
+-rw-r--r--   0 runner    (1001) docker     (127)    13742 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   308498 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/botocore_a_la_carte_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigateway-1.34.9/botocore_a_la_carte_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigateway-1.34.9/botocore_a_la_carte_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigateway-1.34.9/botocore_a_la_carte_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigateway-1.34.9/botocore_a_la_carte_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:36.846241 botocore-a-la-carte-apigateway-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigateway-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-apigateway-1.34.80/LICENSE.txt` & `botocore-a-la-carte-apigateway-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-apigateway-1.34.80/PKG-INFO` & `botocore-a-la-carte-apigateway-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-apigateway
-Version: 1.34.80
+Version: 1.34.9
 Summary: apigateway data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/endpoint-rule-set-1.json` & `botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/endpoint-rule-set-1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999991069387288%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {1: {'rules': {0: {'conditions': {0: {'argv': {insert: "*

 * *            "[(1, OrderedDict([('fn', 'getAttr'), ('argv', [OrderedDict([('ref', "*

 * *            "'PartitionResult')]), 'supportsFIPS'])]))], delete: [0]}}}}}}}}}}}"}*

```diff
@@ -198,24 +198,24 @@
                                 }
                             ],
                             "rules": [
                                 {
                                     "conditions": [
                                         {
                                             "argv": [
+                                                true,
                                                 {
                                                     "argv": [
                                                         {
                                                             "ref": "PartitionResult"
                                                         },
                                                         "supportsFIPS"
                                                     ],
                                                     "fn": "getAttr"
-                                                },
-                                                true
+                                                }
                                             ],
                                             "fn": "booleanEquals"
                                         }
                                     ],
                                     "rules": [
                                         {
                                             "conditions": [],
```

### Comparing `botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/paginators-1.json` & `botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-apigateway-1.34.80/botocore/data/apigateway/2015-07-09/service-2.json` & `botocore-a-la-carte-apigateway-1.34.9/botocore/data/apigateway/2015-07-09/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999640499488599%*

 * *Differences: {"'operations'": "{'UpdateModel': {'documentation': '<p>Changes information about a model.</p>'}}",*

 * * "'shapes'": "{'CreateModelRequest': {'members': {'schema': {'documentation': '<p>The schema for "*

 * *             'the model. For <code>application/json</code> models, this should be JSON schema '*

 * *             "draft 4 model.</p>'}}}, 'MethodSetting': {'members': {'dataTraceEnabled': "*

 * *             "{'documentation': '<p>Specifies whether data trace logging is enabled for this "*

 * *             "method, which affe […]*

```diff
@@ -3453,15 +3453,15 @@
             },
             "name": "UpdateMethodResponse",
             "output": {
                 "shape": "MethodResponse"
             }
         },
         "UpdateModel": {
-            "documentation": "<p>Changes information about a model. The maximum size of the model is 400 KB.</p>",
+            "documentation": "<p>Changes information about a model.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
                     "shape": "ConflictException"
                 },
@@ -4407,15 +4407,15 @@
                 "restApiId": {
                     "documentation": "<p>The RestApi identifier under which the Model will be created.</p>",
                     "location": "uri",
                     "locationName": "restapi_id",
                     "shape": "String"
                 },
                 "schema": {
-                    "documentation": "<p>The schema for the model. For <code>application/json</code> models, this should be JSON schema draft 4 model. The maximum size of the model is 400 KB.</p>",
+                    "documentation": "<p>The schema for the model. For <code>application/json</code> models, this should be JSON schema draft 4 model.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "restApiId",
                 "name",
                 "contentType"
@@ -7290,15 +7290,15 @@
                     "shape": "Integer"
                 },
                 "cachingEnabled": {
                     "documentation": "<p>Specifies whether responses should be cached and returned for requests. A cache cluster must be enabled on the stage for responses to be cached.</p>",
                     "shape": "Boolean"
                 },
                 "dataTraceEnabled": {
-                    "documentation": "<p>Specifies whether data trace logging is enabled for this method, which affects the log entries pushed to Amazon CloudWatch Logs. This can be useful to troubleshoot APIs, but can result in logging sensitive data. We recommend that you don't enable this option for production APIs.</p>",
+                    "documentation": "<p>Specifies whether data trace logging is enabled for this method, which affects the log entries pushed to Amazon CloudWatch Logs.</p>",
                     "shape": "Boolean"
                 },
                 "loggingLevel": {
                     "documentation": "<p>Specifies the logging level for this method, which affects the log entries pushed to Amazon CloudWatch Logs. Valid values are <code>OFF</code>, <code>ERROR</code>, and <code>INFO</code>. Choose <code>ERROR</code> to write only error-level entries to CloudWatch Logs, or choose <code>INFO</code> to include all <code>ERROR</code> events as well as extra informational events.</p>",
                     "shape": "String"
                 },
                 "metricsEnabled": {
@@ -8090,15 +8090,15 @@
             "documentation": "<p>Represents a unique identifier for a version of a deployed RestApi that is callable by users.</p>",
             "members": {
                 "accessLogSettings": {
                     "documentation": "<p>Settings for logging access in this stage.</p>",
                     "shape": "AccessLogSettings"
                 },
                 "cacheClusterEnabled": {
-                    "documentation": "<p>Specifies whether a cache cluster is enabled for the stage. To activate a method-level cache, set <code>CachingEnabled</code> to <code>true</code> for a method. </p>",
+                    "documentation": "<p>Specifies whether a cache cluster is enabled for the stage.</p>",
                     "shape": "Boolean"
                 },
                 "cacheClusterSize": {
                     "documentation": "<p>The stage's cache capacity in GB. For more information about choosing a cache size, see <a href=\"https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-caching.html\">Enabling API caching to enhance responsiveness</a>.</p>",
                     "shape": "CacheClusterSize"
                 },
                 "cacheClusterStatus": {
```

### Comparing `botocore-a-la-carte-apigateway-1.34.80/botocore_a_la_carte_apigateway.egg-info/PKG-INFO` & `botocore-a-la-carte-apigateway-1.34.9/botocore_a_la_carte_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-apigateway
-Version: 1.34.80
+Version: 1.34.9
 Summary: apigateway data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-apigateway-1.34.80/setup.py` & `botocore-a-la-carte-apigateway-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-apigateway',
-    version="1.34.80",
+    version="1.34.9",
     description='apigateway data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/apigateway/*/*.json'],
```

