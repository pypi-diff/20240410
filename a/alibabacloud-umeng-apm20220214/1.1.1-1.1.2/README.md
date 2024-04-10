# Comparing `tmp/alibabacloud_umeng-apm20220214-1.1.1.tar.gz` & `tmp/alibabacloud_umeng-apm20220214-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_umeng-apm20220214-1.1.1.tar", last modified: Tue Apr  9 02:18:34 2024, max compression
+gzip compressed data, was "dist/alibabacloud_umeng-apm20220214-1.1.2.tar", last modified: Wed Apr 10 07:15:00 2024, max compression
```

## Comparing `alibabacloud_umeng-apm20220214-1.1.1.tar` & `alibabacloud_umeng-apm20220214-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2443 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41744 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/client.py
--rw-r--r--   0 root         (0) root         (0)    57226 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2443 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2834 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41744 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/client.py
+-rw-r--r--   0 root         (0) root         (0)    57230 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/setup.py
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/LICENSE` & `alibabacloud_umeng-apm20220214-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/PKG-INFO` & `alibabacloud_umeng-apm20220214-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_umeng-apm20220214
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/README-CN.md` & `alibabacloud_umeng-apm20220214-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/README.md` & `alibabacloud_umeng-apm20220214-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/client.py` & `alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/models.py` & `alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1341,17 +1341,17 @@
         return self
 
 
 class GetTodayStatTrendResponseBodyData(TeaModel):
     def __init__(
         self,
         affected_user_count: int = None,
-        affected_user_rate: int = None,
+        affected_user_rate: float = None,
         error_count: int = None,
-        error_rate: int = None,
+        error_rate: float = None,
         time_point: str = None,
     ):
         self.affected_user_count = affected_user_count
         self.affected_user_rate = affected_user_rate
         self.error_count = error_count
         self.error_rate = error_rate
         self.time_point = time_point
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO` & `alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-umeng-apm20220214
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.1/setup.py` & `alibabacloud_umeng-apm20220214-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_umeng-apm20220214.
 
-Created on 09/04/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_umeng_apm20220214"
 NAME = "alibabacloud_umeng-apm20220214" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud umeng-apm (20220214) SDK Library for Python"
```

