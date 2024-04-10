# Comparing `tmp/pih-plb-0.11.tar.gz` & `tmp/pih-plb-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.11.tar", last modified: Tue Feb 27 00:57:24 2024, max compression
+gzip compressed data, was "pih-plb-0.12.tar", last modified: Wed Apr 10 02:11:07 2024, max compression
```

## Comparing `pih-plb-0.11.tar` & `pih-plb-0.12.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 00:57:24.403935 pih-plb-0.11/
--rw-rw-rw-   0        0        0      247 2024-02-27 00:57:24.814809 pih-plb-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-27 00:57:24.419560 pih-plb-0.11/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.11/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.11/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45675 2024-02-27 00:56:04.000000 pih-plb-0.11/PolibaseService/api.py
--rw-rw-rw-   0        0        0     1631 2024-02-14 06:59:50.000000 pih-plb-0.11/PolibaseService/api_test.py
--rw-rw-rw-   0        0        0     2962 2024-02-09 14:42:12.000000 pih-plb-0.11/PolibaseService/collection.py
--rw-rw-rw-   0        0        0     3548 2024-02-27 00:43:21.000000 pih-plb-0.11/PolibaseService/const.py
--rw-rw-rw-   0        0        0     1180 2024-02-10 10:21:21.000000 pih-plb-0.11/PolibaseService/create_all_barcodes.py
--rw-rw-rw-   0        0        0    14584 2024-02-27 00:46:55.000000 pih-plb-0.11/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-02-27 00:57:24.654892 pih-plb-0.11/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      247 2024-02-27 00:57:23.000000 pih-plb-0.11/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-02-27 00:57:23.000000 pih-plb-0.11/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 00:57:23.000000 pih-plb-0.11/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-02-27 00:57:23.000000 pih-plb-0.11/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-02-27 00:57:23.000000 pih-plb-0.11/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-02-27 00:57:23.000000 pih-plb-0.11/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-02-14 06:58:23.000000 pih-plb-0.11/plb_build.py
--rw-rw-rw-   0        0        0       42 2024-02-27 00:57:24.830447 pih-plb-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:11:07.241485 pih-plb-0.12/
+-rw-rw-rw-   0        0        0      293 2024-04-10 02:11:07.225860 pih-plb-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:11:06.848841 pih-plb-0.12/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.12/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.12/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45675 2024-02-27 00:56:04.000000 pih-plb-0.12/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     1631 2024-02-14 06:59:50.000000 pih-plb-0.12/PolibaseService/api_test.py
+-rw-rw-rw-   0        0        0     3553 2024-04-10 02:05:31.000000 pih-plb-0.12/PolibaseService/const.py
+-rw-rw-rw-   0        0        0     1180 2024-02-10 10:21:21.000000 pih-plb-0.12/PolibaseService/create_all_barcodes.py
+-rw-rw-rw-   0        0        0    14584 2024-02-27 00:46:55.000000 pih-plb-0.12/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:11:07.194609 pih-plb-0.12/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-04-10 02:11:06.000000 pih-plb-0.12/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-10 02:11:06.000000 pih-plb-0.12/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:11:06.000000 pih-plb-0.12/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-10 02:11:06.000000 pih-plb-0.12/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 02:11:06.000000 pih-plb-0.12/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-10 02:11:06.000000 pih-plb-0.12/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:11:07.257108 pih-plb-0.12/setup.cfg
```

### Comparing `pih-plb-0.11/PolibaseService/api.py` & `pih-plb-0.12/PolibaseService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb-0.11/PolibaseService/api_test.py` & `pih-plb-0.12/PolibaseService/api_test.py`

 * *Files identical despite different names*

### Comparing `pih-plb-0.11/PolibaseService/const.py` & `pih-plb-0.12/PolibaseService/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import ipih
 
-from pih import A, UNKNOWN
+from pih import A
 from pih.tools import j
+from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
-
 NAME: str = "Polibase"
 
-#handle DB error
-
-VERSION: str = "0.11"
+VERSION: str = "0.12"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
@@ -39,15 +37,15 @@
         "set_barcode_for_polibase_person",
         "check_polibase_person_card_registry_folder_name",
         "set_polibase_person_telephone_number",
         "get_polibase_person_operator_by_pin",
         "get_polibase_person_by_email",
         "update_person_change_date",
     ),
-    python_executable_path=UNKNOWN,
+    python_executable_path=CONST.UNKNOWN,
     standalone_name="plb",
     use_standalone=True,
     packages=PACKAGES,
     version=VERSION
 )
 
 TEST: bool = False
```

### Comparing `pih-plb-0.11/PolibaseService/create_all_barcodes.py` & `pih-plb-0.12/PolibaseService/create_all_barcodes.py`

 * *Files identical despite different names*

### Comparing `pih-plb-0.11/PolibaseService/service.py` & `pih-plb-0.12/PolibaseService/service.py`

 * *Files identical despite different names*

