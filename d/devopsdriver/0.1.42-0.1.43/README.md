# Comparing `tmp/devopsdriver-0.1.42.tar.gz` & `tmp/devopsdriver-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.42.tar", last modified: Wed Apr 10 06:50:06 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.43.tar", last modified: Wed Apr 10 07:15:37 2024, max compression
```

## Comparing `devopsdriver-0.1.42.tar` & `devopsdriver-0.1.43.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.631888 devopsdriver-0.1.42/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.42/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 06:50:06.631680 devopsdriver-0.1.42/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-10 06:49:15.000000 devopsdriver-0.1.42/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.627342 devopsdriver-0.1.42/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-10 06:49:03.000000 devopsdriver-0.1.42/devopsdriver/__init__.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.628554 devopsdriver-0.1.42/devopsdriver/azdo/
--rw-r--r--   0 marcp      (501) staff       (20)      431 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)      843 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/azureobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     2107 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/clients.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.629079 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/
--rw-r--r--   0 marcp      (501) staff       (20)        0 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)      672 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/client.py
--rw-r--r--   0 marcp      (501) staff       (20)      667 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/log.py
--rw-r--r--   0 marcp      (501) staff       (20)      918 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/pipeline.py
--rw-r--r--   0 marcp      (501) staff       (20)     1186 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/run.py
--rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.42/devopsdriver/azdo/timestamp.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.629426 devopsdriver-0.1.42/devopsdriver/azdo/workitem/
--rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.42/devopsdriver/azdo/workitem/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     2966 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/workitem/client.py
--rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.42/devopsdriver/azdo/workitem/wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     1477 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/dataobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/devopsdriver/manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.42/devopsdriver/sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/devopsdriver/settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.42/devopsdriver/template.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.629575 devopsdriver-0.1.42/devopsdriver/templates/
--rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/devopsdriver/templates/manage_settings.txt.mako
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.631255 devopsdriver-0.1.42/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     1256 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/entry_points.txt
--rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-08 16:56:00.000000 devopsdriver-0.1.42/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-10 06:50:06.631925 devopsdriver-0.1.42/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.631090 devopsdriver-0.1.42/tests/
--rw-r--r--   0 marcp      (501) staff       (20)     4787 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_azureobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     5497 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     1097 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_pipeline.py
--rw-r--r--   0 marcp      (501) staff       (20)      888 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_pipeline_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     1685 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_pipeline_run.py
--rw-r--r--   0 marcp      (501) staff       (20)     9588 2024-04-10 05:10:33.000000 devopsdriver-0.1.42/tests/test_azure_timestamp.py
--rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.42/tests/test_azure_workitem_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.42/tests/test_azure_workitem_wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)      830 2024-04-10 05:10:33.000000 devopsdriver-0.1.42/tests/test_dataobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/tests/test_manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.42/tests/test_sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/tests/test_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.42/tests/test_template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.497947 devopsdriver-0.1.43/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.43/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 07:15:37.497742 devopsdriver-0.1.43/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-10 07:14:06.000000 devopsdriver-0.1.43/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.493303 devopsdriver-0.1.43/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-10 07:14:08.000000 devopsdriver-0.1.43/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.494478 devopsdriver-0.1.43/devopsdriver/azdo/
+-rw-r--r--   0 marcp      (501) staff       (20)      431 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)      843 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/azureobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2107 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/clients.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.495035 devopsdriver-0.1.43/devopsdriver/azdo/pipeline/
+-rw-r--r--   0 marcp      (501) staff       (20)        0 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/pipeline/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)      672 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/pipeline/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)      667 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/pipeline/log.py
+-rw-r--r--   0 marcp      (501) staff       (20)      918 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/pipeline/pipeline.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1191 2024-04-10 07:14:31.000000 devopsdriver-0.1.43/devopsdriver/azdo/pipeline/run.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.43/devopsdriver/azdo/timestamp.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.495391 devopsdriver-0.1.43/devopsdriver/azdo/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.43/devopsdriver/azdo/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2966 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/azdo/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.43/devopsdriver/azdo/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1477 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/devopsdriver/dataobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.43/devopsdriver/manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.43/devopsdriver/sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.43/devopsdriver/settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.43/devopsdriver/template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.495548 devopsdriver-0.1.43/devopsdriver/templates/
+-rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.43/devopsdriver/templates/manage_settings.txt.mako
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.497304 devopsdriver-0.1.43/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 07:15:37.000000 devopsdriver-0.1.43/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     1256 2024-04-10 07:15:37.000000 devopsdriver-0.1.43/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-10 07:15:37.000000 devopsdriver-0.1.43/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-10 07:15:37.000000 devopsdriver-0.1.43/devopsdriver.egg-info/entry_points.txt
+-rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-10 07:15:37.000000 devopsdriver-0.1.43/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-10 07:15:37.000000 devopsdriver-0.1.43/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-08 16:56:00.000000 devopsdriver-0.1.43/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-10 07:15:37.497981 devopsdriver-0.1.43/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 07:15:37.497159 devopsdriver-0.1.43/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     4787 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/tests/test_azure_azureobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     5497 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1097 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/tests/test_azure_pipeline.py
+-rw-r--r--   0 marcp      (501) staff       (20)      888 2024-04-10 06:48:39.000000 devopsdriver-0.1.43/tests/test_azure_pipeline_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1707 2024-04-10 07:14:31.000000 devopsdriver-0.1.43/tests/test_azure_pipeline_run.py
+-rw-r--r--   0 marcp      (501) staff       (20)     9588 2024-04-10 05:10:33.000000 devopsdriver-0.1.43/tests/test_azure_timestamp.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.43/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.43/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)      830 2024-04-10 05:10:33.000000 devopsdriver-0.1.43/tests/test_dataobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.43/tests/test_manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.43/tests/test_sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.43/tests/test_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.43/tests/test_template.py
```

### Comparing `devopsdriver-0.1.42/LICENSE` & `devopsdriver-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/PKG-INFO` & `devopsdriver-0.1.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.42
+Version: 0.1.43
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -56,15 +56,15 @@
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: coverage>=7.4.4; extra == "test"
 Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.42&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.42/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.43&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.43/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.42/README.md` & `devopsdriver-0.1.43/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.42&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.42/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.43&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.43/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/azureobject.py` & `devopsdriver-0.1.43/devopsdriver/azdo/azureobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/clients.py` & `devopsdriver-0.1.43/devopsdriver/azdo/clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/pipeline/client.py` & `devopsdriver-0.1.43/devopsdriver/azdo/pipeline/client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/pipeline/log.py` & `devopsdriver-0.1.43/devopsdriver/azdo/pipeline/log.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/pipeline/pipeline.py` & `devopsdriver-0.1.43/devopsdriver/azdo/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/pipeline/run.py` & `devopsdriver-0.1.43/devopsdriver/azdo/pipeline/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,9 +37,9 @@
 
     def logs(self):
         """Get Logs for the run"""
         return [
             Log(l)
             for l in self.client.list_logs(
                 self.project, self.pipeline.id, self.raw.id, expand="signedContent"
-            )
+            ).logs
         ]
```

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/timestamp.py` & `devopsdriver-0.1.43/devopsdriver/azdo/timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/workitem/client.py` & `devopsdriver-0.1.43/devopsdriver/azdo/workitem/client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/azdo/workitem/wiql.py` & `devopsdriver-0.1.43/devopsdriver/azdo/workitem/wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/dataobject.py` & `devopsdriver-0.1.43/devopsdriver/dataobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/manage_settings.py` & `devopsdriver-0.1.43/devopsdriver/manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/sendmail.py` & `devopsdriver-0.1.43/devopsdriver/sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/settings.py` & `devopsdriver-0.1.43/devopsdriver/settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver/template.py` & `devopsdriver-0.1.43/devopsdriver/template.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.43/devopsdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.42
+Version: 0.1.43
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -56,15 +56,15 @@
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: coverage>=7.4.4; extra == "test"
 Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.42&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.42/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.43&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.43/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.42/devopsdriver.egg-info/SOURCES.txt` & `devopsdriver-0.1.43/devopsdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/pyproject.toml` & `devopsdriver-0.1.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_azureobject.py` & `devopsdriver-0.1.43/tests/test_azure_azureobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_clients.py` & `devopsdriver-0.1.43/tests/test_azure_clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_pipeline.py` & `devopsdriver-0.1.43/tests/test_azure_pipeline.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_pipeline_client.py` & `devopsdriver-0.1.43/tests/test_azure_pipeline_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_pipeline_run.py` & `devopsdriver-0.1.43/tests/test_azure_pipeline_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def list_logs(self, project, pipeline_id, run_id, expand):
         """mock list_logs"""
         self.project = project
         self.pipeline_id = pipeline_id
         self.run_id = run_id
         self.expand = expand
-        return [MockLog("log 1"), MockLog("log 2")]
+        return SimpleNamespace(logs=[MockLog("log 1"), MockLog("log 2")])
 
 
 class MockPipeline:  # pylint: disable=too-few-public-methods
     """mock pipeline object"""
 
     def __init__(self, pipeline_id):
         self.id = pipeline_id
```

### Comparing `devopsdriver-0.1.42/tests/test_azure_timestamp.py` & `devopsdriver-0.1.43/tests/test_azure_timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_workitem_client.py` & `devopsdriver-0.1.43/tests/test_azure_workitem_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_azure_workitem_wiql.py` & `devopsdriver-0.1.43/tests/test_azure_workitem_wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_dataobject.py` & `devopsdriver-0.1.43/tests/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_manage_settings.py` & `devopsdriver-0.1.43/tests/test_manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_sendmail.py` & `devopsdriver-0.1.43/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_settings.py` & `devopsdriver-0.1.43/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.42/tests/test_template.py` & `devopsdriver-0.1.43/tests/test_template.py`

 * *Files identical despite different names*

