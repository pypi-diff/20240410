# Comparing `tmp/alibabacloud_adb20211201_py2-1.5.1.tar.gz` & `tmp/alibabacloud_adb20211201_py2-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adb20211201_py2-1.5.1.tar", last modified: Mon Mar 25 17:12:31 2024, max compression
+gzip compressed data, was "dist/alibabacloud_adb20211201_py2-1.5.2.tar", last modified: Tue Apr  9 17:13:09 2024, max compression
```

## Comparing `alibabacloud_adb20211201_py2-1.5.1.tar` & `alibabacloud_adb20211201_py2-1.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/
--rw-r--r--   0 root         (0) root         (0)     3999 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180113 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201/client.py
--rw-r--r--   0 root         (0) root         (0)   925914 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 17:12:31.000000 alibabacloud_adb20211201_py2-1.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2024-03-25 17:12:29.000000 alibabacloud_adb20211201_py2-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180113 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201/client.py
+-rw-r--r--   0 root         (0) root         (0)   926284 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:13:09.000000 alibabacloud_adb20211201_py2-1.5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-09 17:13:08.000000 alibabacloud_adb20211201_py2-1.5.2/setup.py
```

### Comparing `alibabacloud_adb20211201_py2-1.5.1/ChangeLog.md` & `alibabacloud_adb20211201_py2-1.5.2/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2024-03-25 Version: 1.5.1
+- Update API CreateDBResourceGroup: add param Rules.
+- Update API DescribeDBResourceGroup: update response param.
+- Update API ModifyDBResourceGroup: add param Rules.
+
+
 2024-03-23 Version: 1.5.0
 - Support API DescribeDBClusterSpaceSummary.
 - Update API CreateDBResourceGroup: add param EnableSpot.
 - Update API DescribeApsActionLogs: update response param.
 - Update API DescribeClusterResourceDetail: update response param.
 - Update API DescribeDBResourceGroup: add param RegionId.
 - Update API DescribeDBResourceGroup: update response param.
```

### Comparing `alibabacloud_adb20211201_py2-1.5.1/LICENSE` & `alibabacloud_adb20211201_py2-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201_py2-1.5.1/PKG-INFO` & `alibabacloud_adb20211201_py2-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_adb20211201_py2
-Version: 1.5.1
+Version: 1.5.2
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201_py2-1.5.1/README-CN.md` & `alibabacloud_adb20211201_py2-1.5.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201_py2-1.5.1/README.md` & `alibabacloud_adb20211201_py2-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201/client.py` & `alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201/models.py` & `alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3731,15 +3731,15 @@
 
 class DeleteDBResourceGroupRequest(TeaModel):
     def __init__(self, dbcluster_id=None, group_name=None):
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id  # type: str
         # The name of the resource group.
         # 
-        # > You can call the [DescribeDBResourceGroup](~~612410~~) operation to query the resource group information of a cluster, including the resource group name.
+        # >  You can call the [DescribeDBResourceGroup](~~612410~~) operation to query the information about resource groups of an AnalyticDB for MySQL cluster, including resource group names.
         self.group_name = group_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDBResourceGroupRequest, self).to_map()
@@ -7736,14 +7736,20 @@
     def __init__(self, cluster_mode=None, cluster_size_resource=None, enable_spot=None, max_cluster_count=None,
                  max_compute_resource=None, min_cluster_count=None, min_compute_resource=None, pool_id=None, pool_name=None,
                  pool_type=None, pool_users=None, running_cluster_count=None, status=None):
         # A reserved parameter.
         self.cluster_mode = cluster_mode  # type: str
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource  # type: str
+        # Indicates whether the preemptible instance feature is enabled for the resource group. After the preemptible instance feature is enabled, you are charged for resources at a lower unit price but the resources are probably released. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
+        # 
+        # The True value is returned only for job resource groups.
         self.enable_spot = enable_spot  # type: bool
         # A reserved parameter.
         self.max_cluster_count = max_cluster_count  # type: int
         # The maximum amount of reserved computing resources. Unit: ACUs.
         self.max_compute_resource = max_compute_resource  # type: str
         # A reserved parameter.
         self.min_cluster_count = min_cluster_count  # type: int
@@ -7755,15 +7761,15 @@
         self.pool_name = pool_name  # type: str
         # The type of the resource group.
         self.pool_type = pool_type  # type: str
         # The user of the resource group.
         self.pool_users = pool_users  # type: str
         # A reserved parameter.
         self.running_cluster_count = running_cluster_count  # type: int
-        # The state of the resource group. Valid values:
+        # The status of the resource group. Valid values:
         # 
         # *   **running**\
         # *   **deleting**\
         # *   **scaling**\
         self.status = status  # type: str
 
     def validate(self):
@@ -10629,40 +10635,40 @@
                  status=None, update_time=None):
         # A reserved parameter.
         self.cluster_mode = cluster_mode  # type: str
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource  # type: str
         # The time when the resource group was created. The time follows the ISO 8601 standard in the *yyyy-MM-ddTHH:mm:ssZ* format. The time is displayed in UTC.
         self.create_time = create_time  # type: str
-        # The minimum amount of elastic computing resources. Unit: ACUs.
+        # The minimum amount of elastic computing resources. Unit: ACU.
         self.elastic_min_compute_resource = elastic_min_compute_resource  # type: str
         self.enable_spot = enable_spot  # type: str
         # The name of the resource group.
         self.group_name = group_name  # type: str
         # The type of the resource group. Valid values:
         # 
         # *   **Interactive**\
         # *   **Job**\
         # 
         # >  For more information about resource groups, see [Resource groups](~~428610~~).
         self.group_type = group_type  # type: str
-        # The Resource Access Management (RAM) user with which the resource group is associated.
+        # The Resource Access Management (RAM) user that is associated with the resource group.
         self.group_users = group_users  # type: str
         # A reserved parameter.
         self.max_cluster_count = max_cluster_count  # type: int
-        # The maximum amount of reserved computing resources. Unit: ACUs.
+        # The maximum amount of reserved computing resources. Unit: ACU.
         self.max_compute_resource = max_compute_resource  # type: str
         # A reserved parameter.
         self.min_cluster_count = min_cluster_count  # type: int
-        # The minimum amount of reserved computing resources. Unit: AnalyticDB compute units (ACUs).
+        # The minimum amount of reserved computing resources. Unit: AnalyticDB compute unit (ACU).
         self.min_compute_resource = min_compute_resource  # type: str
         self.rules = rules  # type: list[DescribeDBResourceGroupResponseBodyGroupsInfoRules]
         # A reserved parameter.
         self.running_cluster_count = running_cluster_count  # type: int
-        # The state of the resource group. Valid values:
+        # The status of the resource group. Valid values:
         # 
         # *   **creating**: The resource group is being created.
         # *   **ok**: The resource group is created.
         # *   **pendingdelete**: The resource group is pending to be deleted.
         self.status = status  # type: str
         # The time when the resource group was updated. The time follows the ISO 8601 standard in the *yyyy-MM-ddTHH:mm:ssZ* format. The time is displayed in UTC.
         self.update_time = update_time  # type: str
@@ -16458,15 +16464,15 @@
     def __init__(self, app_id=None, dbcluster_id=None, log_content=None, log_size=None, message=None):
         # The application ID.
         self.app_id = app_id  # type: str
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id  # type: str
         # The content of the log.
         self.log_content = log_content  # type: str
-        # The number of entries per page. A value of 0 indicates that no valid logs are returned.
+        # The number of log entries. A value of 0 indicates that no valid logs are returned.
         self.log_size = log_size  # type: int
         # The alert message returned for the request, such as task execution failure or insufficient resources. If no alert occurs, null is returned.
         self.message = message  # type: str
 
     def validate(self):
         pass
 
@@ -20317,17 +20323,17 @@
             temp_model = ListSparkTemplateFileIdsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class LoadSampleDataSetRequest(TeaModel):
     def __init__(self, dbcluster_id=None):
-        # The ID of the AnalyticDB for MySQL Data Warehouse Edition (V3.0) cluster.
+        # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         # 
-        # >  You can call the [DescribeDBClusters](~~129857~~) operation to query the IDs of all AnalyticDB for MySQL Data Warehouse Edition (V3.0) clusters within a region.
+        # >  You can call the [DescribeDBClusters](~~454250~~) operation to query the IDs of all AnalyticDB for MySQL Data Lakehouse Edition (V3.0) clusters within a region.
         self.dbcluster_id = dbcluster_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(LoadSampleDataSetRequest, self).to_map()
@@ -20344,15 +20350,15 @@
         if m.get('DBClusterId') is not None:
             self.dbcluster_id = m.get('DBClusterId')
         return self
 
 
 class LoadSampleDataSetResponseBody(TeaModel):
     def __init__(self, dbcluster_id=None, request_id=None):
-        # The ID of the AnalyticDB for MySQL Data Warehouse Edition (V3.0) cluster.
+        # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id  # type: str
         # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -21181,19 +21187,19 @@
 class ModifyClusterConnectionStringRequest(TeaModel):
     def __init__(self, connection_string_prefix=None, current_connection_string=None, dbcluster_id=None, port=None):
         # The prefix of the public endpoint.
         # 
         # *   The prefix can contain lowercase letters, digits, and hyphens (-). It must start with a lowercase letter.
         # *   The prefix can be up to 30 characters in length.
         self.connection_string_prefix = connection_string_prefix  # type: str
-        # The current public endpoint of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
+        # The public endpoint of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.current_connection_string = current_connection_string  # type: str
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id  # type: str
-        # The port number that is used to connect to the cluster. Set the value to **3306**.
+        # The port number. Set the value to **3306**.
         self.port = port  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyClusterConnectionStringRequest, self).to_map()
@@ -21222,15 +21228,15 @@
         if m.get('Port') is not None:
             self.port = m.get('Port')
         return self
 
 
 class ModifyClusterConnectionStringResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyClusterConnectionStringResponseBody, self).to_map()
@@ -23224,15 +23230,15 @@
         return self
 
 
 class UnbindAccountRequest(TeaModel):
     def __init__(self, account_name=None, dbcluster_id=None):
         # The name of the database account.
         # 
-        # > You can call the [DescribeAccounts](~~612430~~) operation to view the information about a database account in a cluster, including the name of the database account.
+        # >  You can call the [DescribeAccounts](~~612430~~) operation to query the information about database accounts of an AnalyticDB for MySQL cluster, including database account names.
         self.account_name = account_name  # type: str
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_adb20211201_py2-1.5.1/alibabacloud_adb20211201_py2.egg-info/PKG-INFO` & `alibabacloud_adb20211201_py2-1.5.2/alibabacloud_adb20211201_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-adb20211201-py2
-Version: 1.5.1
+Version: 1.5.2
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201_py2-1.5.1/setup.py` & `alibabacloud_adb20211201_py2-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adb20211201_py2.
 
-Created on 25/03/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adb20211201"
 NAME = "alibabacloud_adb20211201_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adb (20211201) SDK Library for Python2"
```

