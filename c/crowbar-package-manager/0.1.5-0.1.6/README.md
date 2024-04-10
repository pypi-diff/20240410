# Comparing `tmp/crowbar_package_manager-0.1.5.tar.gz` & `tmp/crowbar_package_manager-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.5.tar", last modified: Tue Apr  9 23:49:55 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.6.tar", last modified: Wed Apr 10 00:12:47 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.5.tar` & `crowbar_package_manager-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:49:55.481610 crowbar_package_manager-0.1.5/
--rw-r--r--   0 coryfitz   (501) staff       (20)     1005 2024-04-09 23:49:55.481500 crowbar_package_manager-0.1.5/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      896 2024-04-09 23:41:35.000000 crowbar_package_manager-0.1.5/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:49:55.480510 crowbar_package_manager-0.1.5/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.5/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     7210 2024-04-09 23:19:15.000000 crowbar_package_manager-0.1.5/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:49:55.481329 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)     1005 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-09 23:49:55.481655 crowbar_package_manager-0.1.5/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      571 2024-04-09 23:49:38.000000 crowbar_package_manager-0.1.5/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-10 00:12:47.008301 crowbar_package_manager-0.1.6/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1005 2024-04-10 00:12:47.008180 crowbar_package_manager-0.1.6/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      896 2024-04-09 23:41:35.000000 crowbar_package_manager-0.1.6/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-10 00:12:47.007065 crowbar_package_manager-0.1.6/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.6/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     7210 2024-04-09 23:19:15.000000 crowbar_package_manager-0.1.6/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-10 00:12:47.007973 crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1005 2024-04-10 00:12:46.000000 crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-10 00:12:46.000000 crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-10 00:12:46.000000 crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-10 00:12:46.000000 crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-10 00:12:46.000000 crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-10 00:12:47.008349 crowbar_package_manager-0.1.6/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      649 2024-04-10 00:12:25.000000 crowbar_package_manager-0.1.6/setup.py
```

### Comparing `crowbar_package_manager-0.1.5/PKG-INFO` & `crowbar_package_manager-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: crowbar_package_manager
-Version: 0.1.5
-Description-Content-Type: text/markdown
-
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
 
 ```
 crowbar install <package_name>
@@ -31,8 +26,8 @@
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
 ### conda support
 
-Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
+Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
```

### Comparing `crowbar_package_manager-0.1.5/README.md` & `crowbar_package_manager-0.1.6/crowbar_package_manager.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: crowbar-package-manager
+Version: 0.1.6
+Description-Content-Type: text/markdown
+
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
 
 ```
 crowbar install <package_name>
@@ -26,8 +31,8 @@
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
 ### conda support
 
-Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
+Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
```

### Comparing `crowbar_package_manager-0.1.5/crowbar/crowbar.py` & `crowbar_package_manager-0.1.6/crowbar/crowbar.py`

 * *Files identical despite different names*

### Comparing `crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/PKG-INFO` & `crowbar_package_manager-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crowbar-package-manager
-Version: 0.1.5
+Name: crowbar_package_manager
+Version: 0.1.6
 Description-Content-Type: text/markdown
 
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
```

### Comparing `crowbar_package_manager-0.1.5/setup.py` & `crowbar_package_manager-0.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='crowbar_package_manager',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'crowbar=crowbar:main',
             'cb=crowbar:main',
         ],
     },
+    summary = 'a local-first tool for managing python dependencies with pip',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This line is important for Markdown rendering on PyPI
 )
```

