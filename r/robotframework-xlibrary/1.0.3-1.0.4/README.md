# Comparing `tmp/robotframework-xlibrary-1.0.3.tar.gz` & `tmp/robotframework-xlibrary-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-1.0.3.tar", last modified: Tue Apr  9 09:52:33 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-1.0.4.tar", last modified: Tue Apr  9 09:55:36 2024, max compression
```

## Comparing `robotframework-xlibrary-1.0.3.tar` & `robotframework-xlibrary-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1584 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-09 09:52:28.000000 robotframework-xlibrary-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/XLibrary/
--rw-rw-rw-   0        0        0     1792 2024-04-09 09:39:59.000000 robotframework-xlibrary-1.0.3/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-1.0.3/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 09:52:12.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.3/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     1584 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 09:52:33.000000 robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1584 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-09 09:54:07.000000 robotframework-xlibrary-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/XLibrary/
+-rw-rw-rw-   0        0        0     1792 2024-04-09 09:39:59.000000 robotframework-xlibrary-1.0.4/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-1.0.4/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 09:53:52.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.4/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     1584 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 09:55:36.000000 robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-1.0.3/PKG-INFO` & `robotframework-xlibrary-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 1.0.3
+Version: 1.0.4
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-1.0.3/README.md` & `robotframework-xlibrary-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-1.0.3/setup.py` & `robotframework-xlibrary-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="1.0.3",
+    version="1.0.4",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Test Library for robotframework-xlibrary",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-1.0.3/src/XLibrary/__init__.py` & `robotframework-xlibrary-1.0.4/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-1.0.3/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-1.0.4/src/XLibrary/submodule1/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 1.0.3
+Version: 1.0.4
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-1.0.3/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-1.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

