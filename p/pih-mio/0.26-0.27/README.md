# Comparing `tmp/pih-mio-0.26.tar.gz` & `tmp/pih-mio-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.26.tar", last modified: Wed Apr 10 01:48:51 2024, max compression
+gzip compressed data, was "pih-mio-0.27.tar", last modified: Wed Apr 10 05:20:35 2024, max compression
```

## Comparing `pih-mio-0.26.tar` & `pih-mio-0.27.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:51.476647 pih-mio-0.26/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:49.845473 pih-mio-0.26/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.26/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.26/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   361212 2024-04-09 23:32:25.000000 pih-mio-0.26/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5980 2024-03-12 09:02:04.000000 pih-mio-0.26/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.26/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4461 2024-04-10 00:33:44.000000 pih-mio-0.26/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.26/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    16596 2024-03-21 06:21:36.000000 pih-mio-0.26/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      329 2024-04-10 01:48:51.460008 pih-mio-0.26/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:51.428757 pih-mio-0.26/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:48:51.476647 pih-mio-0.26/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 05:20:35.356546 pih-mio-0.27/
+drwxrwxrwx   0        0        0        0 2024-04-10 05:20:34.885729 pih-mio-0.27/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.27/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.27/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   361191 2024-04-10 05:19:48.000000 pih-mio-0.27/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5980 2024-03-12 09:02:04.000000 pih-mio-0.27/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.27/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4461 2024-04-10 05:19:44.000000 pih-mio-0.27/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.27/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    16542 2024-04-10 05:18:33.000000 pih-mio-0.27/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      329 2024-04-10 05:20:35.339889 pih-mio-0.27/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 05:20:35.308642 pih-mio-0.27/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-10 05:20:33.000000 pih-mio-0.27/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-10 05:20:33.000000 pih-mio-0.27/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 05:20:33.000000 pih-mio-0.27/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-10 05:20:33.000000 pih-mio-0.27/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-10 05:20:33.000000 pih-mio-0.27/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 05:20:33.000000 pih-mio-0.27/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 05:20:35.388095 pih-mio-0.27/setup.cfg
```

### Comparing `pih-mio-0.26/MobileHelperService/api.py` & `pih-mio-0.27/MobileHelperService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,15 @@
     while_not_do,
 )
 from pih.consts import (
     CheckableSections,
     Actions,
     JournalType,
     Tags,
-    A.CT.SPLITTER,
-    EmailVerificationMethods,
+    EmailVerificationMethods
 )
 from MobileHelperService.collection import MobileHelperUserSettings
 from pih.consts.polibase import PolibaseDocumentTypes
 from pih.consts.ssh_hosts import SSHHosts
 from MobileHelperService.const import *
 
 from pih.consts.errors import BarcodeNotFound, NotFound, Error
```

### Comparing `pih-mio-0.26/MobileHelperService/client.py` & `pih-mio-0.27/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.26/MobileHelperService/const.py` & `pih-mio-0.27/MobileHelperService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.26"
+VERSION: str = "0.27"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
```

### Comparing `pih-mio-0.26/MobileHelperService/service.py` & `pih-mio-0.27/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.26/MobileHelperService/service_api.py` & `pih-mio-0.27/MobileHelperService/service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     lw,
     one,
     if_else,
     ParameterList,
     BitMask as BM,
 )
 from pih.collections import WhatsAppMessage, User, Message
-from MobileHelperService.client import Client as MIO
 from pih.collections.service import ServiceDescription, SubscribtionResult
 
 
 from collections import defaultdict
 from typing import Callable, Any
 
 SC = A.CT_SC
```

