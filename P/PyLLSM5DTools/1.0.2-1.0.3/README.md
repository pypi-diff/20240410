# Comparing `tmp/PyLLSM5DTools-1.0.2.tar.gz` & `tmp/PyLLSM5DTools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLLSM5DTools-1.0.2.tar", last modified: Fri Apr  5 06:00:57 2024, max compression
+gzip compressed data, was "PyLLSM5DTools-1.0.3.tar", last modified: Wed Apr 10 02:04:58 2024, max compression
```

## Comparing `PyLLSM5DTools-1.0.2.tar` & `PyLLSM5DTools-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 PyLLSM5DTools-1.0.2/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2805 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2782 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 PyLLSM5DTools-1.0.2/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-05 04:47:16.000000 PyLLSM5DTools-1.0.2/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 PyLLSM5DTools-1.0.3/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-10 02:04:58.756821 PyLLSM5DTools-1.0.3/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2885 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2782 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 PyLLSM5DTools-1.0.3/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-10 01:59:56.000000 PyLLSM5DTools-1.0.3/setup.py
```

### Comparing `PyLLSM5DTools-1.0.2/LICENSE.txt` & `PyLLSM5DTools-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_FSC_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_MIP_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 def XR_MIP_wrapper(dataPaths, **kwargs):
     function_name = "XR_MIP_wrapper"
     XR_MIP_wrapper_dict = {
         "axis": [kwargs.get("axis", [0,0,1]), "numericArr"],
         "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "largeZarr": [kwargs.get("largeZarr", False), "logical"],
+        "BatchSize": [kwargs.get("BatchSize", [2048,2048,2048]), "numericArr"],
         "Save16bit": [kwargs.get("Save16bit", True), "logical"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "parseParfor": [kwargs.get("parseParfor", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "cpusPerTask": [kwargs.get("cpusPerTask", 3), "numericScalar"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs/"), "char"],
         "uuid": [kwargs.get("uuid", ""), "char"],
```

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_crop_dataset.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_decon_data_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_resample_dataset.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/__init__.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/generatePythonWrapper.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/generatePythonWrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools/generate_config_file.py` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/SOURCES.txt` & `PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/README.md` & `PyLLSM5DTools-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.2/setup.py` & `PyLLSM5DTools-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.0.2'
+version = '1.0.3'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

