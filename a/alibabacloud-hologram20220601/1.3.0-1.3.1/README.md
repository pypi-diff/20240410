# Comparing `tmp/alibabacloud_hologram20220601-1.3.0.tar.gz` & `tmp/alibabacloud_hologram20220601-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hologram20220601-1.3.0.tar", last modified: Thu Mar 14 17:14:36 2024, max compression
+gzip compressed data, was "dist/alibabacloud_hologram20220601-1.3.1.tar", last modified: Wed Apr 10 17:10:21 2024, max compression
```

## Comparing `alibabacloud_hologram20220601-1.3.0.tar` & `alibabacloud_hologram20220601-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      827 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67272 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601/client.py
--rw-r--r--   0 root         (0) root         (0)   119287 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-14 17:14:36.000000 alibabacloud_hologram20220601-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67900 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601/client.py
+-rw-r--r--   0 root         (0) root         (0)   120091 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-10 17:10:21.000000 alibabacloud_hologram20220601-1.3.1/setup.py
```

### Comparing `alibabacloud_hologram20220601-1.3.0/ChangeLog.md` & `alibabacloud_hologram20220601-1.3.1/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2024-03-14 Version: 1.3.0
+- Support API ChangeResourceGroup.
+- Support API DisableHiveAccess.
+- Support API EnableHiveAccess.
+- Support API GetWarehouseDetail.
+- Support API ListWarehouses.
+- Update API GetInstance: update response param.
+
+
 2024-02-21 Version: 1.2.0
 - Support API ChangeResourceGroup.
 - Support API DisableHiveAccess.
 - Support API EnableHiveAccess.
 - Support API GetWarehouseDetail.
 - Support API ListWarehouses.
```

### Comparing `alibabacloud_hologram20220601-1.3.0/LICENSE` & `alibabacloud_hologram20220601-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.3.0/PKG-INFO` & `alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_hologram20220601
-Version: 1.3.0
+Name: alibabacloud-hologram20220601
+Version: 1.3.1
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.3.0/README-CN.md` & `alibabacloud_hologram20220601-1.3.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.3.0/README.md` & `alibabacloud_hologram20220601-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601/client.py` & `alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,16 @@
             body['chargeType'] = request.charge_type
         if not UtilClient.is_unset(request.cold_storage_size):
             body['coldStorageSize'] = request.cold_storage_size
         if not UtilClient.is_unset(request.cpu):
             body['cpu'] = request.cpu
         if not UtilClient.is_unset(request.duration):
             body['duration'] = request.duration
+        if not UtilClient.is_unset(request.enable_serverless_computing):
+            body['enableServerlessComputing'] = request.enable_serverless_computing
         if not UtilClient.is_unset(request.gateway_count):
             body['gatewayCount'] = request.gateway_count
         if not UtilClient.is_unset(request.initial_databases):
             body['initialDatabases'] = request.initial_databases
         if not UtilClient.is_unset(request.instance_name):
             body['instanceName'] = request.instance_name
         if not UtilClient.is_unset(request.instance_type):
@@ -253,14 +255,16 @@
             body['chargeType'] = request.charge_type
         if not UtilClient.is_unset(request.cold_storage_size):
             body['coldStorageSize'] = request.cold_storage_size
         if not UtilClient.is_unset(request.cpu):
             body['cpu'] = request.cpu
         if not UtilClient.is_unset(request.duration):
             body['duration'] = request.duration
+        if not UtilClient.is_unset(request.enable_serverless_computing):
+            body['enableServerlessComputing'] = request.enable_serverless_computing
         if not UtilClient.is_unset(request.gateway_count):
             body['gatewayCount'] = request.gateway_count
         if not UtilClient.is_unset(request.initial_databases):
             body['initialDatabases'] = request.initial_databases
         if not UtilClient.is_unset(request.instance_name):
             body['instanceName'] = request.instance_name
         if not UtilClient.is_unset(request.instance_type):
@@ -1202,14 +1206,16 @@
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.cold_storage_size):
             body['coldStorageSize'] = request.cold_storage_size
         if not UtilClient.is_unset(request.cpu):
             body['cpu'] = request.cpu
+        if not UtilClient.is_unset(request.enable_serverless_computing):
+            body['enableServerlessComputing'] = request.enable_serverless_computing
         if not UtilClient.is_unset(request.gateway_count):
             body['gatewayCount'] = request.gateway_count
         if not UtilClient.is_unset(request.scale_type):
             body['scaleType'] = request.scale_type
         if not UtilClient.is_unset(request.storage_size):
             body['storageSize'] = request.storage_size
         req = open_api_models.OpenApiRequest(
@@ -1251,14 +1257,16 @@
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.cold_storage_size):
             body['coldStorageSize'] = request.cold_storage_size
         if not UtilClient.is_unset(request.cpu):
             body['cpu'] = request.cpu
+        if not UtilClient.is_unset(request.enable_serverless_computing):
+            body['enableServerlessComputing'] = request.enable_serverless_computing
         if not UtilClient.is_unset(request.gateway_count):
             body['gatewayCount'] = request.gateway_count
         if not UtilClient.is_unset(request.scale_type):
             body['scaleType'] = request.scale_type
         if not UtilClient.is_unset(request.storage_size):
             body['storageSize'] = request.storage_size
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601/models.py` & `alibabacloud_hologram20220601-1.3.1/alibabacloud_hologram20220601/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         self,
         auto_pay: bool = None,
         auto_renew: bool = None,
         charge_type: str = None,
         cold_storage_size: int = None,
         cpu: int = None,
         duration: int = None,
+        enable_serverless_computing: bool = None,
         gateway_count: int = None,
         initial_databases: str = None,
         instance_name: str = None,
         instance_type: str = None,
         leader_instance_id: str = None,
         pricing_cycle: str = None,
         region_id: str = None,
@@ -177,14 +178,15 @@
         # 
         # *   The specifications of 8-core 32 GB (number of compute nodes: 1) are for trial use only and cannot be used for production.
         self.cpu = cpu
         # The validity period of the instance that you want to purchase. For example, you can specify a validity period of two months.
         # 
         # > You do not need to configure this parameter for pay-as-you-go instances.
         self.duration = duration
+        self.enable_serverless_computing = enable_serverless_computing
         # The number of gateways. Valid values: 2 to 50.
         # 
         # > This parameter is required only for virtual warehouse instances.
         self.gateway_count = gateway_count
         self.initial_databases = initial_databases
         # The name of the Hologres instance that you want to purchase. The name must be 2 to 64 characters in length.
         self.instance_name = instance_name
@@ -254,14 +256,16 @@
             result['chargeType'] = self.charge_type
         if self.cold_storage_size is not None:
             result['coldStorageSize'] = self.cold_storage_size
         if self.cpu is not None:
             result['cpu'] = self.cpu
         if self.duration is not None:
             result['duration'] = self.duration
+        if self.enable_serverless_computing is not None:
+            result['enableServerlessComputing'] = self.enable_serverless_computing
         if self.gateway_count is not None:
             result['gatewayCount'] = self.gateway_count
         if self.initial_databases is not None:
             result['initialDatabases'] = self.initial_databases
         if self.instance_name is not None:
             result['instanceName'] = self.instance_name
         if self.instance_type is not None:
@@ -294,14 +298,16 @@
             self.charge_type = m.get('chargeType')
         if m.get('coldStorageSize') is not None:
             self.cold_storage_size = m.get('coldStorageSize')
         if m.get('cpu') is not None:
             self.cpu = m.get('cpu')
         if m.get('duration') is not None:
             self.duration = m.get('duration')
+        if m.get('enableServerlessComputing') is not None:
+            self.enable_serverless_computing = m.get('enableServerlessComputing')
         if m.get('gatewayCount') is not None:
             self.gateway_count = m.get('gatewayCount')
         if m.get('initialDatabases') is not None:
             self.initial_databases = m.get('initialDatabases')
         if m.get('instanceName') is not None:
             self.instance_name = m.get('instanceName')
         if m.get('instanceType') is not None:
@@ -3058,14 +3064,15 @@
 
 
 class ScaleInstanceRequest(TeaModel):
     def __init__(
         self,
         cold_storage_size: int = None,
         cpu: int = None,
+        enable_serverless_computing: bool = None,
         gateway_count: int = None,
         scale_type: str = None,
         storage_size: int = None,
     ):
         # The infrequent access (IA) storage space of the instance. Unit: GB.
         # 
         # > Ignore this parameter for pay-as-you-go instances.
@@ -3086,14 +3093,15 @@
         # 
         # *   If you want to set this parameter to specifications with more than 1,024 compute units (CUs), you must submit a ticket.
         # 
         # *   This parameter is invalid for Hologres Shared Cluster instances.
         # 
         # *   The specifications of 8-core 32GB (number of compute nodes: 1) are for trial use only and cannot be used for production.
         self.cpu = cpu
+        self.enable_serverless_computing = enable_serverless_computing
         # The number of gateways. Valid values: 2 to 50.
         # 
         # > This parameter is required only for virtual warehouse instances.
         self.gateway_count = gateway_count
         # The specification change type. Valid values:
         # 
         # *   UPGRADE
@@ -3119,28 +3127,32 @@
             return _map
 
         result = dict()
         if self.cold_storage_size is not None:
             result['coldStorageSize'] = self.cold_storage_size
         if self.cpu is not None:
             result['cpu'] = self.cpu
+        if self.enable_serverless_computing is not None:
+            result['enableServerlessComputing'] = self.enable_serverless_computing
         if self.gateway_count is not None:
             result['gatewayCount'] = self.gateway_count
         if self.scale_type is not None:
             result['scaleType'] = self.scale_type
         if self.storage_size is not None:
             result['storageSize'] = self.storage_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('coldStorageSize') is not None:
             self.cold_storage_size = m.get('coldStorageSize')
         if m.get('cpu') is not None:
             self.cpu = m.get('cpu')
+        if m.get('enableServerlessComputing') is not None:
+            self.enable_serverless_computing = m.get('enableServerlessComputing')
         if m.get('gatewayCount') is not None:
             self.gateway_count = m.get('gatewayCount')
         if m.get('scaleType') is not None:
             self.scale_type = m.get('scaleType')
         if m.get('storageSize') is not None:
             self.storage_size = m.get('storageSize')
         return self
```

### Comparing `alibabacloud_hologram20220601-1.3.0/alibabacloud_hologram20220601.egg-info/PKG-INFO` & `alibabacloud_hologram20220601-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-hologram20220601
-Version: 1.3.0
+Name: alibabacloud_hologram20220601
+Version: 1.3.1
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.3.0/setup.py` & `alibabacloud_hologram20220601-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hologram20220601.
 
-Created on 14/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hologram20220601"
 NAME = "alibabacloud_hologram20220601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Hologres (20220601) SDK Library for Python"
```

