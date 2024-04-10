# Comparing `tmp/ft-drift-0.0.3.tar.gz` & `tmp/ft-drift-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-drift-0.0.3.tar", last modified: Wed Apr 10 07:18:50 2024, max compression
+gzip compressed data, was "ft-drift-0.0.4.tar", last modified: Wed Apr 10 07:31:12 2024, max compression
```

## Comparing `ft-drift-0.0.3.tar` & `ft-drift-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:18:50.485460 ft-drift-0.0.3/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.3/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.3/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1788 2024-04-10 07:18:50.485229 ft-drift-0.0.3/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     1012 2024-04-10 07:18:35.000000 ft-drift-0.0.3/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:18:50.483954 ft-drift-0.0.3/ft_drift/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/cli.py
--rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/compare_funcs.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.3/ft_drift/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/model.py
--rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 07:18:19.000000 ft-drift-0.0.3/ft_drift/parse.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:18:50.485036 ft-drift-0.0.3/ft_drift.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1788 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.3/ft_drift.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 07:18:50.000000 ft-drift-0.0.3/ft_drift.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 07:18:15.000000 ft-drift-0.0.3/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 07:18:50.485506 ft-drift-0.0.3/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.3/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:31:12.874698 ft-drift-0.0.4/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.4/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.4/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1882 2024-04-10 07:31:12.874492 ft-drift-0.0.4/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     1106 2024-04-10 07:30:58.000000 ft-drift-0.0.4/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:31:12.873208 ft-drift-0.0.4/ft_drift/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/cli.py
+-rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/compare_funcs.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.4/ft_drift/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/model.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 07:31:03.000000 ft-drift-0.0.4/ft_drift/parse.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:31:12.874313 ft-drift-0.0.4/ft_drift.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1882 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.4/ft_drift.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 07:31:12.000000 ft-drift-0.0.4/ft_drift.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 07:31:03.000000 ft-drift-0.0.4/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 07:31:12.874740 ft-drift-0.0.4/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.4/setup.py
```

### Comparing `ft-drift-0.0.3/LICENSE` & `ft-drift-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.3/PKG-INFO` & `ft-drift-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.3
+Version: 0.0.4
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -33,26 +33,27 @@
 
 ``` sh
 pip install ft_drift
 ```
 
 ## Background
 
-Common situations where you want to check for dataset drift:
+Checking for dataset drift can help you debug if:
 
-1.  You fine-tuned a new model but it doesn’t work the way you expect
-    compared to a previous model trained on different data.
-2.  Your model is trained on data that doesn’t reflect production.
-
-In either situation, you can collect your data from the relevant sources
-and compare them to see if the data has changed in ways that are
-undesirable.
-
-In the demo below, we detect data drift between two datasets where the
-following tokens were found to be different:
+1.  Your model is trained on data that doesn’t reflect production
+    (different prompts, functions, etc).
+2.  Your training data contains unexpected or accidental artifacts.
+
+In either situation, you can compare data from relevant sources
+(i.e. production vs fine-tuning) to find unwanted changes. This is one
+of the most common source of errors when fine-tuning models!
+
+The demo below shows a cli tool used to detect data drift between two
+files, `file_a.jsonl` and `file_b.jsonl`. Afterwards, a table of
+important tokens that account for the drift are shown, such as:
 
 - `END-UI-FORMAT`
 - `UI-FORMAT`
 - “\`\`\`json”
 - etc.
 
 ## Usage
```

### Comparing `ft-drift-0.0.3/README.md` & `ft-drift-0.0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 ``` sh
 pip install ft_drift
 ```
 
 ## Background
 
-Common situations where you want to check for dataset drift:
+Checking for dataset drift can help you debug if:
 
-1.  You fine-tuned a new model but it doesn’t work the way you expect
-    compared to a previous model trained on different data.
-2.  Your model is trained on data that doesn’t reflect production.
-
-In either situation, you can collect your data from the relevant sources
-and compare them to see if the data has changed in ways that are
-undesirable.
-
-In the demo below, we detect data drift between two datasets where the
-following tokens were found to be different:
+1.  Your model is trained on data that doesn’t reflect production
+    (different prompts, functions, etc).
+2.  Your training data contains unexpected or accidental artifacts.
+
+In either situation, you can compare data from relevant sources
+(i.e. production vs fine-tuning) to find unwanted changes. This is one
+of the most common source of errors when fine-tuning models!
+
+The demo below shows a cli tool used to detect data drift between two
+files, `file_a.jsonl` and `file_b.jsonl`. Afterwards, a table of
+important tokens that account for the drift are shown, such as:
 
 - `END-UI-FORMAT`
 - `UI-FORMAT`
 - “\`\`\`json”
 - etc.
 
 ## Usage
```

### Comparing `ft-drift-0.0.3/ft_drift/_modidx.py` & `ft-drift-0.0.4/ft_drift/_modidx.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.3/ft_drift/cli.py` & `ft-drift-0.0.4/ft_drift/cli.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.3/ft_drift/compare_funcs.py` & `ft-drift-0.0.4/ft_drift/compare_funcs.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.3/ft_drift/model.py` & `ft-drift-0.0.4/ft_drift/model.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.3/ft_drift/parse.py` & `ft-drift-0.0.4/ft_drift/parse.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.3/ft_drift.egg-info/PKG-INFO` & `ft-drift-0.0.4/ft_drift.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-drift
-Version: 0.0.3
+Version: 0.0.4
 Summary: Check for data drift with OAI data
 Home-page: https://github.com/hamelsmu/ft-drift
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -33,26 +33,27 @@
 
 ``` sh
 pip install ft_drift
 ```
 
 ## Background
 
-Common situations where you want to check for dataset drift:
+Checking for dataset drift can help you debug if:
 
-1.  You fine-tuned a new model but it doesn’t work the way you expect
-    compared to a previous model trained on different data.
-2.  Your model is trained on data that doesn’t reflect production.
-
-In either situation, you can collect your data from the relevant sources
-and compare them to see if the data has changed in ways that are
-undesirable.
-
-In the demo below, we detect data drift between two datasets where the
-following tokens were found to be different:
+1.  Your model is trained on data that doesn’t reflect production
+    (different prompts, functions, etc).
+2.  Your training data contains unexpected or accidental artifacts.
+
+In either situation, you can compare data from relevant sources
+(i.e. production vs fine-tuning) to find unwanted changes. This is one
+of the most common source of errors when fine-tuning models!
+
+The demo below shows a cli tool used to detect data drift between two
+files, `file_a.jsonl` and `file_b.jsonl`. Afterwards, a table of
+important tokens that account for the drift are shown, such as:
 
 - `END-UI-FORMAT`
 - `UI-FORMAT`
 - “\`\`\`json”
 - etc.
 
 ## Usage
```

### Comparing `ft-drift-0.0.3/settings.ini` & `ft-drift-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ft-drift
 lib_name = ft-drift
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ft_drift
 nbs_path = nbs
 recursive = True
```

### Comparing `ft-drift-0.0.3/setup.py` & `ft-drift-0.0.4/setup.py`

 * *Files identical despite different names*

