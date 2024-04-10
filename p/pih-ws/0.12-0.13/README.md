# Comparing `tmp/pih-ws-0.12.tar.gz` & `tmp/pih-ws-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ws-0.12.tar", last modified: Wed Mar 13 14:48:07 2024, max compression
+gzip compressed data, was "pih-ws-0.13.tar", last modified: Wed Apr 10 02:32:43 2024, max compression
```

## Comparing `pih-ws-0.12.tar` & `pih-ws-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 14:48:07.600741 pih-ws-0.12/
--rw-rw-rw-   0        0        0      270 2024-03-13 14:48:07.553868 pih-ws-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-13 14:48:07.194568 pih-ws-0.12/WSService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-ws-0.12/WSService/__init__.py
--rw-rw-rw-   0        0        0      142 2024-02-16 00:56:17.000000 pih-ws-0.12/WSService/__main__.py
--rw-rw-rw-   0        0        0      522 2024-03-13 14:47:57.000000 pih-ws-0.12/WSService/const.py
--rw-rw-rw-   0        0        0     3262 2024-03-13 14:47:38.000000 pih-ws-0.12/WSService/service.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:48:07.506997 pih-ws-0.12/pih_ws.egg-info/
--rw-rw-rw-   0        0        0      270 2024-03-13 14:48:06.000000 pih-ws-0.12/pih_ws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-03-13 14:48:06.000000 pih-ws-0.12/pih_ws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 14:48:06.000000 pih-ws-0.12/pih_ws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-03-13 14:48:06.000000 pih-ws-0.12/pih_ws.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-13 14:48:06.000000 pih-ws-0.12/pih_ws.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-13 14:48:06.000000 pih-ws-0.12/pih_ws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 14:48:07.600741 pih-ws-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:32:43.795804 pih-ws-0.13/
+-rw-rw-rw-   0        0        0      270 2024-04-10 02:32:43.695996 pih-ws-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:32:43.288689 pih-ws-0.13/WSService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-ws-0.13/WSService/__init__.py
+-rw-rw-rw-   0        0        0      142 2024-02-16 00:56:17.000000 pih-ws-0.13/WSService/__main__.py
+-rw-rw-rw-   0        0        0      522 2024-04-10 01:16:06.000000 pih-ws-0.13/WSService/const.py
+-rw-rw-rw-   0        0        0     3262 2024-03-13 14:47:38.000000 pih-ws-0.13/WSService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:32:43.633515 pih-ws-0.13/pih_ws.egg-info/
+-rw-rw-rw-   0        0        0      270 2024-04-10 02:32:42.000000 pih-ws-0.13/pih_ws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-10 02:32:43.000000 pih-ws-0.13/pih_ws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:32:42.000000 pih-ws-0.13/pih_ws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-10 02:32:42.000000 pih-ws-0.13/pih_ws.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 02:32:42.000000 pih-ws-0.13/pih_ws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 02:32:42.000000 pih-ws-0.13/pih_ws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:32:43.795804 pih-ws-0.13/setup.cfg
```

### Comparing `pih-ws-0.12/WSService/const.py` & `pih-ws-0.13/WSService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "WS"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.12"
+VERSION: str = "0.13"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Workstation service",
     host=HOST.NAME,
     commands=(
         "reboot",
```

### Comparing `pih-ws-0.12/WSService/service.py` & `pih-ws-0.13/WSService/service.py`

 * *Files identical despite different names*

