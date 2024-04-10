# Comparing `tmp/alibabacloud_avatar20220130_py2-2.5.2.tar.gz` & `tmp/alibabacloud_avatar20220130_py2-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_avatar20220130_py2-2.5.2.tar", last modified: Tue Feb 27 03:13:28 2024, max compression
+gzip compressed data, was "dist/alibabacloud_avatar20220130_py2-2.5.3.tar", last modified: Wed Apr 10 09:10:00 2024, max compression
```

## Comparing `alibabacloud_avatar20220130_py2-2.5.2.tar` & `alibabacloud_avatar20220130_py2-2.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52349 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130/client.py
--rw-r--r--   0 root         (0) root         (0)   259425 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2024-02-27 03:13:28.000000 alibabacloud_avatar20220130_py2-2.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52349 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130/client.py
+-rw-r--r--   0 root         (0) root         (0)   259425 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 09:10:00.000000 alibabacloud_avatar20220130_py2-2.5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-10 09:09:59.000000 alibabacloud_avatar20220130_py2-2.5.3/setup.py
```

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/ChangeLog.md` & `alibabacloud_avatar20220130_py2-2.5.3/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-02-27 Version: 2.5.2
+- Update API QueryAvatar: update response param.
+- Update API QueryAvatarList: update response param.
+
+
 2024-01-24 Version: 2.5.1
 - Generated python2 2022-01-30 for avatar.
 
 2024-01-17 Version: 2.5.0
 - Generated python2 2022-01-30 for avatar.
 
 2024-01-09 Version: 2.4.2
```

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/LICENSE` & `alibabacloud_avatar20220130_py2-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/PKG-INFO` & `alibabacloud_avatar20220130_py2-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_avatar20220130_py2
-Version: 2.5.2
+Version: 2.5.3
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/README-CN.md` & `alibabacloud_avatar20220130_py2-2.5.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/README.md` & `alibabacloud_avatar20220130_py2-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130/client.py` & `alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130/models.py` & `alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO` & `alibabacloud_avatar20220130_py2-2.5.3/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-avatar20220130-py2
-Version: 2.5.2
+Version: 2.5.3
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130_py2-2.5.2/setup.py` & `alibabacloud_avatar20220130_py2-2.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_avatar20220130_py2.
 
-Created on 27/02/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_avatar20220130"
 NAME = "alibabacloud_avatar20220130_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud avatar (20220130) SDK Library for Python2"
```

