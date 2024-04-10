# Comparing `tmp/alibabacloud_alinlp20200629_py2-1.5.0.tar.gz` & `tmp/alibabacloud_alinlp20200629_py2-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alinlp20200629_py2-1.5.0.tar", last modified: Fri Mar 29 01:34:59 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alinlp20200629_py2-1.5.1.tar", last modified: Wed Apr 10 03:27:56 2024, max compression
```

## Comparing `alibabacloud_alinlp20200629_py2-1.5.0.tar` & `alibabacloud_alinlp20200629_py2-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/
--rw-r--r--   0 root         (0) root         (0)      767 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88849 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629/client.py
--rw-r--r--   0 root         (0) root         (0)   249906 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2024-03-29 01:34:59.000000 alibabacloud_alinlp20200629_py2-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)      834 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88953 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629/client.py
+-rw-r--r--   0 root         (0) root         (0)   250390 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-10 03:27:56.000000 alibabacloud_alinlp20200629_py2-1.5.1/setup.py
```

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/ChangeLog.md` & `alibabacloud_alinlp20200629_py2-1.5.1/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-29 Version: 1.5.0
+- Support API PostMSServiceDataImport.
+
+
 2024-03-27 Version: 1.4.0
 - Support API ImportServiceDataV2.
 
 
 2024-03-23 Version: 1.3.0
 - Support API PostISConvRewriter.
 - Support API PostISRetrieveRouter.
```

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/LICENSE` & `alibabacloud_alinlp20200629_py2-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/PKG-INFO` & `alibabacloud_alinlp20200629_py2-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alinlp20200629_py2
-Version: 1.5.0
+Version: 1.5.1
 Summary: Alibaba Cloud alinlp (20200629) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/README-CN.md` & `alibabacloud_alinlp20200629_py2-1.5.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/README.md` & `alibabacloud_alinlp20200629_py2-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629/client.py` & `alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2107,14 +2107,16 @@
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

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629/models.py` & `alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6888,21 +6888,22 @@
         if m.get('body') is not None:
             temp_model = PostMSDataProcessingCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PostMSSearchEnhanceRequest(TeaModel):
-    def __init__(self, body=None, custom_config_info=None, debug=None, fields=None, filters=None, page=None,
-                 queries=None, rank_model_info=None, rows=None, service_id=None, sort=None, type=None, uq=None):
+    def __init__(self, body=None, custom_config_info=None, debug=None, fields=None, filters=None, min_score=None,
+                 page=None, queries=None, rank_model_info=None, rows=None, service_id=None, sort=None, type=None, uq=None):
         self.body = body  # type: str
         self.custom_config_info = custom_config_info  # type: dict[str, any]
         self.debug = debug  # type: bool
         self.fields = fields  # type: list[str]
         self.filters = filters  # type: str
+        self.min_score = min_score  # type: float
         self.page = page  # type: int
         self.queries = queries  # type: str
         self.rank_model_info = rank_model_info  # type: dict[str, any]
         self.rows = rows  # type: int
         self.service_id = service_id  # type: long
         self.sort = sort  # type: list[str]
         self.type = type  # type: str
@@ -6923,14 +6924,16 @@
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
@@ -6953,14 +6956,16 @@
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
@@ -6974,21 +6979,22 @@
         if m.get('Uq') is not None:
             self.uq = m.get('Uq')
         return self
 
 
 class PostMSSearchEnhanceShrinkRequest(TeaModel):
     def __init__(self, body=None, custom_config_info_shrink=None, debug=None, fields_shrink=None, filters=None,
-                 page=None, queries=None, rank_model_info_shrink=None, rows=None, service_id=None, sort_shrink=None,
-                 type=None, uq=None):
+                 min_score=None, page=None, queries=None, rank_model_info_shrink=None, rows=None, service_id=None,
+                 sort_shrink=None, type=None, uq=None):
         self.body = body  # type: str
         self.custom_config_info_shrink = custom_config_info_shrink  # type: str
         self.debug = debug  # type: bool
         self.fields_shrink = fields_shrink  # type: str
         self.filters = filters  # type: str
+        self.min_score = min_score  # type: float
         self.page = page  # type: int
         self.queries = queries  # type: str
         self.rank_model_info_shrink = rank_model_info_shrink  # type: str
         self.rows = rows  # type: int
         self.service_id = service_id  # type: long
         self.sort_shrink = sort_shrink  # type: str
         self.type = type  # type: str
@@ -7009,14 +7015,16 @@
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
@@ -7039,14 +7047,16 @@
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

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/alibabacloud_alinlp20200629_py2.egg-info/PKG-INFO` & `alibabacloud_alinlp20200629_py2-1.5.1/alibabacloud_alinlp20200629_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alinlp20200629-py2
-Version: 1.5.0
+Version: 1.5.1
 Summary: Alibaba Cloud alinlp (20200629) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alinlp20200629_py2-1.5.0/setup.py` & `alibabacloud_alinlp20200629_py2-1.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alinlp20200629_py2.
 
-Created on 29/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alinlp20200629"
 NAME = "alibabacloud_alinlp20200629_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud alinlp (20200629) SDK Library for Python2"
```

