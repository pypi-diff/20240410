# Comparing `tmp/pih-zabbix-0.12.tar.gz` & `tmp/pih-zabbix-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-zabbix-0.12.tar", last modified: Wed Mar 27 01:51:40 2024, max compression
+gzip compressed data, was "pih-zabbix-0.13.tar", last modified: Wed Apr 10 02:33:41 2024, max compression
```

## Comparing `pih-zabbix-0.12.tar` & `pih-zabbix-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 01:51:40.782719 pih-zabbix-0.12/
--rw-rw-rw-   0        0        0      323 2024-03-27 01:51:40.735844 pih-zabbix-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-27 01:51:40.092050 pih-zabbix-0.12/ZabbixService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-zabbix-0.12/ZabbixService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-03-06 10:34:07.000000 pih-zabbix-0.12/ZabbixService/__main__.py
--rw-rw-rw-   0        0        0      653 2024-03-26 23:37:44.000000 pih-zabbix-0.12/ZabbixService/const.py
--rw-rw-rw-   0        0        0     3253 2024-03-27 01:18:35.000000 pih-zabbix-0.12/ZabbixService/service.py
-drwxrwxrwx   0        0        0        0 2024-03-27 01:51:40.657900 pih-zabbix-0.12/pih_zabbix.egg-info/
--rw-rw-rw-   0        0        0      323 2024-03-27 01:51:39.000000 pih-zabbix-0.12/pih_zabbix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-03-27 01:51:39.000000 pih-zabbix-0.12/pih_zabbix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 01:51:39.000000 pih-zabbix-0.12/pih_zabbix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-03-27 01:51:39.000000 pih-zabbix-0.12/pih_zabbix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2024-03-27 01:51:39.000000 pih-zabbix-0.12/pih_zabbix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-27 01:51:39.000000 pih-zabbix-0.12/pih_zabbix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 01:51:40.813969 pih-zabbix-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:33:41.559977 pih-zabbix-0.13/
+-rw-rw-rw-   0        0        0      323 2024-04-10 02:33:41.544354 pih-zabbix-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:33:41.277707 pih-zabbix-0.13/ZabbixService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-zabbix-0.13/ZabbixService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-03-06 10:34:07.000000 pih-zabbix-0.13/ZabbixService/__main__.py
+-rw-rw-rw-   0        0        0      653 2024-04-10 01:15:07.000000 pih-zabbix-0.13/ZabbixService/const.py
+-rw-rw-rw-   0        0        0     3225 2024-04-09 23:32:53.000000 pih-zabbix-0.13/ZabbixService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:33:41.513104 pih-zabbix-0.13/pih_zabbix.egg-info/
+-rw-rw-rw-   0        0        0      323 2024-04-10 02:33:40.000000 pih-zabbix-0.13/pih_zabbix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:33:40.000000 pih-zabbix-0.13/pih_zabbix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:33:41.575601 pih-zabbix-0.13/setup.cfg
```

### Comparing `pih-zabbix-0.12/ZabbixService/const.py` & `pih-zabbix-0.13/ZabbixService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Zabbix"
 
 HOST = A.CT_H.WS255
 
-VERSION: str = "0.12"
+VERSION: str = "0.13"
 
 PACKAGES: tuple[str, ...] = ("pyzabbix", "zabbix_utils")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Zabbix service",
     host=HOST.NAME,
```

### Comparing `pih-zabbix-0.12/ZabbixService/service.py` & `pih-zabbix-0.13/ZabbixService/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import ipih
 
 from pih import A
 from pih.tools import j
-from pih.consts import SPLITTER
 from ZabbixService.const import *
 from pih.consts.zabbix import ZABBIX
 
 from zabbix_utils import Sender
 
 
 def start(as_standalone: bool = False) -> None:
@@ -70,15 +69,15 @@
                     )
 
         def service_starts_handler() -> None:
             zabbix_server_url: str = j(
                 (
                     A.CT.UNTRUST_SITE_PROTOCOL,
                     ZABBIX_SERVER_HOST,
-                    SPLITTER,
+                    A.CT.SPLITTER,
                     ZABBIX_SERVER_WEB_INTERFACE_PORT,
                 )
             )
             zabbix = ZabbixAPI(zabbix_server_url)
             zabbix.login(ZABBIX_SERVER_LOGIN, ZABBIX_SERVER_PASSWORD)
             DH.zabbix = zabbix
```

