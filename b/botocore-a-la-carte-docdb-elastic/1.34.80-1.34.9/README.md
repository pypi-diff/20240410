# Comparing `tmp/botocore-a-la-carte-docdb-elastic-1.34.80.tar.gz` & `tmp/botocore-a-la-carte-docdb-elastic-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-docdb-elastic-1.34.80.tar", last modified: Tue Apr  9 01:00:43 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-docdb-elastic-1.34.9.tar", last modified: Thu Dec 28 01:06:45 2023, max compression
```

## Comparing `botocore-a-la-carte-docdb-elastic-1.34.80.tar` & `botocore-a-la-carte-docdb-elastic-1.34.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 01:00:42.000000 botocore-a-la-carte-docdb-elastic-1.34.80/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/2022-11-28/
--rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-04-09 01:00:23.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/2022-11-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 01:00:23.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/2022-11-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    52875 2024-04-09 01:00:23.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/2022-11-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/botocore_a_la_carte_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-09 01:00:43.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore_a_la_carte_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 01:00:43.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore_a_la_carte_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:00:43.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore_a_la_carte_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:00:43.000000 botocore-a-la-carte-docdb-elastic-1.34.80/botocore_a_la_carte_docdb_elastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:00:43.112125 botocore-a-la-carte-docdb-elastic-1.34.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 01:00:42.000000 botocore-a-la-carte-docdb-elastic-1.34.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:44.000000 botocore-a-la-carte-docdb-elastic-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/2022-11-28/
+-rw-r--r--   0 runner    (1001) docker     (127)    17652 2023-12-28 01:06:26.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/2022-11-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-28 01:06:26.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/2022-11-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39463 2023-12-28 01:06:26.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/2022-11-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/botocore_a_la_carte_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-28 01:06:45.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore_a_la_carte_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-28 01:06:45.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore_a_la_carte_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:45.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore_a_la_carte_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:45.000000 botocore-a-la-carte-docdb-elastic-1.34.9/botocore_a_la_carte_docdb_elastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:45.154305 botocore-a-la-carte-docdb-elastic-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-28 01:06:44.000000 botocore-a-la-carte-docdb-elastic-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-docdb-elastic-1.34.80/LICENSE.txt` & `botocore-a-la-carte-docdb-elastic-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-docdb-elastic-1.34.80/PKG-INFO` & `botocore-a-la-carte-docdb-elastic-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-docdb-elastic
-Version: 1.34.80
+Version: 1.34.9
 Summary: docdb-elastic data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/2022-11-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/2022-11-28/endpoint-rule-set-1.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999888367341%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {0: {'rules': {1: {'rules': {0: {'conditions': {0: "*

 * *            "{'argv': {insert: [(1, OrderedDict([('fn', 'getAttr'), ('argv', [OrderedDict([('ref', "*

 * *            "'PartitionResult')]), 'supportsFIPS'])]))], delete: [0]}}}}}}}}}}}}}"}*

```diff
@@ -213,24 +213,24 @@
                                         }
                                     ],
                                     "rules": [
                                         {
                                             "conditions": [
                                                 {
                                                     "argv": [
+                                                        true,
                                                         {
                                                             "argv": [
                                                                 {
                                                                     "ref": "PartitionResult"
                                                                 },
                                                                 "supportsFIPS"
                                                             ],
                                                             "fn": "getAttr"
-                                                        },
-                                                        true
+                                                        }
                                                     ],
                                                     "fn": "booleanEquals"
                                                 }
                                             ],
                                             "rules": [
                                                 {
                                                     "conditions": [],
```

### Comparing `botocore-a-la-carte-docdb-elastic-1.34.80/botocore/data/docdb-elastic/2022-11-28/service-2.json` & `botocore-a-la-carte-docdb-elastic-1.34.9/botocore/data/docdb-elastic/2022-11-28/service-2.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8609659532474744%*

 * *Differences: {"'documentation'": "'<p>The new Amazon Elastic DocumentDB service endpoint.</p>'",*

 * * "'operations'": "{'CreateCluster': {'documentation': '<p>Creates a new Elastic DocumentDB cluster "*

 * *                 "and returns its Cluster structure.</p>'}, 'CreateClusterSnapshot': "*

 * *                 "{'documentation': '<p>Creates a snapshot of a cluster.</p>'}, 'DeleteCluster': "*

 * *                 "{'documentation': '<p>Delete a Elastic DocumentDB cluster.</p>'}, "*

 * *                 "'DeleteClusterSnapshot': {'documentat […]*

```diff
@@ -1,63 +1,24 @@
 {
-    "documentation": "<p><fullname>Amazon DocumentDB elastic clusters</fullname> <p>Amazon DocumentDB elastic-clusters support workloads with millions of reads/writes per second and petabytes of storage capacity. Amazon DocumentDB elastic clusters also simplify how developers interact with Amazon DocumentDB elastic-clusters by eliminating the need to choose, manage or upgrade instances.</p> <p>Amazon DocumentDB elastic-clusters were created to:</p> <ul> <li> <p>provide a solution for customers looking for a database that provides virtually limitless scale with rich query capabilities and MongoDB API compatibility.</p> </li> <li> <p>give customers higher connection limits, and to reduce downtime from patching.</p> </li> <li> <p>continue investing in a cloud-native, elastic, and class leading architecture for JSON workloads.</p> </li> </ul></p>",
+    "documentation": "<p>The new Amazon Elastic DocumentDB service endpoint.</p>",
     "metadata": {
         "apiVersion": "2022-11-28",
         "endpointPrefix": "docdb-elastic",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceAbbreviation": "DocDB Elastic",
         "serviceFullName": "Amazon DocumentDB Elastic Clusters",
         "serviceId": "DocDB Elastic",
         "signatureVersion": "v4",
         "signingName": "docdb-elastic",
         "uid": "docdb-elastic-2022-11-28"
     },
     "operations": {
-        "CopyClusterSnapshot": {
-            "documentation": "<p>Copies a snapshot of an elastic cluster.</p>",
-            "errors": [
-                {
-                    "shape": "ThrottlingException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "ServiceQuotaExceededException"
-                },
-                {
-                    "shape": "ConflictException"
-                },
-                {
-                    "shape": "InternalServerException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/cluster-snapshot/{snapshotArn}/copy",
-                "responseCode": 200
-            },
-            "idempotent": true,
-            "input": {
-                "shape": "CopyClusterSnapshotInput"
-            },
-            "name": "CopyClusterSnapshot",
-            "output": {
-                "shape": "CopyClusterSnapshotOutput"
-            }
-        },
         "CreateCluster": {
-            "documentation": "<p>Creates a new Amazon DocumentDB elastic cluster and returns its cluster structure.</p>",
+            "documentation": "<p>Creates a new Elastic DocumentDB cluster and returns its Cluster structure.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -85,15 +46,15 @@
             },
             "name": "CreateCluster",
             "output": {
                 "shape": "CreateClusterOutput"
             }
         },
         "CreateClusterSnapshot": {
-            "documentation": "<p>Creates a snapshot of an elastic cluster.</p>",
+            "documentation": "<p>Creates a snapshot of a cluster.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -124,15 +85,15 @@
             },
             "name": "CreateClusterSnapshot",
             "output": {
                 "shape": "CreateClusterSnapshotOutput"
             }
         },
         "DeleteCluster": {
-            "documentation": "<p>Delete an elastic cluster.</p>",
+            "documentation": "<p>Delete a Elastic DocumentDB cluster.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -160,15 +121,15 @@
             },
             "name": "DeleteCluster",
             "output": {
                 "shape": "DeleteClusterOutput"
             }
         },
         "DeleteClusterSnapshot": {
-            "documentation": "<p>Delete an elastic cluster snapshot.</p>",
+            "documentation": "<p>Delete a Elastic DocumentDB snapshot.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -196,15 +157,15 @@
             },
             "name": "DeleteClusterSnapshot",
             "output": {
                 "shape": "DeleteClusterSnapshotOutput"
             }
         },
         "GetCluster": {
-            "documentation": "<p>Returns information about a specific elastic cluster.</p>",
+            "documentation": "<p>Returns information about a specific Elastic DocumentDB cluster.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -228,15 +189,15 @@
             },
             "name": "GetCluster",
             "output": {
                 "shape": "GetClusterOutput"
             }
         },
         "GetClusterSnapshot": {
-            "documentation": "<p>Returns information about a specific elastic cluster snapshot</p>",
+            "documentation": "<p>Returns information about a specific Elastic DocumentDB snapshot</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -260,15 +221,15 @@
             },
             "name": "GetClusterSnapshot",
             "output": {
                 "shape": "GetClusterSnapshotOutput"
             }
         },
         "ListClusterSnapshots": {
-            "documentation": "<p>Returns information about snapshots for a specified elastic cluster.</p>",
+            "documentation": "<p>Returns information about Elastic DocumentDB snapshots for a specified cluster.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -289,15 +250,15 @@
             },
             "name": "ListClusterSnapshots",
             "output": {
                 "shape": "ListClusterSnapshotsOutput"
             }
         },
         "ListClusters": {
-            "documentation": "<p>Returns information about provisioned Amazon DocumentDB elastic clusters.</p>",
+            "documentation": "<p>Returns information about provisioned Elastic DocumentDB clusters.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -318,15 +279,15 @@
             },
             "name": "ListClusters",
             "output": {
                 "shape": "ListClustersOutput"
             }
         },
         "ListTagsForResource": {
-            "documentation": "<p>Lists all tags on a elastic cluster resource</p>",
+            "documentation": "<p>Lists all tags on a Elastic DocumentDB resource</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -347,15 +308,15 @@
             },
             "name": "ListTagsForResource",
             "output": {
                 "shape": "ListTagsForResourceResponse"
             }
         },
         "RestoreClusterFromSnapshot": {
-            "documentation": "<p>Restores an elastic cluster from a snapshot.</p>",
+            "documentation": "<p>Restores a Elastic DocumentDB cluster from a snapshot.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -385,82 +346,16 @@
                 "shape": "RestoreClusterFromSnapshotInput"
             },
             "name": "RestoreClusterFromSnapshot",
             "output": {
                 "shape": "RestoreClusterFromSnapshotOutput"
             }
         },
-        "StartCluster": {
-            "documentation": "<p>Restarts the stopped elastic cluster that is specified by <code>clusterARN</code>.</p>",
-            "errors": [
-                {
-                    "shape": "ThrottlingException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "InternalServerException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/cluster/{clusterArn}/start",
-                "responseCode": 200
-            },
-            "idempotent": true,
-            "input": {
-                "shape": "StartClusterInput"
-            },
-            "name": "StartCluster",
-            "output": {
-                "shape": "StartClusterOutput"
-            }
-        },
-        "StopCluster": {
-            "documentation": "<p>Stops the running elastic cluster that is specified by <code>clusterArn</code>. The elastic cluster must be in the <i>available</i> state. </p>",
-            "errors": [
-                {
-                    "shape": "ThrottlingException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "InternalServerException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/cluster/{clusterArn}/stop",
-                "responseCode": 200
-            },
-            "idempotent": true,
-            "input": {
-                "shape": "StopClusterInput"
-            },
-            "name": "StopCluster",
-            "output": {
-                "shape": "StopClusterOutput"
-            }
-        },
         "TagResource": {
-            "documentation": "<p>Adds metadata tags to an elastic cluster resource</p>",
+            "documentation": "<p>Adds metadata tags to a Elastic DocumentDB resource</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -481,15 +376,15 @@
             },
             "name": "TagResource",
             "output": {
                 "shape": "TagResourceResponse"
             }
         },
         "UntagResource": {
-            "documentation": "<p>Removes metadata tags from an elastic cluster resource</p>",
+            "documentation": "<p>Removes metadata tags to a Elastic DocumentDB resource</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -511,15 +406,15 @@
             },
             "name": "UntagResource",
             "output": {
                 "shape": "UntagResourceResponse"
             }
         },
         "UpdateCluster": {
-            "documentation": "<p>Modifies an elastic cluster. This includes updating admin-username/password, upgrading the API version, and setting up a backup window and maintenance window</p>",
+            "documentation": "<p>Modifies a Elastic DocumentDB cluster. This includes updating admin-username/password, upgrading API version setting up a backup window and maintenance window</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -578,87 +473,67 @@
         "Auth": {
             "enum": [
                 "PLAIN_TEXT",
                 "SECRET_ARN"
             ],
             "type": "string"
         },
-        "Boolean": {
-            "box": true,
-            "type": "boolean"
-        },
         "Cluster": {
-            "documentation": "<p>Returns information about a specific elastic cluster.</p>",
+            "documentation": "<p>Returns information about a specific Elastic DocumentDB cluster.</p>",
             "members": {
                 "adminUserName": {
-                    "documentation": "<p>The name of the elastic cluster administrator.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB cluster administrator.</p>",
                     "shape": "String"
                 },
                 "authType": {
-                    "documentation": "<p>The authentication type for the elastic cluster.</p>",
+                    "documentation": "<p>The authentication type for the Elastic DocumentDB cluster.</p>",
                     "shape": "Auth"
                 },
-                "backupRetentionPeriod": {
-                    "documentation": "<p>The number of days for which automatic snapshots are retained.</p>",
-                    "shape": "Integer"
-                },
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "clusterEndpoint": {
-                    "documentation": "<p>The URL used to connect to the elastic cluster.</p>",
+                    "documentation": "<p>The URL used to connect to the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "clusterName": {
-                    "documentation": "<p>The name of the elastic cluster.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "createTime": {
-                    "documentation": "<p>The time when the elastic cluster was created in Universal Coordinated Time (UTC).</p>",
+                    "documentation": "<p>The time when the Elastic DocumentDB cluster was created in Universal Coordinated Time (UTC).</p>",
                     "shape": "String"
                 },
                 "kmsKeyId": {
-                    "documentation": "<p>The KMS key identifier to use to encrypt the elastic cluster.</p>",
-                    "shape": "String"
-                },
-                "preferredBackupWindow": {
-                    "documentation": "<p>The daily time range during which automated backups are created if automated backups are enabled, as determined by <code>backupRetentionPeriod</code>.</p>",
+                    "documentation": "<p>The KMS key identifier to use to encrypt the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "preferredMaintenanceWindow": {
                     "documentation": "<p>The weekly time range during which system maintenance can occur, in Universal Coordinated Time (UTC).</p> <p> <i>Format</i>: <code>ddd:hh24:mi-ddd:hh24:mi</code> </p>",
                     "shape": "String"
                 },
                 "shardCapacity": {
-                    "documentation": "<p>The number of vCPUs assigned to each elastic cluster shard. Maximum is 64. Allowed values are 2, 4, 8, 16, 32, 64.</p>",
+                    "documentation": "<p>The capacity of each shard in the Elastic DocumentDB cluster.</p>",
                     "shape": "Integer"
                 },
                 "shardCount": {
-                    "documentation": "<p>The number of shards assigned to the elastic cluster. Maximum is 32.</p>",
+                    "documentation": "<p>The number of shards in the Elastic DocumentDB cluster.</p>",
                     "shape": "Integer"
                 },
-                "shardInstanceCount": {
-                    "documentation": "<p>The number of replica instances applying to all shards in the cluster. A <code>shardInstanceCount</code> value of 1 means there is one writer instance, and any additional instances are replicas that can be used for reads and to improve availability.</p>",
-                    "shape": "Integer"
-                },
-                "shards": {
-                    "documentation": "<p>The total number of shards in the cluster.</p>",
-                    "shape": "ShardList"
-                },
                 "status": {
-                    "documentation": "<p>The status of the elastic cluster.</p>",
+                    "documentation": "<p>The status of the Elastic DocumentDB cluster.</p>",
                     "shape": "Status"
                 },
                 "subnetIds": {
-                    "documentation": "<p>The Amazon EC2 subnet IDs for the elastic cluster.</p>",
+                    "documentation": "<p>The Amazon EC2 subnet IDs for the Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 },
                 "vpcSecurityGroupIds": {
-                    "documentation": "<p>A list of EC2 VPC security groups associated with thie elastic cluster.</p>",
+                    "documentation": "<p>A list of EC2 VPC security groups associated with this cluster.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "adminUserName",
                 "authType",
                 "clusterArn",
@@ -672,26 +547,26 @@
                 "status",
                 "subnetIds",
                 "vpcSecurityGroupIds"
             ],
             "type": "structure"
         },
         "ClusterInList": {
-            "documentation": "<p>A list of Amazon DocumentDB elastic clusters.</p>",
+            "documentation": "<p>A list of Elastic DocumentDB cluster.</p>",
             "members": {
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "clusterName": {
-                    "documentation": "<p>The name of the elastic cluster.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "status": {
-                    "documentation": "<p>The status of the elastic cluster.</p>",
+                    "documentation": "<p>The status of the Elastic DocumentDB cluster.</p>",
                     "shape": "Status"
                 }
             },
             "required": [
                 "clusterArn",
                 "clusterName",
                 "status"
@@ -701,58 +576,54 @@
         "ClusterList": {
             "member": {
                 "shape": "ClusterInList"
             },
             "type": "list"
         },
         "ClusterSnapshot": {
-            "documentation": "<p>Returns information about a specific elastic cluster snapshot.</p>",
+            "documentation": "<p>Returns information about a specific Elastic DocumentDB snapshot.</p>",
             "members": {
                 "adminUserName": {
-                    "documentation": "<p>The name of the elastic cluster administrator.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB cluster administrator.</p>",
                     "shape": "String"
                 },
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "clusterCreationTime": {
-                    "documentation": "<p>The time when the elastic cluster was created in Universal Coordinated Time (UTC).</p>",
+                    "documentation": "<p>The time when the Elastic DocumentDB cluster was created in Universal Coordinated Time (UTC).</p>",
                     "shape": "String"
                 },
                 "kmsKeyId": {
-                    "documentation": "<p>The KMS key identifier is the Amazon Resource Name (ARN) for the KMS encryption key. If you are creating a cluster using the same Amazon account that owns this KMS encryption key, you can use the KMS key alias instead of the ARN as the KMS encryption key. If an encryption key is not specified here, Amazon DocumentDB uses the default encryption key that KMS creates for your account. Your account has a different default encryption key for each Amazon Region. </p>",
+                    "documentation": "<p>The KMS key identifier to use to encrypt the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "snapshotArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB snapshot</p>",
                     "shape": "String"
                 },
                 "snapshotCreationTime": {
-                    "documentation": "<p>The time when the elastic cluster snapshot was created in Universal Coordinated Time (UTC).</p>",
+                    "documentation": "<p>The time when the Elastic DocumentDB snapshot was created in Universal Coordinated Time (UTC).</p>",
                     "shape": "String"
                 },
                 "snapshotName": {
-                    "documentation": "<p>The name of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB snapshot.</p>",
                     "shape": "String"
                 },
-                "snapshotType": {
-                    "documentation": "<p>The type of cluster snapshots to be returned. You can specify one of the following values:</p> <ul> <li> <p> <code>automated</code> - Return all cluster snapshots that Amazon DocumentDB has automatically created for your Amazon Web Services account.</p> </li> <li> <p> <code>manual</code> - Return all cluster snapshots that you have manually created for your Amazon Web Services account.</p> </li> </ul>",
-                    "shape": "SnapshotType"
-                },
                 "status": {
-                    "documentation": "<p>The status of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The status of the Elastic DocumentDB snapshot.</p>",
                     "shape": "Status"
                 },
                 "subnetIds": {
-                    "documentation": "<p>The Amazon EC2 subnet IDs for the elastic cluster.</p>",
+                    "documentation": "<p>A list of the IDs of subnets associated with the DB cluster snapshot.</p>",
                     "shape": "StringList"
                 },
                 "vpcSecurityGroupIds": {
-                    "documentation": "<p>A list of EC2 VPC security groups to associate with the elastic cluster.</p>",
+                    "documentation": "<p>A list of the IDs of the VPC security groups associated with the cluster snapshot.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "adminUserName",
                 "clusterArn",
                 "clusterCreationTime",
@@ -763,34 +634,34 @@
                 "status",
                 "subnetIds",
                 "vpcSecurityGroupIds"
             ],
             "type": "structure"
         },
         "ClusterSnapshotInList": {
-            "documentation": "<p>A list of elastic cluster snapshots.</p>",
+            "documentation": "<p>A list of Elastic DocumentDB snapshots.</p>",
             "members": {
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "snapshotArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB snapshot</p>",
                     "shape": "String"
                 },
                 "snapshotCreationTime": {
-                    "documentation": "<p>The time when the elastic cluster snapshot was created in Universal Coordinated Time (UTC).</p>",
+                    "documentation": "<p>The time when the Elastic DocumentDB snapshot was created in Universal Coordinated Time (UTC).</p>",
                     "shape": "String"
                 },
                 "snapshotName": {
-                    "documentation": "<p>The name of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB snapshot.</p>",
                     "shape": "String"
                 },
                 "status": {
-                    "documentation": "<p>The status of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The status of the Elastic DocumentDB snapshot.</p>",
                     "shape": "Status"
                 }
             },
             "required": [
                 "clusterArn",
                 "snapshotArn",
                 "snapshotCreationTime",
@@ -828,122 +699,63 @@
             "required": [
                 "message",
                 "resourceId",
                 "resourceType"
             ],
             "type": "structure"
         },
-        "CopyClusterSnapshotInput": {
-            "members": {
-                "copyTags": {
-                    "documentation": "<p>Set to <code>true</code> to copy all tags from the source cluster snapshot to the target elastic cluster snapshot. The default is <code>false</code>.</p>",
-                    "shape": "Boolean"
-                },
-                "kmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services KMS key ID for an encrypted elastic cluster snapshot. The Amazon Web Services KMS key ID is the Amazon Resource Name (ARN), Amazon Web Services KMS key identifier, or the Amazon Web Services KMS key alias for the Amazon Web Services KMS encryption key.</p> <p>If you copy an encrypted elastic cluster snapshot from your Amazon Web Services account, you can specify a value for <code>KmsKeyId</code> to encrypt the copy with a new Amazon Web ServicesS KMS encryption key. If you don't specify a value for <code>KmsKeyId</code>, then the copy of the elastic cluster snapshot is encrypted with the same <code>AWS</code> KMS key as the source elastic cluster snapshot.</p> <p>To copy an encrypted elastic cluster snapshot to another Amazon Web Services region, set <code>KmsKeyId</code> to the Amazon Web Services KMS key ID that you want to use to encrypt the copy of the elastic cluster snapshot in the destination region. Amazon Web Services KMS encryption keys are specific to the Amazon Web Services region that they are created in, and you can't use encryption keys from one Amazon Web Services region in another Amazon Web Services region.</p> <p>If you copy an unencrypted elastic cluster snapshot and specify a value for the <code>KmsKeyId</code> parameter, an error is returned.</p>",
-                    "shape": "String"
-                },
-                "snapshotArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) identifier of the elastic cluster snapshot.</p>",
-                    "location": "uri",
-                    "locationName": "snapshotArn",
-                    "shape": "String"
-                },
-                "tags": {
-                    "documentation": "<p>The tags to be assigned to the elastic cluster snapshot.</p>",
-                    "shape": "TagMap"
-                },
-                "targetSnapshotName": {
-                    "documentation": "<p>The identifier of the new elastic cluster snapshot to create from the source cluster snapshot. This parameter is not case sensitive.</p> <p>Constraints:</p> <ul> <li> <p>Must contain from 1 to 63 letters, numbers, or hyphens.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Cannot end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p>Example: <code>elastic-cluster-snapshot-5</code> </p>",
-                    "shape": "CopyClusterSnapshotInputTargetSnapshotNameString"
-                }
-            },
-            "required": [
-                "snapshotArn",
-                "targetSnapshotName"
-            ],
-            "type": "structure"
-        },
-        "CopyClusterSnapshotInputTargetSnapshotNameString": {
-            "max": 63,
-            "min": 1,
-            "type": "string"
-        },
-        "CopyClusterSnapshotOutput": {
-            "members": {
-                "snapshot": {
-                    "shape": "ClusterSnapshot"
-                }
-            },
-            "required": [
-                "snapshot"
-            ],
-            "type": "structure"
-        },
         "CreateClusterInput": {
             "members": {
                 "adminUserName": {
-                    "documentation": "<p>The name of the Amazon DocumentDB elastic clusters administrator.</p> <p> <i>Constraints</i>:</p> <ul> <li> <p>Must be from 1 to 63 letters or numbers.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Cannot be a reserved word.</p> </li> </ul>",
+                    "documentation": "<p>The name of the Elastic DocumentDB cluster administrator.</p> <p> <i>Constraints</i>:</p> <ul> <li> <p>Must be from 1 to 63 letters or numbers.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Cannot be a reserved word.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "adminUserPassword": {
-                    "documentation": "<p>The password for the Amazon DocumentDB elastic clusters administrator. The password can contain any printable ASCII characters.</p> <p> <i>Constraints</i>:</p> <ul> <li> <p>Must contain from 8 to 100 characters.</p> </li> <li> <p>Cannot contain a forward slash (/), double quote (\"), or the \"at\" symbol (@).</p> </li> </ul>",
+                    "documentation": "<p>The password for the Elastic DocumentDB cluster administrator and can contain any printable ASCII characters.</p> <p> <i>Constraints</i>:</p> <ul> <li> <p>Must contain from 8 to 100 characters.</p> </li> <li> <p>Cannot contain a forward slash (/), double quote (\"), or the \"at\" symbol (@).</p> </li> </ul>",
                     "shape": "Password"
                 },
                 "authType": {
-                    "documentation": "<p>The authentication type used to determine where to fetch the password used for accessing the elastic cluster. Valid types are <code>PLAIN_TEXT</code> or <code>SECRET_ARN</code>.</p>",
+                    "documentation": "<p>The authentication type for the Elastic DocumentDB cluster.</p>",
                     "shape": "Auth"
                 },
-                "backupRetentionPeriod": {
-                    "documentation": "<p>The number of days for which automatic snapshots are retained.</p>",
-                    "shape": "Integer"
-                },
                 "clientToken": {
-                    "documentation": "<p>The client token for the elastic cluster.</p>",
+                    "documentation": "<p>The client token for the Elastic DocumentDB cluster.</p>",
                     "idempotencyToken": true,
                     "shape": "String"
                 },
                 "clusterName": {
-                    "documentation": "<p>The name of the new elastic cluster. This parameter is stored as a lowercase string.</p> <p> <i>Constraints</i>:</p> <ul> <li> <p>Must contain from 1 to 63 letters, numbers, or hyphens.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Cannot end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p> <i>Example</i>: <code>my-cluster</code> </p>",
+                    "documentation": "<p>The name of the new Elastic DocumentDB cluster. This parameter is stored as a lowercase string.</p> <p> <i>Constraints</i>:</p> <ul> <li> <p>Must contain from 1 to 63 letters, numbers, or hyphens.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Cannot end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p> <i>Example</i>: <code>my-cluster</code> </p>",
                     "shape": "String"
                 },
                 "kmsKeyId": {
-                    "documentation": "<p>The KMS key identifier to use to encrypt the new elastic cluster.</p> <p>The KMS key identifier is the Amazon Resource Name (ARN) for the KMS encryption key. If you are creating a cluster using the same Amazon account that owns this KMS encryption key, you can use the KMS key alias instead of the ARN as the KMS encryption key.</p> <p>If an encryption key is not specified, Amazon DocumentDB uses the default encryption key that KMS creates for your account. Your account has a different default encryption key for each Amazon Region.</p>",
-                    "shape": "String"
-                },
-                "preferredBackupWindow": {
-                    "documentation": "<p>The daily time range during which automated backups are created if automated backups are enabled, as determined by the <code>backupRetentionPeriod</code>.</p>",
+                    "documentation": "<p>The KMS key identifier to use to encrypt the new Elastic DocumentDB cluster.</p> <p>The KMS key identifier is the Amazon Resource Name (ARN) for the KMS encryption key. If you are creating a cluster using the same Amazon account that owns this KMS encryption key, you can use the KMS key alias instead of the ARN as the KMS encryption key.</p> <p>If an encryption key is not specified, Elastic DocumentDB uses the default encryption key that KMS creates for your account. Your account has a different default encryption key for each Amazon Region.</p>",
                     "shape": "String"
                 },
                 "preferredMaintenanceWindow": {
                     "documentation": "<p>The weekly time range during which system maintenance can occur, in Universal Coordinated Time (UTC).</p> <p> <i>Format</i>: <code>ddd:hh24:mi-ddd:hh24:mi</code> </p> <p> <i>Default</i>: a 30-minute window selected at random from an 8-hour block of time for each Amazon Web Services Region, occurring on a random day of the week.</p> <p> <i>Valid days</i>: Mon, Tue, Wed, Thu, Fri, Sat, Sun</p> <p> <i>Constraints</i>: Minimum 30-minute window.</p>",
                     "shape": "String"
                 },
                 "shardCapacity": {
-                    "documentation": "<p>The number of vCPUs assigned to each elastic cluster shard. Maximum is 64. Allowed values are 2, 4, 8, 16, 32, 64.</p>",
+                    "documentation": "<p>The capacity of each shard in the new Elastic DocumentDB cluster.</p>",
                     "shape": "Integer"
                 },
                 "shardCount": {
-                    "documentation": "<p>The number of shards assigned to the elastic cluster. Maximum is 32.</p>",
-                    "shape": "Integer"
-                },
-                "shardInstanceCount": {
-                    "documentation": "<p>The number of replica instances applying to all shards in the elastic cluster. A <code>shardInstanceCount</code> value of 1 means there is one writer instance, and any additional instances are replicas that can be used for reads and to improve availability.</p>",
+                    "documentation": "<p>The number of shards to create in the new Elastic DocumentDB cluster.</p>",
                     "shape": "Integer"
                 },
                 "subnetIds": {
-                    "documentation": "<p>The Amazon EC2 subnet IDs for the new elastic cluster.</p>",
+                    "documentation": "<p>The Amazon EC2 subnet IDs for the new Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 },
                 "tags": {
-                    "documentation": "<p>The tags to be assigned to the new elastic cluster.</p>",
+                    "documentation": "<p>The tags to be assigned to the new Elastic DocumentDB cluster.</p>",
                     "shape": "TagMap"
                 },
                 "vpcSecurityGroupIds": {
-                    "documentation": "<p>A list of EC2 VPC security groups to associate with the new elastic cluster.</p>",
+                    "documentation": "<p>A list of EC2 VPC security groups to associate with the new Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "adminUserName",
                 "adminUserPassword",
                 "authType",
@@ -952,35 +764,35 @@
                 "shardCount"
             ],
             "type": "structure"
         },
         "CreateClusterOutput": {
             "members": {
                 "cluster": {
-                    "documentation": "<p>The new elastic cluster that has been created.</p>",
+                    "documentation": "<p>The new Elastic DocumentDB cluster that has been created.</p>",
                     "shape": "Cluster"
                 }
             },
             "required": [
                 "cluster"
             ],
             "type": "structure"
         },
         "CreateClusterSnapshotInput": {
             "members": {
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster of which you want to create a snapshot.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster that the snapshot will be taken from.</p>",
                     "shape": "String"
                 },
                 "snapshotName": {
-                    "documentation": "<p>The name of the new elastic cluster snapshot.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB snapshot.</p>",
                     "shape": "CreateClusterSnapshotInputSnapshotNameString"
                 },
                 "tags": {
-                    "documentation": "<p>The tags to be assigned to the new elastic cluster snapshot.</p>",
+                    "documentation": "<p>The tags to be assigned to the new Elastic DocumentDB snapshot.</p>",
                     "shape": "TagMap"
                 }
             },
             "required": [
                 "clusterArn",
                 "snapshotName"
             ],
@@ -990,119 +802,119 @@
             "max": 63,
             "min": 1,
             "type": "string"
         },
         "CreateClusterSnapshotOutput": {
             "members": {
                 "snapshot": {
-                    "documentation": "<p>Returns information about the new elastic cluster snapshot.</p>",
+                    "documentation": "<p>Returns information about the new Elastic DocumentDB snapshot.</p>",
                     "shape": "ClusterSnapshot"
                 }
             },
             "required": [
                 "snapshot"
             ],
             "type": "structure"
         },
         "DeleteClusterInput": {
             "members": {
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster that is to be deleted.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster that is to be deleted.</p>",
                     "location": "uri",
                     "locationName": "clusterArn",
                     "shape": "String"
                 }
             },
             "required": [
                 "clusterArn"
             ],
             "type": "structure"
         },
         "DeleteClusterOutput": {
             "members": {
                 "cluster": {
-                    "documentation": "<p>Returns information about the newly deleted elastic cluster.</p>",
+                    "documentation": "<p>Returns information about the newly deleted Elastic DocumentDB cluster.</p>",
                     "shape": "Cluster"
                 }
             },
             "required": [
                 "cluster"
             ],
             "type": "structure"
         },
         "DeleteClusterSnapshotInput": {
             "members": {
                 "snapshotArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster snapshot that is to be deleted.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB snapshot that is to be deleted.</p>",
                     "location": "uri",
                     "locationName": "snapshotArn",
                     "shape": "String"
                 }
             },
             "required": [
                 "snapshotArn"
             ],
             "type": "structure"
         },
         "DeleteClusterSnapshotOutput": {
             "members": {
                 "snapshot": {
-                    "documentation": "<p>Returns information about the newly deleted elastic cluster snapshot.</p>",
+                    "documentation": "<p>Returns information about the newly deleted Elastic DocumentDB snapshot.</p>",
                     "shape": "ClusterSnapshot"
                 }
             },
             "required": [
                 "snapshot"
             ],
             "type": "structure"
         },
         "GetClusterInput": {
             "members": {
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "location": "uri",
                     "locationName": "clusterArn",
                     "shape": "String"
                 }
             },
             "required": [
                 "clusterArn"
             ],
             "type": "structure"
         },
         "GetClusterOutput": {
             "members": {
                 "cluster": {
-                    "documentation": "<p>Returns information about a specific elastic cluster.</p>",
+                    "documentation": "<p>Returns information about a specific Elastic DocumentDB cluster.</p>",
                     "shape": "Cluster"
                 }
             },
             "required": [
                 "cluster"
             ],
             "type": "structure"
         },
         "GetClusterSnapshotInput": {
             "members": {
                 "snapshotArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB snapshot.</p>",
                     "location": "uri",
                     "locationName": "snapshotArn",
                     "shape": "String"
                 }
             },
             "required": [
                 "snapshotArn"
             ],
             "type": "structure"
         },
         "GetClusterSnapshotOutput": {
             "members": {
                 "snapshot": {
-                    "documentation": "<p>Returns information about a specific elastic cluster snapshot.</p>",
+                    "documentation": "<p>Returns information about a specific Elastic DocumentDB snapshot.</p>",
                     "shape": "ClusterSnapshot"
                 }
             },
             "required": [
                 "snapshot"
             ],
             "type": "structure"
@@ -1130,69 +942,63 @@
                 "throttling": false
             },
             "type": "structure"
         },
         "ListClusterSnapshotsInput": {
             "members": {
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "location": "querystring",
                     "locationName": "clusterArn",
                     "shape": "String"
                 },
                 "maxResults": {
-                    "documentation": "<p>The maximum number of elastic cluster snapshot results to receive in the response.</p>",
+                    "documentation": "<p>The maximum number of entries to recieve in the response.</p>",
                     "location": "querystring",
                     "locationName": "maxResults",
                     "shape": "ListClusterSnapshotsInputMaxResultsInteger"
                 },
                 "nextToken": {
-                    "documentation": "<p>A pagination token provided by a previous request. If this parameter is specified, the response includes only records beyond this token, up to the value specified by <code>max-results</code>.</p> <p>If there is no more data in the responce, the <code>nextToken</code> will not be returned.</p>",
+                    "documentation": "<p>The nextToken which is used the get the next page of data.</p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "PaginationToken"
-                },
-                "snapshotType": {
-                    "documentation": "<p>The type of cluster snapshots to be returned. You can specify one of the following values:</p> <ul> <li> <p> <code>automated</code> - Return all cluster snapshots that Amazon DocumentDB has automatically created for your Amazon Web Services account.</p> </li> <li> <p> <code>manual</code> - Return all cluster snapshots that you have manually created for your Amazon Web Services account.</p> </li> </ul>",
-                    "location": "querystring",
-                    "locationName": "snapshotType",
-                    "shape": "String"
                 }
             },
             "type": "structure"
         },
         "ListClusterSnapshotsInputMaxResultsInteger": {
             "box": true,
             "max": 100,
             "min": 20,
             "type": "integer"
         },
         "ListClusterSnapshotsOutput": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>A pagination token provided by a previous request. If this parameter is specified, the response includes only records beyond this token, up to the value specified by <code>max-results</code>.</p> <p>If there is no more data in the responce, the <code>nextToken</code> will not be returned.</p>",
+                    "documentation": "<p>The response will provide a nextToken if there is more data beyond the maxResults.</p> <p>If there is no more data in the responce, the nextToken will not be returned.</p>",
                     "shape": "PaginationToken"
                 },
                 "snapshots": {
-                    "documentation": "<p>A list of snapshots for a specified elastic cluster.</p>",
+                    "documentation": "<p>A list of Elastic DocumentDB snapshots for a specified cluster.</p>",
                     "shape": "ClusterSnapshotList"
                 }
             },
             "type": "structure"
         },
         "ListClustersInput": {
             "members": {
                 "maxResults": {
-                    "documentation": "<p>The maximum number of elastic cluster snapshot results to receive in the response.</p>",
+                    "documentation": "<p>The maximum number of entries to recieve in the response.</p>",
                     "location": "querystring",
                     "locationName": "maxResults",
                     "shape": "ListClustersInputMaxResultsInteger"
                 },
                 "nextToken": {
-                    "documentation": "<p>A pagination token provided by a previous request. If this parameter is specified, the response includes only records beyond this token, up to the value specified by <code>max-results</code>.</p> <p>If there is no more data in the responce, the <code>nextToken</code> will not be returned.</p>",
+                    "documentation": "<p>The nextToken which is used the get the next page of data.</p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "PaginationToken"
                 }
             },
             "type": "structure"
         },
@@ -1201,42 +1007,42 @@
             "max": 100,
             "min": 1,
             "type": "integer"
         },
         "ListClustersOutput": {
             "members": {
                 "clusters": {
-                    "documentation": "<p>A list of Amazon DocumentDB elastic clusters.</p>",
+                    "documentation": "<p>A list of Elastic DocumentDB cluster.</p>",
                     "shape": "ClusterList"
                 },
                 "nextToken": {
-                    "documentation": "<p>A pagination token provided by a previous request. If this parameter is specified, the response includes only records beyond this token, up to the value specified by <code>max-results</code>.</p> <p>If there is no more data in the responce, the <code>nextToken</code> will not be returned.</p>",
+                    "documentation": "<p>The response will provide a nextToken if there is more data beyond the maxResults.</p> <p>If there is no more data in the responce, the nextToken will not be returned.</p>",
                     "shape": "PaginationToken"
                 }
             },
             "type": "structure"
         },
         "ListTagsForResourceRequest": {
             "members": {
                 "resourceArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster resource.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB resource.</p>",
                     "location": "uri",
                     "locationName": "resourceArn",
                     "shape": "Arn"
                 }
             },
             "required": [
                 "resourceArn"
             ],
             "type": "structure"
         },
         "ListTagsForResourceResponse": {
             "members": {
                 "tags": {
-                    "documentation": "<p>The list of tags for the specified elastic cluster resource.</p>",
+                    "documentation": "<p>The list of tags for the specified Elastic DocumentDB resource.</p>",
                     "shape": "TagMap"
                 }
             },
             "type": "structure"
         },
         "PaginationToken": {
             "documentation": "<p>Token or cursor used in paginated operations.</p> <p>When this value is provided as operation input, the service returns results from where the previous response left off. When this value is present in operation output, it indicates that there are more results to retrieve.</p> <p>This should be opaque to not expose implementation details and potentially versioned to allow evolution of pagination strategy.</p>",
@@ -1273,58 +1079,50 @@
                 "resourceType"
             ],
             "type": "structure"
         },
         "RestoreClusterFromSnapshotInput": {
             "members": {
                 "clusterName": {
-                    "documentation": "<p>The name of the elastic cluster.</p>",
+                    "documentation": "<p>The name of the Elastic DocumentDB cluster.</p>",
                     "shape": "String"
                 },
                 "kmsKeyId": {
-                    "documentation": "<p>The KMS key identifier to use to encrypt the new Amazon DocumentDB elastic clusters cluster.</p> <p>The KMS key identifier is the Amazon Resource Name (ARN) for the KMS encryption key. If you are creating a cluster using the same Amazon account that owns this KMS encryption key, you can use the KMS key alias instead of the ARN as the KMS encryption key.</p> <p>If an encryption key is not specified here, Amazon DocumentDB uses the default encryption key that KMS creates for your account. Your account has a different default encryption key for each Amazon Region.</p>",
+                    "documentation": "<p>The KMS key identifier to use to encrypt the new Elastic DocumentDB cluster.</p> <p>The KMS key identifier is the Amazon Resource Name (ARN) for the KMS encryption key. If you are creating a cluster using the same Amazon account that owns this KMS encryption key, you can use the KMS key alias instead of the ARN as the KMS encryption key.</p> <p>If an encryption key is not specified here, Elastic DocumentDB uses the default encryption key that KMS creates for your account. Your account has a different default encryption key for each Amazon Region.</p>",
                     "shape": "String"
                 },
-                "shardCapacity": {
-                    "documentation": "<p>The capacity of each shard in the new restored elastic cluster.</p>",
-                    "shape": "Integer"
-                },
-                "shardInstanceCount": {
-                    "documentation": "<p>The number of replica instances applying to all shards in the elastic cluster. A <code>shardInstanceCount</code> value of 1 means there is one writer instance, and any additional instances are replicas that can be used for reads and to improve availability.</p>",
-                    "shape": "Integer"
-                },
                 "snapshotArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster snapshot.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB snapshot.</p>",
                     "location": "uri",
                     "locationName": "snapshotArn",
                     "shape": "String"
                 },
                 "subnetIds": {
-                    "documentation": "<p>The Amazon EC2 subnet IDs for the elastic cluster.</p>",
+                    "documentation": "<p>The Amazon EC2 subnet IDs for the Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 },
                 "tags": {
-                    "documentation": "<p>A list of the tag names to be assigned to the restored elastic cluster, in the form of an array of key-value pairs in which the key is the tag name and the value is the key value.</p>",
+                    "documentation": "<p>A list of the tag names to be assigned to the restored DB cluster, in the form of an array of key-value pairs in which the key is the tag name and the value is the key value.</p>",
                     "shape": "TagMap"
                 },
                 "vpcSecurityGroupIds": {
-                    "documentation": "<p>A list of EC2 VPC security groups to associate with the elastic cluster.</p>",
+                    "documentation": "<p>A list of EC2 VPC security groups to associate with the Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "clusterName",
                 "snapshotArn"
             ],
             "type": "structure"
         },
         "RestoreClusterFromSnapshotOutput": {
             "members": {
                 "cluster": {
-                    "documentation": "<p>Returns information about a the restored elastic cluster.</p>",
+                    "documentation": "<p>Returns information about a the restored Elastic DocumentDB cluster.</p>",
                     "shape": "Cluster"
                 }
             },
             "required": [
                 "cluster"
             ],
             "type": "structure"
@@ -1342,124 +1140,28 @@
                 }
             },
             "required": [
                 "message"
             ],
             "type": "structure"
         },
-        "Shard": {
-            "documentation": "<p>The name of the shard.</p>",
-            "members": {
-                "createTime": {
-                    "documentation": "<p>The time when the shard was created in Universal Coordinated Time (UTC).</p>",
-                    "shape": "String"
-                },
-                "shardId": {
-                    "documentation": "<p>The ID of the shard.</p>",
-                    "shape": "String"
-                },
-                "status": {
-                    "documentation": "<p>The current status of the shard.</p>",
-                    "shape": "Status"
-                }
-            },
-            "required": [
-                "createTime",
-                "shardId",
-                "status"
-            ],
-            "type": "structure"
-        },
-        "ShardList": {
-            "member": {
-                "shape": "Shard"
-            },
-            "type": "list"
-        },
-        "SnapshotType": {
-            "enum": [
-                "MANUAL",
-                "AUTOMATED"
-            ],
-            "type": "string"
-        },
-        "StartClusterInput": {
-            "members": {
-                "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
-                    "location": "uri",
-                    "locationName": "clusterArn",
-                    "shape": "String"
-                }
-            },
-            "required": [
-                "clusterArn"
-            ],
-            "type": "structure"
-        },
-        "StartClusterOutput": {
-            "members": {
-                "cluster": {
-                    "shape": "Cluster"
-                }
-            },
-            "required": [
-                "cluster"
-            ],
-            "type": "structure"
-        },
         "Status": {
             "enum": [
                 "CREATING",
                 "ACTIVE",
                 "DELETING",
                 "UPDATING",
                 "VPC_ENDPOINT_LIMIT_EXCEEDED",
                 "IP_ADDRESS_LIMIT_EXCEEDED",
                 "INVALID_SECURITY_GROUP_ID",
                 "INVALID_SUBNET_ID",
-                "INACCESSIBLE_ENCRYPTION_CREDS",
-                "INACCESSIBLE_SECRET_ARN",
-                "INACCESSIBLE_VPC_ENDPOINT",
-                "INCOMPATIBLE_NETWORK",
-                "MERGING",
-                "MODIFYING",
-                "SPLITTING",
-                "COPYING",
-                "STARTING",
-                "STOPPING",
-                "STOPPED"
+                "INACCESSIBLE_ENCRYPTION_CREDS"
             ],
             "type": "string"
         },
-        "StopClusterInput": {
-            "members": {
-                "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
-                    "location": "uri",
-                    "locationName": "clusterArn",
-                    "shape": "String"
-                }
-            },
-            "required": [
-                "clusterArn"
-            ],
-            "type": "structure"
-        },
-        "StopClusterOutput": {
-            "members": {
-                "cluster": {
-                    "shape": "Cluster"
-                }
-            },
-            "required": [
-                "cluster"
-            ],
-            "type": "structure"
-        },
         "String": {
             "type": "string"
         },
         "StringList": {
             "member": {
                 "shape": "String"
             },
@@ -1487,21 +1189,21 @@
             "value": {
                 "shape": "TagValue"
             }
         },
         "TagResourceRequest": {
             "members": {
                 "resourceArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster resource.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB resource.</p>",
                     "location": "uri",
                     "locationName": "resourceArn",
                     "shape": "Arn"
                 },
                 "tags": {
-                    "documentation": "<p>The tags that are assigned to the elastic cluster resource.</p>",
+                    "documentation": "<p>The tags to be assigned to the Elastic DocumentDB resource.</p>",
                     "shape": "TagMap"
                 }
             },
             "required": [
                 "resourceArn",
                 "tags"
             ],
@@ -1541,21 +1243,21 @@
                 "throttling": false
             },
             "type": "structure"
         },
         "UntagResourceRequest": {
             "members": {
                 "resourceArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster resource.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB resource.</p>",
                     "location": "uri",
                     "locationName": "resourceArn",
                     "shape": "Arn"
                 },
                 "tagKeys": {
-                    "documentation": "<p>The tag keys to be removed from the elastic cluster resource.</p>",
+                    "documentation": "<p>The tag keys to be removed from the Elastic DocumentDB resource.</p>",
                     "location": "querystring",
                     "locationName": "tagKeys",
                     "shape": "TagKeyList"
                 }
             },
             "required": [
                 "resourceArn",
@@ -1566,74 +1268,62 @@
         "UntagResourceResponse": {
             "members": {},
             "type": "structure"
         },
         "UpdateClusterInput": {
             "members": {
                 "adminUserPassword": {
-                    "documentation": "<p>The password associated with the elastic cluster administrator. This password can contain any printable ASCII character except forward slash (/), double quote (\"), or the \"at\" symbol (@).</p> <p> <i>Constraints</i>: Must contain from 8 to 100 characters.</p>",
+                    "documentation": "<p>The password for the Elastic DocumentDB cluster administrator. This password can contain any printable ASCII character except forward slash (/), double quote (\"), or the \"at\" symbol (@).</p> <p> <i>Constraints</i>: Must contain from 8 to 100 characters.</p>",
                     "shape": "Password"
                 },
                 "authType": {
-                    "documentation": "<p>The authentication type used to determine where to fetch the password used for accessing the elastic cluster. Valid types are <code>PLAIN_TEXT</code> or <code>SECRET_ARN</code>.</p>",
+                    "documentation": "<p>The authentication type for the Elastic DocumentDB cluster.</p>",
                     "shape": "Auth"
                 },
-                "backupRetentionPeriod": {
-                    "documentation": "<p>The number of days for which automatic snapshots are retained.</p>",
-                    "shape": "Integer"
-                },
                 "clientToken": {
-                    "documentation": "<p>The client token for the elastic cluster.</p>",
+                    "documentation": "<p>The client token for the Elastic DocumentDB cluster.</p>",
                     "idempotencyToken": true,
                     "shape": "String"
                 },
                 "clusterArn": {
-                    "documentation": "<p>The ARN identifier of the elastic cluster.</p>",
+                    "documentation": "<p>The arn of the Elastic DocumentDB cluster.</p>",
                     "location": "uri",
                     "locationName": "clusterArn",
                     "shape": "String"
                 },
-                "preferredBackupWindow": {
-                    "documentation": "<p>The daily time range during which automated backups are created if automated backups are enabled, as determined by the <code>backupRetentionPeriod</code>.</p>",
-                    "shape": "String"
-                },
                 "preferredMaintenanceWindow": {
                     "documentation": "<p>The weekly time range during which system maintenance can occur, in Universal Coordinated Time (UTC).</p> <p> <i>Format</i>: <code>ddd:hh24:mi-ddd:hh24:mi</code> </p> <p> <i>Default</i>: a 30-minute window selected at random from an 8-hour block of time for each Amazon Web Services Region, occurring on a random day of the week.</p> <p> <i>Valid days</i>: Mon, Tue, Wed, Thu, Fri, Sat, Sun</p> <p> <i>Constraints</i>: Minimum 30-minute window.</p>",
                     "shape": "String"
                 },
                 "shardCapacity": {
-                    "documentation": "<p>The number of vCPUs assigned to each elastic cluster shard. Maximum is 64. Allowed values are 2, 4, 8, 16, 32, 64.</p>",
+                    "documentation": "<p>The capacity of each shard in the Elastic DocumentDB cluster.</p>",
                     "shape": "Integer"
                 },
                 "shardCount": {
-                    "documentation": "<p>The number of shards assigned to the elastic cluster. Maximum is 32.</p>",
-                    "shape": "Integer"
-                },
-                "shardInstanceCount": {
-                    "documentation": "<p>The number of replica instances applying to all shards in the elastic cluster. A <code>shardInstanceCount</code> value of 1 means there is one writer instance, and any additional instances are replicas that can be used for reads and to improve availability.</p>",
+                    "documentation": "<p>The number of shards to create in the Elastic DocumentDB cluster.</p>",
                     "shape": "Integer"
                 },
                 "subnetIds": {
-                    "documentation": "<p>The Amazon EC2 subnet IDs for the elastic cluster.</p>",
+                    "documentation": "<p>The number of shards to create in the Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 },
                 "vpcSecurityGroupIds": {
-                    "documentation": "<p>A list of EC2 VPC security groups to associate with the elastic cluster.</p>",
+                    "documentation": "<p>A list of EC2 VPC security groups to associate with the new Elastic DocumentDB cluster.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "clusterArn"
             ],
             "type": "structure"
         },
         "UpdateClusterOutput": {
             "members": {
                 "cluster": {
-                    "documentation": "<p>Returns information about the updated elastic cluster.</p>",
+                    "documentation": "<p>Returns information about the updated Elastic DocumentDB cluster.</p>",
                     "shape": "Cluster"
                 }
             },
             "required": [
                 "cluster"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-docdb-elastic-1.34.80/botocore_a_la_carte_docdb_elastic.egg-info/PKG-INFO` & `botocore-a-la-carte-docdb-elastic-1.34.9/botocore_a_la_carte_docdb_elastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-docdb-elastic
-Version: 1.34.80
+Version: 1.34.9
 Summary: docdb-elastic data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-docdb-elastic-1.34.80/setup.py` & `botocore-a-la-carte-docdb-elastic-1.34.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-docdb-elastic',
-    version="1.34.80",
+    version="1.34.9",
     description='docdb-elastic data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/docdb-elastic/*/*.json'],
```

