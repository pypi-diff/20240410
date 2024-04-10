# Comparing `tmp/SudachiDict-full-20240109.tar.gz` & `tmp/SudachiDict-full-20240409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SudachiDict-full-20240109.tar", last modified: Wed Jan 17 02:29:37 2024, max compression
+gzip compressed data, was "SudachiDict-full-20240409.tar", last modified: Wed Apr 10 07:06:13 2024, max compression
```

## Comparing `SudachiDict-full-20240109.tar` & `SudachiDict-full-20240409.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-01-17 02:29:37.777856 SudachiDict-full-20240109/
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       85 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/INFO.json
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     6037 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/LEGAL
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)    11358 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/LICENSE-2.0.txt
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       84 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/MANIFEST.in
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2451 2024-01-17 02:29:37.777856 SudachiDict-full-20240109/PKG-INFO
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2097 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/README.md
-drwxr-xr-x   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-01-17 02:29:37.777856 SudachiDict-full-20240109/SudachiDict_full.egg-info/
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2451 2024-01-17 02:29:37.000000 SudachiDict-full-20240109/SudachiDict_full.egg-info/PKG-INFO
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)      290 2024-01-17 02:29:37.000000 SudachiDict-full-20240109/SudachiDict_full.egg-info/SOURCES.txt
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)        1 2024-01-17 02:29:37.000000 SudachiDict-full-20240109/SudachiDict_full.egg-info/dependency_links.txt
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       20 2024-01-17 02:29:37.000000 SudachiDict-full-20240109/SudachiDict_full.egg-info/requires.txt
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       17 2024-01-17 02:29:37.000000 SudachiDict-full-20240109/SudachiDict_full.egg-info/top_level.txt
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       38 2024-01-17 02:29:37.777856 SudachiDict-full-20240109/setup.cfg
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2543 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/setup.py
-drwxr-xr-x   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-01-17 02:29:37.777856 SudachiDict-full-20240109/sudachidict_full/
--rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-01-17 02:26:52.000000 SudachiDict-full-20240109/sudachidict_full/__init__.py
+drwxr-xr-x   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-04-10 07:06:13.022251 SudachiDict-full-20240409/
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       85 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/INFO.json
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     6037 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/LEGAL
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)    11358 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/LICENSE-2.0.txt
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       84 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/MANIFEST.in
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2451 2024-04-10 07:06:13.022251 SudachiDict-full-20240409/PKG-INFO
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2097 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/README.md
+drwxr-xr-x   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-04-10 07:06:13.022251 SudachiDict-full-20240409/SudachiDict_full.egg-info/
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2451 2024-04-10 07:06:13.000000 SudachiDict-full-20240409/SudachiDict_full.egg-info/PKG-INFO
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)      290 2024-04-10 07:06:13.000000 SudachiDict-full-20240409/SudachiDict_full.egg-info/SOURCES.txt
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)        1 2024-04-10 07:06:13.000000 SudachiDict-full-20240409/SudachiDict_full.egg-info/dependency_links.txt
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       20 2024-04-10 07:06:13.000000 SudachiDict-full-20240409/SudachiDict_full.egg-info/requires.txt
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       17 2024-04-10 07:06:13.000000 SudachiDict-full-20240409/SudachiDict_full.egg-info/top_level.txt
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)       38 2024-04-10 07:06:13.022251 SudachiDict-full-20240409/setup.cfg
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)     2543 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/setup.py
+drwxr-xr-x   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-04-10 07:06:13.022251 SudachiDict-full-20240409/sudachidict_full/
+-rw-r--r--   0 katsuta_a  (1000) katsuta_a  (1000)        0 2024-04-10 07:04:38.000000 SudachiDict-full-20240409/sudachidict_full/__init__.py
```

### Comparing `SudachiDict-full-20240109/LEGAL` & `SudachiDict-full-20240409/LEGAL`

 * *Files identical despite different names*

### Comparing `SudachiDict-full-20240109/LICENSE-2.0.txt` & `SudachiDict-full-20240409/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `SudachiDict-full-20240109/PKG-INFO` & `SudachiDict-full-20240409/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SudachiDict-full
-Version: 20240109
+Version: 20240409
 Summary: Sudachi Dictionary for SudachiPy - Full Edition
 Home-page: https://github.com/WorksApplications/SudachiDict
 Author: Works Applications
 Author-email: sudachi@worksap.co.jp
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `SudachiDict-full-20240109/README.md` & `SudachiDict-full-20240409/README.md`

 * *Files identical despite different names*

### Comparing `SudachiDict-full-20240109/SudachiDict_full.egg-info/PKG-INFO` & `SudachiDict-full-20240409/SudachiDict_full.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SudachiDict-full
-Version: 20240109
+Version: 20240409
 Summary: Sudachi Dictionary for SudachiPy - Full Edition
 Home-page: https://github.com/WorksApplications/SudachiDict
 Author: Works Applications
 Author-email: sudachi@worksap.co.jp
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `SudachiDict-full-20240109/setup.py` & `SudachiDict-full-20240409/setup.py`

 * *Files identical despite different names*

