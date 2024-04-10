# Comparing `tmp/ft-drift-0.0.5.tar.gz` & `tmp/ft-drift-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-drift-0.0.5.tar", last modified: Wed Apr 10 13:59:31 2024, max compression
+gzip compressed data, was "ft-drift-0.0.6.tar", last modified: Wed Apr 10 14:34:42 2024, max compression
```

## Comparing `ft-drift-0.0.5.tar` & `ft-drift-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 13:59:31.711691 ft-drift-0.0.5/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.5/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.5/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1886 2024-04-10 13:59:31.711489 ft-drift-0.0.5/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     1110 2024-04-10 13:58:24.000000 ft-drift-0.0.5/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 13:59:31.710436 ft-drift-0.0.5/ft_drift/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 13:59:16.000000 ft-drift-0.0.5/ft_drift/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/cli.py
--rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/compare_funcs.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.5/ft_drift/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/model.py
--rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 13:59:13.000000 ft-drift-0.0.5/ft_drift/parse.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 13:59:31.711326 ft-drift-0.0.5/ft_drift.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1886 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.5/ft_drift.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 13:59:31.000000 ft-drift-0.0.5/ft_drift.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 13:59:13.000000 ft-drift-0.0.5/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 13:59:31.711735 ft-drift-0.0.5/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.5/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 14:34:42.247031 ft-drift-0.0.6/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.6/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.6/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     2874 2024-04-10 14:34:42.246789 ft-drift-0.0.6/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2098 2024-04-10 14:34:25.000000 ft-drift-0.0.6/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 14:34:42.245452 ft-drift-0.0.6/ft_drift/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 14:34:36.000000 ft-drift-0.0.6/ft_drift/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 14:34:36.000000 ft-drift-0.0.6/ft_drift/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 14:34:36.000000 ft-drift-0.0.6/ft_drift/cli.py
+-rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 14:34:36.000000 ft-drift-0.0.6/ft_drift/compare_funcs.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.6/ft_drift/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 14:34:36.000000 ft-drift-0.0.6/ft_drift/model.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 14:34:36.000000 ft-drift-0.0.6/ft_drift/parse.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 14:34:42.246592 ft-drift-0.0.6/ft_drift.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     2874 2024-04-10 14:34:42.000000 ft-drift-0.0.6/ft_drift.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 14:34:42.000000 ft-drift-0.0.6/ft_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 14:34:42.000000 ft-drift-0.0.6/ft_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 14:34:42.000000 ft-drift-0.0.6/ft_drift.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.6/ft_drift.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 14:34:42.000000 ft-drift-0.0.6/ft_drift.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 14:34:42.000000 ft-drift-0.0.6/ft_drift.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 14:34:36.000000 ft-drift-0.0.6/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 14:34:42.247080 ft-drift-0.0.6/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.6/setup.py
```

### Comparing `ft-drift-0.0.5/LICENSE` & `ft-drift-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.5/PKG-INFO` & `ft-drift-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.5
+Version: 0.0.6
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -58,7 +58,33 @@
 
 ## Usage
 
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
 ![](drift_cli.gif)
+
+## How Does it Work?
+
+This works by doing the following steps:
+
+1.  Fit a binary classifier (random forest) to discriminate between two
+    datasets.
+2.  If the classifier can predict a material difference (ex: AUC \>=
+    0.60) then we know there is drift (something is systematically
+    different b/w the two datasets).
+3.  We show the most important features from the classifier which are
+    tokens (segments of text) to help you debug what is different.
+
+If this tool doesn’t detect drift, it doesn’t mean drift doesn’t exist.
+It just means we didn’t find it. However, I’ve found run into this
+simple kind of drift enough times that having a way to quickly check
+saves time.
+
+## TODO
+
+This is a very basic drift detector! Other things that could be added:
+
+- [ ] Semantic drift by incorporating embeddings.
+- [ ] More features: length of messages, \# of turns, etc etc.
+- [ ] Wiring up the function definition diff to the CLI (I don’t need
+  this yet for my use case).
```

### Comparing `ft-drift-0.0.5/ft_drift/_modidx.py` & `ft-drift-0.0.6/ft_drift/_modidx.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.5/ft_drift/cli.py` & `ft-drift-0.0.6/ft_drift/cli.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.5/ft_drift/compare_funcs.py` & `ft-drift-0.0.6/ft_drift/compare_funcs.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.5/ft_drift/model.py` & `ft-drift-0.0.6/ft_drift/model.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.5/ft_drift/parse.py` & `ft-drift-0.0.6/ft_drift/parse.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.5/ft_drift.egg-info/PKG-INFO` & `ft-drift-0.0.6/ft_drift.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.5
+Version: 0.0.6
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -58,7 +58,33 @@
 
 ## Usage
 
 After installing `ft_drift`, the cli command `detect_drift` will be
 available to you.
 
 ![](drift_cli.gif)
+
+## How Does it Work?
+
+This works by doing the following steps:
+
+1.  Fit a binary classifier (random forest) to discriminate between two
+    datasets.
+2.  If the classifier can predict a material difference (ex: AUC \>=
+    0.60) then we know there is drift (something is systematically
+    different b/w the two datasets).
+3.  We show the most important features from the classifier which are
+    tokens (segments of text) to help you debug what is different.
+
+If this tool doesn’t detect drift, it doesn’t mean drift doesn’t exist.
+It just means we didn’t find it. However, I’ve found run into this
+simple kind of drift enough times that having a way to quickly check
+saves time.
+
+## TODO
+
+This is a very basic drift detector! Other things that could be added:
+
+- [ ] Semantic drift by incorporating embeddings.
+- [ ] More features: length of messages, \# of turns, etc etc.
+- [ ] Wiring up the function definition diff to the CLI (I don’t need
+  this yet for my use case).
```

### Comparing `ft-drift-0.0.5/settings.ini` & `ft-drift-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ft-drift
 lib_name = ft-drift
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ft_drift
 nbs_path = nbs
 recursive = True
```

### Comparing `ft-drift-0.0.5/setup.py` & `ft-drift-0.0.6/setup.py`

 * *Files identical despite different names*

