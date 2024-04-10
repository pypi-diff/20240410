# Comparing `tmp/pih-printer-0.1.tar.gz` & `tmp/pih-printer-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-printer-0.1.tar", last modified: Mon Feb 26 10:16:00 2024, max compression
+gzip compressed data, was "pih-printer-0.11.tar", last modified: Wed Apr 10 02:25:07 2024, max compression
```

## Comparing `pih-printer-0.1.tar` & `pih-printer-0.11.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 10:15:59.739668 pih-printer-0.1/
--rw-rw-rw-   0        0        0      249 2024-02-26 10:16:00.842540 pih-printer-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-26 10:15:59.974032 pih-printer-0.1/PrinterService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-printer-0.1/PrinterService/__init__.py
--rw-rw-rw-   0        0        0      149 2024-02-15 01:28:26.000000 pih-printer-0.1/PrinterService/__main__.py
--rw-rw-rw-   0        0        0    18204 2024-02-26 08:55:15.000000 pih-printer-0.1/PrinterService/api.py
--rw-rw-rw-   0        0        0      689 2024-02-26 08:55:14.000000 pih-printer-0.1/PrinterService/const.py
--rw-rw-rw-   0        0        0     4244 2024-02-19 03:01:06.000000 pih-printer-0.1/PrinterService/service.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:16:00.592544 pih-printer-0.1/pih_printer.egg-info/
--rw-rw-rw-   0        0        0      249 2024-02-26 10:15:58.000000 pih-printer-0.1/pih_printer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-02-26 10:15:59.000000 pih-printer-0.1/pih_printer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 10:15:58.000000 pih-printer-0.1/pih_printer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-02-26 10:15:58.000000 pih-printer-0.1/pih_printer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2024-02-26 10:15:58.000000 pih-printer-0.1/pih_printer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-26 10:15:58.000000 pih-printer-0.1/pih_printer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       94 2024-02-15 00:01:29.000000 pih-printer-0.1/printer_build.py
--rw-rw-rw-   0        0        0       42 2024-02-26 10:16:00.842540 pih-printer-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:25:07.806889 pih-printer-0.11/
+-rw-rw-rw-   0        0        0      391 2024-04-10 02:25:07.743359 pih-printer-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:25:07.368369 pih-printer-0.11/PrinterService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-printer-0.11/PrinterService/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-02-15 01:28:26.000000 pih-printer-0.11/PrinterService/__main__.py
+-rw-rw-rw-   0        0        0    20675 2024-04-10 00:41:30.000000 pih-printer-0.11/PrinterService/api.py
+-rw-rw-rw-   0        0        0      692 2024-04-10 01:18:17.000000 pih-printer-0.11/PrinterService/const.py
+-rw-rw-rw-   0        0        0     4243 2024-03-15 07:49:59.000000 pih-printer-0.11/PrinterService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:25:07.696486 pih-printer-0.11/pih_printer.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-04-10 02:25:06.000000 pih-printer-0.11/pih_printer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-04-10 02:25:07.000000 pih-printer-0.11/pih_printer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:25:06.000000 pih-printer-0.11/pih_printer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-10 02:25:06.000000 pih-printer-0.11/pih_printer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       61 2024-04-10 02:25:06.000000 pih-printer-0.11/pih_printer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 02:25:06.000000 pih-printer-0.11/pih_printer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:25:07.806889 pih-printer-0.11/setup.cfg
```

### Comparing `pih-printer-0.1/PrinterService/const.py` & `pih-printer-0.11/PrinterService/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from enum import Enum
 
 NAME: str = "Printer"
 
 HOST = Hosts.WS255
 
-VERSION: str = "0.1"
+VERSION: str = "0.11"
 
 PACKAGES: tuple[str, ...] = (
     "pyasn1==0.4.8",
     "pycryptodomex==3.15.0",
     "pysmi==0.3.4",
     "pysnmp",
 )
@@ -28,8 +28,8 @@
     packages=PACKAGES,
     version=VERSION,
 )
 
 
 class PrinterCommands(Enum):
     REPORT = "report"
-    STATUS = "status"
+    STATUS = "status"
```

### Comparing `pih-printer-0.1/PrinterService/service.py` & `pih-printer-0.11/PrinterService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ipih
 
 from pih import A
 
 SC = A.CT_SC
 
-ISOLATED: bool = False
+ISOLATED: bool = True
 
 
 def start(as_standalone: bool = False) -> None:
 
     from PrinterService.const import SD
 
     if A.U.for_service(SD, as_standalone=as_standalone):
```

