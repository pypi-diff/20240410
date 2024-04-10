# Comparing `tmp/shipdataprocess-0.8.3.tar.gz` & `tmp/shipdataprocess-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shipdataprocess-0.8.3.tar", last modified: Fri Apr  5 09:26:01 2024, max compression
+gzip compressed data, was "dist/shipdataprocess-0.8.4.tar", last modified: Tue Apr  9 17:44:49 2024, max compression
```

## Comparing `shipdataprocess-0.8.3.tar` & `shipdataprocess-0.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/
--rw-r--r--   0 root         (0) root         (0)     1414 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)      488 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess/
--rw-r--r--   0 root         (0) root         (0)     5154 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/collapse.py
--rw-r--r--   0 root         (0) root         (0)    17757 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/shiptype.py
--rw-r--r--   0 root         (0) root         (0)      905 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9071 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/normalize.py
--rw-r--r--   0 root         (0) root         (0)    19542 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/standardize.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess/_version.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      277 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      879 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/setup.py
--rw-r--r--   0 root         (0) root         (0)     3667 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)    83607 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:44:49.000000 shipdataprocess-0.8.4/
+-rw-r--r--   0 root         (0) root         (0)     1414 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:44:49.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-09 17:44:48.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:44:48.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)      488 2024-04-09 17:44:48.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-09 17:44:48.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 17:44:48.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:44:48.000000 shipdataprocess-0.8.4/shipdataprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:44:49.000000 shipdataprocess-0.8.4/shipdataprocess/
+-rw-r--r--   0 root         (0) root         (0)     5154 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/shipdataprocess/collapse.py
+-rw-r--r--   0 root         (0) root         (0)    17757 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/shipdataprocess/shiptype.py
+-rw-r--r--   0 root         (0) root         (0)      905 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/shipdataprocess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/shipdataprocess/normalize.py
+-rw-r--r--   0 root         (0) root         (0)    19565 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/shipdataprocess/standardize.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-09 17:44:49.000000 shipdataprocess-0.8.4/shipdataprocess/_version.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-09 17:44:49.000000 shipdataprocess-0.8.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      277 2024-04-09 17:44:49.000000 shipdataprocess-0.8.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3734 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)    83607 2024-04-09 17:44:19.000000 shipdataprocess-0.8.4/versioneer.py
```

### Comparing `shipdataprocess-0.8.3/README.md` & `shipdataprocess-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/shipdataprocess.egg-info/PKG-INFO` & `shipdataprocess-0.8.4/shipdataprocess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipdataprocess
-Version: 0.8.3
+Version: 0.8.4
 Summary: Useful modules to process vessel data
 Home-page: https://github.com/GlobalFishingWatch/shipdataprocess
 Author: Jaeyoon Park
 Author-email: jaeyoon@globalfishingwatch.org
 License: Apache 2.0
 Keywords: ship,vessel,fishing,normalization
 Platform: UNKNOWN
```

### Comparing `shipdataprocess-0.8.3/shipdataprocess/collapse.py` & `shipdataprocess-0.8.4/shipdataprocess/collapse.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/shipdataprocess/shiptype.py` & `shipdataprocess-0.8.4/shipdataprocess/shiptype.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/shipdataprocess/__init__.py` & `shipdataprocess-0.8.4/shipdataprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/shipdataprocess/normalize.py` & `shipdataprocess-0.8.4/shipdataprocess/normalize.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/shipdataprocess/standardize.py` & `shipdataprocess-0.8.4/shipdataprocess/standardize.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,15 @@
                 if not pd.isna(x)
                 else None )
         elif (elem != elem) | (elem is None) | (elem == ""):
             return None
         elif (type(elem) == str) | (type(elem) == int) | (type(elem) == float):
             return clean_int_str(elem)
         else:
-            raise ValueError("Unknown type received")
+            raise ValueError("Unknown type received in standardize_int_str")
     else:
         return None
 
 
 def standardize_time(elem, check_field=True):
     """
     This modules standardizes a timestamp
```

### Comparing `shipdataprocess-0.8.3/PKG-INFO` & `shipdataprocess-0.8.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipdataprocess
-Version: 0.8.3
+Version: 0.8.4
 Summary: Useful modules to process vessel data
 Home-page: https://github.com/GlobalFishingWatch/shipdataprocess
 Author: Jaeyoon Park
 Author-email: jaeyoon@globalfishingwatch.org
 License: Apache 2.0
 Keywords: ship,vessel,fishing,normalization
 Platform: UNKNOWN
```

### Comparing `shipdataprocess-0.8.3/LICENSE` & `shipdataprocess-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/setup.py` & `shipdataprocess-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.3/CHANGES.md` & `shipdataprocess-0.8.4/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,9 +39,10 @@
 v0.6.17, 2021-07-30 -- Add Indonesian prefix and Chinese HAO suffix to the list of prefix/suffix to be removed 
 v0.6.18, 2021-08-04 -- Fix a bug in normalize_callsign() regarding NULL/NONE  
 v0.7.0, 2022-01-26 -- Fix it to work only in Python 3.6 or above, codes are compliant with PEP8, dependencies are clearer (Django removed)   
 v0.7.1, 2022-01-27 -- Fix a bug related to the shift to Python 3.6 or above compatibility  
 v0.8.0, 2023-06-07 -- Improve normalize_shipname() to replace STA and STA. values to SANTA and fix discrepancy with the trailing 0s and suffix N
 v0.8.2, 2023-08-21 -- Fix a bug in normalize_shipname() regarding STA./STA replace feature.
 v0.8.3, 2024-04-04 -- Fix a bug in standardize_int_str(). Check if string is an integer before trying to cast.
+v0.8.4, 2024-04-05 -- Minor improvements in standardize_int_str().
```

### Comparing `shipdataprocess-0.8.3/versioneer.py` & `shipdataprocess-0.8.4/versioneer.py`

 * *Files identical despite different names*

