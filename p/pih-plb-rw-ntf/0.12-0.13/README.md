# Comparing `tmp/pih-plb_rw_ntf-0.12.tar.gz` & `tmp/pih-plb_rw_ntf-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_rw_ntf-0.12.tar", last modified: Wed Mar 13 12:27:29 2024, max compression
+gzip compressed data, was "pih-plb_rw_ntf-0.13.tar", last modified: Wed Apr 10 02:24:23 2024, max compression
```

## Comparing `pih-plb_rw_ntf-0.12.tar` & `pih-plb_rw_ntf-0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 12:27:30.076216 pih-plb_rw_ntf-0.12/
--rw-rw-rw-   0        0        0      302 2024-03-13 12:27:30.044969 pih-plb_rw_ntf-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-13 12:27:29.685615 pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/__init__.py
--rw-rw-rw-   0        0        0      174 2024-02-15 00:20:05.000000 pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/__main__.py
--rw-rw-rw-   0        0        0     2525 2024-02-09 14:42:12.000000 pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/api.py
--rw-rw-rw-   0        0        0      575 2024-03-13 12:27:19.000000 pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/const.py
--rw-rw-rw-   0        0        0     8479 2024-03-13 12:27:12.000000 pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/service.py
-drwxrwxrwx   0        0        0        0 2024-03-13 12:27:29.998094 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/
--rw-rw-rw-   0        0        0      302 2024-03-13 12:27:29.000000 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2024-03-13 12:27:29.000000 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 12:27:29.000000 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-03-13 12:27:29.000000 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-13 12:27:29.000000 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2024-03-13 12:27:29.000000 pih-plb_rw_ntf-0.12/pih_plb_rw_ntf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 12:27:30.076216 pih-plb_rw_ntf-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:24:23.785639 pih-plb_rw_ntf-0.13/
+-rw-rw-rw-   0        0        0      302 2024-04-10 02:24:23.753311 pih-plb_rw_ntf-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:24:23.358940 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-02-15 00:20:05.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/__main__.py
+-rw-rw-rw-   0        0        0     2508 2024-03-13 12:29:09.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/api.py
+-rw-rw-rw-   0        0        0      579 2024-04-10 02:23:34.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/const.py
+-rw-rw-rw-   0        0        0     8481 2024-04-10 00:36:48.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:24:23.722058 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/
+-rw-rw-rw-   0        0        0      302 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2024-04-10 02:24:23.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:24:23.801262 pih-plb_rw_ntf-0.13/setup.cfg
```

### Comparing `pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/api.py` & `pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import ipih
 
 from pih import A
 from pih.collections import Result
 
-# version 0.2
-
 from pih.collections import PolibasePerson
 from PolibasePersonNotificationService.api import PolibasePersonNotificationApi as Api
 
 
 class PolibasePersonReviewNotificationApi:
     @staticmethod
     def start_review_notification_distribution_action(test: bool = False) -> bool:
```

### Comparing `pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/const.py` & `pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import ipih
 
-from pih.consts import UNKNOWN
+from pih.consts import CONST
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibasePersonReviewNotification"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.12"
+VERSION: str = "0.13"
 
 SD: ServiceDescription = ServiceDescription(
        name=NAME,
        description="Polibase Person Review Notification service",
        host=HOST.NAME,
        use_standalone=True,
        version=VERSION,
        standalone_name="plb_rw_ntf",
        run_from_system_account=True,
-       python_executable_path=UNKNOWN,
+       python_executable_path=CONST.UNKNOWN,
 )
```

### Comparing `pih-plb_rw_ntf-0.12/PolibasePersonReviewNotificationService/service.py` & `pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import ipih
 
 from pih import A, PIHThread
-from pih.tools import j, nn, ne, one, FullNameTool, ParameterList
 from pih.collections import EventDS
 from PolibasePersonReviewNotificationService.api import (
     PolibasePersonReviewNotificationApi as Api,
 )
 from PolibasePersonReviewNotificationService.const import SD
+from pih.tools import j, nn, ne, one, FullNameTool, ParameterList
+
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 def start(as_standalone: bool = False) -> None:
     from datetime import datetime
```

