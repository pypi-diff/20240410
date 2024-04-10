# Comparing `tmp/alibabacloud_nis20211216_py2-2.0.1.tar.gz` & `tmp/alibabacloud_nis20211216_py2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_nis20211216_py2-2.0.1.tar", last modified: Thu Mar 21 17:13:09 2024, max compression
+gzip compressed data, was "dist/alibabacloud_nis20211216_py2-2.0.2.tar", last modified: Wed Apr 10 03:23:33 2024, max compression
```

## Comparing `alibabacloud_nis20211216_py2-2.0.1.tar` & `alibabacloud_nis20211216_py2-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:09.000000 alibabacloud_nis20211216_py2-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      243 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-21 17:13:09.000000 alibabacloud_nis20211216_py2-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:09.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26511 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216/client.py
--rw-r--r--   0 root         (0) root         (0)   127148 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:09.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-21 17:13:09.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-21 17:13:09.000000 alibabacloud_nis20211216_py2-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2024-03-21 17:13:08.000000 alibabacloud_nis20211216_py2-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)      447 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26844 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216/client.py
+-rw-r--r--   0 root         (0) root         (0)   127838 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-10 03:23:33.000000 alibabacloud_nis20211216_py2-2.0.2/setup.py
```

### Comparing `alibabacloud_nis20211216_py2-2.0.1/LICENSE` & `alibabacloud_nis20211216_py2-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216_py2-2.0.1/PKG-INFO` & `alibabacloud_nis20211216_py2-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_nis20211216_py2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud nis (20211216) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nis20211216_py2-2.0.1/README-CN.md` & `alibabacloud_nis20211216_py2-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216_py2-2.0.1/README.md` & `alibabacloud_nis20211216_py2-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216/client.py` & `alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,23 +270,27 @@
         runtime = util_models.RuntimeOptions()
         return self.delete_network_reachable_analysis_with_options(request, runtime)
 
     def get_internet_tuple_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = nis_20211216_models.GetInternetTupleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.cloud_ip_list):
+            request.cloud_ip_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.cloud_ip_list, 'CloudIpList', 'json')
         if not UtilClient.is_unset(tmp_req.instance_list):
             request.instance_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.instance_list, 'InstanceList', 'json')
         query = {}
         if not UtilClient.is_unset(request.account_ids):
             query['AccountIds'] = request.account_ids
         if not UtilClient.is_unset(request.begin_time):
             query['BeginTime'] = request.begin_time
         if not UtilClient.is_unset(request.cloud_ip):
             query['CloudIp'] = request.cloud_ip
+        if not UtilClient.is_unset(request.cloud_ip_list_shrink):
+            query['CloudIpList'] = request.cloud_ip_list_shrink
         if not UtilClient.is_unset(request.cloud_isp):
             query['CloudIsp'] = request.cloud_isp
         if not UtilClient.is_unset(request.cloud_port):
             query['CloudPort'] = request.cloud_port
         if not UtilClient.is_unset(request.direction):
             query['Direction'] = request.direction
         if not UtilClient.is_unset(request.end_time):
```

### Comparing `alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216/models.py` & `alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -855,24 +855,26 @@
         if m.get('body') is not None:
             temp_model = DeleteNetworkReachableAnalysisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetInternetTupleRequest(TeaModel):
-    def __init__(self, account_ids=None, begin_time=None, cloud_ip=None, cloud_isp=None, cloud_port=None,
-                 direction=None, end_time=None, instance_id=None, instance_list=None, order_by=None, other_city=None,
-                 other_country=None, other_ip=None, other_isp=None, other_port=None, protocol=None, region_id=None, sort=None,
-                 top_n=None, tuple_type=None, use_multi_account=None):
+    def __init__(self, account_ids=None, begin_time=None, cloud_ip=None, cloud_ip_list=None, cloud_isp=None,
+                 cloud_port=None, direction=None, end_time=None, instance_id=None, instance_list=None, order_by=None,
+                 other_city=None, other_country=None, other_ip=None, other_isp=None, other_port=None, protocol=None,
+                 region_id=None, sort=None, top_n=None, tuple_type=None, use_multi_account=None):
         # The IDs of member accounts.
         self.account_ids = account_ids  # type: list[long]
         # The beginning of the time range to query. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.begin_time = begin_time  # type: long
         # The local IP address.
         self.cloud_ip = cloud_ip  # type: str
+        # The local IP addresses for filtering.
+        self.cloud_ip_list = cloud_ip_list  # type: list[str]
         # The local Internet service provider (ISP).
         # 
         # >  In most cases, the value is Alibaba or Alibaba Cloud.
         self.cloud_isp = cloud_isp  # type: str
         # The local port.
         # 
         # >  This parameter is required only if you set GroupBy to CloudPort.
@@ -965,14 +967,16 @@
         result = dict()
         if self.account_ids is not None:
             result['AccountIds'] = self.account_ids
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.cloud_ip is not None:
             result['CloudIp'] = self.cloud_ip
+        if self.cloud_ip_list is not None:
+            result['CloudIpList'] = self.cloud_ip_list
         if self.cloud_isp is not None:
             result['CloudIsp'] = self.cloud_isp
         if self.cloud_port is not None:
             result['CloudPort'] = self.cloud_port
         if self.direction is not None:
             result['Direction'] = self.direction
         if self.end_time is not None:
@@ -1011,14 +1015,16 @@
         m = m or dict()
         if m.get('AccountIds') is not None:
             self.account_ids = m.get('AccountIds')
         if m.get('BeginTime') is not None:
             self.begin_time = m.get('BeginTime')
         if m.get('CloudIp') is not None:
             self.cloud_ip = m.get('CloudIp')
+        if m.get('CloudIpList') is not None:
+            self.cloud_ip_list = m.get('CloudIpList')
         if m.get('CloudIsp') is not None:
             self.cloud_isp = m.get('CloudIsp')
         if m.get('CloudPort') is not None:
             self.cloud_port = m.get('CloudPort')
         if m.get('Direction') is not None:
             self.direction = m.get('Direction')
         if m.get('EndTime') is not None:
@@ -1051,24 +1057,26 @@
             self.tuple_type = m.get('TupleType')
         if m.get('UseMultiAccount') is not None:
             self.use_multi_account = m.get('UseMultiAccount')
         return self
 
 
 class GetInternetTupleShrinkRequest(TeaModel):
-    def __init__(self, account_ids=None, begin_time=None, cloud_ip=None, cloud_isp=None, cloud_port=None,
-                 direction=None, end_time=None, instance_id=None, instance_list_shrink=None, order_by=None, other_city=None,
-                 other_country=None, other_ip=None, other_isp=None, other_port=None, protocol=None, region_id=None, sort=None,
-                 top_n=None, tuple_type=None, use_multi_account=None):
+    def __init__(self, account_ids=None, begin_time=None, cloud_ip=None, cloud_ip_list_shrink=None, cloud_isp=None,
+                 cloud_port=None, direction=None, end_time=None, instance_id=None, instance_list_shrink=None, order_by=None,
+                 other_city=None, other_country=None, other_ip=None, other_isp=None, other_port=None, protocol=None,
+                 region_id=None, sort=None, top_n=None, tuple_type=None, use_multi_account=None):
         # The IDs of member accounts.
         self.account_ids = account_ids  # type: list[long]
         # The beginning of the time range to query. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.begin_time = begin_time  # type: long
         # The local IP address.
         self.cloud_ip = cloud_ip  # type: str
+        # The local IP addresses for filtering.
+        self.cloud_ip_list_shrink = cloud_ip_list_shrink  # type: str
         # The local Internet service provider (ISP).
         # 
         # >  In most cases, the value is Alibaba or Alibaba Cloud.
         self.cloud_isp = cloud_isp  # type: str
         # The local port.
         # 
         # >  This parameter is required only if you set GroupBy to CloudPort.
@@ -1161,14 +1169,16 @@
         result = dict()
         if self.account_ids is not None:
             result['AccountIds'] = self.account_ids
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.cloud_ip is not None:
             result['CloudIp'] = self.cloud_ip
+        if self.cloud_ip_list_shrink is not None:
+            result['CloudIpList'] = self.cloud_ip_list_shrink
         if self.cloud_isp is not None:
             result['CloudIsp'] = self.cloud_isp
         if self.cloud_port is not None:
             result['CloudPort'] = self.cloud_port
         if self.direction is not None:
             result['Direction'] = self.direction
         if self.end_time is not None:
@@ -1207,14 +1217,16 @@
         m = m or dict()
         if m.get('AccountIds') is not None:
             self.account_ids = m.get('AccountIds')
         if m.get('BeginTime') is not None:
             self.begin_time = m.get('BeginTime')
         if m.get('CloudIp') is not None:
             self.cloud_ip = m.get('CloudIp')
+        if m.get('CloudIpList') is not None:
+            self.cloud_ip_list_shrink = m.get('CloudIpList')
         if m.get('CloudIsp') is not None:
             self.cloud_isp = m.get('CloudIsp')
         if m.get('CloudPort') is not None:
             self.cloud_port = m.get('CloudPort')
         if m.get('Direction') is not None:
             self.direction = m.get('Direction')
         if m.get('EndTime') is not None:
```

### Comparing `alibabacloud_nis20211216_py2-2.0.1/alibabacloud_nis20211216_py2.egg-info/PKG-INFO` & `alibabacloud_nis20211216_py2-2.0.2/alibabacloud_nis20211216_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-nis20211216-py2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud nis (20211216) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nis20211216_py2-2.0.1/setup.py` & `alibabacloud_nis20211216_py2-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_nis20211216_py2.
 
-Created on 21/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_nis20211216"
 NAME = "alibabacloud_nis20211216_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud nis (20211216) SDK Library for Python2"
```

