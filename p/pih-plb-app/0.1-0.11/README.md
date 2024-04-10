# Comparing `tmp/pih-plb_app-0.1.tar.gz` & `tmp/pih-plb_app-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_app-0.1.tar", last modified: Mon Feb 26 09:03:57 2024, max compression
+gzip compressed data, was "pih-plb_app-0.11.tar", last modified: Wed Apr 10 02:14:00 2024, max compression
```

## Comparing `pih-plb_app-0.1.tar` & `pih-plb_app-0.11.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 09:03:57.569494 pih-plb_app-0.1/
--rw-rw-rw-   0        0        0      262 2024-02-26 09:03:58.069487 pih-plb_app-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-26 09:03:57.569494 pih-plb_app-0.1/PolibaseAppService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb_app-0.1/PolibaseAppService/__init__.py
--rw-rw-rw-   0        0        0      153 2024-02-14 23:43:23.000000 pih-plb_app-0.1/PolibaseAppService/__main__.py
--rw-rw-rw-   0        0        0      506 2024-02-26 08:55:15.000000 pih-plb_app-0.1/PolibaseAppService/const.py
--rw-rw-rw-   0        0        0    13610 2024-02-24 09:18:10.000000 pih-plb_app-0.1/PolibaseAppService/service.py
-drwxrwxrwx   0        0        0        0 2024-02-26 09:03:58.038229 pih-plb_app-0.1/pih_plb_app.egg-info/
--rw-rw-rw-   0        0        0      262 2024-02-26 09:03:56.000000 pih-plb_app-0.1/pih_plb_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-02-26 09:03:57.000000 pih-plb_app-0.1/pih_plb_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 09:03:56.000000 pih-plb_app-0.1/pih_plb_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-02-26 09:03:56.000000 pih-plb_app-0.1/pih_plb_app.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-02-26 09:03:56.000000 pih-plb_app-0.1/pih_plb_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-02-26 09:03:56.000000 pih-plb_app-0.1/pih_plb_app.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       98 2024-02-14 23:35:08.000000 pih-plb_app-0.1/plb_app_build.py
--rw-rw-rw-   0        0        0       42 2024-02-26 09:03:58.085102 pih-plb_app-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:14:00.382295 pih-plb_app-0.11/
+-rw-rw-rw-   0        0        0      284 2024-04-10 02:14:00.335426 pih-plb_app-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:13:59.943759 pih-plb_app-0.11/PolibaseAppService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb_app-0.11/PolibaseAppService/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-02-14 23:43:23.000000 pih-plb_app-0.11/PolibaseAppService/__main__.py
+-rw-rw-rw-   0        0        0      511 2024-04-10 00:34:34.000000 pih-plb_app-0.11/PolibaseAppService/const.py
+-rw-rw-rw-   0        0        0    13590 2024-04-10 00:34:39.000000 pih-plb_app-0.11/PolibaseAppService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:14:00.304200 pih-plb_app-0.11/pih_plb_app.egg-info/
+-rw-rw-rw-   0        0        0      284 2024-04-10 02:13:59.000000 pih-plb_app-0.11/pih_plb_app.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-10 02:13:59.000000 pih-plb_app-0.11/pih_plb_app.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:13:59.000000 pih-plb_app-0.11/pih_plb_app.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-10 02:13:59.000000 pih-plb_app-0.11/pih_plb_app.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 02:13:59.000000 pih-plb_app-0.11/pih_plb_app.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 02:13:59.000000 pih-plb_app-0.11/pih_plb_app.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:14:00.382295 pih-plb_app-0.11/setup.cfg
```

### Comparing `pih-plb_app-0.1/PolibaseAppService/service.py` & `pih-plb_app-0.11/PolibaseAppService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import ipih
 
 from pih import A, PIHThread, PIHThreadPoolExecutor
 
-
-# version 0.97
-
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
```

