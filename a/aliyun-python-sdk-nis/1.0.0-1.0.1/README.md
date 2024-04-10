# Comparing `tmp/aliyun-python-sdk-nis-1.0.0.tar.gz` & `tmp/aliyun-python-sdk-nis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-nis-1.0.0.tar", last modified: Tue Aug 16 08:56:26 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-nis-1.0.1.tar", last modified: Wed Apr 10 03:21:05 2024, max compression
```

## Comparing `aliyun-python-sdk-nis-1.0.0.tar` & `aliyun-python-sdk-nis-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      575 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      426 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/request/v20211216/
--rw-r--r--   0 root         (0) root         (0)     2029 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/request/v20211216/GetNatTopNRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/aliyunsdknis/request/v20211216/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-08-16 08:56:26.000000 aliyun-python-sdk-nis-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2022-08-16 08:56:25.000000 aliyun-python-sdk-nis-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/
+-rw-r--r--   0 root         (0) root         (0)     2783 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/CreateAndAnalyzeNetworkPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3888 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/CreateNetworkPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/CreateNetworkReachableAnalysisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/DeleteNetworkPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/DeleteNetworkReachableAnalysisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4979 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/GetInternetTupleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/GetNatTopNRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/GetNetworkReachableAnalysisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4325 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/GetTransitRouterFlowTopNRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/GetVbrFlowTopNRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-10 03:21:05.000000 aliyun-python-sdk-nis-1.0.1/setup.py
```

### Comparing `aliyun-python-sdk-nis-1.0.0/LICENSE` & `aliyun-python-sdk-nis-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nis-1.0.0/PKG-INFO` & `aliyun-python-sdk-nis-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-nis
-Version: 1.0.0
+Version: 1.0.1
 Summary: The nis module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-nis
```

### Comparing `aliyun-python-sdk-nis-1.0.0/README.rst` & `aliyun-python-sdk-nis-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nis-1.0.0/aliyun_python_sdk_nis.egg-info/PKG-INFO` & `aliyun-python-sdk-nis-1.0.1/aliyun_python_sdk_nis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-nis
-Version: 1.0.0
+Version: 1.0.1
 Summary: The nis module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-nis
```

### Comparing `aliyun-python-sdk-nis-1.0.0/aliyunsdknis/request/v20211216/GetNatTopNRequest.py` & `aliyun-python-sdk-nis-1.0.1/aliyunsdknis/request/v20211216/GetNatTopNRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nis-1.0.0/setup.py` & `aliyun-python-sdk-nis-1.0.1/setup.py`

 * *Files identical despite different names*

