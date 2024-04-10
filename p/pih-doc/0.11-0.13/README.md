# Comparing `tmp/pih-doc-0.11.tar.gz` & `tmp/pih-doc-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-doc-0.11.tar", last modified: Mon Mar 11 13:56:37 2024, max compression
+gzip compressed data, was "pih-doc-0.13.tar", last modified: Wed Apr 10 01:38:39 2024, max compression
```

## Comparing `pih-doc-0.11.tar` & `pih-doc-0.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 13:56:37.328822 pih-doc-0.11/
-drwxrwxrwx   0        0        0        0 2024-03-11 13:56:36.875726 pih-doc-0.11/DocsService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.11/DocsService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.11/DocsService/__main__.py
--rw-rw-rw-   0        0        0    41330 2024-02-09 18:14:29.000000 pih-doc-0.11/DocsService/api.py
--rw-rw-rw-   0        0        0      536 2024-01-15 10:05:42.000000 pih-doc-0.11/DocsService/api_test.py
--rw-rw-rw-   0        0        0     1634 2024-03-11 13:47:02.000000 pih-doc-0.11/DocsService/const.py
--rw-rw-rw-   0        0        0     5275 2024-03-11 13:46:49.000000 pih-doc-0.11/DocsService/service.py
--rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.11/DocsService/tools.py
--rw-rw-rw-   0        0        0      595 2024-03-11 13:56:37.281951 pih-doc-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-11 13:56:37.235077 pih-doc-0.11/pih_doc.egg-info/
--rw-rw-rw-   0        0        0      595 2024-03-11 13:56:36.000000 pih-doc-0.11/pih_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-03-11 13:56:36.000000 pih-doc-0.11/pih_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 13:56:36.000000 pih-doc-0.11/pih_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-11 13:56:36.000000 pih-doc-0.11/pih_doc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2024-03-11 13:56:36.000000 pih-doc-0.11/pih_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-11 13:56:36.000000 pih-doc-0.11/pih_doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-11 13:56:37.344449 pih-doc-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:38:40.027397 pih-doc-0.13/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:38:39.640781 pih-doc-0.13/DocsService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.13/DocsService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.13/DocsService/__main__.py
+-rw-rw-rw-   0        0        0    41330 2024-02-09 18:14:29.000000 pih-doc-0.13/DocsService/api.py
+-rw-rw-rw-   0        0        0      536 2024-01-15 10:05:42.000000 pih-doc-0.13/DocsService/api_test.py
+-rw-rw-rw-   0        0        0     1634 2024-04-10 00:00:05.000000 pih-doc-0.13/DocsService/const.py
+-rw-rw-rw-   0        0        0     5275 2024-03-11 13:46:49.000000 pih-doc-0.13/DocsService/service.py
+-rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.13/DocsService/tools.py
+-rw-rw-rw-   0        0        0      595 2024-04-10 01:38:40.007807 pih-doc-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:38:39.976558 pih-doc-0.13/pih_doc.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-04-10 01:38:38.000000 pih-doc-0.13/pih_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:38:40.043037 pih-doc-0.13/setup.cfg
```

### Comparing `pih-doc-0.11/DocsService/api.py` & `pih-doc-0.13/DocsService/api.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.11/DocsService/api_test.py` & `pih-doc-0.13/DocsService/api_test.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.11/DocsService/const.py` & `pih-doc-0.13/DocsService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     QUANTITY_COLUMN_NAME: str = "фактическое наличие"
     NAME_MAX_LENTH: int = 120
     QUANTITY_NOT_SET: str = "-"
 
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.11"
+VERSION: str = "0.13"
 
 PACKAGES: tuple[str, ...] = (
     "xlsxwriter",
     "xlrd",
     "xlutils",
     "openpyxl",
     "python-barcode",
```

### Comparing `pih-doc-0.11/DocsService/service.py` & `pih-doc-0.13/DocsService/service.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.11/DocsService/tools.py` & `pih-doc-0.13/DocsService/tools.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.11/PKG-INFO` & `pih-doc-0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.11
+Version: 0.13
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-doc-0.11/pih_doc.egg-info/PKG-INFO` & `pih-doc-0.13/pih_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.11
+Version: 0.13
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

