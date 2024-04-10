# Comparing `tmp/nifti2dicom-1.2.1.tar.gz` & `tmp/nifti2dicom-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti2dicom-1.2.1.tar", last modified: Wed Apr 10 12:44:07 2024, max compression
+gzip compressed data, was "nifti2dicom-1.2.2.tar", last modified: Wed Apr 10 12:48:25 2024, max compression
```

## Comparing `nifti2dicom-1.2.1.tar` & `nifti2dicom-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/nifti2dicom/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    30023 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/nifti2dicom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:48:25.390395 nifti2dicom-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 12:48:25.390395 nifti2dicom-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:48:25.390395 nifti2dicom-1.2.2/nifti2dicom/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/nifti2dicom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/nifti2dicom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30019 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/nifti2dicom/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/nifti2dicom/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/nifti2dicom/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:48:25.390395 nifti2dicom-1.2.2/nifti2dicom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 12:48:25.000000 nifti2dicom-1.2.2/nifti2dicom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 12:48:25.000000 nifti2dicom-1.2.2/nifti2dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:48:25.000000 nifti2dicom-1.2.2/nifti2dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 12:48:25.000000 nifti2dicom-1.2.2/nifti2dicom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 12:48:25.000000 nifti2dicom-1.2.2/nifti2dicom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 12:48:25.000000 nifti2dicom-1.2.2/nifti2dicom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:48:25.390395 nifti2dicom-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 12:48:19.000000 nifti2dicom-1.2.2/setup.py
```

### Comparing `nifti2dicom-1.2.1/LICENSE` & `nifti2dicom-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.1/PKG-INFO` & `nifti2dicom-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.2.1/README.md` & `nifti2dicom-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.1/nifti2dicom/constants.py` & `nifti2dicom-1.2.2/nifti2dicom/constants.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.1/nifti2dicom/converter.py` & `nifti2dicom-1.2.2/nifti2dicom/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,17 +430,17 @@
             for idx, future in enumerate(futures):
                 future.result()
                 progress.update(task, advance=1,
                                 description=f"[white] Writing DICOM slices... [{idx + 1}/{total_slices}]")
 
 
 def nifti_to_dicom_with_resampling(nifti_image_path: str, original_dicom_directory: str, dicom_output_directory: str,
-                                     spatial_info_dicom_directory: str,
+                                   spatial_info_dicom_directory: str,
                                    series_description: str = "converted by nifti2dicom",
-                                     verbose=False) -> None:
+                                   verbose=False) -> None:
     """
     Convert a nifti image which has a different size/spatial information to its original dicom series.
     :param nifti_image_path: Path to the NIFTI file.
     :type nifti_image_path: str
     :param original_dicom_directory: Path to the directory containing the reference DICOM series.
     :type original_dicom_directory: str
     :param dicom_output_directory: Path to the directory where the converted DICOM files will be saved.
```

### Comparing `nifti2dicom-1.2.1/nifti2dicom/display.py` & `nifti2dicom-1.2.2/nifti2dicom/display.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.1/nifti2dicom/viewer.py` & `nifti2dicom-1.2.2/nifti2dicom/viewer.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.1/nifti2dicom.egg-info/PKG-INFO` & `nifti2dicom-1.2.2/nifti2dicom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.2.1/setup.py` & `nifti2dicom-1.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='nifti2dicom',
-    version='1.2.1',
+    version='1.2.2',
     packages=find_packages(),
     install_requires=[
         'pydicom',
         'nibabel',
         'numpy',
         'emoji',
         'rich',
```

