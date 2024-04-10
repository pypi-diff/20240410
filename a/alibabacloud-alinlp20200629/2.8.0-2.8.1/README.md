# Comparing `tmp/alibabacloud_alinlp20200629-2.8.0.tar.gz` & `tmp/alibabacloud_alinlp20200629-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alinlp20200629-2.8.0.tar", last modified: Fri Mar 29 01:36:08 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alinlp20200629-2.8.1.tar", last modified: Wed Apr 10 03:29:34 2024, max compression
```

## Comparing `alibabacloud_alinlp20200629-2.8.0.tar` & `alibabacloud_alinlp20200629-2.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/
--rw-r--r--   0 root         (0) root         (0)     1106 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2422 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1107 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1192 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629/__init__.py
--rw-r--r--   0 root         (0) root         (0)   218118 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629/client.py
--rw-r--r--   0 root         (0) root         (0)   248835 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2422 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2626 2024-03-29 01:36:08.000000 alibabacloud_alinlp20200629-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   218326 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629/client.py
+-rw-r--r--   0 root         (0) root         (0)   249323 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-10 03:29:34.000000 alibabacloud_alinlp20200629-2.8.1/setup.py
```

### Comparing `alibabacloud_alinlp20200629-2.8.0/ChangeLog.md` & `alibabacloud_alinlp20200629-2.8.1/ChangeLog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-29 Version: 2.8.0
+- Support API PostMSServiceDataImport.
+
+
 2024-03-27 Version: 2.7.0
 - Support API ImportServiceDataV2.
 
 
 2024-03-23 Version: 2.6.0
 - Support API PostISConvRewriter.
 - Support API PostISRetrieveRouter.
```

### Comparing `alibabacloud_alinlp20200629-2.8.0/LICENSE` & `alibabacloud_alinlp20200629-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629-2.8.0/PKG-INFO` & `alibabacloud_alinlp20200629-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alinlp20200629
-Version: 2.8.0
+Version: 2.8.1
 Summary: Alibaba Cloud alinlp (20200629) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alinlp20200629-2.8.0/README-CN.md` & `alibabacloud_alinlp20200629-2.8.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629-2.8.0/README.md` & `alibabacloud_alinlp20200629-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629/client.py` & `alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5046,14 +5046,16 @@
             body['CustomConfigInfo'] = request.custom_config_info_shrink
         if not UtilClient.is_unset(request.debug):
             body['Debug'] = request.debug
         if not UtilClient.is_unset(request.fields_shrink):
             body['Fields'] = request.fields_shrink
         if not UtilClient.is_unset(request.filters):
             body['Filters'] = request.filters
+        if not UtilClient.is_unset(request.min_score):
+            body['MinScore'] = request.min_score
         if not UtilClient.is_unset(request.page):
             body['Page'] = request.page
         if not UtilClient.is_unset(request.queries):
             body['Queries'] = request.queries
         if not UtilClient.is_unset(request.rank_model_info_shrink):
             body['RankModelInfo'] = request.rank_model_info_shrink
         if not UtilClient.is_unset(request.rows):
@@ -5108,14 +5110,16 @@
             body['CustomConfigInfo'] = request.custom_config_info_shrink
         if not UtilClient.is_unset(request.debug):
             body['Debug'] = request.debug
         if not UtilClient.is_unset(request.fields_shrink):
             body['Fields'] = request.fields_shrink
         if not UtilClient.is_unset(request.filters):
             body['Filters'] = request.filters
+        if not UtilClient.is_unset(request.min_score):
+            body['MinScore'] = request.min_score
         if not UtilClient.is_unset(request.page):
             body['Page'] = request.page
         if not UtilClient.is_unset(request.queries):
             body['Queries'] = request.queries
         if not UtilClient.is_unset(request.rank_model_info_shrink):
             body['RankModelInfo'] = request.rank_model_info_shrink
         if not UtilClient.is_unset(request.rows):
```

### Comparing `alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629/models.py` & `alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7878,28 +7878,30 @@
     def __init__(
         self,
         body: str = None,
         custom_config_info: Dict[str, Any] = None,
         debug: bool = None,
         fields: List[str] = None,
         filters: str = None,
+        min_score: float = None,
         page: int = None,
         queries: str = None,
         rank_model_info: Dict[str, Any] = None,
         rows: int = None,
         service_id: int = None,
         sort: List[str] = None,
         type: str = None,
         uq: str = None,
     ):
         self.body = body
         self.custom_config_info = custom_config_info
         self.debug = debug
         self.fields = fields
         self.filters = filters
+        self.min_score = min_score
         self.page = page
         self.queries = queries
         self.rank_model_info = rank_model_info
         self.rows = rows
         self.service_id = service_id
         self.sort = sort
         self.type = type
@@ -7920,14 +7922,16 @@
             result['CustomConfigInfo'] = self.custom_config_info
         if self.debug is not None:
             result['Debug'] = self.debug
         if self.fields is not None:
             result['Fields'] = self.fields
         if self.filters is not None:
             result['Filters'] = self.filters
+        if self.min_score is not None:
+            result['MinScore'] = self.min_score
         if self.page is not None:
             result['Page'] = self.page
         if self.queries is not None:
             result['Queries'] = self.queries
         if self.rank_model_info is not None:
             result['RankModelInfo'] = self.rank_model_info
         if self.rows is not None:
@@ -7950,14 +7954,16 @@
             self.custom_config_info = m.get('CustomConfigInfo')
         if m.get('Debug') is not None:
             self.debug = m.get('Debug')
         if m.get('Fields') is not None:
             self.fields = m.get('Fields')
         if m.get('Filters') is not None:
             self.filters = m.get('Filters')
+        if m.get('MinScore') is not None:
+            self.min_score = m.get('MinScore')
         if m.get('Page') is not None:
             self.page = m.get('Page')
         if m.get('Queries') is not None:
             self.queries = m.get('Queries')
         if m.get('RankModelInfo') is not None:
             self.rank_model_info = m.get('RankModelInfo')
         if m.get('Rows') is not None:
@@ -7977,28 +7983,30 @@
     def __init__(
         self,
         body: str = None,
         custom_config_info_shrink: str = None,
         debug: bool = None,
         fields_shrink: str = None,
         filters: str = None,
+        min_score: float = None,
         page: int = None,
         queries: str = None,
         rank_model_info_shrink: str = None,
         rows: int = None,
         service_id: int = None,
         sort_shrink: str = None,
         type: str = None,
         uq: str = None,
     ):
         self.body = body
         self.custom_config_info_shrink = custom_config_info_shrink
         self.debug = debug
         self.fields_shrink = fields_shrink
         self.filters = filters
+        self.min_score = min_score
         self.page = page
         self.queries = queries
         self.rank_model_info_shrink = rank_model_info_shrink
         self.rows = rows
         self.service_id = service_id
         self.sort_shrink = sort_shrink
         self.type = type
@@ -8019,14 +8027,16 @@
             result['CustomConfigInfo'] = self.custom_config_info_shrink
         if self.debug is not None:
             result['Debug'] = self.debug
         if self.fields_shrink is not None:
             result['Fields'] = self.fields_shrink
         if self.filters is not None:
             result['Filters'] = self.filters
+        if self.min_score is not None:
+            result['MinScore'] = self.min_score
         if self.page is not None:
             result['Page'] = self.page
         if self.queries is not None:
             result['Queries'] = self.queries
         if self.rank_model_info_shrink is not None:
             result['RankModelInfo'] = self.rank_model_info_shrink
         if self.rows is not None:
@@ -8049,14 +8059,16 @@
             self.custom_config_info_shrink = m.get('CustomConfigInfo')
         if m.get('Debug') is not None:
             self.debug = m.get('Debug')
         if m.get('Fields') is not None:
             self.fields_shrink = m.get('Fields')
         if m.get('Filters') is not None:
             self.filters = m.get('Filters')
+        if m.get('MinScore') is not None:
+            self.min_score = m.get('MinScore')
         if m.get('Page') is not None:
             self.page = m.get('Page')
         if m.get('Queries') is not None:
             self.queries = m.get('Queries')
         if m.get('RankModelInfo') is not None:
             self.rank_model_info_shrink = m.get('RankModelInfo')
         if m.get('Rows') is not None:
```

### Comparing `alibabacloud_alinlp20200629-2.8.0/alibabacloud_alinlp20200629.egg-info/PKG-INFO` & `alibabacloud_alinlp20200629-2.8.1/alibabacloud_alinlp20200629.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alinlp20200629
-Version: 2.8.0
+Version: 2.8.1
 Summary: Alibaba Cloud alinlp (20200629) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alinlp20200629-2.8.0/setup.py` & `alibabacloud_alinlp20200629-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alinlp20200629.
 
-Created on 29/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alinlp20200629"
 NAME = "alibabacloud_alinlp20200629" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud alinlp (20200629) SDK Library for Python"
```

