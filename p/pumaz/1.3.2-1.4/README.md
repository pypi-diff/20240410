# Comparing `tmp/pumaz-1.3.2.tar.gz` & `tmp/pumaz-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pumaz-1.3.2.tar", last modified: Fri Mar 15 19:23:07 2024, max compression
+gzip compressed data, was "pumaz-1.4.tar", last modified: Wed Apr 10 13:26:08 2024, max compression
```

## Comparing `pumaz-1.3.2.tar` & `pumaz-1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:23:07.910761 pumaz-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-03-15 19:23:07.910761 pumaz-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-03-15 19:23:00.000000 pumaz-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:23:07.910761 pumaz-1.3.2/pumaz/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    42590 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/pumaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-15 19:23:00.000000 pumaz-1.3.2/pumaz/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:23:07.910761 pumaz-1.3.2/pumaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-03-15 19:23:07.000000 pumaz-1.3.2/pumaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-15 19:23:07.000000 pumaz-1.3.2/pumaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:23:07.000000 pumaz-1.3.2/pumaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-15 19:23:07.000000 pumaz-1.3.2/pumaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-15 19:23:07.000000 pumaz-1.3.2/pumaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 19:23:07.000000 pumaz-1.3.2/pumaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 19:23:07.914761 pumaz-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-15 19:23:00.000000 pumaz-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:26:08.482655 pumaz-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-10 13:26:08.482655 pumaz-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-10 13:26:01.000000 pumaz-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:26:08.478654 pumaz-1.4/pumaz/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16931 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42656 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/pumaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:26:08.478654 pumaz-1.4/pumaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:26:08.482655 pumaz-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-10 13:26:01.000000 pumaz-1.4/setup.py
```

### Comparing `pumaz-1.3.2/PKG-INFO` & `pumaz-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 1.3.2
+Version: 1.4
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
-Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
-Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
+Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires
+Author-email: Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, Manuel.pires@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -30,19 +30,21 @@
 Requires-Dist: pyfiglet~=0.8.post1
 Requires-Dist: natsort~=8.1.0
 Requires-Dist: pillow>=9.2.0
 Requires-Dist: colorama~=0.4.6
 Requires-Dist: rich
 Requires-Dist: pandas
 Requires-Dist: dicom2nifti
+Requires-Dist: nifti2dicom
 Requires-Dist: requests
 Requires-Dist: moosez
 Requires-Dist: halo
 Requires-Dist: psutil
 Requires-Dist: gputil
+Requires-Dist: dask
 Requires-Dist: lionz
 
 ![Puma-logo](Images/Puma-logo.png)
 
 ## PUMA 1.2 🐾 - Agile. Precision-Driven. Empowering 💪
 [![PyPI version](https://img.shields.io/pypi/v/pumaz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/pumaz/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Monthly Downloads](https://img.shields.io/pypi/dm/pumaz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) [![Daily Downloads](https://img.shields.io/pypi/dd/pumaz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/)
```

### Comparing `pumaz-1.3.2/README.md` & `pumaz-1.4/README.md`

 * *Files identical despite different names*

### Comparing `pumaz-1.3.2/pumaz/constants.py` & `pumaz-1.4/pumaz/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy')
     C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d')
 else:
     raise ValueError('Unsupported OS')
 
-
 # COLOR CODES
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[38;5;40m'
 ANSI_VIOLET = '\033[38;5;141m'
 ANSI_RED = '\033[38;5;196m'
 ANSI_RESET = '\033[0m'
 
@@ -72,31 +71,32 @@
 MOOSE_MODEL_BODY = "clin_ct_body"
 MOOSE_MODEL_PUMA_GPU = "clin_ct_PUMA"
 MOOSE_MODEL_PUMA_CPU = "clin_ct_PUMA4"
 MOOSE_PREFIX_BODY = 'CT_Body_'
 MOOSE_PREFIX_PUMA_GPU = 'Clin_CT_PUMA_'
 MOOSE_PREFIX_PUMA_CPU = 'Clin_CT_PUMA4_'
 MOOSE_LABEL_INDEX = {
-        1: "legs",
-        2: "body",
-        3: "head",
-        4: "arms"
-    }
+    1: "legs",
+    2: "body",
+    3: "head",
+    4: "arms"
+}
 
 # FOLDER NAMES
 
 PUMA_WORKING_FOLDER = 'PUMAZ-v1' + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 TRANSFORMS_FOLDER = 'transforms'
 ALIGNED_MASK_FOLDER = 'aligned_MASK'
 ALIGNED_CT_FOLDER = 'aligned_CT'
 ALIGNED_PET_FOLDER = 'aligned_PT'
 BODY_MASK_FOLDER = 'body_masks'
 PUMA_MASK_FOLDER = 'puma_masks'
 COMMON_FOV_MASK_FOLDER = 'common_fov_masks'
 SEGMENTATION_FOLDER = 'segmentation'
+DICOM_FOLDER = 'dicom'
 
 # HYPERPARAMETERS
 
 MULTI_RESOLUTION_SCHEME = '100x50x25'
 
 # RGB LINEAR TRANSFORMATION PARAMETERS TO GRAYSCALE BASED ON IMAGEMAGICK FORMULA
 
@@ -105,7 +105,11 @@
 BLUE_WEIGHT = 0.1140
 
 # LIONZ PARAMETERS
 
 LIONZ_MODEL = "mpx"
 LIONZ_PREFIX = "PT_"
 LIONZ_OUTPUT_DIR = "seg_output"
+
+# DICOM DESCRIPTIONS
+
+DESCRIPTION = 'Processed-by-PUMA-AND-DICOM-conversion-by-nifti2dicom'
```

### Comparing `pumaz-1.3.2/pumaz/display.py` & `pumaz-1.4/pumaz/display.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.3.2/pumaz/download.py` & `pumaz-1.4/pumaz/download.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.3.2/pumaz/file_utilities.py` & `pumaz-1.4/pumaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.3.2/pumaz/image_processing.py` & `pumaz-1.4/pumaz/image_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,22 +559,22 @@
     if corresponding_images:
         return corresponding_images[0]
     else:
         logging.error(f"No corresponding image found in {modality_dir} for {reference_basename}")
         raise FileNotFoundError(f"No corresponding image found in {modality_dir} for {reference_basename}")
 
 
-def align(puma_working_dir: str, ct_dir: str, pt_dir: str, mask_dir: str):
+def align(puma_working_dir: str, ct_dir: str, pt_dir: str, mask_dir: str) -> str:
     """
     Align the images in the PUMA working directory.
     :param puma_working_dir: The path to the PUMA working directory.
     :param ct_dir: The path to the CT directory.
     :param pt_dir: The path to the PET directory.
     :param mask_dir: The path to the mask directory.
-    :return: None
+    :return: The path to the reference mask image.
     """
     reference_image = find_images(mask_dir)[0]
     logging.info(f"Reference image selected: {os.path.basename(reference_image)}")
 
     aligner = setup_aligner(reference_image)
     moving_images = find_images(mask_dir)
     moving_images.remove(reference_image)
@@ -636,14 +636,15 @@
                          constants.ALIGNED_PREFIX_MASK)
     reference_ct = find_corresponding_image(ct_dir, os.path.basename(reference_image))
     copy_reference_image(reference_ct, os.path.join(puma_working_dir, constants.ALIGNED_CT_FOLDER),
                          constants.ALIGNED_PREFIX_CT)
     reference_pt = find_corresponding_image(pt_dir, os.path.basename(reference_image))
     copy_reference_image(reference_pt, os.path.join(puma_working_dir, constants.ALIGNED_PET_FOLDER),
                          constants.ALIGNED_PREFIX_PT)
+    return reference_image
 
 
 def calculate_bbox(mask_np):
     """
     Calculate the bounding box of a binary mask.
 
     :param mask_np: A binary mask represented as a NumPy array.
@@ -948,8 +949,7 @@
     :type output_dir: str
     :return: None
     """
     device = check_device()
     logging.info(f" Running LIONz for segmenting tumors from {input_dir}")
     lion(LIONZ_MODEL, input_dir, output_dir, device)
     logging.info(f" Tumor segmentation completed.")
-
```

### Comparing `pumaz-1.3.2/pumaz/pumaz.py` & `pumaz-1.4/pumaz/pumaz.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,22 +76,26 @@
 
     parser.add_argument("-st", "--segment_tumors", action='store_true', default=False,
                         help="Segment tumors in the multiplexed images.", required=False)
 
     parser.add_argument("-cs", "--custom_colors", action='store_true', default=False,
                         help="Manually assign colors to tracer images.", required=False)
 
+    parser.add_argument("-c2d", "--convert_to_dicom", action='store_true', default=False,
+                        help="Convert DICOM images to NIFTI format. Set this to true only if your input is DICOM",
+                        required=False)
+
     args = parser.parse_args()
 
     subject_folder = os.path.abspath(args.subject_directory)
     regions_to_ignore = args.ignore_regions
     multiplex = args.multiplex
     custom_colors = args.custom_colors
     segment_tumors = args.segment_tumors
-
+    convert_to_dicom = args.convert_to_dicom
 
     display.logo()
     display.citation()
 
     logging.info('----------------------------------------------------------------------------------------------------')
     logging.info('                                     STARTING PUMA-Z V.1.0.0                                       ')
     logging.info('----------------------------------------------------------------------------------------------------')
@@ -109,15 +113,16 @@
     display.expectations()
 
     # ----------------------------------
     # DISPLAYING INPUT CHOICES
     # ----------------------------------
     console.print(f' Multiplexing: {multiplex} | '
                   f'Custom Colors: {custom_colors} | '
-                  f'Segment Tumors: {segment_tumors} ',
+                  f'Segment Tumors: {segment_tumors} | ',
+                  f'Convert to DICOM: {convert_to_dicom}',
                   style='bold magenta')
 
     # ----------------------------------
     # DOWNLOADING THE BINARIES
     # ----------------------------------
 
     print('')
@@ -128,15 +133,14 @@
     file_utilities.create_directory(binary_path)
     system_os, system_arch = file_utilities.get_system()
     console.print(f' Detected system: {system_os} | Detected architecture: {system_arch}', style='bold magenta')
     download.download(item_name=f'puma-{system_os}-{system_arch}', item_path=binary_path,
                       item_dict=resources.PUMA_BINARIES)
     file_utilities.set_permissions(constants.GREEDY_PATH, system_os)
     file_utilities.set_permissions(constants.C3D_PATH, system_os)
-    
 
     # ----------------------------------
     # INPUT STANDARDIZATION
     # ----------------------------------
 
     print('')
     print(f'{constants.ANSI_VIOLET} {emoji.emojize(":magnifying_glass_tilted_left:")} STANDARDIZING INPUT DATA TO '
@@ -173,15 +177,15 @@
     print('')
     logging.info(' ')
     logging.info(' RUNNING PREPROCESSING AND REGISTRATION PIPELINE:')
     logging.info(' ')
     puma_dir, ct_dir, pt_dir, mask_dir = image_processing.preprocess(
         puma_compliant_subjects=puma_compliant_subject_folders,
         regions_to_ignore=regions_to_ignore)
-    image_processing.align(puma_dir, ct_dir, pt_dir, mask_dir)
+    reference_img = image_processing.align(puma_dir, ct_dir, pt_dir, mask_dir)
 
     # ----------------------------------
     # MULTIPLEXING
     # ----------------------------------
 
     if multiplex:
         print('')
@@ -194,23 +198,39 @@
         rgb_image = os.path.join(aligned_pt_dir, constants.MULTIPLEXED_COMPOSITE_IMAGE)
         image_processing.multiplex(aligned_pt_dir, '*nii*', 'PET',
                                    rgb_image, custom_colors)
         grayscale_image = os.path.join(aligned_pt_dir, constants.GRAYSCALE_COMPOSITE_IMAGE)
         image_processing.rgb2gray(rgb_image, grayscale_image)
         if segment_tumors:
             print('')
-            print(f'{constants.ANSI_VIOLET} {emoji.emojize(":face_with_medical_mask:")} SEGMENTING TUMORS:{constants.ANSI_RESET}')
+            print(
+                f'{constants.ANSI_VIOLET} {emoji.emojize(":face_with_medical_mask:")} SEGMENTING TUMORS:{constants.ANSI_RESET}')
             print('')
             print(f' {constants.ANSI_ORANGE}Segmentation may take a few minutes...{constants.ANSI_RESET}')
             seg_dir = os.path.join(puma_dir, constants.SEGMENTATION_FOLDER)
             file_utilities.create_directory(seg_dir)
             file_utilities.copy_reference_image(grayscale_image, seg_dir, constants.LIONZ_PREFIX)
             output_dir = os.path.join(seg_dir, constants.LIONZ_OUTPUT_DIR)
             file_utilities.create_directory(output_dir)
             image_processing.segment_tumors(seg_dir, output_dir)
             console.print(f' Segmentation complete.', style='bold green')
+
+    if convert_to_dicom:
+        print('')
+        print(f'{constants.ANSI_VIOLET} {emoji.emojize(":file_folder:")} CONVERTING TO DICOM:{constants.ANSI_RESET}')
+        print('')
+        logging.info(' ')
+        logging.info(' CONVERTING TO DICOM:')
+        logging.info(' ')
+        n2dConverter = image_conversion.NiftiToDicomConverter(
+            subject_folder=subject_folder,
+            puma_dir=puma_dir,
+        )
+        n2dConverter.set_reference_image(reference_img)
+        n2dConverter.convert_to_dicom(puma_compliant_subject_folders=puma_compliant_subject_folders)
+
     end_time = time.time()
     elapsed_time = end_time - start_time
     # show elapsed time in minutes and round it to 2 decimal places
     elapsed_time = round(elapsed_time / 60, 2)
     console.print(f" 🐾 PUMA has successfully completed the hunt in {elapsed_time} minutes."
                   f" Track down your results in the directory: {puma_dir} 🐾", style='white')
```

### Comparing `pumaz-1.3.2/pumaz/resources.py` & `pumaz-1.4/pumaz/resources.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.3.2/pumaz.egg-info/PKG-INFO` & `pumaz-1.4/pumaz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 1.3.2
+Version: 1.4
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
-Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
-Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
+Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires
+Author-email: Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, Manuel.pires@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -30,19 +30,21 @@
 Requires-Dist: pyfiglet~=0.8.post1
 Requires-Dist: natsort~=8.1.0
 Requires-Dist: pillow>=9.2.0
 Requires-Dist: colorama~=0.4.6
 Requires-Dist: rich
 Requires-Dist: pandas
 Requires-Dist: dicom2nifti
+Requires-Dist: nifti2dicom
 Requires-Dist: requests
 Requires-Dist: moosez
 Requires-Dist: halo
 Requires-Dist: psutil
 Requires-Dist: gputil
+Requires-Dist: dask
 Requires-Dist: lionz
 
 ![Puma-logo](Images/Puma-logo.png)
 
 ## PUMA 1.2 🐾 - Agile. Precision-Driven. Empowering 💪
 [![PyPI version](https://img.shields.io/pypi/v/pumaz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/pumaz/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Monthly Downloads](https://img.shields.io/pypi/dm/pumaz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) [![Daily Downloads](https://img.shields.io/pypi/dd/pumaz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/)
```

