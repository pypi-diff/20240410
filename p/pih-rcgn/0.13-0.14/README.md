# Comparing `tmp/pih-rcgn-0.13.tar.gz` & `tmp/pih-rcgn-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rcgn-0.13.tar", last modified: Sat Mar 16 17:36:16 2024, max compression
+gzip compressed data, was "pih-rcgn-0.14.tar", last modified: Wed Apr 10 02:27:02 2024, max compression
```

## Comparing `pih-rcgn-0.13.tar` & `pih-rcgn-0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 17:36:16.161940 pih-rcgn-0.13/
--rw-rw-rw-   0        0        0      610 2024-03-16 17:36:16.130756 pih-rcgn-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-16 17:36:15.716722 pih-rcgn-0.13/RecognizeService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-rcgn-0.13/RecognizeService/__init__.py
--rw-rw-rw-   0        0        0      143 2024-02-15 01:35:08.000000 pih-rcgn-0.13/RecognizeService/__main__.py
--rw-rw-rw-   0        0        0    57730 2024-02-16 14:04:38.000000 pih-rcgn-0.13/RecognizeService/api.py
--rw-rw-rw-   0        0        0     1224 2024-02-09 14:42:12.000000 pih-rcgn-0.13/RecognizeService/collection.py
--rw-rw-rw-   0        0        0     4656 2024-03-15 03:48:41.000000 pih-rcgn-0.13/RecognizeService/const.py
--rw-rw-rw-   0        0        0    28795 2024-03-15 07:37:36.000000 pih-rcgn-0.13/RecognizeService/service.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:36:16.083845 pih-rcgn-0.13/pih_rcgn.egg-info/
--rw-rw-rw-   0        0        0      610 2024-03-16 17:36:15.000000 pih-rcgn-0.13/pih_rcgn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-03-16 17:36:15.000000 pih-rcgn-0.13/pih_rcgn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 17:36:15.000000 pih-rcgn-0.13/pih_rcgn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-16 17:36:15.000000 pih-rcgn-0.13/pih_rcgn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2024-03-16 17:36:15.000000 pih-rcgn-0.13/pih_rcgn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-16 17:36:15.000000 pih-rcgn-0.13/pih_rcgn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 17:36:16.177851 pih-rcgn-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:27:02.482201 pih-rcgn-0.14/
+-rw-rw-rw-   0        0        0      610 2024-04-10 02:27:02.450951 pih-rcgn-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:27:02.018833 pih-rcgn-0.14/RecognizeService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-rcgn-0.14/RecognizeService/__init__.py
+-rw-rw-rw-   0        0        0      143 2024-02-15 01:35:08.000000 pih-rcgn-0.14/RecognizeService/__main__.py
+-rw-rw-rw-   0        0        0    57769 2024-03-28 02:50:14.000000 pih-rcgn-0.14/RecognizeService/api.py
+-rw-rw-rw-   0        0        0     1224 2024-02-09 14:42:12.000000 pih-rcgn-0.14/RecognizeService/collection.py
+-rw-rw-rw-   0        0        0     4656 2024-04-10 02:26:25.000000 pih-rcgn-0.14/RecognizeService/const.py
+-rw-rw-rw-   0        0        0    29045 2024-03-19 22:16:00.000000 pih-rcgn-0.14/RecognizeService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:27:02.416676 pih-rcgn-0.14/pih_rcgn.egg-info/
+-rw-rw-rw-   0        0        0      610 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-10 02:27:01.000000 pih-rcgn-0.14/pih_rcgn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      137 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 02:27:00.000000 pih-rcgn-0.14/pih_rcgn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:27:02.482201 pih-rcgn-0.14/setup.cfg
```

### Comparing `pih-rcgn-0.13/PKG-INFO` & `pih-rcgn-0.14/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-rcgn
-Version: 0.13
+Version: 0.14
 Summary: PIH Recognize service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-rcgn-0.13/RecognizeService/api.py` & `pih-rcgn-0.14/RecognizeService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     PolibasePerson,
     BarcodeInformation,
     DocumentDescription,
     MedicalResearchType,
     ChillerIndicationsValue,
     PolibaseDocumentDescription,
 )
+from pih.consts import CHARSETS
 from RecognizeService.const import *
 from RecognizeService.collection import *
 from pih.tools import ne, e, js, j, one, escs
 
 
 class ImagePreprocessing:
     @staticmethod
@@ -611,15 +612,15 @@
         barcode_list = decode(image_array, symbols)
         result: list[tuple[str, str, Rect]] = []
         if ne(barcode_list):
             for barcode in barcode_list:
                 if ne(barcode.data):
                     result.append(
                         BarcodeInformation(
-                            barcode.data.decode("utf-8"),
+                            barcode.data.decode(CHARSETS.UTF8),
                             str(barcode.type).lower(),
                             barcode.rect,
                         )
                     )
         return result
 
     @staticmethod
```

### Comparing `pih-rcgn-0.13/RecognizeService/collection.py` & `pih-rcgn-0.14/RecognizeService/collection.py`

 * *Files identical despite different names*

### Comparing `pih-rcgn-0.13/RecognizeService/const.py` & `pih-rcgn-0.14/RecognizeService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "reportlab",
         "python-Levenshtein",
         "numpy",
         "opencv-python",
         "deskew"
     )
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Recognize service",
     host=HOST.NAME,
     host_changeable=False,
     commands=(
```

### Comparing `pih-rcgn-0.13/RecognizeService/service.py` & `pih-rcgn-0.14/RecognizeService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from pih import A
 from RecognizeService.const import *
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
+
 def start(as_standalone: bool = False) -> None:
-    if A.U.for_service(
-        SD
-    ):
+    if A.U.for_service(SD):
 
         from pih.collections import (
             PolibaseDocument,
             BarcodeInformation,
             ChillerIndicationsValue,
             MedicalDirectionDocument,
             PolibaseDocumentDescription,
@@ -60,18 +59,25 @@
                 document_type: A.CT_DT | None = A.D.get_by_value(
                     A.CT_DT, parameter_list.next()
                 )
                 try:
                     result: (
                         bool | PolibaseDocument | list[MedicalDirectionDocument] | None
                     ) = recognize_document(
-                        path, document_type, parameter_list.next(), parameter_list.next()
+                        path,
+                        document_type,
+                        parameter_list.next(),
+                        parameter_list.next(),
                     )
                     return A.R.pack(
-                        A.CT_FCA.VALUE_LIST if isinstance(result, list) else A.CT_FCA.VALUE,
+                        (
+                            A.CT_FCA.VALUE_LIST
+                            if isinstance(result, list)
+                            else A.CT_FCA.VALUE
+                        ),
                         result,
                     )
                 except Redirection as redirection:
                     return redirection.arg
 
             if sc == SC.document_type_exists:
                 return recognize_document(
@@ -103,15 +109,17 @@
                             break
                         except Exception as _:
                             time.sleep(2)
                     result: list[list[BarcodeInformation]] = []
                     if len(page_image_list) > 0:
                         for page_image in page_image_list:
                             barcode_information_list: list[BarcodeInformation] = (
-                                recognize_api.extruct_barcode_information_from_image(page_image)
+                                recognize_api.extruct_barcode_information_from_image(
+                                    page_image
+                                )
                             )
                             result.append(barcode_information_list)
                     return A.R.pack(A.CT_FCA.VALUE_LIST, result)
             return None
 
         def recognize_document(
             document_file_path: str,
```

### Comparing `pih-rcgn-0.13/pih_rcgn.egg-info/PKG-INFO` & `pih-rcgn-0.14/pih_rcgn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-rcgn
-Version: 0.13
+Version: 0.14
 Summary: PIH Recognize service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

