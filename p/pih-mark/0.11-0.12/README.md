# Comparing `tmp/pih-mark-0.11.tar.gz` & `tmp/pih-mark-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mark-0.11.tar", last modified: Tue Mar 19 05:44:27 2024, max compression
+gzip compressed data, was "pih-mark-0.12.tar", last modified: Wed Apr 10 01:45:27 2024, max compression
```

## Comparing `pih-mark-0.11.tar` & `pih-mark-0.12.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 05:44:27.372776 pih-mark-0.11/
-drwxrwxrwx   0        0        0        0 2024-03-19 05:44:26.945842 pih-mark-0.11/MarkService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mark-0.11/MarkService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 23:54:48.000000 pih-mark-0.11/MarkService/__main__.py
--rw-rw-rw-   0        0        0    38542 2024-02-14 00:46:43.000000 pih-mark-0.11/MarkService/api.py
--rw-rw-rw-   0        0        0     1626 2024-02-09 14:42:12.000000 pih-mark-0.11/MarkService/api_test.py
--rw-rw-rw-   0        0        0     7014 2024-02-14 00:46:57.000000 pih-mark-0.11/MarkService/checkAndModify.py
--rw-rw-rw-   0        0        0     1815 2024-03-19 05:44:08.000000 pih-mark-0.11/MarkService/const.py
--rw-rw-rw-   0        0        0      839 2024-03-04 12:59:57.000000 pih-mark-0.11/MarkService/createEmptyPerson.py
--rw-rw-rw-   0        0        0     2309 2024-02-09 14:42:12.000000 pih-mark-0.11/MarkService/markChange.py
--rw-rw-rw-   0        0        0     6218 2024-03-19 05:42:55.000000 pih-mark-0.11/MarkService/service.py
--rw-rw-rw-   0        0        0      315 2024-03-19 05:44:27.279029 pih-mark-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 05:44:27.242721 pih-mark-0.11/pih_mark.egg-info/
--rw-rw-rw-   0        0        0      315 2024-03-19 05:44:26.000000 pih-mark-0.11/pih_mark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-03-19 05:44:26.000000 pih-mark-0.11/pih_mark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 05:44:26.000000 pih-mark-0.11/pih_mark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-19 05:44:26.000000 pih-mark-0.11/pih_mark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-03-19 05:44:26.000000 pih-mark-0.11/pih_mark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-19 05:44:26.000000 pih-mark-0.11/pih_mark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 05:44:27.372776 pih-mark-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:45:28.110693 pih-mark-0.12/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:45:27.731063 pih-mark-0.12/MarkService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mark-0.12/MarkService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 23:54:48.000000 pih-mark-0.12/MarkService/__main__.py
+-rw-rw-rw-   0        0        0    38542 2024-02-14 00:46:43.000000 pih-mark-0.12/MarkService/api.py
+-rw-rw-rw-   0        0        0     1626 2024-02-09 14:42:12.000000 pih-mark-0.12/MarkService/api_test.py
+-rw-rw-rw-   0        0        0     7014 2024-02-14 00:46:57.000000 pih-mark-0.12/MarkService/checkAndModify.py
+-rw-rw-rw-   0        0        0     1815 2024-04-10 00:28:14.000000 pih-mark-0.12/MarkService/const.py
+-rw-rw-rw-   0        0        0      839 2024-03-04 12:59:57.000000 pih-mark-0.12/MarkService/createEmptyPerson.py
+-rw-rw-rw-   0        0        0     2309 2024-02-09 14:42:12.000000 pih-mark-0.12/MarkService/markChange.py
+-rw-rw-rw-   0        0        0     6218 2024-03-19 05:42:55.000000 pih-mark-0.12/MarkService/service.py
+-rw-rw-rw-   0        0        0      315 2024-04-10 01:45:28.079432 pih-mark-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:45:28.048178 pih-mark-0.12/pih_mark.egg-info/
+-rw-rw-rw-   0        0        0      315 2024-04-10 01:45:27.000000 pih-mark-0.12/pih_mark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-04-10 01:45:27.000000 pih-mark-0.12/pih_mark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:45:27.000000 pih-mark-0.12/pih_mark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-10 01:45:27.000000 pih-mark-0.12/pih_mark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-10 01:45:27.000000 pih-mark-0.12/pih_mark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 01:45:27.000000 pih-mark-0.12/pih_mark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:45:28.126307 pih-mark-0.12/setup.cfg
```

### Comparing `pih-mark-0.11/MarkService/api.py` & `pih-mark-0.12/MarkService/api.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.11/MarkService/api_test.py` & `pih-mark-0.12/MarkService/api_test.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.11/MarkService/checkAndModify.py` & `pih-mark-0.12/MarkService/checkAndModify.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.11/MarkService/const.py` & `pih-mark-0.12/MarkService/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import ipih
 
-from pih.collections.service import ServiceDescription
 from pih.consts.hosts import Hosts
+from pih.collections.service import ServiceDescription
 
 NAME: str = "Mark"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.11"
+VERSION: str = "0.12"
 
 PACKAGES: tuple[str, ...] = ("pymssql", "schedule")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Orion service",
     host=HOST.NAME,
```

### Comparing `pih-mark-0.11/MarkService/createEmptyPerson.py` & `pih-mark-0.12/MarkService/createEmptyPerson.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.11/MarkService/markChange.py` & `pih-mark-0.12/MarkService/markChange.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.11/MarkService/service.py` & `pih-mark-0.12/MarkService/service.py`

 * *Files identical despite different names*

