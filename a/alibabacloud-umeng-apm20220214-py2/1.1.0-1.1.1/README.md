# Comparing `tmp/alibabacloud_umeng-apm20220214_py2-1.1.0.tar.gz` & `tmp/alibabacloud_umeng-apm20220214_py2-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_umeng-apm20220214_py2-1.1.0.tar", last modified: Fri Aug 11 09:51:03 2023, max compression
+gzip compressed data, was "dist/alibabacloud_umeng-apm20220214_py2-1.1.1.tar", last modified: Tue Apr  9 02:18:13 2024, max compression
```

## Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0.tar` & `alibabacloud_umeng-apm20220214_py2-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      471 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18549 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214/client.py
--rw-r--r--   0 root         (0) root         (0)    58865 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3142 2023-08-11 09:51:03.000000 alibabacloud_umeng-apm20220214_py2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      544 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18549 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214/client.py
+-rw-r--r--   0 root         (0) root         (0)    57337 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-09 02:18:13.000000 alibabacloud_umeng-apm20220214_py2-1.1.1/setup.py
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/LICENSE` & `alibabacloud_umeng-apm20220214_py2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/PKG-INFO` & `alibabacloud_umeng-apm20220214_py2-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_umeng-apm20220214_py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/README-CN.md` & `alibabacloud_umeng-apm20220214_py2-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/README.md` & `alibabacloud_umeng-apm20220214_py2-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214/client.py` & `alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214/models.py` & `alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,17 +229,14 @@
 class GetH5PageTrendResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetH5PageTrendResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetH5PageTrendResponse, self).to_map()
         if _map is not None:
             return _map
@@ -414,17 +411,14 @@
 class GetLaunchTrendResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetLaunchTrendResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetLaunchTrendResponse, self).to_map()
         if _map is not None:
             return _map
@@ -588,17 +582,14 @@
 class GetNativePageTrendResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetNativePageTrendResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetNativePageTrendResponse, self).to_map()
         if _map is not None:
             return _map
@@ -763,17 +754,14 @@
 class GetNetworkTrendResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetNetworkTrendResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetNetworkTrendResponse, self).to_map()
         if _map is not None:
             return _map
@@ -843,17 +831,17 @@
         return self
 
 
 class GetStatTrendResponseBodyData(TeaModel):
     def __init__(self, affected_user_count=None, affected_user_rate=None, error_count=None, error_rate=None,
                  time_point=None):
         self.affected_user_count = affected_user_count  # type: long
-        self.affected_user_rate = affected_user_rate  # type: long
+        self.affected_user_rate = affected_user_rate  # type: float
         self.error_count = error_count  # type: long
-        self.error_rate = error_rate  # type: long
+        self.error_rate = error_rate  # type: float
         self.time_point = time_point  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetStatTrendResponseBodyData, self).to_map()
@@ -938,17 +926,14 @@
 class GetStatTrendResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetStatTrendResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetStatTrendResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1118,17 +1103,14 @@
 class GetSymUploadParamResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetSymUploadParamResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetSymUploadParamResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1283,17 +1265,14 @@
 class GetTodayStatTrendResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetTodayStatTrendResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetTodayStatTrendResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1390,17 +1369,14 @@
 class UpdateAlertPlanResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateAlertPlanResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateAlertPlanResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1575,17 +1551,14 @@
 class UploadSymbolFileResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UploadSymbolFileResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UploadSymbolFileResponse, self).to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO` & `alibabacloud_umeng-apm20220214_py2-1.1.1/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-umeng-apm20220214-py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.1.0/setup.py` & `alibabacloud_umeng-apm20220214_py2-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_umeng-apm20220214_py2.
 
-Created on 11/08/2023
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_umeng_apm20220214"
 NAME = "alibabacloud_umeng-apm20220214_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud umeng-apm (20220214) SDK Library for Python2"
@@ -39,15 +39,15 @@
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_oss_sdk_py2>=0.0.1, <1.0.0",
     "alibabacloud_openplatform20191219_py2>=1.0.0, <2.0.0",
     "alibabacloud_oss_util_py2>=0.0.1, <1.0.0",
     "alibabacloud_tea_fileform_py2>=0.0.1, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```

