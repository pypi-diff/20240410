# Comparing `tmp/socktalk-0.1.0.tar.gz` & `tmp/socktalk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.0.tar", last modified: Wed Apr 10 10:36:59 2024, max compression
+gzip compressed data, was "socktalk-0.1.1.tar", last modified: Wed Apr 10 10:53:06 2024, max compression
```

## Comparing `socktalk-0.1.0.tar` & `socktalk-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:36:59.243013 socktalk-0.1.0/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.0/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)      328 2024-04-10 10:36:59.243013 socktalk-0.1.0/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3288 2024-04-10 09:26:06.000000 socktalk-0.1.0/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:36:59.243013 socktalk-0.1.0/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.0/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5408 2024-04-09 11:09:29.000000 socktalk-0.1.0/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.0/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.0/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2527 2024-04-10 09:05:25.000000 socktalk-0.1.0/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-10 10:36:59.243013 socktalk-0.1.0/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)      672 2024-04-10 10:36:47.000000 socktalk-0.1.0/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:36:59.243013 socktalk-0.1.0/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)      328 2024-04-10 10:36:59.000000 socktalk-0.1.0/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-10 10:36:59.000000 socktalk-0.1.0/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-10 10:36:59.000000 socktalk-0.1.0/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-10 10:36:59.000000 socktalk-0.1.0/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-10 10:36:59.000000 socktalk-0.1.0/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-10 10:36:59.000000 socktalk-0.1.0/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:53:06.627013 socktalk-0.1.1/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.1/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     3721 2024-04-10 10:53:06.627013 socktalk-0.1.1/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3288 2024-04-10 09:26:06.000000 socktalk-0.1.1/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:53:06.627013 socktalk-0.1.1/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.1/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5408 2024-04-09 11:09:29.000000 socktalk-0.1.1/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.1/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.1/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2527 2024-04-10 09:05:25.000000 socktalk-0.1.1/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-10 10:53:06.627013 socktalk-0.1.1/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)      922 2024-04-10 10:52:38.000000 socktalk-0.1.1/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:53:06.627013 socktalk-0.1.1/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     3721 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.0/LICENSE` & `socktalk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.0/README.md` & `socktalk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.0/server_client/ai_client.py` & `socktalk-0.1.1/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.0/server_client/client.py` & `socktalk-0.1.1/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.0/server_client/server.py` & `socktalk-0.1.1/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.0/server_client/start_server_with_ai_client.py` & `socktalk-0.1.1/server_client/start_server_with_ai_client.py`

 * *Files identical despite different names*

