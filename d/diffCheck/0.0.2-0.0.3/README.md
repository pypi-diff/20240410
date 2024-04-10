# Comparing `tmp/diffCheck-0.0.2.tar.gz` & `tmp/diffCheck-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffCheck-0.0.2.tar", last modified: Sun Apr  7 18:44:32 2024, max compression
+gzip compressed data, was "diffCheck-0.0.3.tar", last modified: Wed Apr 10 15:22:46 2024, max compression
```

## Comparing `diffCheck-0.0.2.tar` & `diffCheck-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 18:44:32.433028 diffCheck-0.0.2/
--rw-rw-rw-   0        0        0      806 2024-04-07 18:44:32.432521 diffCheck-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-07 14:57:49.000000 diffCheck-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 18:44:32.422495 diffCheck-0.0.2/diffCheck/
--rw-rw-rw-   0        0        0       21 2024-04-07 17:25:37.000000 diffCheck-0.0.2/diffCheck/__init__.py
--rw-rw-rw-   0        0        0     6574 2024-04-07 10:16:07.000000 diffCheck-0.0.2/diffCheck/df_geometries.py
--rw-rw-rw-   0        0        0      773 2024-04-07 10:17:05.000000 diffCheck-0.0.2/diffCheck/diffCheck_app.py
--rw-rw-rw-   0        0        0        0 2024-04-07 09:23:57.000000 diffCheck-0.0.2/diffCheck/joint_detector.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:44:32.431014 diffCheck-0.0.2/diffCheck.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-07 18:44:32.000000 diffCheck-0.0.2/diffCheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-07 18:44:32.000000 diffCheck-0.0.2/diffCheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 18:44:32.000000 diffCheck-0.0.2/diffCheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-07 18:44:32.000000 diffCheck-0.0.2/diffCheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 18:44:32.433028 diffCheck-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-07 17:25:35.000000 diffCheck-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:22:46.862109 diffCheck-0.0.3/
+-rw-rw-rw-   0        0        0      806 2024-04-10 15:22:46.861610 diffCheck-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-07 14:57:49.000000 diffCheck-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 15:22:46.839573 diffCheck-0.0.3/diffCheck/
+-rw-rw-rw-   0        0        0       21 2024-04-09 13:29:53.000000 diffCheck-0.0.3/diffCheck/__init__.py
+-rw-rw-rw-   0        0        0     9485 2024-04-10 15:13:00.000000 diffCheck-0.0.3/diffCheck/df_geometries.py
+-rw-rw-rw-   0        0        0     7622 2024-04-09 13:40:15.000000 diffCheck-0.0.3/diffCheck/df_joint_detector.py
+-rw-rw-rw-   0        0        0     4604 2024-04-08 14:43:34.000000 diffCheck-0.0.3/diffCheck/df_transformations.py
+-rw-rw-rw-   0        0        0     4166 2024-04-08 14:44:50.000000 diffCheck-0.0.3/diffCheck/df_util.py
+-rw-rw-rw-   0        0        0     1065 2024-04-10 15:14:55.000000 diffCheck-0.0.3/diffCheck/diffCheck_app.py
+-rw-rw-rw-   0        0        0      202 2024-04-10 11:03:44.000000 diffCheck-0.0.3/diffCheck/test.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:22:46.860109 diffCheck-0.0.3/diffCheck.egg-info/
+-rw-rw-rw-   0        0        0      806 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 15:22:46.862610 diffCheck-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-09 13:29:53.000000 diffCheck-0.0.3/setup.py
```

### Comparing `diffCheck-0.0.2/PKG-INFO` & `diffCheck-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.2/diffCheck.egg-info/PKG-INFO` & `diffCheck-0.0.3/diffCheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.2/setup.py` & `diffCheck-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='diffCheck',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     description='DiffCheck is a package to check the differences between two timber structures',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand',
     author_email='andrea.settimi@epfl.ch',
     url='https://github.com/diffCheckOrg/diffCheck',
```

