# Comparing `tmp/HSR-0.1.5.tar.gz` & `tmp/HSR-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HSR-0.1.5.tar", last modified: Tue Apr  9 12:36:46 2024, max compression
+gzip compressed data, was "HSR-0.1.6.tar", last modified: Wed Apr 10 11:05:15 2024, max compression
```

## Comparing `HSR-0.1.5.tar` & `HSR-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.459101 HSR-0.1.5/
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.345162 HSR-0.1.5/HSR/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/hsr_cli.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 HSR-0.1.5/HSR/pca_transform.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 HSR-0.1.5/HSR/pre_processing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 HSR-0.1.5/HSR/similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/utils.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-09 12:36:17.000000 HSR-0.1.5/HSR/version.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.456802 HSR-0.1.5/HSR.egg-info/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      615 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/SOURCES.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/dependency_links.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/entry_points.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/requires.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       10 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/top_level.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 HSR-0.1.5/LICENSE
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 HSR-0.1.5/MANIFEST.in
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-09 12:36:46.457781 HSR-0.1.5/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 HSR-0.1.5/README.md
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-09 12:36:46.459242 HSR-0.1.5/setup.cfg
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      990 2024-03-20 12:38:27.000000 HSR-0.1.5/setup.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.455278 HSR-0.1.5/tests/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 HSR-0.1.5/tests/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 HSR-0.1.5/tests/test_fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 HSR-0.1.5/tests/test_pca.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 HSR-0.1.5/tests/test_preprocessing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 HSR-0.1.5/tests/test_similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 HSR-0.1.5/tests/test_utils.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 11:05:15.681684 HSR-0.1.6/
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 11:05:15.668992 HSR-0.1.6/HSR/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 HSR-0.1.6/HSR/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 HSR-0.1.6/HSR/fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 HSR-0.1.6/HSR/hsr_cli.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 HSR-0.1.6/HSR/pca_transform.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 HSR-0.1.6/HSR/pre_processing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 HSR-0.1.6/HSR/similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 HSR-0.1.6/HSR/utils.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-10 11:03:55.000000 HSR-0.1.6/HSR/version.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 11:05:15.679479 HSR-0.1.6/HSR.egg-info/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-10 11:05:15.000000 HSR-0.1.6/HSR.egg-info/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      615 2024-04-10 11:05:15.000000 HSR-0.1.6/HSR.egg-info/SOURCES.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-10 11:05:15.000000 HSR-0.1.6/HSR.egg-info/dependency_links.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-10 11:05:15.000000 HSR-0.1.6/HSR.egg-info/entry_points.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-10 11:05:15.000000 HSR-0.1.6/HSR.egg-info/requires.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        4 2024-04-10 11:05:15.000000 HSR-0.1.6/HSR.egg-info/top_level.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 HSR-0.1.6/LICENSE
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 HSR-0.1.6/MANIFEST.in
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-10 11:05:15.680677 HSR-0.1.6/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 HSR-0.1.6/README.md
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-10 11:05:15.681829 HSR-0.1.6/setup.cfg
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1018 2024-04-10 11:03:44.000000 HSR-0.1.6/setup.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 11:05:15.678418 HSR-0.1.6/tests/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 HSR-0.1.6/tests/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 HSR-0.1.6/tests/test_fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 HSR-0.1.6/tests/test_pca.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 HSR-0.1.6/tests/test_preprocessing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 HSR-0.1.6/tests/test_similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 HSR-0.1.6/tests/test_utils.py
```

### Comparing `HSR-0.1.5/HSR/fingerprint.py` & `HSR-0.1.6/HSR/fingerprint.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/HSR/hsr_cli.py` & `HSR-0.1.6/HSR/hsr_cli.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/HSR/pca_transform.py` & `HSR-0.1.6/HSR/pca_transform.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/HSR/pre_processing.py` & `HSR-0.1.6/HSR/pre_processing.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/HSR/similarity.py` & `HSR-0.1.6/HSR/similarity.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/HSR/utils.py` & `HSR-0.1.6/HSR/utils.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/HSR.egg-info/PKG-INFO` & `HSR-0.1.6/HSR.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSR
-Version: 0.1.5
+Version: 0.1.6
 Author: Marcello Costamagna
 License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
```

### Comparing `HSR-0.1.5/HSR.egg-info/SOURCES.txt` & `HSR-0.1.6/HSR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/LICENSE` & `HSR-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/PKG-INFO` & `HSR-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSR
-Version: 0.1.5
+Version: 0.1.6
 Author: Marcello Costamagna
 License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
```

### Comparing `HSR-0.1.5/README.md` & `HSR-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/setup.py` & `HSR-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     name="HSR",
     version=__version__,
     author="Marcello Costamagna", 
     license="AGPL-3.0",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         "numpy",
         "scipy",
         "rdkit"
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `HSR-0.1.5/tests/test_fingerprint.py` & `HSR-0.1.6/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/tests/test_pca.py` & `HSR-0.1.6/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/tests/test_preprocessing.py` & `HSR-0.1.6/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/tests/test_similarity.py` & `HSR-0.1.6/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.5/tests/test_utils.py` & `HSR-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

