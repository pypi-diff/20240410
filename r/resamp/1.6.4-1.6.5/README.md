# Comparing `tmp/resamp-1.6.4.tar.gz` & `tmp/resamp-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.4.tar", last modified: Tue Apr  9 20:47:25 2024, max compression
+gzip compressed data, was "resamp-1.6.5.tar", last modified: Tue Apr  9 22:28:41 2024, max compression
```

## Comparing `resamp-1.6.4.tar` & `resamp-1.6.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:47:25.440391 resamp-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 20:47:21.000000 resamp-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:47:25.440391 resamp-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-04-09 20:47:21.000000 resamp-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:47:25.436391 resamp-1.6.4/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 20:47:21.000000 resamp-1.6.4/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31802 2024-04-09 20:47:21.000000 resamp-1.6.4/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:47:25.436391 resamp-1.6.4/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:47:25.440391 resamp-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 20:47:21.000000 resamp-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:28:41.291058 resamp-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 22:28:37.000000 resamp-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-09 22:28:41.291058 resamp-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-09 22:28:37.000000 resamp-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:28:41.287058 resamp-1.6.5/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 22:28:37.000000 resamp-1.6.5/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-04-09 22:28:37.000000 resamp-1.6.5/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:28:41.291058 resamp-1.6.5/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:28:41.000000 resamp-1.6.5/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:28:41.291058 resamp-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 22:28:37.000000 resamp-1.6.5/setup.py
```

### Comparing `resamp-1.6.4/LICENSE` & `resamp-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.4/PKG-INFO` & `resamp-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.4
+Version: 1.6.5
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -29,34 +29,34 @@
 
 RESAMP Library Documentation
 
 - Author: Vishanth Hari Raj
 - GitHub Repository: https://github.com/vishanth10/resamp
 
 
-`resamp.py` Version 1.5 Documentation
+`resamp.py` Version 1.6.4 Documentation
 Overview
 `resamp.py` is a comprehensive Python library designed for statistical analysis and resampling techniques. This document serves as a guide for utilizing the library's functions, including statistical tests, data analysis, and visualization tools.
 Installation
 To install `resamp.py`, run the following command in your terminal:
 ```bash
 pip install statistics_library
 ```
 Functions:
 
-Mean Absolute Deviation (MAD)
-`mean_absolute_deviation(data)`
-Calculates the Mean Absolute Deviation of a dataset.
+Median Absolute Deviation (MAD)
+`median_absolute_deviation(data)`
+Calculates the Median Absolute Deviation of a dataset.
 - **Parameters**:
   - `data` (_array-like or str_): A 1D array or list containing the dataset, or a filename pointing to a CSV or Excel file containing a single column of numbers.
 - **Returns**:
-  - _float_: The Mean Absolute Deviation of the dataset.
+  - _float_: The Median Absolute Deviation of the dataset.
 - **Usage Example**:
   ```python
-  mad = mean_absolute_deviation([1, 2, 3, 4, 5])
+  mad = median_absolute_deviation([1, 2, 3, 4, 5])
   print(mad)
   ```
 **Chi-Squared Test**
 `calculate_chi_squared(observed, expected)`
 Calculates the chi-squared statistic given observed and expected frequencies.
 - **Parameters**:
   - `observed` (_DataFrame_): Observed frequencies.
```

### Comparing `resamp-1.6.4/README.md` & `resamp-1.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 
 RESAMP Library Documentation
 
 - Author: Vishanth Hari Raj
 - GitHub Repository: https://github.com/vishanth10/resamp
 
 
-`resamp.py` Version 1.5 Documentation
+`resamp.py` Version 1.6.4 Documentation
 Overview
 `resamp.py` is a comprehensive Python library designed for statistical analysis and resampling techniques. This document serves as a guide for utilizing the library's functions, including statistical tests, data analysis, and visualization tools.
 Installation
 To install `resamp.py`, run the following command in your terminal:
 ```bash
 pip install statistics_library
 ```
 Functions:
 
-Mean Absolute Deviation (MAD)
-`mean_absolute_deviation(data)`
-Calculates the Mean Absolute Deviation of a dataset.
+Median Absolute Deviation (MAD)
+`median_absolute_deviation(data)`
+Calculates the Median Absolute Deviation of a dataset.
 - **Parameters**:
   - `data` (_array-like or str_): A 1D array or list containing the dataset, or a filename pointing to a CSV or Excel file containing a single column of numbers.
 - **Returns**:
-  - _float_: The Mean Absolute Deviation of the dataset.
+  - _float_: The Median Absolute Deviation of the dataset.
 - **Usage Example**:
   ```python
-  mad = mean_absolute_deviation([1, 2, 3, 4, 5])
+  mad = median_absolute_deviation([1, 2, 3, 4, 5])
   print(mad)
   ```
 **Chi-Squared Test**
 `calculate_chi_squared(observed, expected)`
 Calculates the chi-squared statistic given observed and expected frequencies.
 - **Parameters**:
   - `observed` (_DataFrame_): Observed frequencies.
```

### Comparing `resamp-1.6.4/resamp/__init__.py` & `resamp-1.6.5/resamp/__init__.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.4/resamp/resamp.py` & `resamp-1.6.5/resamp/resamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,37 +541,39 @@
 
 
 ###############################################################################################################################
 
 # 1-Sample Tests
 import numpy as np
 
-def resample_one_group_count(box, sample_stat, count_what="A", two_tailed=False, sims=10000, proportion=False, return_resamples=False):
+def resample_one_group_count(box, sample_stat, sample_size, count_what="A", two_tailed=True, sims=10000, proportion=False, return_resamples=False):
     """
     Calculate a p-value for a count or proportion. Used to compare a sample to a population/base rate.
     
     Parameters:
         box (np array or list): Box model representing population
         sample_stat (float): Statistic for the sample
+        sample_size (int): Number of individuals (or sites, etc.) in sample
         count_what (char): What character in the box model should be counted. Default "A".
+        two_tailed (bool): Whether to compute a two-tailed p-value. If False, do one-tailed.
         sims (int): How many simulations to run. Default 10,000
-        proportion (boolean): Calculate count or proportion (default count)
-        tails (int): One or two tails
+        proportion (bool): Calculate count or proportion (default count)
+        return_resamples (bool): Whether to return resampling results used to generate p-value. Primarily for pedagogical purposes.
     
     Returns:
         p-value
         resampling data (if desired)
     """
 
     dataArr = np.array(box)  #Converts box model to NumPy array
 
     #Resampling loop
     resampleArr = np.zeros(sims)  #Preallocates array to store resampling results
     for i in range(sims):
-        p_sample = np.random.choice(box, len(box), replace=True)  #Samples from the box model (with replacement)
+        p_sample = np.random.choice(box, sample_size, replace=True)  #Samples from the box model (with replacement)
         p_count = np.sum(p_sample == count_what)
         resampleArr[i] = p_count
     
     #Compute p-value
     if proportion == False:
         observed = np.sum(dataArr == count_what)
     else:
@@ -581,15 +583,15 @@
     #Return results
     if return_resamples:
         return p, resampleArr
     else:
         return p
 
 
-    
+
 # Additional this function also do the same job : def calculate_confidence_interval(simulated_rr, percentile=95):
 def cal_ci_one_sample(data, confidence_level=99):
     """
     Calculate a custom confidence interval for a 1-D array based on the specified confidence level.
     
     Parameters:
         data (np.array): The 1-D array of resampled values or any numeric data.
```

### Comparing `resamp-1.6.4/resamp.egg-info/PKG-INFO` & `resamp-1.6.5/resamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.4
+Version: 1.6.5
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -29,34 +29,34 @@
 
 RESAMP Library Documentation
 
 - Author: Vishanth Hari Raj
 - GitHub Repository: https://github.com/vishanth10/resamp
 
 
-`resamp.py` Version 1.5 Documentation
+`resamp.py` Version 1.6.4 Documentation
 Overview
 `resamp.py` is a comprehensive Python library designed for statistical analysis and resampling techniques. This document serves as a guide for utilizing the library's functions, including statistical tests, data analysis, and visualization tools.
 Installation
 To install `resamp.py`, run the following command in your terminal:
 ```bash
 pip install statistics_library
 ```
 Functions:
 
-Mean Absolute Deviation (MAD)
-`mean_absolute_deviation(data)`
-Calculates the Mean Absolute Deviation of a dataset.
+Median Absolute Deviation (MAD)
+`median_absolute_deviation(data)`
+Calculates the Median Absolute Deviation of a dataset.
 - **Parameters**:
   - `data` (_array-like or str_): A 1D array or list containing the dataset, or a filename pointing to a CSV or Excel file containing a single column of numbers.
 - **Returns**:
-  - _float_: The Mean Absolute Deviation of the dataset.
+  - _float_: The Median Absolute Deviation of the dataset.
 - **Usage Example**:
   ```python
-  mad = mean_absolute_deviation([1, 2, 3, 4, 5])
+  mad = median_absolute_deviation([1, 2, 3, 4, 5])
   print(mad)
   ```
 **Chi-Squared Test**
 `calculate_chi_squared(observed, expected)`
 Calculates the chi-squared statistic given observed and expected frequencies.
 - **Parameters**:
   - `observed` (_DataFrame_): Observed frequencies.
```

### Comparing `resamp-1.6.4/setup.py` & `resamp-1.6.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.4',
+    version='1.6.5',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
     description='A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
```

