# Comparing `tmp/pdfmarker-0.1.0.tar.gz` & `tmp/pdfmarker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfmarker-0.1.0.tar", max compression
+gzip compressed data, was "pdfmarker-0.1.1.tar", max compression
```

## Comparing `pdfmarker-0.1.0.tar` & `pdfmarker-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-04-10 15:58:12.747397 pdfmarker-0.1.0/LICENSE
--rw-r--r--   0        0        0     2051 2024-04-10 15:58:12.747397 pdfmarker-0.1.0/README.md
--rw-r--r--   0        0        0      129 2024-04-10 15:58:12.747397 pdfmarker-0.1.0/pdfmarker/__init__.py
--rw-r--r--   0        0        0     1236 2024-04-10 15:58:12.747397 pdfmarker-0.1.0/pdfmarker/colors.py
--rw-r--r--   0        0        0     5212 2024-04-10 15:58:12.747397 pdfmarker-0.1.0/pdfmarker/pdfmarker.py
--rw-r--r--   0        0        0      467 2024-04-10 15:58:12.747397 pdfmarker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2663 1970-01-01 00:00:00.000000 pdfmarker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-10 16:05:29.490823 pdfmarker-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2051 2024-04-10 16:05:29.490823 pdfmarker-0.1.1/README.md
+-rw-r--r--   0        0        0      129 2024-04-10 16:05:29.490823 pdfmarker-0.1.1/pdfmarker/__init__.py
+-rw-r--r--   0        0        0     1236 2024-04-10 16:05:29.490823 pdfmarker-0.1.1/pdfmarker/colors.py
+-rw-r--r--   0        0        0     5212 2024-04-10 16:05:29.494823 pdfmarker-0.1.1/pdfmarker/pdfmarker.py
+-rw-r--r--   0        0        0      471 2024-04-10 16:05:29.494823 pdfmarker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 pdfmarker-0.1.1/PKG-INFO
```

### Comparing `pdfmarker-0.1.0/LICENSE` & `pdfmarker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfmarker-0.1.0/README.md` & `pdfmarker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pdfmarker-0.1.0/pdfmarker/colors.py` & `pdfmarker-0.1.1/pdfmarker/colors.py`

 * *Files identical despite different names*

### Comparing `pdfmarker-0.1.0/pdfmarker/pdfmarker.py` & `pdfmarker-0.1.1/pdfmarker/pdfmarker.py`

 * *Files identical despite different names*

### Comparing `pdfmarker-0.1.0/PKG-INFO` & `pdfmarker-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pdfmarker
-Version: 0.1.0
-Summary: Simple tool to add highlights/markers to pdf documents.
-Author: Your Name
-Author-email: you@example.com
+Version: 0.1.1
+Summary: Simple tool to mark/add highlights to pdf documents.
+Author: Tom Uijtdehaag
+Author-email: tjl.udh@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyMuPDF (>=1.24.0,<2.0.0)
```

