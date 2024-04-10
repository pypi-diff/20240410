# Comparing `tmp/pih-med_auto-0.12.tar.gz` & `tmp/pih-med_auto-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-med_auto-0.12.tar", last modified: Sun Mar 17 12:25:22 2024, max compression
+gzip compressed data, was "pih-med_auto-0.13.tar", last modified: Wed Apr 10 01:46:38 2024, max compression
```

## Comparing `pih-med_auto-0.12.tar` & `pih-med_auto-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 12:25:23.018208 pih-med_auto-0.12/
-drwxrwxrwx   0        0        0        0 2024-03-17 12:25:22.565111 pih-med_auto-0.12/MedicalAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-med_auto-0.12/MedicalAutomationService/__init__.py
--rw-rw-rw-   0        0        0      161 2024-02-15 02:15:00.000000 pih-med_auto-0.12/MedicalAutomationService/__main__.py
--rw-rw-rw-   0        0        0      586 2024-03-17 12:25:07.000000 pih-med_auto-0.12/MedicalAutomationService/const.py
--rw-rw-rw-   0        0        0    20943 2024-03-16 18:18:31.000000 pih-med_auto-0.12/MedicalAutomationService/service.py
--rw-rw-rw-   0        0        0      307 2024-03-17 12:25:22.971333 pih-med_auto-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-17 12:25:22.940087 pih-med_auto-0.12/pih_med_auto.egg-info/
--rw-rw-rw-   0        0        0      307 2024-03-17 12:25:22.000000 pih-med_auto-0.12/pih_med_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-03-17 12:25:22.000000 pih-med_auto-0.12/pih_med_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 12:25:22.000000 pih-med_auto-0.12/pih_med_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-03-17 12:25:22.000000 pih-med_auto-0.12/pih_med_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-03-17 12:25:22.000000 pih-med_auto-0.12/pih_med_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-03-17 12:25:22.000000 pih-med_auto-0.12/pih_med_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-17 12:25:23.033872 pih-med_auto-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:46:38.825724 pih-med_auto-0.13/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:46:37.436566 pih-med_auto-0.13/MedicalAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-med_auto-0.13/MedicalAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-02-15 02:15:00.000000 pih-med_auto-0.13/MedicalAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      586 2024-04-10 00:33:12.000000 pih-med_auto-0.13/MedicalAutomationService/const.py
+-rw-rw-rw-   0        0        0    20992 2024-04-10 00:31:50.000000 pih-med_auto-0.13/MedicalAutomationService/service.py
+-rw-rw-rw-   0        0        0      307 2024-04-10 01:46:38.763241 pih-med_auto-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:46:38.669443 pih-med_auto-0.13/pih_med_auto.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-10 01:46:36.000000 pih-med_auto-0.13/pih_med_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:46:38.825724 pih-med_auto-0.13/setup.cfg
```

### Comparing `pih-med_auto-0.12/MedicalAutomationService/const.py` & `pih-med_auto-0.13/MedicalAutomationService/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.collections.service import ServiceDescription
 
 NAME: str = "MedicalAutomation"
 
 HOST = A.CT_H.BACKUP_WORKER
 
-VERSION: str = "0.12"
+VERSION: str = "0.13"
 
 PACKAGES: tuple[str, ...] = (
     A.PTH_FCD_DIST.NAME(A.CT_SR.MOBILE_HELPER.standalone_name),  # type: ignore
 )
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-med_auto-0.12/MedicalAutomationService/service.py` & `pih-med_auto-0.13/MedicalAutomationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 import shutil
 import locale
 from time import sleep
 from typing import Any
 
 import ipih
 
-from pih import A, subscribe_on, serve
-from pih.consts.errors import NotFound
-from pih.collections import PolibaseDocument
-from MobileHelperService.client import Client as MIO
-from MobileHelperService.const import COMMAND_KEYWORDS
-from pih.tools import j, js, one, while_not_do, nn, n, ln
-from MobileHelperService.api import MobileOutput, mio_command
-from pih.consts.errors import OperationExit, OperationCanceled
+from pih import A
+
 from MedicalAutomationService.const import SD, VALENTA_SOURCE_HOST
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
-target_GROUP: A.CT_ME_WH.GROUP = A.CT_ME_WH.GROUP.SCANNED_DOCUMENT_HELPER_CLI
-target: MobileOutput = MIO.create_output(target_GROUP)
-
-
 def start(as_standalone: bool = False) -> None:
     if A.U.for_service(SD, as_standalone=as_standalone):
 
+        from pih import subscribe_on, serve
         from pih.tools import ParameterList
+        from pih.consts.errors import NotFound
+        from pih.collections import PolibaseDocument
         from pih.collections import User, ActionWasDone
+        from MobileHelperService.client import Client as MIO
         from pih.collections.service import SubscribtionResult
+        from MobileHelperService.const import COMMAND_KEYWORDS
+        from pih.tools import j, js, one, while_not_do, nn, n, ln
+        from MobileHelperService.api import MobileOutput, mio_command
+        from pih.consts.errors import OperationExit, OperationCanceled
+        
+        target_GROUP: A.CT_ME_WH.GROUP = A.CT_ME_WH.GROUP.SCANNED_DOCUMENT_HELPER_CLI
+        target: MobileOutput = MIO.create_output(target_GROUP)
 
         def new_polibase_scanned_document_processed(path: str) -> None:
             A.E.new_polibase_scanned_document_processed(path)
             A.PTH.confirm_file(path)
 
         def service_call_handler(
             sc: SC,
@@ -146,19 +147,19 @@
                         file_path: str = A.PTH.path(event_parameters[0])
                         if A.PTH.get_extension(file_path) in (
                             A.CT_F_E.JPEG,
                             A.CT_F_E.JPG,
                         ):
                             if not valenta_source_host_is_available():
                                 A.L.it_bot(
-                                    j(
+                                    js(
                                         (
-                                            "Компьютер ",
+                                            "Компьютер",
                                             VALENTA_SOURCE_HOST,
-                                            " недоступен или выключен. Синхронизация продолжиться автоматически после того, как компьютер станет доступным",
+                                            "недоступен или выключен. Синхронизация продолжиться автоматически после того, как компьютер станет доступным",
                                         )
                                     )
                                 )
                                 while True:
                                     if A.C_R.accessibility_by_smb_port(
                                         VALENTA_SOURCE_HOST
                                     ):
@@ -344,15 +345,14 @@
                     if A.E.on_robocopy_job_complete(robocopy_job_name):
                         break
                     else:
                         time.sleep(2)
                         close_valenta_clients()
 
         def service_starts_handler() -> None:
-            locale.setlocale(locale.LC_ALL, "ru_RU")
             subscribe_on(SC.heart_beat)
             subscribe_on(SC.send_event)
 
         def service_started_handler() -> None:
             A.A_PTH.listen(A.PTH.MEDICAL_DATA.VALUE)
 
         serve(
```

