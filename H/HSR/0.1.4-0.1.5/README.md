# Comparing `tmp/HSR-0.1.4.tar.gz` & `tmp/HSR-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HSR-0.1.4.tar", last modified: Thu Mar  7 10:19:22 2024, max compression
+gzip compressed data, was "HSR-0.1.5.tar", last modified: Tue Apr  9 12:36:46 2024, max compression
```

## Comparing `HSR-0.1.4.tar` & `HSR-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-03-07 10:19:22.516579 HSR-0.1.4/
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-03-07 10:19:22.504849 HSR-0.1.4/HSR/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 HSR-0.1.4/HSR/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 HSR-0.1.4/HSR/fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 HSR-0.1.4/HSR/hsr_cli.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 HSR-0.1.4/HSR/pca_transform.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 HSR-0.1.4/HSR/pre_processing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-02-21 11:44:17.000000 HSR-0.1.4/HSR/similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 HSR-0.1.4/HSR/utils.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-03-07 10:15:29.000000 HSR-0.1.4/HSR/version.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-03-07 10:19:22.515208 HSR-0.1.4/HSR.egg-info/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1956 2024-03-07 10:19:22.000000 HSR-0.1.4/HSR.egg-info/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      605 2024-03-07 10:19:22.000000 HSR-0.1.4/HSR.egg-info/SOURCES.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-03-07 10:19:22.000000 HSR-0.1.4/HSR.egg-info/dependency_links.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-03-07 10:19:22.000000 HSR-0.1.4/HSR.egg-info/entry_points.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-03-07 10:19:22.000000 HSR-0.1.4/HSR.egg-info/requires.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       10 2024-03-07 10:19:22.000000 HSR-0.1.4/HSR.egg-info/top_level.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 HSR-0.1.4/LICENSE
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       15 2024-02-21 11:44:17.000000 HSR-0.1.4/MANIFEST.in
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1956 2024-03-07 10:19:22.515989 HSR-0.1.4/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-03-07 10:19:22.516672 HSR-0.1.4/setup.cfg
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1016 2024-02-28 13:05:06.000000 HSR-0.1.4/setup.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-03-07 10:19:22.514568 HSR-0.1.4/tests/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        0 2024-02-21 11:44:17.000000 HSR-0.1.4/tests/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-02-21 11:44:17.000000 HSR-0.1.4/tests/test_fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-02-21 11:44:17.000000 HSR-0.1.4/tests/test_pca.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-02-21 11:44:17.000000 HSR-0.1.4/tests/test_preprocessing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-02-21 11:44:17.000000 HSR-0.1.4/tests/test_similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-02-21 11:44:17.000000 HSR-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.459101 HSR-0.1.5/
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.345162 HSR-0.1.5/HSR/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/hsr_cli.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 HSR-0.1.5/HSR/pca_transform.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 HSR-0.1.5/HSR/pre_processing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 HSR-0.1.5/HSR/similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 HSR-0.1.5/HSR/utils.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-09 12:36:17.000000 HSR-0.1.5/HSR/version.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.456802 HSR-0.1.5/HSR.egg-info/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      615 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/SOURCES.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/dependency_links.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/entry_points.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/requires.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       10 2024-04-09 12:36:45.000000 HSR-0.1.5/HSR.egg-info/top_level.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 HSR-0.1.5/LICENSE
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 HSR-0.1.5/MANIFEST.in
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-09 12:36:46.457781 HSR-0.1.5/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 HSR-0.1.5/README.md
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-09 12:36:46.459242 HSR-0.1.5/setup.cfg
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      990 2024-03-20 12:38:27.000000 HSR-0.1.5/setup.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-09 12:36:46.455278 HSR-0.1.5/tests/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 HSR-0.1.5/tests/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 HSR-0.1.5/tests/test_fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 HSR-0.1.5/tests/test_pca.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 HSR-0.1.5/tests/test_preprocessing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 HSR-0.1.5/tests/test_similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 HSR-0.1.5/tests/test_utils.py
```

### Comparing `HSR-0.1.4/HSR/fingerprint.py` & `HSR-0.1.5/HSR/fingerprint.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/HSR/hsr_cli.py` & `HSR-0.1.5/HSR/hsr_cli.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/HSR/pca_transform.py` & `HSR-0.1.5/HSR/pca_transform.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/HSR/pre_processing.py` & `HSR-0.1.5/HSR/pre_processing.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/HSR/similarity.py` & `HSR-0.1.5/HSR/similarity.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/HSR/utils.py` & `HSR-0.1.5/HSR/utils.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/HSR.egg-info/PKG-INFO` & `HSR-0.1.5/HSR.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: HSR
-Version: 0.1.4
+Version: 0.1.5
 Author: Marcello Costamagna
-License: GNU Affero General Public License
+License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
 
 # Hyper Shape recognition (HSR): a general framework for moment-based similarity measures
```

### Comparing `HSR-0.1.4/HSR.egg-info/SOURCES.txt` & `HSR-0.1.5/HSR.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+README.md
 setup.py
 HSR/__init__.py
 HSR/fingerprint.py
 HSR/hsr_cli.py
 HSR/pca_transform.py
 HSR/pre_processing.py
 HSR/similarity.py
```

### Comparing `HSR-0.1.4/LICENSE` & `HSR-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/PKG-INFO` & `HSR-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: HSR
-Version: 0.1.4
+Version: 0.1.5
 Author: Marcello Costamagna
-License: GNU Affero General Public License
+License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
 
 # Hyper Shape recognition (HSR): a general framework for moment-based similarity measures
```

### Comparing `HSR-0.1.4/setup.py` & `HSR-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="HSR",
     version=__version__,
     author="Marcello Costamagna", 
-    license="GNU Affero General Public License", 
+    license="AGPL-3.0",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "rdkit"
```

### Comparing `HSR-0.1.4/tests/test_fingerprint.py` & `HSR-0.1.5/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/tests/test_pca.py` & `HSR-0.1.5/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/tests/test_preprocessing.py` & `HSR-0.1.5/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/tests/test_similarity.py` & `HSR-0.1.5/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `HSR-0.1.4/tests/test_utils.py` & `HSR-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

