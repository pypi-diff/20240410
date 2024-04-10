# Comparing `tmp/pih-plb_db-0.14.tar.gz` & `tmp/pih-plb_db-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.14.tar", last modified: Sat Mar 30 03:32:55 2024, max compression
+gzip compressed data, was "pih-plb_db-0.15.tar", last modified: Wed Apr 10 02:14:51 2024, max compression
```

## Comparing `pih-plb_db-0.14.tar` & `pih-plb_db-0.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 03:32:55.562483 pih-plb_db-0.14/
--rw-rw-rw-   0        0        0      276 2024-03-30 03:32:55.546850 pih-plb_db-0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-30 03:32:55.183389 pih-plb_db-0.14/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.14/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.14/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0     6528 2024-03-30 01:06:51.000000 pih-plb_db-0.14/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0      560 2024-03-30 00:58:59.000000 pih-plb_db-0.14/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1130 2024-03-30 00:50:29.000000 pih-plb_db-0.14/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-03-30 03:32:55.515605 pih-plb_db-0.14/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      276 2024-03-30 03:32:54.000000 pih-plb_db-0.14/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-03-30 03:32:54.000000 pih-plb_db-0.14/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 03:32:54.000000 pih-plb_db-0.14/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-03-30 03:32:54.000000 pih-plb_db-0.14/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-30 03:32:54.000000 pih-plb_db-0.14/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-03-30 03:32:54.000000 pih-plb_db-0.14/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 03:32:55.593859 pih-plb_db-0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:14:51.499494 pih-plb_db-0.15/
+-rw-rw-rw-   0        0        0      276 2024-04-10 02:14:51.451561 pih-plb_db-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:14:51.076582 pih-plb_db-0.15/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.15/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.15/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0     6528 2024-03-30 01:06:51.000000 pih-plb_db-0.15/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0      564 2024-04-10 00:38:15.000000 pih-plb_db-0.15/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1146 2024-04-10 00:35:00.000000 pih-plb_db-0.15/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:14:51.404686 pih-plb_db-0.15/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-10 02:14:50.000000 pih-plb_db-0.15/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:14:51.499494 pih-plb_db-0.15/setup.cfg
```

### Comparing `pih-plb_db-0.14/PolibaseDatabaseService/api.py` & `pih-plb_db-0.15/PolibaseDatabaseService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb_db-0.14/PolibaseDatabaseService/const.py` & `pih-plb_db-0.15/PolibaseDatabaseService/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import ipih
 
 
-from pih.consts import UNKNOWN
+from pih.consts import CONST
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = Hosts.POLIBASE
 
-VERSION: str = "0.14"
+VERSION: str = "0.15"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database api",
     commands=("create_polibase_database_backup",),
     version=VERSION,
     use_standalone=True,
     standalone_name="plb_db",
     run_from_system_account=True,
-    python_executable_path=UNKNOWN,
+    python_executable_path=CONST.UNKNOWN,
 )
```

### Comparing `pih-plb_db-0.14/PolibaseDatabaseService/service.py` & `pih-plb_db-0.15/PolibaseDatabaseService/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import ipih
 
 from pih import A, PIHThread
 from PolibaseDatabaseService.const import SD
 
-# version 1.0
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 def start(as_standalone: bool = False) -> None:
 
+    from pih import PIHThread
     from pih.tools import ParameterList
     from PolibaseDatabaseService.api import PolibaseDBApi as Api
     
     from typing import Any
 
     def service_call_handler(sc: SC, pl: ParameterList) -> Any:
         if sc == SC.create_polibase_database_backup:
```

