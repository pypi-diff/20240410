# Comparing `tmp/jemma-0.1.1284.tar.gz` & `tmp/jemma-0.1.1285.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1284.tar", last modified: Tue Apr  9 19:43:55 2024, max compression
+gzip compressed data, was "jemma-0.1.1285.tar", last modified: Tue Apr  9 19:56:04 2024, max compression
```

## Comparing `jemma-0.1.1284.tar` & `jemma-0.1.1285.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.466258 jemma-0.1.1284/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:43:55.465335 jemma-0.1.1284/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      751 2024-04-09 19:09:59.000000 jemma-0.1.1284/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.432497 jemma-0.1.1284/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1284/jemma/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.439232 jemma-0.1.1284/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1284/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.441157 jemma-0.1.1284/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1284/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1284/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.446028 jemma-0.1.1284/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1284/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1284/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15402 2024-04-09 18:44:55.000000 jemma-0.1.1284/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.449391 jemma-0.1.1284/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1284/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1284/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.452804 jemma-0.1.1284/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1284/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1284/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.460413 jemma-0.1.1284/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1284/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1284/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.1284/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1284/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1284/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1284/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1284/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.463356 jemma-0.1.1284/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1284/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1284/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:43:55.437924 jemma-0.1.1284/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:43:55.000000 jemma-0.1.1284/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-09 19:43:55.000000 jemma-0.1.1284/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 19:43:55.000000 jemma-0.1.1284/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 19:43:55.000000 jemma-0.1.1284/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 19:43:55.000000 jemma-0.1.1284/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 19:43:55.000000 jemma-0.1.1284/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 19:43:55.466462 jemma-0.1.1284/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 19:43:49.000000 jemma-0.1.1284/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.761820 jemma-0.1.1285/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:56:04.761368 jemma-0.1.1285/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      751 2024-04-09 19:09:59.000000 jemma-0.1.1285/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.739819 jemma-0.1.1285/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1285/jemma/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.744412 jemma-0.1.1285/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1285/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.746129 jemma-0.1.1285/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1285/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1285/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.749571 jemma-0.1.1285/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1285/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1285/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1285/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.751201 jemma-0.1.1285/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1285/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1285/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.753334 jemma-0.1.1285/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1285/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1285/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.758638 jemma-0.1.1285/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1285/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1285/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.1285/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1285/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1285/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1285/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1285/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.760336 jemma-0.1.1285/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1285/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1285/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.743548 jemma-0.1.1285/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 19:56:04.761957 jemma-0.1.1285/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 19:56:00.000000 jemma-0.1.1285/setup.py
```

### Comparing `jemma-0.1.1284/README.md` & `jemma-0.1.1285/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/prompt/business/owner.py` & `jemma-0.1.1285/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/prompt/engineer/clarify.py` & `jemma-0.1.1285/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/prompt/engineer/code.py` & `jemma-0.1.1285/jemma/prompt/engineer/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 (!) make sure ALL the requirements and actions are addressed in the CSS file.
 """
 
 
 def create_javascript_file(requirements, css):
     return f"""
 You are a JavaScript expert who specializes in jQuery with a focus on Twitter Bootstrap and DataTables libraries.
-In case you are building a game, feel free to bring in PixiJS, Phaser, ArcadeJS, or any other game library.
-In case of charts, feel free to bring in Highcharts, D3.js, Chart.js, or any other charting library.
 
 Given requirements and a CSS file (based on "bootstrap.css") your task is to generate a JavaScript file that utilizes the jQuery library to create an interactive and dynamic web prototype based on these requirements that relies on that CSS file.
 
 for tables, use a DataTables jQuery plugin to enhance the functionality and appearance of the tables.
 
 This JavaScript file should be self-contained as this would be the only file that would be used to run the web prototype.
```

### Comparing `jemma-0.1.1284/jemma/prompt/tester/test.py` & `jemma-0.1.1285/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/requirements/feature.py` & `jemma-0.1.1285/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/team/business_owner.py` & `jemma-0.1.1285/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/team/engineer.py` & `jemma-0.1.1285/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/team/project_manager.py` & `jemma-0.1.1285/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/team/tester.py` & `jemma-0.1.1285/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/thinker.py` & `jemma-0.1.1285/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/tools.py` & `jemma-0.1.1285/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma/work/flow.py` & `jemma-0.1.1285/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1284/jemma.egg-info/SOURCES.txt` & `jemma-0.1.1285/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

