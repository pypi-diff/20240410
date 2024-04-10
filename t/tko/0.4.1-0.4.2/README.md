# Comparing `tmp/tko-0.4.1.tar.gz` & `tmp/tko-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.4.1.tar", last modified: Mon Apr  8 14:40:46 2024, max compression
+gzip compressed data, was "tko-0.4.2.tar", last modified: Wed Apr 10 16:33:59 2024, max compression
```

## Comparing `tko-0.4.1.tar` & `tko-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.176667 tko-0.4.1/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.4.1/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.4.1/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-08 14:40:46.176667 tko-0.4.1/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.4.1/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     3431 2024-04-08 14:39:41.000000 tko-0.4.1/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.4.1/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-08 14:40:46.176667 tko-0.4.1/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.4.1/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.160000 tko-0.4.1/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.173334 tko-0.4.1/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-08 14:39:18.000000 tko-0.4.1/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.4.1/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6677 2024-04-08 14:20:36.000000 tko-0.4.1/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.4.1/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.4.1/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7528 2024-04-07 14:18:50.000000 tko-0.4.1/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.4.1/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.4.1/src/tko/guide.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.4.1/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.4.1/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.4.1/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.4.1/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3928 2024-04-07 16:10:03.000000 tko-0.4.1/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.4.1/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.4.1/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-08 14:40:46.173334 tko-0.4.1/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      536 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-08 14:40:46.000000 tko-0.4.1/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-10 16:33:59.430101 tko-0.4.2/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.4.2/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.4.2/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)    15575 2024-04-10 16:33:59.430101 tko-0.4.2/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)    14721 2024-04-10 12:42:10.000000 tko-0.4.2/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     3500 2024-04-10 16:33:44.000000 tko-0.4.2/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.4.2/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-10 16:33:59.433435 tko-0.4.2/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.4.2/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-10 16:33:59.420102 tko-0.4.2/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-10 16:33:59.426768 tko-0.4.2/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-10 16:32:53.000000 tko-0.4.2/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.4.2/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6677 2024-04-08 14:20:36.000000 tko-0.4.2/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.4.2/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.4.2/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7499 2024-04-09 17:36:51.000000 tko-0.4.2/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.4.2/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.4.2/src/tko/guide.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.4.2/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.4.2/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.4.2/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.4.2/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3928 2024-04-07 16:10:03.000000 tko-0.4.2/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.4.2/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.4.2/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-10 16:33:59.430101 tko-0.4.2/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)    15575 2024-04-10 16:33:59.000000 tko-0.4.2/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      536 2024-04-10 16:33:59.000000 tko-0.4.2/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-10 16:33:59.000000 tko-0.4.2/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-10 16:33:59.000000 tko-0.4.2/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-10 16:33:59.000000 tko-0.4.2/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-10 16:33:59.000000 tko-0.4.2/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.4.1/LICENSE` & `tko-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/changelog.md` & `tko-0.4.2/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+- 0.4.2
+  - fix: removed debug on down
+  - add: improved description
 - 0.4.1
   - fix: removing duplicated parameters in run command
 - 0.4.0
 - 0.3.9
   - fix: down dont create src folder
 - 0.3.8
   - fix: filter mode calling filter command from feno package
```

### Comparing `tko-0.4.1/setup.py` & `tko-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/__main__.py` & `tko-0.4.2/src/tko/__main__.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/actions.py` & `tko-0.4.2/src/tko/actions.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/basic.py` & `tko-0.4.2/src/tko/basic.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/diff.py` & `tko-0.4.2/src/tko/diff.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/down.py` & `tko-0.4.2/src/tko/down.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         index_url = course_url + activity + "/"
         cache_url = index_url + ".cache/"
         
 
         # downloading Readme
         try:
             destiny = Down.create_problem_folder(course, activity)
-            print(cache_url)
             [_readme_path, mapi_path] = Down.down_problem_def(destiny, cache_url)
         except urllib.error.HTTPError:
             print("fail: activity not found in course")
             # verifi if destiny folder is empty and remove it
             if len(os.listdir(destiny)) == 0:
                 os.rmdir(destiny)
```

### Comparing `tko-0.4.1/src/tko/format.py` & `tko-0.4.2/src/tko/format.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/guide.py` & `tko-0.4.2/src/tko/guide.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/loader.py` & `tko-0.4.2/src/tko/loader.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/pattern.py` & `tko-0.4.2/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/runner.py` & `tko-0.4.2/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/settings.py` & `tko-0.4.2/src/tko/settings.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/solver.py` & `tko-0.4.2/src/tko/solver.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/wdir.py` & `tko-0.4.2/src/tko/wdir.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko/writer.py` & `tko-0.4.2/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.4.1/src/tko.egg-info/SOURCES.txt` & `tko-0.4.2/src/tko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

