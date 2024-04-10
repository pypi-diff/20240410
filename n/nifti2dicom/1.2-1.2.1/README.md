# Comparing `tmp/nifti2dicom-1.2.tar.gz` & `tmp/nifti2dicom-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti2dicom-1.2.tar", last modified: Wed Apr 10 11:43:47 2024, max compression
+gzip compressed data, was "nifti2dicom-1.2.1.tar", last modified: Wed Apr 10 12:44:07 2024, max compression
```

## Comparing `nifti2dicom-1.2.tar` & `nifti2dicom-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:43:47.054737 nifti2dicom-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 11:43:42.000000 nifti2dicom-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-10 11:43:47.054737 nifti2dicom-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-10 11:43:42.000000 nifti2dicom-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:43:47.050737 nifti2dicom-1.2/nifti2dicom/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:43:47.054737 nifti2dicom-1.2/nifti2dicom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:43:47.054737 nifti2dicom-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-10 11:43:42.000000 nifti2dicom-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/nifti2dicom/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30023 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/nifti2dicom/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/nifti2dicom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 12:44:07.000000 nifti2dicom-1.2.1/nifti2dicom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:44:07.834982 nifti2dicom-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 12:44:00.000000 nifti2dicom-1.2.1/setup.py
```

### Comparing `nifti2dicom-1.2/LICENSE` & `nifti2dicom-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2/PKG-INFO` & `nifti2dicom-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.2
+Version: 1.2.1
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.2/README.md` & `nifti2dicom-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2/nifti2dicom/constants.py` & `nifti2dicom-1.2.1/nifti2dicom/constants.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2/nifti2dicom/converter.py` & `nifti2dicom-1.2.1/nifti2dicom/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,25 +431,28 @@
                 future.result()
                 progress.update(task, advance=1,
                                 description=f"[white] Writing DICOM slices... [{idx + 1}/{total_slices}]")
 
 
 def nifti_to_dicom_with_resampling(nifti_image_path: str, original_dicom_directory: str, dicom_output_directory: str,
                                      spatial_info_dicom_directory: str,
+                                   series_description: str = "converted by nifti2dicom",
                                      verbose=False) -> None:
     """
     Convert a nifti image which has a different size/spatial information to its original dicom series.
     :param nifti_image_path: Path to the NIFTI file.
     :type nifti_image_path: str
     :param original_dicom_directory: Path to the directory containing the reference DICOM series.
     :type original_dicom_directory: str
     :param dicom_output_directory: Path to the directory where the converted DICOM files will be saved.
     :type dicom_output_directory: str
     :param spatial_info_dicom_directory: Path to the directory containing the DICOM series to extract spatial tags.
     :type spatial_info_dicom_directory: str
+    :param series_description: Series description to be added to the DICOM header.
+    :type series_description: str
     :param verbose: If True, print messages during the process
     :type verbose: bool
     """
 
     # Ensure output directory exists
     if not os.path.exists(dicom_output_directory):
         os.makedirs(dicom_output_directory)
@@ -497,22 +500,22 @@
     vprint(f' {ANSI_GREEN}* Saving DICOM series to: {dicom_output_directory}{ANSI_RESET}', verbose=verbose)
     reader = sitk.ImageSeriesReader()
     dicom_names = reader.GetGDCMSeriesFileNames(original_dicom_directory)
     dicom_slices = [pydicom.dcmread(f) for f in dicom_names]
 
     total_slices = len(dicom_slices)
     with Progress() as progress:
-        task = progress.add_task("[cyan] Writing DICOM slices:", total=total_slices)
+        task = progress.add_task("[cyan] Writing DICOM slices...", total=total_slices)
 
         def process_slice(idx, slice, output_dir, nifti_img):
             slice.ImagePositionPatient = list(nifti_img.TransformIndexToPhysicalPoint((0, 0, idx)))
             image_array_slice = sitk.GetArrayFromImage(nifti_img)[idx]
             filename = f"slice_{idx}.dcm"
-            save_slice(slice, image_array_slice, "converted by nifti2dicom", filename, output_dir, slice.Modality)
-            progress.update(task, advance=1)
+            save_slice(slice, image_array_slice, series_description, filename, output_dir, slice.Modality)
+            progress.update(task, advance=1, description=f"[white] Writing RGB DICOM slices... [{idx}/{total_slices}]")
 
         with ThreadPoolExecutor() as executor:
             for idx, slice in enumerate(dicom_slices):
                 executor.submit(process_slice, idx, slice, dicom_output_directory, resampled_nifti_img)
 
 
 def save_dicom_from_nifti_seg(nifti_file: str, ref_dicom_series_dir: str, output_path: str, ORGAN_INDEX: dict,
```

### Comparing `nifti2dicom-1.2/nifti2dicom/display.py` & `nifti2dicom-1.2.1/nifti2dicom/display.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2/nifti2dicom/viewer.py` & `nifti2dicom-1.2.1/nifti2dicom/viewer.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2/nifti2dicom.egg-info/PKG-INFO` & `nifti2dicom-1.2.1/nifti2dicom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.2
+Version: 1.2.1
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.2/setup.py` & `nifti2dicom-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='nifti2dicom',
-    version='1.2',
+    version='1.2.1',
     packages=find_packages(),
     install_requires=[
         'pydicom',
         'nibabel',
         'numpy',
         'emoji',
         'rich',
```

