# Comparing `tmp/vision_oslo_extension-1.0.0.tar.gz` & `tmp/vision_oslo_extension-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_oslo_extension-1.0.0.tar", max compression
+gzip compressed data, was "vision_oslo_extension-1.0.1.tar", max compression
```

## Comparing `vision_oslo_extension-1.0.0.tar` & `vision_oslo_extension-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1091 2023-11-24 08:42:31.102210 vision_oslo_extension-1.0.0/LICENSE
--rw-r--r--   0        0        0      967 2024-04-05 09:48:37.868449 vision_oslo_extension-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1388 2024-04-05 09:52:31.461806 vision_oslo_extension-1.0.0/README.md
--rw-r--r--   0        0        0      800 2024-03-12 08:16:23.915038 vision_oslo_extension-1.0.0/src/vision_oslo_extension/__init__.py
--rw-r--r--   0        0        0    56562 2024-03-15 11:25:29.975386 vision_oslo_extension-1.0.0/src/vision_oslo_extension/average_load.py
--rw-r--r--   0        0        0     2790 2024-03-07 15:22:57.695190 vision_oslo_extension-1.0.0/src/vision_oslo_extension/base_frame.py
--rw-r--r--   0        0        0    36838 2024-03-14 10:29:12.757605 vision_oslo_extension-1.0.0/src/vision_oslo_extension/batch_processing.py
--rw-r--r--   0        0        0    28780 2024-03-14 10:39:09.702140 vision_oslo_extension-1.0.0/src/vision_oslo_extension/bhtpbank_check.py
--rw-r--r--   0        0        0    10224 2024-02-27 08:17:18.552995 vision_oslo_extension-1.0.0/src/vision_oslo_extension/check_frame.py
--rw-r--r--   0        0        0    29465 2024-03-14 10:41:08.331062 vision_oslo_extension-1.0.0/src/vision_oslo_extension/cif_prepare.py
--rw-r--r--   0        0        0    49860 2024-03-22 14:25:07.497914 vision_oslo_extension-1.0.0/src/vision_oslo_extension/dc_summary.py
--rw-r--r--   0        0        0    55732 2024-03-11 10:53:03.395998 vision_oslo_extension-1.0.0/src/vision_oslo_extension/extraction_frame.py
--rw-r--r--   0        0        0    41235 2024-03-14 11:00:07.181515 vision_oslo_extension-1.0.0/src/vision_oslo_extension/grid_connection.py
--rw-r--r--   0        0        0    14347 2024-04-05 10:03:14.714768 vision_oslo_extension-1.0.0/src/vision_oslo_extension/gui_start.py
--rw-r--r--   0        0        0    19401 2024-03-18 12:01:45.003388 vision_oslo_extension-1.0.0/src/vision_oslo_extension/input_frame.py
--rw-r--r--   0        0        0    21527 2024-03-07 15:58:07.329651 vision_oslo_extension-1.0.0/src/vision_oslo_extension/main_page_frame.py
--rw-r--r--   0        0        0     2468 2024-02-14 15:01:28.265376 vision_oslo_extension-1.0.0/src/vision_oslo_extension/master.py
--rw-r--r--   0        0        0    23521 2024-03-19 15:41:41.257250 vision_oslo_extension-1.0.0/src/vision_oslo_extension/model_check.py
--rw-r--r--   0        0        0    24213 2024-03-14 11:11:12.534785 vision_oslo_extension-1.0.0/src/vision_oslo_extension/ole_processing.py
--rw-r--r--   0        0        0    33127 2024-03-14 14:09:10.633765 vision_oslo_extension-1.0.0/src/vision_oslo_extension/oslo_extraction.py
--rwxr-xr-x   0        0        0   512073 2024-02-23 08:35:18.497365 vision_oslo_extension-1.0.0/src/vision_oslo_extension/osop.exe
--rw-r--r--   0        0        0    31290 2024-03-15 11:23:35.812514 vision_oslo_extension-1.0.0/src/vision_oslo_extension/post_processing.py
--rw-r--r--   0        0        0    61198 2024-03-05 11:01:50.726193 vision_oslo_extension-1.0.0/src/vision_oslo_extension/processing_frame.py
--rw-r--r--   0        0        0    29381 2024-03-14 12:34:43.381464 vision_oslo_extension-1.0.0/src/vision_oslo_extension/protection_if.py
--rw-r--r--   0        0        0    14408 2024-04-05 10:03:10.240540 vision_oslo_extension-1.0.0/src/vision_oslo_extension/shared_contents.py
--rw-r--r--   0        0        0   139454 2024-03-04 14:01:10.148626 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ac_extra_oslo_creator.xlsm
--rw-r--r--   0        0        0    51054 2024-03-11 08:52:49.000000 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ac_oslo_section_impedance.xlsx
--rw-r--r--   0        0        0   202327 2024-03-04 14:02:12.315689 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/bhtpbank_file_creator.xlsm
--rw-r--r--   0        0        0       10 2023-12-12 16:30:41.792954 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/BranchList.txt
--rw-r--r--   0        0        0       14 2023-12-12 16:30:54.664313 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/BranchNodeList.txt
--rw-r--r--   0        0        0      168 2024-03-08 07:06:33.861525 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/CIF_selection.csv
--rw-r--r--   0        0        0    98110 2024-03-04 13:30:37.445612 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/dc_extra_oslo_creator.xlsm
--rw-r--r--   0        0        0   200982 2024-03-21 10:54:17.507491 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/dc_oslo_section_impedance.xlsx
--rw-r--r--   0        0        0    23516 2024-02-06 07:23:18.000000 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/DCBB_rating_template.xlsx
--rw-r--r--   0        0        0       12 2023-12-12 16:31:41.027810 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/FeederList.txt
--rw-r--r--   0        0        0      204 2024-01-29 08:28:07.669991 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/GridAllocation.csv
--rw-r--r--   0        0        0    25546 2024-02-06 17:35:07.673973 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ImpBond_rating_template.xlsx
--rw-r--r--   0        0        0    23629 2024-02-05 14:39:20.749901 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/mainCB_rating_template.xlsx
--rw-r--r--   0        0        0    22310 2024-02-06 16:34:48.542131 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/NegETE_rating_template.xlsx
--rw-r--r--   0        0        0    61049 2024-01-25 07:57:22.185403 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/new_connection_template.xlsx
--rw-r--r--   0        0        0    62531 2024-03-04 15:23:28.000000 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ole_rating_template.xlsx
--rw-r--r--   0        0        0    22258 2024-02-07 09:05:02.000000 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/PosETE_rating_template.xlsx
--rw-r--r--   0        0        0    63059 2024-02-19 13:57:26.000000 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/power_template.xlsx
--rw-r--r--   0        0        0    60930 2024-02-19 13:57:52.000000 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/protection_template.xlsx
--rw-r--r--   0        0        0   444346 2022-10-04 09:49:09.635913 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/tiploc_library.csv
--rw-r--r--   0        0        0    23500 2024-02-07 09:04:47.963547 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/trackCB_rating_template.xlsx
--rw-r--r--   0        0        0       12 2023-12-12 16:31:17.496788 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/TrainList.txt
--rw-r--r--   0        0        0    26245 2024-02-07 13:21:54.163792 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/trainV_template.xlsx
--rw-r--r--   0        0        0       12 2023-12-12 16:31:29.665658 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/TransformerList.txt
--rw-r--r--   0        0        0    45992 2024-02-19 15:01:03.043210 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/TRU_rating_template.xlsx
--rw-r--r--   0        0        0  5005796 2024-03-26 07:35:46.772733 vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/VISION-OSLO Extension User Guide.pdf
--rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 vision_oslo_extension-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-11-24 08:42:31.102210 vision_oslo_extension-1.0.1/LICENSE
+-rw-r--r--   0        0        0      967 2024-04-10 10:16:09.118514 vision_oslo_extension-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1462 2024-04-10 10:17:07.661549 vision_oslo_extension-1.0.1/README.md
+-rw-r--r--   0        0        0      800 2024-03-12 08:16:23.915038 vision_oslo_extension-1.0.1/src/vision_oslo_extension/__init__.py
+-rw-r--r--   0        0        0    56562 2024-03-15 11:25:29.975386 vision_oslo_extension-1.0.1/src/vision_oslo_extension/average_load.py
+-rw-r--r--   0        0        0     2790 2024-03-07 15:22:57.695190 vision_oslo_extension-1.0.1/src/vision_oslo_extension/base_frame.py
+-rw-r--r--   0        0        0    36838 2024-03-14 10:29:12.757605 vision_oslo_extension-1.0.1/src/vision_oslo_extension/batch_processing.py
+-rw-r--r--   0        0        0    28780 2024-03-14 10:39:09.702140 vision_oslo_extension-1.0.1/src/vision_oslo_extension/bhtpbank_check.py
+-rw-r--r--   0        0        0    10224 2024-02-27 08:17:18.552995 vision_oslo_extension-1.0.1/src/vision_oslo_extension/check_frame.py
+-rw-r--r--   0        0        0    29465 2024-03-14 10:41:08.331062 vision_oslo_extension-1.0.1/src/vision_oslo_extension/cif_prepare.py
+-rw-r--r--   0        0        0    50613 2024-04-09 08:38:33.456091 vision_oslo_extension-1.0.1/src/vision_oslo_extension/dc_summary.py
+-rw-r--r--   0        0        0    55732 2024-03-11 10:53:03.395998 vision_oslo_extension-1.0.1/src/vision_oslo_extension/extraction_frame.py
+-rw-r--r--   0        0        0    41235 2024-03-14 11:00:07.181515 vision_oslo_extension-1.0.1/src/vision_oslo_extension/grid_connection.py
+-rw-r--r--   0        0        0    14347 2024-04-05 10:03:14.714768 vision_oslo_extension-1.0.1/src/vision_oslo_extension/gui_start.py
+-rw-r--r--   0        0        0    19401 2024-03-18 12:01:45.003388 vision_oslo_extension-1.0.1/src/vision_oslo_extension/input_frame.py
+-rw-r--r--   0        0        0    21527 2024-03-07 15:58:07.329651 vision_oslo_extension-1.0.1/src/vision_oslo_extension/main_page_frame.py
+-rw-r--r--   0        0        0     2468 2024-02-14 15:01:28.265376 vision_oslo_extension-1.0.1/src/vision_oslo_extension/master.py
+-rw-r--r--   0        0        0    23521 2024-03-19 15:41:41.257250 vision_oslo_extension-1.0.1/src/vision_oslo_extension/model_check.py
+-rw-r--r--   0        0        0    24213 2024-03-14 11:11:12.534785 vision_oslo_extension-1.0.1/src/vision_oslo_extension/ole_processing.py
+-rw-r--r--   0        0        0    33127 2024-03-14 14:09:10.633765 vision_oslo_extension-1.0.1/src/vision_oslo_extension/oslo_extraction.py
+-rwxr-xr-x   0        0        0   512073 2024-02-23 08:35:18.497365 vision_oslo_extension-1.0.1/src/vision_oslo_extension/osop.exe
+-rw-r--r--   0        0        0    31290 2024-03-15 11:23:35.812514 vision_oslo_extension-1.0.1/src/vision_oslo_extension/post_processing.py
+-rw-r--r--   0        0        0    61198 2024-03-05 11:01:50.726193 vision_oslo_extension-1.0.1/src/vision_oslo_extension/processing_frame.py
+-rw-r--r--   0        0        0    29381 2024-03-14 12:34:43.381464 vision_oslo_extension-1.0.1/src/vision_oslo_extension/protection_if.py
+-rw-r--r--   0        0        0    14408 2024-04-05 10:03:10.240540 vision_oslo_extension-1.0.1/src/vision_oslo_extension/shared_contents.py
+-rw-r--r--   0        0        0   139454 2024-03-04 14:01:10.148626 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ac_extra_oslo_creator.xlsm
+-rw-r--r--   0        0        0    51054 2024-03-11 08:52:49.000000 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ac_oslo_section_impedance.xlsx
+-rw-r--r--   0        0        0   202327 2024-03-04 14:02:12.315689 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/bhtpbank_file_creator.xlsm
+-rw-r--r--   0        0        0       10 2023-12-12 16:30:41.792954 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/BranchList.txt
+-rw-r--r--   0        0        0       14 2023-12-12 16:30:54.664313 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/BranchNodeList.txt
+-rw-r--r--   0        0        0      168 2024-03-08 07:06:33.861525 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/CIF_selection.csv
+-rw-r--r--   0        0        0    98110 2024-03-04 13:30:37.445612 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/dc_extra_oslo_creator.xlsm
+-rw-r--r--   0        0        0   200982 2024-03-21 10:54:17.507491 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/dc_oslo_section_impedance.xlsx
+-rw-r--r--   0        0        0    23516 2024-02-06 07:23:18.000000 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/DCBB_rating_template.xlsx
+-rw-r--r--   0        0        0       12 2023-12-12 16:31:41.027810 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/FeederList.txt
+-rw-r--r--   0        0        0      204 2024-01-29 08:28:07.669991 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/GridAllocation.csv
+-rw-r--r--   0        0        0    25546 2024-02-06 17:35:07.673973 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ImpBond_rating_template.xlsx
+-rw-r--r--   0        0        0    23629 2024-02-05 14:39:20.749901 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/mainCB_rating_template.xlsx
+-rw-r--r--   0        0        0    22310 2024-02-06 16:34:48.542131 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/NegETE_rating_template.xlsx
+-rw-r--r--   0        0        0    61049 2024-01-25 07:57:22.185403 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/new_connection_template.xlsx
+-rw-r--r--   0        0        0    62531 2024-03-04 15:23:28.000000 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ole_rating_template.xlsx
+-rw-r--r--   0        0        0    22258 2024-02-07 09:05:02.000000 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/PosETE_rating_template.xlsx
+-rw-r--r--   0        0        0    63059 2024-02-19 13:57:26.000000 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/power_template.xlsx
+-rw-r--r--   0        0        0    60930 2024-02-19 13:57:52.000000 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/protection_template.xlsx
+-rw-r--r--   0        0        0   444346 2022-10-04 09:49:09.635913 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/tiploc_library.csv
+-rw-r--r--   0        0        0    23500 2024-02-07 09:04:47.963547 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/trackCB_rating_template.xlsx
+-rw-r--r--   0        0        0       12 2023-12-12 16:31:17.496788 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/TrainList.txt
+-rw-r--r--   0        0        0    26245 2024-02-07 13:21:54.163792 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/trainV_template.xlsx
+-rw-r--r--   0        0        0       12 2023-12-12 16:31:29.665658 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/TransformerList.txt
+-rw-r--r--   0        0        0    45992 2024-02-19 15:01:03.043210 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/TRU_rating_template.xlsx
+-rw-r--r--   0        0        0  5005796 2024-03-26 07:35:46.772733 vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/VISION-OSLO Extension User Guide.pdf
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 vision_oslo_extension-1.0.1/PKG-INFO
```

### Comparing `vision_oslo_extension-1.0.0/LICENSE` & `vision_oslo_extension-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/pyproject.toml` & `vision_oslo_extension-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "vision_oslo_extension"
-version = "1.0.0"
+version = "1.0.1"
 description = "This is the package to support additional features on VISION-OSLO, software owned by Network Rail Infrastructure Limited."
 authors = ["Jieming Ye <Jieming.Ye@networkrail.co.uk>"]
 readme = "README.md"
 include = ["README.md", "src", "src/vision_oslo_extension/**/*.exe", "src/vision_oslo_extension/support/**/*"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `vision_oslo_extension-1.0.0/README.md` & `vision_oslo_extension-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 https://github.com/NR-JYe/Vision-Oslo-Extension
 
 ## Usage
 Pre-installtion of Python and VISION-OSLO required.
 
 ## What's New
 
-This version bumped the number to 1.0.0 and ready for proper usage.
+This version fixed the unit calculation error in TRU summary
 
 ## History / Key Upgrade
+Version 1.0.1 (Stable version): Fix the unit calculation error in TRU summary
+
 Version 1.0.0 (Stable version): First official version to all stakeholders
 
 Version 0.7.3 (Beta version): Restructure For packaging and distribution and add User Manual / Guidance / Help Doc
 
 Version 0.6.3 (Beta version): Bug Fix, Import Feature Completed
 
 Version 0.5.0 (Beta version): This version introduced model checking.
```

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/__init__.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/average_load.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/average_load.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/base_frame.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/base_frame.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/batch_processing.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/batch_processing.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/bhtpbank_check.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/bhtpbank_check.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/check_frame.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/check_frame.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/cif_prepare.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/cif_prepare.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/dc_summary.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/dc_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,16 +398,20 @@
                 sim = sim + "_branch_1800_rms_sum_max.csv"
             
             if not option == "8":
                 # if in double, move this under subtaiton section and do customised one for each option
                 file_path = os.path.join(os.getcwd(),folder,sim)
                 #result_df = pd.read_csv(file_path,usecols=csv_columns,nrows=oslo_total,header = None, skiprows=2, names= result_header)
                 result_df = pd.read_csv(file_path,usecols=csv_columns,header = None, skiprows=2, names= result_header)
-                # Divide all columns by 1000 except the first column
-                result_df.iloc[:, 1:] = result_df.iloc[:, 1:].divide(1000)
+                if option == "1": # For TRU assessment, the last column is power in MW
+                    # Divide all columns by 1000 except the first column and last column (updated to consider the P30min power)
+                    result_df.iloc[:, 1:-1] = result_df.iloc[:, 1:-1].divide(1000)
+                else:
+                    # Divide all columns by 1000 except the first column
+                    result_df.iloc[:, 1:] = result_df.iloc[:, 1:].divide(1000)
                 r_df_sum.append(result_df)
             else:
                 sim = sim + ".osop.vlt"
                 file_path = os.path.join(os.getcwd(),folder,sim)
 
                 # Define column widths based on your data
                 col_widths = [4, 1, 5, 10, 8, 2, 9]  # Replace ... with the widths of your columns
@@ -951,14 +955,18 @@
                 for cell in row:
                     cell.font = Font(bold = True, italic = True, size = 11)
                     cell.fill = PatternFill(start_color="DDDDDD", end_color="DDDDDD", fill_type="solid")
                     cell.alignment = Alignment(horizontal='center', vertical='center', wrap_text=True)
         
         condtional_formating(sheet,range_list,scenariolist,1,option)
 
+        if time[0] == "P":
+            sheet['B2'].value = name + " " + time + " Average Power Summary"
+            sheet['D7'].value = "N-0 Rating (MW)"
+            sheet['E7'].value = "N-1 Rating (MW)"
 
         # Auto-size columns after applying formatting
         for col_letter in ['A','B',"C","D"]:
             sheet.column_dimensions[col_letter].auto_size = True
         
         if option == "8":
             sheet.column_dimensions["E"].auto_size = True
@@ -1019,14 +1027,18 @@
 
         cell = sheet[range_list[6][index][2]]
         cell.value = "Result"
         cell.font = Font(bold=True)
 
         cell = sheet[range_list[6][index][3]]
         cell.value = range_list[6][index][4]
+
+        if time[0] == "P": # time
+            cell = sheet[range_list[6][index][1]]
+            cell.value = time + " " + assess + " Assessment (Average Power) - Note that the Rating Unit Below should be MW"
     
     print("Apply Numbering Format ...")
     # Define a custom style for formatting with two decimal places
     for range_name in range_list[4]:
         for row in sheet[range_name]:
             for cell in row:
                 cell.number_format = '0.00'
```

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/extraction_frame.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/extraction_frame.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/grid_connection.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/grid_connection.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/gui_start.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/gui_start.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/input_frame.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/input_frame.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/main_page_frame.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/main_page_frame.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/master.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/master.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/model_check.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/model_check.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/ole_processing.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/ole_processing.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/oslo_extraction.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/oslo_extraction.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/osop.exe` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/osop.exe`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/post_processing.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/post_processing.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/processing_frame.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/processing_frame.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/protection_if.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/protection_if.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/shared_contents.py` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/shared_contents.py`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ac_extra_oslo_creator.xlsm` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ac_extra_oslo_creator.xlsm`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ac_oslo_section_impedance.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ac_oslo_section_impedance.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/bhtpbank_file_creator.xlsm` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/bhtpbank_file_creator.xlsm`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/dc_extra_oslo_creator.xlsm` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/dc_extra_oslo_creator.xlsm`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/dc_oslo_section_impedance.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/dc_oslo_section_impedance.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/DCBB_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/DCBB_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ImpBond_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ImpBond_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/mainCB_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/mainCB_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/NegETE_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/NegETE_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/new_connection_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/new_connection_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/ole_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/ole_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/PosETE_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/PosETE_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/power_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/power_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/protection_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/protection_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/tiploc_library.csv` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/tiploc_library.csv`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/trackCB_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/trackCB_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/trainV_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/trainV_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/TRU_rating_template.xlsx` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/TRU_rating_template.xlsx`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/src/vision_oslo_extension/support/VISION-OSLO Extension User Guide.pdf` & `vision_oslo_extension-1.0.1/src/vision_oslo_extension/support/VISION-OSLO Extension User Guide.pdf`

 * *Files identical despite different names*

### Comparing `vision_oslo_extension-1.0.0/PKG-INFO` & `vision_oslo_extension-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_oslo_extension
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is the package to support additional features on VISION-OSLO, software owned by Network Rail Infrastructure Limited.
 License: MIT
 Author: Jieming Ye
 Author-email: Jieming.Ye@networkrail.co.uk
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,17 +43,19 @@
 https://github.com/NR-JYe/Vision-Oslo-Extension
 
 ## Usage
 Pre-installtion of Python and VISION-OSLO required.
 
 ## What's New
 
-This version bumped the number to 1.0.0 and ready for proper usage.
+This version fixed the unit calculation error in TRU summary
 
 ## History / Key Upgrade
+Version 1.0.1 (Stable version): Fix the unit calculation error in TRU summary
+
 Version 1.0.0 (Stable version): First official version to all stakeholders
 
 Version 0.7.3 (Beta version): Restructure For packaging and distribution and add User Manual / Guidance / Help Doc
 
 Version 0.6.3 (Beta version): Bug Fix, Import Feature Completed
 
 Version 0.5.0 (Beta version): This version introduced model checking.
```

