# Comparing `tmp/alibabacloud_dm20170622-1.2.1.tar.gz` & `tmp/alibabacloud_dm20170622-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dm20170622-1.2.1.tar", last modified: Tue Feb 20 17:12:45 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dm20170622-1.2.2.tar", last modified: Wed Apr 10 17:10:04 2024, max compression
```

## Comparing `alibabacloud_dm20170622-1.2.1.tar` & `alibabacloud_dm20170622-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      258 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152318 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622/client.py
--rw-r--r--   0 root         (0) root         (0)   235544 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-20 17:12:45.000000 alibabacloud_dm20170622-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2024-02-20 17:12:44.000000 alibabacloud_dm20170622-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)      530 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   152318 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622/client.py
+-rw-r--r--   0 root         (0) root         (0)   236112 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-10 17:10:04.000000 alibabacloud_dm20170622-1.2.2/setup.py
```

### Comparing `alibabacloud_dm20170622-1.2.1/LICENSE` & `alibabacloud_dm20170622-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20170622-1.2.1/PKG-INFO` & `alibabacloud_dm20170622-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dm20170622
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alibaba Cloud Dm (20170622) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20170622-1.2.1/README-CN.md` & `alibabacloud_dm20170622-1.2.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20170622-1.2.1/README.md` & `alibabacloud_dm20170622-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622/client.py` & `alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622/models.py` & `alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6380,60 +6380,72 @@
         return self
 
 
 class SenderStatisticsDetailByParamResponseBodyDataMailDetail(TeaModel):
     def __init__(
         self,
         account_name: str = None,
+        error_classification: str = None,
         last_update_time: str = None,
         message: str = None,
         status: int = None,
+        subject: str = None,
         to_address: str = None,
         utc_last_update_time: str = None,
     ):
         self.account_name = account_name
+        self.error_classification = error_classification
         self.last_update_time = last_update_time
         self.message = message
         self.status = status
+        self.subject = subject
         self.to_address = to_address
         self.utc_last_update_time = utc_last_update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.account_name is not None:
             result['AccountName'] = self.account_name
+        if self.error_classification is not None:
+            result['ErrorClassification'] = self.error_classification
         if self.last_update_time is not None:
             result['LastUpdateTime'] = self.last_update_time
         if self.message is not None:
             result['Message'] = self.message
         if self.status is not None:
             result['Status'] = self.status
+        if self.subject is not None:
+            result['Subject'] = self.subject
         if self.to_address is not None:
             result['ToAddress'] = self.to_address
         if self.utc_last_update_time is not None:
             result['UtcLastUpdateTime'] = self.utc_last_update_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AccountName') is not None:
             self.account_name = m.get('AccountName')
+        if m.get('ErrorClassification') is not None:
+            self.error_classification = m.get('ErrorClassification')
         if m.get('LastUpdateTime') is not None:
             self.last_update_time = m.get('LastUpdateTime')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('Status') is not None:
             self.status = m.get('Status')
+        if m.get('Subject') is not None:
+            self.subject = m.get('Subject')
         if m.get('ToAddress') is not None:
             self.to_address = m.get('ToAddress')
         if m.get('UtcLastUpdateTime') is not None:
             self.utc_last_update_time = m.get('UtcLastUpdateTime')
         return self
```

### Comparing `alibabacloud_dm20170622-1.2.1/alibabacloud_dm20170622.egg-info/PKG-INFO` & `alibabacloud_dm20170622-1.2.2/alibabacloud_dm20170622.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dm20170622
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alibaba Cloud Dm (20170622) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20170622-1.2.1/setup.py` & `alibabacloud_dm20170622-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dm20170622.
 
-Created on 20/02/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dm20170622"
 NAME = "alibabacloud_dm20170622" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dm (20170622) SDK Library for Python"
```

