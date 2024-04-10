# Comparing `tmp/adpipsvcfuncs-0.1.tar.gz` & `tmp/adpipsvcfuncs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipsvcfuncs-0.1.tar", last modified: Wed Apr 10 16:03:10 2024, max compression
+gzip compressed data, was "adpipsvcfuncs-0.1.1.tar", last modified: Wed Apr 10 16:16:20 2024, max compression
```

## Comparing `adpipsvcfuncs-0.1.tar` & `adpipsvcfuncs-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:03:10.779101 adpipsvcfuncs-0.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-10 16:02:36.000000 adpipsvcfuncs-0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-10 16:03:10.775101 adpipsvcfuncs-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-10 16:02:36.000000 adpipsvcfuncs-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:03:10.775101 adpipsvcfuncs-0.1/adpipsvcfuncs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 16:02:36.000000 adpipsvcfuncs-0.1/adpipsvcfuncs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-04-10 16:02:36.000000 adpipsvcfuncs-0.1/adpipsvcfuncs/adpipsvcfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:03:10.775101 adpipsvcfuncs-0.1/adpipsvcfuncs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-10 16:03:10.000000 adpipsvcfuncs-0.1/adpipsvcfuncs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-10 16:03:10.000000 adpipsvcfuncs-0.1/adpipsvcfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 16:03:10.000000 adpipsvcfuncs-0.1/adpipsvcfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-10 16:03:10.000000 adpipsvcfuncs-0.1/adpipsvcfuncs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:03:10.779101 adpipsvcfuncs-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-10 16:02:36.000000 adpipsvcfuncs-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:16:19.998972 adpipsvcfuncs-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-10 16:15:24.000000 adpipsvcfuncs-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-10 16:16:19.998972 adpipsvcfuncs-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-10 16:15:24.000000 adpipsvcfuncs-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:16:19.998972 adpipsvcfuncs-0.1.1/adpipsvcfuncs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 16:15:24.000000 adpipsvcfuncs-0.1.1/adpipsvcfuncs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      969 2024-04-10 16:15:24.000000 adpipsvcfuncs-0.1.1/adpipsvcfuncs/adpipsvcfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:16:19.998972 adpipsvcfuncs-0.1.1/adpipsvcfuncs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-10 16:16:19.000000 adpipsvcfuncs-0.1.1/adpipsvcfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-10 16:16:19.000000 adpipsvcfuncs-0.1.1/adpipsvcfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 16:16:19.000000 adpipsvcfuncs-0.1.1/adpipsvcfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-10 16:16:19.000000 adpipsvcfuncs-0.1.1/adpipsvcfuncs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:16:20.002972 adpipsvcfuncs-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      424 2024-04-10 16:15:24.000000 adpipsvcfuncs-0.1.1/setup.py
```

### Comparing `adpipsvcfuncs-0.1/LICENSE` & `adpipsvcfuncs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adpipsvcfuncs-0.1/adpipsvcfuncs/adpipsvcfuncs.py` & `adpipsvcfuncs-0.1.1/adpipsvcfuncs/adpipsvcfuncs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from google.cloud import pubsub_v1
 import requests
 import logging
 
-logger = logging.get_logger(__name__)
+logger = logging.getLogger(__name__)
 
 def publish_to_pubsub(topic_name : str, data : dict) -> bool:
     """Publishes a message to a Google Cloud Pub/Sub topic."""
     # Fetch Project ID from Metadata Server
     metadata_server_url = "http://metadata/computeMetadata/v1/project/project-id"
     headers = {"Metadata-Flavor": "Google"}
     project_id = requests.get(metadata_server_url, headers=headers).text
```

