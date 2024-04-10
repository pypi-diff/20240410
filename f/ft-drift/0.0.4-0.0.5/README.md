# Comparing `tmp/ft-drift-0.0.4.tar.gz` & `tmp/ft-drift-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-drift-0.0.4.tar", last modified: Wed Apr 10 07:31:12 2024, max compression
+gzip compressed data, was "ft-drift-0.0.5.tar", last modified: Wed Apr 10 13:59:31 2024, max compression
```

## Comparing `ft-drift-0.0.4.tar` & `ft-drift-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:31:12.874698 ft-drift-0.0.4/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.4/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.4/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1882 2024-04-10 07:31:12.874492 ft-drift-0.0.4/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     1106 2024-04-10 07:30:58.000000 ft-drift-0.0.4/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:31:12.873208 ft-drift-0.0.4/ft_drift/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/cli.py
--rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/compare_funcs.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.4/ft_drift/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/model.py
--rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/parse.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:31:12.874313 ft-drift-0.0.4/ft_drift.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1882 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.4/ft_drift.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 07:31:03.000000 ft-drift-0.0.4/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 07:31:12.874740 ft-drift-0.0.4/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.4/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 13:59:31.711691 ft-drift-0.0.5/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.5/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.5/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1886 2024-04-10 13:59:31.711489 ft-drift-0.0.5/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     1110 2024-04-10 13:58:24.000000 ft-drift-0.0.5/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 13:59:31.710436 ft-drift-0.0.5/ft_drift/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 13:59:16.000000 ft-drift-0.0.5/ft_drift/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/cli.py
+-rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/compare_funcs.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.5/ft_drift/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/model.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/parse.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 13:59:31.711326 ft-drift-0.0.5/ft_drift.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1886 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.5/ft_drift.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 13:59:13.000000 ft-drift-0.0.5/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 13:59:31.711735 ft-drift-0.0.5/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.5/setup.py
```

### Comparing `ft-drift-0.0.4/LICENSE` & `ft-drift-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.4/PKG-INFO` & `ft-drift-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.4
+Version: 0.0.5
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -57,8 +57,8 @@
 - etc.
 
 ## Usage
 
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
-![](first.gif)
+![](drift_cli.gif)
```

### Comparing `ft-drift-0.0.4/README.md` & `ft-drift-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 - etc.
 
 ## Usage
 
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
-![](first.gif)
+![](drift_cli.gif)
```

### Comparing `ft-drift-0.0.4/ft_drift/_modidx.py` & `ft-drift-0.0.5/ft_drift/_modidx.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.4/ft_drift/cli.py` & `ft-drift-0.0.5/ft_drift/cli.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.4/ft_drift/compare_funcs.py` & `ft-drift-0.0.5/ft_drift/compare_funcs.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.4/ft_drift/model.py` & `ft-drift-0.0.5/ft_drift/model.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.4/ft_drift/parse.py` & `ft-drift-0.0.5/ft_drift/parse.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.4/ft_drift.egg-info/PKG-INFO` & `ft-drift-0.0.5/ft_drift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.4
+Version: 0.0.5
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -57,8 +57,8 @@
 - etc.
 
 ## Usage
 
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
-![](first.gif)
+![](drift_cli.gif)
```

### Comparing `ft-drift-0.0.4/settings.ini` & `ft-drift-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ft-drift
 lib_name = ft-drift
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ft_drift
 nbs_path = nbs
 recursive = True
```

### Comparing `ft-drift-0.0.4/setup.py` & `ft-drift-0.0.5/setup.py`

 * *Files identical despite different names*

