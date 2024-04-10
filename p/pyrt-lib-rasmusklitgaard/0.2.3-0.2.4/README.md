# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.2.3.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.2.3.tar", last modified: Tue Apr  9 10:33:52 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.2.4.tar", last modified: Wed Apr 10 12:39:04 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.2.3.tar` & `pyrt_lib_rasmusklitgaard-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 10:33:52.112158 pyrt_lib_rasmusklitgaard-0.2.3/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.3/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 10:33:52.112158 pyrt_lib_rasmusklitgaard-0.2.3/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.3/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-09 10:32:58.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 10:33:52.108158 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      126 2024-04-09 08:44:27.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-09 10:33:50.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-09 10:33:50.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12096 2024-04-09 10:33:50.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-09 10:33:50.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-09 10:33:50.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 10:33:52.108158 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 10:33:52.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-09 10:33:52.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-09 10:33:52.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-09 10:33:52.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-09 10:33:52.000000 pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-09 10:33:52.112158 pyrt_lib_rasmusklitgaard-0.2.3/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 12:39:04.538967 pyrt_lib_rasmusklitgaard-0.2.4/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.4/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-10 12:39:04.538967 pyrt_lib_rasmusklitgaard-0.2.4/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.4/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-10 12:38:58.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 12:39:04.538967 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      126 2024-04-09 08:44:27.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-10 12:39:02.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-10 12:39:02.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12115 2024-04-10 12:39:02.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-10 12:39:02.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-10 12:39:02.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 12:39:04.538967 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-10 12:39:04.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-10 12:39:04.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-10 12:39:04.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-10 12:39:04.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-10 12:39:04.000000 pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-10 12:39:04.538967 pyrt_lib_rasmusklitgaard-0.2.4/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/LICENSE` & `pyrt_lib_rasmusklitgaard-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.2.3
+Version: 0.2.4
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/README.md` & `pyrt_lib_rasmusklitgaard-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.2.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 
 	if not absoluteVolume:
 		original_v75gy = len(dose_array_in_structure[dose_array_in_structure>=75]) / len(dose_array_in_structure) * 100
 	else:
 		original_v75gy = len(dose_array_in_structure[dose_array_in_structure>=75]) * voxel_volume / 1000
 		
 	return original_v75gy
-def calculate_relative_change_in_v75gy_when_applying_lwd(patient: Patient, structure_of_interest, dose_threshold):
+def calculate_relative_change_in_vXgy_when_applying_lwd(patient: Patient, structure_of_interest, dose_threshold):
 	flk_dicom_paths = [s for s in patient.list_of_dicom_file_paths if s.split("/")[-1][:3] == "FLK"]
 	flk_biodose_dicom_path = [s for s in flk_dicom_paths if s.split("/")[-1][:12] == "FLK_Bio-dose"][0]
 	flk_letd_dicom_path = [s for s in flk_dicom_paths if s.split("/")[-1][:8] == "FLK_LETd"][0]
 
 	flk_biodose_dicom = pd.read_file(flk_biodose_dicom_path)
 	flk_letd_dicom = pd.read_file(flk_letd_dicom_path)
 
@@ -251,18 +251,18 @@
 	letd_array_in_structure = letdgrid[structure_indices]
 	dose_array_in_structure = dosegrid[structure_indices]
 
 
 	lwd_rbe = 1+0.055 * letd_array_in_structure
 	lwd_dose_in_structure = lwd_rbe / 1.1 * dose_array_in_structure
 
-	original_v75gy = len(dose_array_in_structure[dose_array_in_structure>=75]) / len(dose_array_in_structure)
-	lwd_rbe_v75gy = len(lwd_dose_in_structure[lwd_dose_in_structure>=75]) / len(lwd_dose_in_structure)
+	original_vXgy = len(dose_array_in_structure[dose_array_in_structure>=dose_threshold]) / len(dose_array_in_structure)
+	lwd_rbe_vXgy = len(lwd_dose_in_structure[lwd_dose_in_structure>=dose_threshold]) / len(lwd_dose_in_structure)
 
-	return lwd_rbe_v75gy / original_v75gy * 100
+	return lwd_rbe_vXgy / original_vXgy * 100
 
 def calculate_let_percentage_over_threshold_rectum(patient : Patient, structure_of_interest, dose_threshold, percentage) -> float:
 	flk_dicom_paths = [s for s in patient.list_of_dicom_file_paths if s.split("/")[-1][:3] == "FLK"]
 	flk_biodose_dicom_path = [s for s in flk_dicom_paths if s.split("/")[-1][:12] == "FLK_Bio-dose"][0]
 	flk_letd_dicom_path = [s for s in flk_dicom_paths if s.split("/")[-1][:8] == "FLK_LETd"][0]
 
 	flk_biodose_dicom = pd.read_file(flk_biodose_dicom_path)
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.2.3
+Version: 0.2.4
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.2.4/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

