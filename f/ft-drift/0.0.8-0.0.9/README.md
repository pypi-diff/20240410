# Comparing `tmp/ft-drift-0.0.8.tar.gz` & `tmp/ft-drift-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-drift-0.0.8.tar", last modified: Wed Apr 10 18:57:27 2024, max compression
+gzip compressed data, was "ft-drift-0.0.9.tar", last modified: Wed Apr 10 18:59:06 2024, max compression
```

## Comparing `ft-drift-0.0.8.tar` & `ft-drift-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 18:57:27.085959 ft-drift-0.0.8/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.8/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.8/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     2869 2024-04-10 18:57:27.085736 ft-drift-0.0.8/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2093 2024-04-10 18:56:40.000000 ft-drift-0.0.8/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 18:57:27.084328 ft-drift-0.0.8/ft_drift/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 18:57:12.000000 ft-drift-0.0.8/ft_drift/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 18:57:12.000000 ft-drift-0.0.8/ft_drift/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 18:57:12.000000 ft-drift-0.0.8/ft_drift/cli.py
--rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 18:57:12.000000 ft-drift-0.0.8/ft_drift/compare_funcs.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.8/ft_drift/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 18:57:12.000000 ft-drift-0.0.8/ft_drift/model.py
--rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 18:57:12.000000 ft-drift-0.0.8/ft_drift/parse.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 18:57:27.085547 ft-drift-0.0.8/ft_drift.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     2869 2024-04-10 18:57:27.000000 ft-drift-0.0.8/ft_drift.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 18:57:27.000000 ft-drift-0.0.8/ft_drift.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 18:57:27.000000 ft-drift-0.0.8/ft_drift.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 18:57:27.000000 ft-drift-0.0.8/ft_drift.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.8/ft_drift.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 18:57:27.000000 ft-drift-0.0.8/ft_drift.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 18:57:27.000000 ft-drift-0.0.8/ft_drift.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 18:57:12.000000 ft-drift-0.0.8/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 18:57:27.086006 ft-drift-0.0.8/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.8/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 18:59:06.001362 ft-drift-0.0.9/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.9/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.9/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     2864 2024-04-10 18:59:06.001147 ft-drift-0.0.9/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2088 2024-04-10 18:58:35.000000 ft-drift-0.0.9/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 18:59:06.000062 ft-drift-0.0.9/ft_drift/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 18:58:57.000000 ft-drift-0.0.9/ft_drift/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 18:58:57.000000 ft-drift-0.0.9/ft_drift/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 18:58:57.000000 ft-drift-0.0.9/ft_drift/cli.py
+-rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 18:58:57.000000 ft-drift-0.0.9/ft_drift/compare_funcs.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.9/ft_drift/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 18:58:57.000000 ft-drift-0.0.9/ft_drift/model.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 18:58:57.000000 ft-drift-0.0.9/ft_drift/parse.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 18:59:06.000964 ft-drift-0.0.9/ft_drift.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     2864 2024-04-10 18:59:05.000000 ft-drift-0.0.9/ft_drift.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 18:59:05.000000 ft-drift-0.0.9/ft_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 18:59:05.000000 ft-drift-0.0.9/ft_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 18:59:05.000000 ft-drift-0.0.9/ft_drift.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.9/ft_drift.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 18:59:05.000000 ft-drift-0.0.9/ft_drift.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 18:59:05.000000 ft-drift-0.0.9/ft_drift.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 18:58:57.000000 ft-drift-0.0.9/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 18:59:06.001406 ft-drift-0.0.9/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.9/setup.py
```

### Comparing `ft-drift-0.0.8/LICENSE` & `ft-drift-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.8/PKG-INFO` & `ft-drift-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.8
+Version: 0.0.9
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -83,10 +83,10 @@
 ![](drift_tfx.png)
 
 ## TODO
 
 Other things that could be added:
 
 - [ ] Semantic drift by incorporating embeddings.
-- [ ] More features: length of messages, \# of turns, etc etc.
+- [ ] More features: length of messages, \# of turns etc.
 - [ ] Wiring up the function definition diff to the CLI (I don’t need
   this yet for my use case).
```

### Comparing `ft-drift-0.0.8/README.md` & `ft-drift-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
 ![](drift_tfx.png)
 
 ## TODO
 
 Other things that could be added:
 
 - [ ] Semantic drift by incorporating embeddings.
-- [ ] More features: length of messages, \# of turns, etc etc.
+- [ ] More features: length of messages, \# of turns etc.
 - [ ] Wiring up the function definition diff to the CLI (I don’t need
   this yet for my use case).
```

### Comparing `ft-drift-0.0.8/ft_drift/_modidx.py` & `ft-drift-0.0.9/ft_drift/_modidx.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.8/ft_drift/cli.py` & `ft-drift-0.0.9/ft_drift/cli.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.8/ft_drift/compare_funcs.py` & `ft-drift-0.0.9/ft_drift/compare_funcs.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.8/ft_drift/model.py` & `ft-drift-0.0.9/ft_drift/model.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.8/ft_drift/parse.py` & `ft-drift-0.0.9/ft_drift/parse.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.8/ft_drift.egg-info/PKG-INFO` & `ft-drift-0.0.9/ft_drift.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.8
+Version: 0.0.9
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -83,10 +83,10 @@
 ![](drift_tfx.png)
 
 ## TODO
 
 Other things that could be added:
 
 - [ ] Semantic drift by incorporating embeddings.
-- [ ] More features: length of messages, \# of turns, etc etc.
+- [ ] More features: length of messages, \# of turns etc.
 - [ ] Wiring up the function definition diff to the CLI (I don’t need
   this yet for my use case).
```

### Comparing `ft-drift-0.0.8/settings.ini` & `ft-drift-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ft-drift
 lib_name = ft-drift
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ft_drift
 nbs_path = nbs
 recursive = True
```

### Comparing `ft-drift-0.0.8/setup.py` & `ft-drift-0.0.9/setup.py`

 * *Files identical despite different names*

