# Comparing `tmp/alibabacloud_adb20211201-1.3.1.tar.gz` & `tmp/alibabacloud_adb20211201-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adb20211201-1.3.1.tar", last modified: Mon Mar 25 17:11:30 2024, max compression
+gzip compressed data, was "dist/alibabacloud_adb20211201-1.3.2.tar", last modified: Tue Apr  9 17:13:38 2024, max compression
```

## Comparing `alibabacloud_adb20211201-1.3.1.tar` & `alibabacloud_adb20211201-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:11:30.000000 alibabacloud_adb20211201-1.3.1/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-25 17:11:30.000000 alibabacloud_adb20211201-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:11:30.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   432546 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201/client.py
--rw-r--r--   0 root         (0) root         (0)   919835 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:11:30.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 17:11:30.000000 alibabacloud_adb20211201-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-03-25 17:11:29.000000 alibabacloud_adb20211201-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   432546 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/client.py
+-rw-r--r--   0 root         (0) root         (0)   920205 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/setup.py
```

### Comparing `alibabacloud_adb20211201-1.3.1/ChangeLog.md` & `alibabacloud_adb20211201-1.3.2/ChangeLog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2024-03-25 Version: 1.3.1
+- Update API CreateDBResourceGroup: add param Rules.
+- Update API DescribeDBResourceGroup: update response param.
+- Update API ModifyDBResourceGroup: add param Rules.
+
+
 2024-03-23 Version: 1.3.0
 - Support API DescribeDBClusterSpaceSummary.
 - Update API CreateDBResourceGroup: add param EnableSpot.
 - Update API DescribeApsActionLogs: update response param.
 - Update API DescribeClusterResourceDetail: update response param.
 - Update API DescribeDBResourceGroup: add param RegionId.
 - Update API DescribeDBResourceGroup: update response param.
```

### Comparing `alibabacloud_adb20211201-1.3.1/LICENSE` & `alibabacloud_adb20211201-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.1/PKG-INFO` & `alibabacloud_adb20211201-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_adb20211201
-Version: 1.3.1
+Version: 1.3.2
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201-1.3.1/README-CN.md` & `alibabacloud_adb20211201-1.3.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.1/README.md` & `alibabacloud_adb20211201-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201/client.py` & `alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201/models.py` & `alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4224,15 +4224,15 @@
         dbcluster_id: str = None,
         group_name: str = None,
     ):
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
         # The name of the resource group.
         # 
-        # > You can call the [DescribeDBResourceGroup](~~612410~~) operation to query the resource group information of a cluster, including the resource group name.
+        # >  You can call the [DescribeDBResourceGroup](~~612410~~) operation to query the information about resource groups of an AnalyticDB for MySQL cluster, including resource group names.
         self.group_name = group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8724,14 +8724,20 @@
         running_cluster_count: int = None,
         status: str = None,
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
+        # Indicates whether the preemptible instance feature is enabled for the resource group. After the preemptible instance feature is enabled, you are charged for resources at a lower unit price but the resources are probably released. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
+        # 
+        # The True value is returned only for job resource groups.
         self.enable_spot = enable_spot
         # A reserved parameter.
         self.max_cluster_count = max_cluster_count
         # The maximum amount of reserved computing resources. Unit: ACUs.
         self.max_compute_resource = max_compute_resource
         # A reserved parameter.
         self.min_cluster_count = min_cluster_count
@@ -8743,15 +8749,15 @@
         self.pool_name = pool_name
         # The type of the resource group.
         self.pool_type = pool_type
         # The user of the resource group.
         self.pool_users = pool_users
         # A reserved parameter.
         self.running_cluster_count = running_cluster_count
-        # The state of the resource group. Valid values:
+        # The status of the resource group. Valid values:
         # 
         # *   **running**\
         # *   **deleting**\
         # *   **scaling**\
         self.status = status
 
     def validate(self):
@@ -11962,40 +11968,40 @@
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
         # The time when the resource group was created. The time follows the ISO 8601 standard in the *yyyy-MM-ddTHH:mm:ssZ* format. The time is displayed in UTC.
         self.create_time = create_time
-        # The minimum amount of elastic computing resources. Unit: ACUs.
+        # The minimum amount of elastic computing resources. Unit: ACU.
         self.elastic_min_compute_resource = elastic_min_compute_resource
         self.enable_spot = enable_spot
         # The name of the resource group.
         self.group_name = group_name
         # The type of the resource group. Valid values:
         # 
         # *   **Interactive**\
         # *   **Job**\
         # 
         # >  For more information about resource groups, see [Resource groups](~~428610~~).
         self.group_type = group_type
-        # The Resource Access Management (RAM) user with which the resource group is associated.
+        # The Resource Access Management (RAM) user that is associated with the resource group.
         self.group_users = group_users
         # A reserved parameter.
         self.max_cluster_count = max_cluster_count
-        # The maximum amount of reserved computing resources. Unit: ACUs.
+        # The maximum amount of reserved computing resources. Unit: ACU.
         self.max_compute_resource = max_compute_resource
         # A reserved parameter.
         self.min_cluster_count = min_cluster_count
-        # The minimum amount of reserved computing resources. Unit: AnalyticDB compute units (ACUs).
+        # The minimum amount of reserved computing resources. Unit: AnalyticDB compute unit (ACU).
         self.min_compute_resource = min_compute_resource
         self.rules = rules
         # A reserved parameter.
         self.running_cluster_count = running_cluster_count
-        # The state of the resource group. Valid values:
+        # The status of the resource group. Valid values:
         # 
         # *   **creating**: The resource group is being created.
         # *   **ok**: The resource group is created.
         # *   **pendingdelete**: The resource group is pending to be deleted.
         self.status = status
         # The time when the resource group was updated. The time follows the ISO 8601 standard in the *yyyy-MM-ddTHH:mm:ssZ* format. The time is displayed in UTC.
         self.update_time = update_time
@@ -18474,15 +18480,15 @@
     ):
         # The application ID.
         self.app_id = app_id
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
         # The content of the log.
         self.log_content = log_content
-        # The number of entries per page. A value of 0 indicates that no valid logs are returned.
+        # The number of log entries. A value of 0 indicates that no valid logs are returned.
         self.log_size = log_size
         # The alert message returned for the request, such as task execution failure or insufficient resources. If no alert occurs, null is returned.
         self.message = message
 
     def validate(self):
         pass
 
@@ -22804,17 +22810,17 @@
 
 
 class LoadSampleDataSetRequest(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
     ):
-        # The ID of the AnalyticDB for MySQL Data Warehouse Edition (V3.0) cluster.
+        # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         # 
-        # >  You can call the [DescribeDBClusters](~~129857~~) operation to query the IDs of all AnalyticDB for MySQL Data Warehouse Edition (V3.0) clusters within a region.
+        # >  You can call the [DescribeDBClusters](~~454250~~) operation to query the IDs of all AnalyticDB for MySQL Data Lakehouse Edition (V3.0) clusters within a region.
         self.dbcluster_id = dbcluster_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22835,15 +22841,15 @@
 
 class LoadSampleDataSetResponseBody(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the AnalyticDB for MySQL Data Warehouse Edition (V3.0) cluster.
+        # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
         # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -23777,19 +23783,19 @@
         port: int = None,
     ):
         # The prefix of the public endpoint.
         # 
         # *   The prefix can contain lowercase letters, digits, and hyphens (-). It must start with a lowercase letter.
         # *   The prefix can be up to 30 characters in length.
         self.connection_string_prefix = connection_string_prefix
-        # The current public endpoint of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
+        # The public endpoint of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.current_connection_string = current_connection_string
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
-        # The port number that is used to connect to the cluster. Set the value to **3306**.
+        # The port number. Set the value to **3306**.
         self.port = port
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23821,15 +23827,15 @@
 
 
 class ModifyClusterConnectionStringResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26071,15 +26077,15 @@
     def __init__(
         self,
         account_name: str = None,
         dbcluster_id: str = None,
     ):
         # The name of the database account.
         # 
-        # > You can call the [DescribeAccounts](~~612430~~) operation to view the information about a database account in a cluster, including the name of the database account.
+        # >  You can call the [DescribeAccounts](~~612430~~) operation to query the information about database accounts of an AnalyticDB for MySQL cluster, including database account names.
         self.account_name = account_name
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_adb20211201-1.3.1/alibabacloud_adb20211201.egg-info/PKG-INFO` & `alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-adb20211201
-Version: 1.3.1
+Version: 1.3.2
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201-1.3.1/setup.py` & `alibabacloud_adb20211201-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adb20211201.
 
-Created on 25/03/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adb20211201"
 NAME = "alibabacloud_adb20211201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adb (20211201) SDK Library for Python"
```

