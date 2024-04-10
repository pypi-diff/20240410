# Comparing `tmp/devopsdriver-0.1.41.tar.gz` & `tmp/devopsdriver-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.41.tar", last modified: Mon Apr  8 22:44:00 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.42.tar", last modified: Wed Apr 10 06:50:06 2024, max compression
```

## Comparing `devopsdriver-0.1.41.tar` & `devopsdriver-0.1.42.tar`

### file list

```diff
@@ -1,40 +1,51 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.881957 devopsdriver-0.1.41/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.41/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-08 22:44:00.881720 devopsdriver-0.1.41/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-08 22:36:24.000000 devopsdriver-0.1.41/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.878256 devopsdriver-0.1.41/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-08 22:36:08.000000 devopsdriver-0.1.41/devopsdriver/__init__.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.879306 devopsdriver-0.1.41/devopsdriver/azdo/
--rw-r--r--   0 marcp      (501) staff       (20)      434 2024-04-08 22:35:57.000000 devopsdriver-0.1.41/devopsdriver/azdo/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     1882 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.41/devopsdriver/azdo/timestamp.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.879764 devopsdriver-0.1.41/devopsdriver/azdo/workitem/
--rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     2963 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/client.py
--rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     1658 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/devopsdriver/manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/devopsdriver/settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.41/devopsdriver/template.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.879874 devopsdriver-0.1.41/devopsdriver/templates/
--rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/devopsdriver/templates/manage_settings.txt.mako
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.881261 devopsdriver-0.1.41/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)      926 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/entry_points.txt
--rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-08 16:56:00.000000 devopsdriver-0.1.41/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-08 22:44:00.881995 devopsdriver-0.1.41/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.881074 devopsdriver-0.1.41/tests/
--rw-r--r--   0 marcp      (501) staff       (20)     5347 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/tests/test_azure_clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     9547 2024-04-07 15:39:41.000000 devopsdriver-0.1.41/tests/test_azure_timestamp.py
--rw-r--r--   0 marcp      (501) staff       (20)     4736 2024-04-06 17:54:48.000000 devopsdriver-0.1.41/tests/test_azure_workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.41/tests/test_azure_workitem_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.41/tests/test_azure_workitem_wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/tests/test_manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/tests/test_sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/tests/test_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.41/tests/test_template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.631888 devopsdriver-0.1.42/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.42/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 06:50:06.631680 devopsdriver-0.1.42/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-10 06:49:15.000000 devopsdriver-0.1.42/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.627342 devopsdriver-0.1.42/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-10 06:49:03.000000 devopsdriver-0.1.42/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.628554 devopsdriver-0.1.42/devopsdriver/azdo/
+-rw-r--r--   0 marcp      (501) staff       (20)      431 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)      843 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/azureobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2107 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/clients.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.629079 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/
+-rw-r--r--   0 marcp      (501) staff       (20)        0 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)      672 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)      667 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/log.py
+-rw-r--r--   0 marcp      (501) staff       (20)      918 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/pipeline.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1186 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/pipeline/run.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.42/devopsdriver/azdo/timestamp.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.629426 devopsdriver-0.1.42/devopsdriver/azdo/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.42/devopsdriver/azdo/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2966 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/azdo/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.42/devopsdriver/azdo/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1477 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/devopsdriver/dataobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/devopsdriver/manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.42/devopsdriver/sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/devopsdriver/settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.42/devopsdriver/template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.629575 devopsdriver-0.1.42/devopsdriver/templates/
+-rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/devopsdriver/templates/manage_settings.txt.mako
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.631255 devopsdriver-0.1.42/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     1256 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/entry_points.txt
+-rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-10 06:50:06.000000 devopsdriver-0.1.42/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-08 16:56:00.000000 devopsdriver-0.1.42/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-10 06:50:06.631925 devopsdriver-0.1.42/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 06:50:06.631090 devopsdriver-0.1.42/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     4787 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_azureobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     5497 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1097 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_pipeline.py
+-rw-r--r--   0 marcp      (501) staff       (20)      888 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_pipeline_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1685 2024-04-10 06:48:39.000000 devopsdriver-0.1.42/tests/test_azure_pipeline_run.py
+-rw-r--r--   0 marcp      (501) staff       (20)     9588 2024-04-10 05:10:33.000000 devopsdriver-0.1.42/tests/test_azure_timestamp.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.42/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.42/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)      830 2024-04-10 05:10:33.000000 devopsdriver-0.1.42/tests/test_dataobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/tests/test_manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.42/tests/test_sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.42/tests/test_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.42/tests/test_template.py
```

### Comparing `devopsdriver-0.1.41/LICENSE` & `devopsdriver-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/PKG-INFO` & `devopsdriver-0.1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.41
+Version: 0.1.42
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
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.41&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.41/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.42&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.42/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.41/README.md` & `devopsdriver-0.1.42/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.41&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.41/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.42&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.42/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.41/devopsdriver/azdo/clients.py` & `devopsdriver-0.1.42/devopsdriver/azdo/clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 from azure.devops.connection import Connection as AzureConnection
 from msrest.authentication import BasicAuthentication as MSBasicAuthentication
 
 from devopsdriver.settings import Settings
 from devopsdriver.azdo.workitem.client import Client as WIClient
+from devopsdriver.azdo.pipeline.client import Client as PLClient
 
 
 # for testing
 CONNECTION = AzureConnection
 AUTHENTICATION = MSBasicAuthentication
 
 
@@ -40,17 +41,19 @@
         ), "azure.token and azure.url not found in:\n" + "\n".join(
             settings.search_files
         )
         url = settings["azure.url"] if url is None else url
         token = settings["azure.token"] if token is None else token
         self.connection = CONNECTION(base_url=url, creds=AUTHENTICATION("", token))
         client_calls = {
-            "workitem": self.connection.clients_v7_1.get_work_item_tracking_client
+            "workitem": self.connection.clients_v7_1.get_work_item_tracking_client,
+            "pipeline": self.connection.clients_v7_1.get_pipelines_client,
         }
         self.workitem = WIClient(Azure.__client("workitem", clients, client_calls))
+        self.pipeline = PLClient(Azure.__client("pipeline", clients, client_calls))
 
     @staticmethod
     def __client(name: str, clients: dict, calls: dict) -> any:
         if clients and not clients.get(name, False):
             return None
 
         return calls[name]()
```

### Comparing `devopsdriver-0.1.41/devopsdriver/azdo/timestamp.py` & `devopsdriver-0.1.42/devopsdriver/azdo/timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/devopsdriver/azdo/workitem/client.py` & `devopsdriver-0.1.42/devopsdriver/azdo/workitem/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """ Azure WorkItem Client """
 
 
 from azure.devops.v7_1.work_item_tracking.models import Wiql as AzureWiql
 from azure.devops.v7_1.work_item_tracking.models import WorkItem as AzureWorkItem
 from azure.devops.v7_1.work_item_tracking.models import TeamContext
 from azure.devops.v7_1.work_item_tracking.models import WorkItemQueryResult
-from devopsdriver.azdo.workitem.workitem import WorkItem
+from devopsdriver.azdo.azureobject import AzureObject
 from devopsdriver.azdo.workitem.wiql import Wiql
 
 
 class Client:
     """Wraps work item client"""
 
     def __init__(self, client):
@@ -71,20 +71,20 @@
         # top-level items: as_of, columns, query_results_type, query_type, work_items
         # work_items fields: id, url
         # query_results_type: workItem
         # query_type: flat
         # columns: list of name, reference_name, url
         return [i.id for i in found.work_items]
 
-    def find(self, wiql: Wiql | str, top: int = None) -> list[list[WorkItem]]:
+    def find(self, wiql: Wiql | str, top: int = None) -> list[list[AzureObject]]:
         """Gets the full history of items found in a WIQL search
 
         Args:
             wiql (Wiql | str): The query
             top (int, optional): The number of work items to return. Defaults to None.
 
         Returns:
             list[list[WorkItem]]: List of work items, each is a history of work items
         """
         return [
-            [WorkItem(e) for e in self.history(i)] for i in self.find_ids(wiql, top)
+            [AzureObject(e) for e in self.history(i)] for i in self.find_ids(wiql, top)
         ]
```

### Comparing `devopsdriver-0.1.41/devopsdriver/azdo/workitem/wiql.py` & `devopsdriver-0.1.42/devopsdriver/azdo/workitem/wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/devopsdriver/manage_settings.py` & `devopsdriver-0.1.42/devopsdriver/manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/devopsdriver/sendmail.py` & `devopsdriver-0.1.42/devopsdriver/sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/devopsdriver/settings.py` & `devopsdriver-0.1.42/devopsdriver/settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/devopsdriver/template.py` & `devopsdriver-0.1.42/devopsdriver/template.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.42/devopsdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.41
+Version: 0.1.42
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
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.41&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.41/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.42&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.42/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.41/devopsdriver.egg-info/SOURCES.txt` & `devopsdriver-0.1.42/devopsdriver.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 LICENSE
 README.md
 pyproject.toml
 devopsdriver/__init__.py
+devopsdriver/dataobject.py
 devopsdriver/manage_settings.py
 devopsdriver/sendmail.py
 devopsdriver/settings.py
 devopsdriver/template.py
 devopsdriver.egg-info/PKG-INFO
 devopsdriver.egg-info/SOURCES.txt
 devopsdriver.egg-info/dependency_links.txt
 devopsdriver.egg-info/entry_points.txt
 devopsdriver.egg-info/requires.txt
 devopsdriver.egg-info/top_level.txt
 devopsdriver/azdo/__init__.py
+devopsdriver/azdo/azureobject.py
 devopsdriver/azdo/clients.py
 devopsdriver/azdo/timestamp.py
+devopsdriver/azdo/pipeline/__init__.py
+devopsdriver/azdo/pipeline/client.py
+devopsdriver/azdo/pipeline/log.py
+devopsdriver/azdo/pipeline/pipeline.py
+devopsdriver/azdo/pipeline/run.py
 devopsdriver/azdo/workitem/__init__.py
 devopsdriver/azdo/workitem/client.py
 devopsdriver/azdo/workitem/wiql.py
-devopsdriver/azdo/workitem/workitem.py
 devopsdriver/templates/manage_settings.txt.mako
+tests/test_azure_azureobject.py
 tests/test_azure_clients.py
+tests/test_azure_pipeline.py
+tests/test_azure_pipeline_client.py
+tests/test_azure_pipeline_run.py
 tests/test_azure_timestamp.py
-tests/test_azure_workitem.py
 tests/test_azure_workitem_client.py
 tests/test_azure_workitem_wiql.py
+tests/test_dataobject.py
 tests/test_manage_settings.py
 tests/test_sendmail.py
 tests/test_settings.py
 tests/test_template.py
```

### Comparing `devopsdriver-0.1.41/pyproject.toml` & `devopsdriver-0.1.42/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/tests/test_azure_clients.py` & `devopsdriver-0.1.42/tests/test_azure_clients.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         class Clients71:  # pylint: disable=too-few-public-methods
             """Fakes a 7.1 clients factory"""
 
             def get_work_item_tracking_client(self) -> str:
                 """fakes getting work item client"""
                 return "work_item_tracking_client"
 
+            def get_pipelines_client(self) -> str:
+                """mocks getting pipeline client"""
+                return "get_pipelines_client"
+
         self.clients_v7_1 = Clients71()
 
 
 def test_basic() -> None:
     """test the basic calling"""
     clients.CONNECTION = MockConnection
     clients.AUTHENTICATION = lambda a, b: SimpleNamespace(empty=a, token=b)
```

### Comparing `devopsdriver-0.1.41/tests/test_azure_timestamp.py` & `devopsdriver-0.1.42/tests/test_azure_timestamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,15 @@
 
 def test_math() -> None:
     """test addition and subtraction"""
     now1 = Timestamp.now()
     now2 = now1 + timedelta(days=7)
     assert (now2 - now1).days == 7
     assert now2 - timedelta(days=7) == now1
+    assert not Timestamp.is_timestamp(5)
 
     try:
         assert now1 - 5 is False
 
     except TypeError as error:
         assert "Timestamp" in str(error) and "int" in str(error), error
```

### Comparing `devopsdriver-0.1.41/tests/test_azure_workitem.py` & `devopsdriver-0.1.42/tests/test_azure_azureobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 """ Test work item """
 
-from devopsdriver.azdo import WorkItem
+from devopsdriver.azdo import AzureObject
 
 
-class MockAzureWorkItem:
+class MockAzureWorkItem:  # pylint: disable=too-few-public-methods
     """mock out work item"""
 
     def as_dict(self):
         """mock out as_dict"""
         return {
             "id": 5,
             "rev": 1,
@@ -72,26 +72,26 @@
                 "Microsoft.VSTS.Common.StateChangeDate": "2023-11-16T03:12:32.94Z",
             },
         }
 
 
 def test_workitem() -> None:
     """test basic work item"""
-    wi = WorkItem(MockAzureWorkItem())
+    wi = AzureObject(MockAzureWorkItem())
     assert wi.id == 5, wi.id
     assert wi.ID == 5, wi.ID
     assert wi.workitemtype == "User Story", wi.workitemtype
     assert wi.system_workitemtype == "User Story", wi.system_workitemtype
     assert wi.microsoft_vsts_common_priority == 2, wi.microsoft_vsts_common_priority
     assert wi.not_a_field is None, wi.not_a_field
 
 
 def test_timestamp() -> None:
     """test timestamps"""
-    wi = WorkItem(MockAzureWorkItem())
+    wi = AzureObject(MockAzureWorkItem())
     assert wi.StateChangeDate.to_string() == "2023-11-16T03:12:32.94Z"
     assert wi.CreatedDate.to_string() == "2023-11-16T03:12:32.94Z"
     assert wi.ChangedDate.to_string() == "2023-11-16T03:12:32.94Z"
     assert wi.IterationPath == "2023-11-16T03:12:32.alphaZ", wi.IterationPath
     assert wi.ChangedBy["displayName"] == "Edna Johnson .Z", wi.changedBy["displayName"]
     assert wi.createdBy.displayName == "Edna Johnson Z", wi.createdBy.displayName
     assert (
```

### Comparing `devopsdriver-0.1.41/tests/test_azure_workitem_client.py` & `devopsdriver-0.1.42/tests/test_azure_workitem_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/tests/test_azure_workitem_wiql.py` & `devopsdriver-0.1.42/tests/test_azure_workitem_wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/tests/test_manage_settings.py` & `devopsdriver-0.1.42/tests/test_manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/tests/test_sendmail.py` & `devopsdriver-0.1.42/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/tests/test_settings.py` & `devopsdriver-0.1.42/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.41/tests/test_template.py` & `devopsdriver-0.1.42/tests/test_template.py`

 * *Files identical despite different names*

