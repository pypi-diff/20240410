# Comparing `tmp/civilpy-0.0.78.tar.gz` & `tmp/civilpy-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.78.tar", last modified: Fri Apr  5 13:49:11 2024, max compression
+gzip compressed data, was "civilpy-0.0.79.tar", last modified: Wed Apr 10 16:02:59 2024, max compression
```

## Comparing `civilpy-0.0.78.tar` & `civilpy-0.0.79.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.162531 civilpy-0.0.78/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.78/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6695 2024-04-05 13:49:11.162531 civilpy-0.0.78/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.78/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 13:49:11.162531 civilpy-0.0.78/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-04 19:12:50.000000 civilpy-0.0.78/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.78/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14167 2024-04-04 19:12:50.000000 civilpy-0.0.78/src/civilpy/structural/arema.py
--rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.78/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)     8479 2024-03-27 12:42:27.000000 civilpy-0.0.78/src/civilpy/structural/midas.py
--rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/structural/rail_tpg_design.py
--rw-rw-rw-   0 root         (0) root         (0)    15183 2024-03-08 15:32:48.000000 civilpy-0.0.78/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6695 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1253 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      719 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.876086 civilpy-0.0.79/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.79/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-04-10 16:02:59.876086 civilpy-0.0.79/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.79/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:02:59.876086 civilpy-0.0.79/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2024-04-10 15:21:28.000000 civilpy-0.0.79/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.79/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.868086 civilpy-0.0.79/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.872086 civilpy-0.0.79/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.872086 civilpy-0.0.79/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14167 2024-04-04 19:12:50.000000 civilpy-0.0.79/src/civilpy/structural/arema.py
+-rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.79/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)     8479 2024-03-27 12:42:27.000000 civilpy-0.0.79/src/civilpy/structural/midas.py
+-rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/structural/rail_tpg_design.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.872086 civilpy-0.0.79/src/civilpy/structural/res/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:02:26.000000 civilpy-0.0.79/src/civilpy/structural/res/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6559 2024-04-10 14:26:23.000000 civilpy-0.0.79/src/civilpy/structural/res/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    18307 2024-04-10 14:26:23.000000 civilpy-0.0.79/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.872086 civilpy-0.0.79/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.872086 civilpy-0.0.79/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.79/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:02:59.872086 civilpy-0.0.79/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-04-10 16:02:59.000000 civilpy-0.0.79/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-04-10 16:02:59.000000 civilpy-0.0.79/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 16:02:59.000000 civilpy-0.0.79/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      719 2024-04-10 16:02:59.000000 civilpy-0.0.79/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-10 16:02:59.000000 civilpy-0.0.79/src/civilpy.egg-info/top_level.txt
```

### Comparing `civilpy-0.0.78/LICENSE` & `civilpy-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/PKG-INFO` & `civilpy-0.0.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.78
+Version: 0.0.79
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.78 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.79 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Environment :: Console :: Curses
```

### Comparing `civilpy-0.0.78/README.md` & `civilpy-0.0.79/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/setup.py` & `civilpy-0.0.79/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.78',
-    packages=find_packages('src', exclude=['test', 'secrets', 'docs', 'res']),
+    version='0.0.79',
+    packages=find_packages('src', exclude=['test', 'Notebooks', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     license='MIT',
     py_modules=[
         "civilpy.state.ohio.dot",
```

### Comparing `civilpy-0.0.78/src/civilpy/general/database_tools.py` & `civilpy-0.0.79/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/general/microstation.py` & `civilpy-0.0.79/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/general/photos.py` & `civilpy-0.0.79/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.79/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.79/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.79/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.79/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/structural/arema.py` & `civilpy-0.0.79/src/civilpy/structural/arema.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.79/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/structural/midas.py` & `civilpy-0.0.79/src/civilpy/structural/midas.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/structural/rail_tpg_design.py` & `civilpy-0.0.79/src/civilpy/structural/rail_tpg_design.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy/structural/steel.py` & `civilpy-0.0.79/src/civilpy/structural/steel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import numpy as np
 import pandas as pd
 from civilpy.general import units
+from civilpy.structural.res.definitions import A325_bolt_weights
 
 steel_tables = pd.read_csv(
     'https://daneparks.com/Dane/civilpy/-/raw/master/src/civilpy/structural/res/steel_shapes.csv?ref_type=heads'
 )
 
 
 def hello_world(user_input="World"):
     return f"Hello {user_input}!"
 
 
-def conv_frac_str(fraction_string: str) -> float():
+def conv_frac_str(fraction_string: str) -> float:
     try:
         return float(fraction_string)
     except ValueError:
         num, denominator = fraction_string.split('/')
         try:
             leading, num = num.split()
             whole = float(leading)
@@ -413,10 +415,107 @@
     def __init__(self, label):
         super(Pipe, self).__init__(label)
         self.OD = conv_frac_str(self.aisc_value['OD'].values[0]) * units('in')
         self.ID = conv_frac_str(self.aisc_value['ID'].values[0]) * units('in')
         self.D_t = conv_frac_str(self.aisc_value['D/t'].values[0])
 
 
+def get_bolt_weights(length: float, diameter: float, no_of_washers: int) -> float:
+    """
+    Function to get the bolt weights from the A325_bolt_weights dictionary and calculate the weight per bolt if it's
+    not contained in the table.
+
+    Original table from:
+    https://www.portlandbolt.com/print/?table=7587
+
+    The A325_bolt_weights dictionary reports the weight indexed by bolt length and diameter, and reports the value in
+    lbs/100 bolts. This function simplifies that by reducing the value to that of a single bolt.
+
+    If bolt weights are not contained in the dictionary, the function will utilize the following formula to calculate
+    the weight per bolt, if no_of_washers is greater than 0, it will include the weight of the washers in the
+    calculation with the following values:
+
+    Per inch Adder (dia):
+        0.5: 5.5
+        0.625: 8.6
+        0.75: 12.4
+        0.875: 16.9
+        1.0: 22.1
+        1.125: 28
+        1.25: 34.4
+        1.375: 42.5
+        1.5: 49.7
+
+    F436 Round Washers
+        0.5: 2.1
+        0.625: 3.6
+        0.75: 4.8
+        0.875: 7
+        1.0: 9.4
+        1.125: 11.3
+        1.25: 13.8
+        1.375: 16.8
+        1.5: 20
+
+    Weight in table includes the weight of nuts.
+
+    Parameters
+    -------
+    length : float
+    diameter : float
+    no_of_washers : int
+
+    Returns
+    -------
+    Weight : float - the weight of the individual bolt
+    """
+
+    # Test if the inputs are in the table or if the formula must be used to calculate weight
+    if length in A325_bolt_weights.keys() and diameter in A325_bolt_weights[9].keys():
+        total_weight = A325_bolt_weights[length][diameter]
+
+    # Make sure user input is one of the available diameters
+    elif diameter not in A325_bolt_weights[9].keys() or length not in A325_bolt_weights.keys():
+        print('\nNon-existant diameter or length used, please use a value from the following list:')
+        print('\n\t0.5\n\t0.625\n\t0.75\n\t0.875\n\t1.0\n\t1.125\n\t1.25\n\t1.375\n\t1.5\n\n')
+
+        return None
+
+    # Calculates the weight of bolts longer than 9", uses 6" bolt to have all dias
+    elif diameter in A325_bolt_weights[9].keys() and length > max(A325_bolt_weights.keys()):
+        length_adder = {
+            0.5: 5.5,
+            0.625: 8.6,
+            0.75: 12.4,
+            0.875: 16.9,
+            1.0: 22.1,
+            1.125: 28,
+            1.25: 34.4,
+            1.375: 42.5,
+            1.5: 49.7
+        }
+
+        added_length = length - 6
+        total_weight = A325_bolt_weights[6][diameter] + added_length * length_adder[diameter]
+
+    # Adds washer weight if no of washers > 0
+    for washer in range(0, no_of_washers, 1):
+        washer_weight = {
+            0.5: 2.1,
+            0.625: 3.6,
+            0.75: 4.8,
+            0.875: 7,
+            1.0: 9.4,
+            1.125: 11.3,
+            1.25: 13.8,
+            1.375: 16.8,
+            1.5: 20,
+        }
+
+        total_weight = total_weight + washer_weight[diameter]
+
+    return round((total_weight / 100), 3) * units.lbs
+
+
 if __name__ == '__main__':
     import doctest
     doctest.testmod()
```

### Comparing `civilpy-0.0.78/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.79/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.78/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.79/src/civilpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.78
+Version: 0.0.79
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.78 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.79 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Environment :: Console :: Curses
```

### Comparing `civilpy-0.0.78/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.79/src/civilpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,10 +30,12 @@
 src/civilpy/state/ohio/snbi.py
 src/civilpy/structural/__init__.py
 src/civilpy/structural/arema.py
 src/civilpy/structural/beam_bending.py
 src/civilpy/structural/midas.py
 src/civilpy/structural/rail_tpg_design.py
 src/civilpy/structural/steel.py
+src/civilpy/structural/res/__init__.py
+src/civilpy/structural/res/definitions.py
 src/civilpy/transportation/__init__.py
 src/civilpy/water_resources/__init__.py
 src/civilpy/water_resources/hydraulics.py
```

### Comparing `civilpy-0.0.78/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.79/src/civilpy.egg-info/requires.txt`

 * *Files identical despite different names*

