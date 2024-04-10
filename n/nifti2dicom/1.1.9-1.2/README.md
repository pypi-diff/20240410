# Comparing `tmp/nifti2dicom-1.1.9.tar.gz` & `tmp/nifti2dicom-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti2dicom-1.1.9.tar", last modified: Mon Mar 25 10:26:16 2024, max compression
+gzip compressed data, was "nifti2dicom-1.2.tar", last modified: Wed Apr 10 11:43:47 2024, max compression
```

## Comparing `nifti2dicom-1.1.9.tar` & `nifti2dicom-1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:26:16.146805 nifti2dicom-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-03-25 10:26:16.146805 nifti2dicom-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:26:16.146805 nifti2dicom-1.1.9/nifti2dicom/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/nifti2dicom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/nifti2dicom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/nifti2dicom/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/nifti2dicom/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:26:16.146805 nifti2dicom-1.1.9/nifti2dicom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-03-25 10:26:16.000000 nifti2dicom-1.1.9/nifti2dicom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-25 10:26:16.000000 nifti2dicom-1.1.9/nifti2dicom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:26:16.000000 nifti2dicom-1.1.9/nifti2dicom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-25 10:26:16.000000 nifti2dicom-1.1.9/nifti2dicom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 10:26:16.000000 nifti2dicom-1.1.9/nifti2dicom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 10:26:16.000000 nifti2dicom-1.1.9/nifti2dicom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 10:26:16.146805 nifti2dicom-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-25 10:26:11.000000 nifti2dicom-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:43:47.054737 nifti2dicom-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 11:43:42.000000 nifti2dicom-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-10 11:43:47.054737 nifti2dicom-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-10 11:43:42.000000 nifti2dicom-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:43:47.050737 nifti2dicom-1.2/nifti2dicom/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 11:43:42.000000 nifti2dicom-1.2/nifti2dicom/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:43:47.054737 nifti2dicom-1.2/nifti2dicom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 11:43:47.000000 nifti2dicom-1.2/nifti2dicom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:43:47.054737 nifti2dicom-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-10 11:43:42.000000 nifti2dicom-1.2/setup.py
```

### Comparing `nifti2dicom-1.1.9/LICENSE` & `nifti2dicom-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.1.9/PKG-INFO` & `nifti2dicom-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.1.9
+Version: 1.2
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.1.9/README.md` & `nifti2dicom-1.2/README.md`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.1.9/nifti2dicom/constants.py` & `nifti2dicom-1.2/nifti2dicom/constants.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.1.9/nifti2dicom/converter.py` & `nifti2dicom-1.2/nifti2dicom/converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,14 +31,77 @@
 from pydicom.dataset import Dataset, FileMetaDataset
 from pydicom.filewriter import write_file
 from pydicom.sr.codedict import codes
 from pydicom.uid import ExplicitVRLittleEndian, generate_uid
 from rich.progress import Progress, track
 
 
+def load_image(path, image_type='dicom'):
+    """
+    Loads medical image from the specified path.
+
+    Args:
+        path (str): Path to the image file or directory.
+        image_type (str): Type of the image, either 'dicom' or 'nifti'.
+
+    Returns:
+        image (SimpleITK.Image): The loaded image.
+    """
+    if image_type == 'dicom':
+        reader = sitk.ImageSeriesReader()
+        dicom_names = reader.GetGDCMSeriesFileNames(path)
+        reader.SetFileNames(dicom_names)
+        image = reader.Execute()
+    elif image_type == 'nifti':
+        image = sitk.ReadImage(path)
+    else:
+        raise ValueError("Unsupported image type. Use 'dicom' or 'nifti'.")
+    return image
+
+def resample_image_SimpleITK(sitk_image: sitk.Image, interpolation: str,
+                             output_spacing: tuple = (1.5, 1.5, 1.5),
+                             output_size: tuple = None) -> sitk.Image:
+    """
+    Resamples an image to a new spacing using SimpleITK.
+
+    :param sitk_image: The input image.
+    :type sitk_image: SimpleITK.Image
+    :param interpolation: The interpolation method to use. Supported methods are 'nearest', 'linear', and 'bspline'.
+    :type interpolation: str
+    :param output_spacing: The new spacing to use. Default is (1.5, 1.5, 1.5).
+    :type output_spacing: tuple
+    :param output_size: The new size to use. Default is None.
+    :type output_size: tuple
+    :return: The resampled image as SimpleITK.Image.
+    :rtype: SimpleITK.Image
+    :raises ValueError: If the interpolation method is not supported.
+    """
+    if interpolation == 'nearest':
+        interpolation_method = sitk.sitkNearestNeighbor
+    elif interpolation == 'linear':
+        interpolation_method = sitk.sitkLinear
+    elif interpolation == 'bspline':
+        interpolation_method = sitk.sitkBSpline
+    else:
+        raise ValueError('The interpolation method is not supported.')
+
+    desired_spacing = np.array(output_spacing).astype(np.float64)
+    if output_size is None:
+        input_size = sitk_image.GetSize()
+        input_spacing = sitk_image.GetSpacing()
+        output_size = [round(input_size[i] * (input_spacing[i] / output_spacing[i])) for i in
+                       range(len(input_size))]
+
+    # Interpolation:
+    resampled_sitk_image = sitk.Resample(sitk_image, output_size, sitk.Transform(), interpolation_method,
+                                         sitk_image.GetOrigin(), desired_spacing,
+                                         sitk_image.GetDirection(), 0.0, sitk_image.GetPixelIDValue())
+
+    return resampled_sitk_image
+
 def create_rgb_dicom_from_slice(slice_array, series_tag_values, reference_metadata, instance_number):
     """
     Create a DICOM dataset from an RGB slice.
 
     :param slice_array: Numpy array of the RGB slice.
     :param series_tag_values: Dictionary of DICOM tag values.
     :param reference_metadata: Reference metadata from the DICOM series.
@@ -90,15 +153,14 @@
     ds.HighBit = 7
 
     # Convert the numpy array to bytes and assign to PixelData
     ds.PixelData = slice_array.tobytes()
 
     # Additional metadata
     ds.ImageType = ["DERIVED", "SECONDARY"]
-    ds.ConversionType = "WSD"
     ds.InstanceCreationDate = time.strftime("%Y%m%d")
     ds.InstanceCreationTime = time.strftime("%H%M%S")
     ds.file_meta.TransferSyntaxUID = ExplicitVRLittleEndian
 
     return ds
 
 
@@ -367,14 +429,96 @@
 
             for idx, future in enumerate(futures):
                 future.result()
                 progress.update(task, advance=1,
                                 description=f"[white] Writing DICOM slices... [{idx + 1}/{total_slices}]")
 
 
+def nifti_to_dicom_with_resampling(nifti_image_path: str, original_dicom_directory: str, dicom_output_directory: str,
+                                     spatial_info_dicom_directory: str,
+                                     verbose=False) -> None:
+    """
+    Convert a nifti image which has a different size/spatial information to its original dicom series.
+    :param nifti_image_path: Path to the NIFTI file.
+    :type nifti_image_path: str
+    :param original_dicom_directory: Path to the directory containing the reference DICOM series.
+    :type original_dicom_directory: str
+    :param dicom_output_directory: Path to the directory where the converted DICOM files will be saved.
+    :type dicom_output_directory: str
+    :param spatial_info_dicom_directory: Path to the directory containing the DICOM series to extract spatial tags.
+    :type spatial_info_dicom_directory: str
+    :param verbose: If True, print messages during the process
+    :type verbose: bool
+    """
+
+    # Ensure output directory exists
+    if not os.path.exists(dicom_output_directory):
+        os.makedirs(dicom_output_directory)
+
+    vprint(verbose=verbose, end='\n')
+    vprint(f'{ANSI_VIOLET} {emoji.emojize(":magnifying_glass_tilted_left:")} IDENTIFIED DATASETS:{ANSI_RESET}',
+           verbose=verbose, end='\n')
+
+    # Load the original DICOM series and display its geometry information
+    vprint(f' {ANSI_GREEN}* Original DICOM series directory: {original_dicom_directory}{ANSI_RESET}', verbose=verbose)
+    vprint(f' {ANSI_GREEN} - Extract geometry information from: {spatial_info_dicom_directory}{ANSI_RESET}',
+           verbose=verbose)
+    native_dicom_img = load_image(original_dicom_directory, image_type='dicom')
+    native_dicom_img_size = native_dicom_img.GetSize()
+    native_dicom_voxel_size = native_dicom_img.GetSpacing()
+    native_dicom_origin = native_dicom_img.GetOrigin()
+    native_dicom_direction = native_dicom_img.GetDirection()
+    vprint(f' {ANSI_GREEN} - Native DICOM size: {native_dicom_img_size}{ANSI_RESET}', verbose=verbose)
+    vprint(f' {ANSI_GREEN} - Native DICOM voxel size: {native_dicom_voxel_size}{ANSI_RESET}', verbose=verbose)
+    vprint(f' {ANSI_GREEN} - Native DICOM origin: {native_dicom_origin}{ANSI_RESET}', verbose=verbose)
+    vprint(f' {ANSI_GREEN} - Native DICOM direction: {native_dicom_direction}{ANSI_RESET}', verbose=verbose)
+
+    # Load the reference DICOM series to extract the critical spatial tags
+    vprint(f' {ANSI_GREEN}* Loading reference DICOM series to extract spatial tags: {spatial_info_dicom_directory}{ANSI_RESET}',
+           verbose=verbose)
+    ref_dicom_img = load_image(spatial_info_dicom_directory, image_type='dicom')
+    ref_dicom_origin = ref_dicom_img.GetOrigin()
+    ref_dicom_direction = ref_dicom_img.GetDirection()
+    vprint(f' {ANSI_GREEN} - Reference Origin: {ref_dicom_origin}{ANSI_RESET}', verbose=verbose)
+    vprint(f' {ANSI_GREEN} - Reference Direction: {ref_dicom_direction}{ANSI_RESET}', verbose=verbose)
+
+    # Load the NIFTI image using SimpleITK and resample it to match its corresponding DICOM series
+    nifti_img = load_image(nifti_image_path, image_type='nifti')
+    flipped_nifti_img = sitk.Flip(nifti_img, [False, True, False]) # flip the image to match the orientation of the dicom series
+    resampled_nifti_img = (resample_image_SimpleITK(flipped_nifti_img, 'linear', native_dicom_voxel_size,
+                                                    native_dicom_img_size)) # the resampled nifti image has the same
+                                                    # size and spacing as the native dicom image series from which the
+                                                    # nifti image was derived
+
+    # set the origin and direction of the resampled nifti image to match the reference dicom series
+    resampled_nifti_img.SetOrigin(ref_dicom_origin)
+    resampled_nifti_img.SetDirection(ref_dicom_direction)
+
+    # Convert the resampled NIFTI image to a DICOM series
+    vprint(f' {ANSI_GREEN}* Saving DICOM series to: {dicom_output_directory}{ANSI_RESET}', verbose=verbose)
+    reader = sitk.ImageSeriesReader()
+    dicom_names = reader.GetGDCMSeriesFileNames(original_dicom_directory)
+    dicom_slices = [pydicom.dcmread(f) for f in dicom_names]
+
+    total_slices = len(dicom_slices)
+    with Progress() as progress:
+        task = progress.add_task("[cyan] Writing DICOM slices:", total=total_slices)
+
+        def process_slice(idx, slice, output_dir, nifti_img):
+            slice.ImagePositionPatient = list(nifti_img.TransformIndexToPhysicalPoint((0, 0, idx)))
+            image_array_slice = sitk.GetArrayFromImage(nifti_img)[idx]
+            filename = f"slice_{idx}.dcm"
+            save_slice(slice, image_array_slice, "converted by nifti2dicom", filename, output_dir, slice.Modality)
+            progress.update(task, advance=1)
+
+        with ThreadPoolExecutor() as executor:
+            for idx, slice in enumerate(dicom_slices):
+                executor.submit(process_slice, idx, slice, dicom_output_directory, resampled_nifti_img)
+
+
 def save_dicom_from_nifti_seg(nifti_file: str, ref_dicom_series_dir: str, output_path: str, ORGAN_INDEX: dict,
                               verbose=False) -> None:
     """
     Convert a NIFTI segmentation image to a DICOM Segmentation object.
     :param nifti_file: Path to the NIFTI segmentation file.
     :type nifti_file: str
     :param ref_dicom_series_dir: Path to the directory containing the reference DICOM series.
```

### Comparing `nifti2dicom-1.1.9/nifti2dicom/display.py` & `nifti2dicom-1.2/nifti2dicom/display.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.1.9/nifti2dicom.egg-info/PKG-INFO` & `nifti2dicom-1.2/nifti2dicom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.1.9
+Version: 1.2
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.1.9/setup.py` & `nifti2dicom-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='nifti2dicom',
-    version='1.1.9',
+    version='1.2',
     packages=find_packages(),
     install_requires=[
         'pydicom',
         'nibabel',
         'numpy',
         'emoji',
         'rich',
```

