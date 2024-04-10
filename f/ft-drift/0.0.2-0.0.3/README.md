# Comparing `tmp/ft-drift-0.0.2.tar.gz` & `tmp/ft-drift-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-drift-0.0.2.tar", last modified: Wed Apr 10 07:17:31 2024, max compression
+gzip compressed data, was "ft-drift-0.0.3.tar", last modified: Wed Apr 10 07:18:50 2024, max compression
```

## Comparing `ft-drift-0.0.2.tar` & `ft-drift-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:17:31.440532 ft-drift-0.0.2/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.2/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.2/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:17:31.440323 ft-drift-0.0.2/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     1002 2024-04-10 07:16:58.000000 ft-drift-0.0.2/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:17:31.439080 ft-drift-0.0.2/ft_drift/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/cli.py
--rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/compare_funcs.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.2/ft_drift/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/model.py
--rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/parse.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:17:31.440140 ft-drift-0.0.2/ft_drift.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.2/ft_drift.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 07:17:23.000000 ft-drift-0.0.2/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 07:17:31.440580 ft-drift-0.0.2/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.2/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:18:50.485460 ft-drift-0.0.3/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.3/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.3/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1788 2024-04-10 07:18:50.485229 ft-drift-0.0.3/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     1012 2024-04-10 07:18:35.000000 ft-drift-0.0.3/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:18:50.483954 ft-drift-0.0.3/ft_drift/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/cli.py
+-rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/compare_funcs.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.3/ft_drift/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/model.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/parse.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:18:50.485036 ft-drift-0.0.3/ft_drift.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1788 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.3/ft_drift.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 07:18:15.000000 ft-drift-0.0.3/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 07:18:50.485506 ft-drift-0.0.3/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.3/setup.py
```

### Comparing `ft-drift-0.0.2/LICENSE` & `ft-drift-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.2/PKG-INFO` & `ft-drift-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.2
+Version: 0.0.3
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,15 +31,15 @@
 
 ## Install
 
 ``` sh
 pip install ft_drift
 ```
 
-## How to use
+## Background
 
 Common situations where you want to check for dataset drift:
 
 1.  You fine-tuned a new model but it doesn’t work the way you expect
     compared to a previous model trained on different data.
 2.  Your model is trained on data that doesn’t reflect production.
 
@@ -51,11 +51,13 @@
 following tokens were found to be different:
 
 - `END-UI-FORMAT`
 - `UI-FORMAT`
 - “\`\`\`json”
 - etc.
 
+## Usage
+
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
 ![](first.gif)
```

### Comparing `ft-drift-0.0.2/README.md` & `ft-drift-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ## Install
 
 ``` sh
 pip install ft_drift
 ```
 
-## How to use
+## Background
 
 Common situations where you want to check for dataset drift:
 
 1.  You fine-tuned a new model but it doesn’t work the way you expect
     compared to a previous model trained on different data.
 2.  Your model is trained on data that doesn’t reflect production.
 
@@ -29,11 +29,13 @@
 following tokens were found to be different:
 
 - `END-UI-FORMAT`
 - `UI-FORMAT`
 - “\`\`\`json”
 - etc.
 
+## Usage
+
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
 ![](first.gif)
```

### Comparing `ft-drift-0.0.2/ft_drift/_modidx.py` & `ft-drift-0.0.3/ft_drift/_modidx.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.2/ft_drift/cli.py` & `ft-drift-0.0.3/ft_drift/cli.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.2/ft_drift/compare_funcs.py` & `ft-drift-0.0.3/ft_drift/compare_funcs.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.2/ft_drift/model.py` & `ft-drift-0.0.3/ft_drift/model.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.2/ft_drift/parse.py` & `ft-drift-0.0.3/ft_drift/parse.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.2/ft_drift.egg-info/PKG-INFO` & `ft-drift-0.0.3/ft_drift.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.2
+Version: 0.0.3
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,15 +31,15 @@
 
 ## Install
 
 ``` sh
 pip install ft_drift
 ```
 
-## How to use
+## Background
 
 Common situations where you want to check for dataset drift:
 
 1.  You fine-tuned a new model but it doesn’t work the way you expect
     compared to a previous model trained on different data.
 2.  Your model is trained on data that doesn’t reflect production.
 
@@ -51,11 +51,13 @@
 following tokens were found to be different:
 
 - `END-UI-FORMAT`
 - `UI-FORMAT`
 - “\`\`\`json”
 - etc.
 
+## Usage
+
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
 ![](first.gif)
```

### Comparing `ft-drift-0.0.2/settings.ini` & `ft-drift-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ft-drift
 lib_name = ft-drift
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ft_drift
 nbs_path = nbs
 recursive = True
```

### Comparing `ft-drift-0.0.2/setup.py` & `ft-drift-0.0.3/setup.py`

 * *Files identical despite different names*

