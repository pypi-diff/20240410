# Comparing `tmp/resamp-1.6.3.tar.gz` & `tmp/resamp-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.3.tar", last modified: Tue Apr  9 20:04:19 2024, max compression
+gzip compressed data, was "resamp-1.6.4.tar", last modified: Tue Apr  9 20:47:25 2024, max compression
```

## Comparing `resamp-1.6.3.tar` & `resamp-1.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:04:19.530227 resamp-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 20:04:15.000000 resamp-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:04:19.530227 resamp-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-04-09 20:04:15.000000 resamp-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:04:19.526227 resamp-1.6.3/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 20:04:15.000000 resamp-1.6.3/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32392 2024-04-09 20:04:15.000000 resamp-1.6.3/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:04:19.530227 resamp-1.6.3/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:04:19.530227 resamp-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 20:04:15.000000 resamp-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:47:25.440391 resamp-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 20:47:21.000000 resamp-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:47:25.440391 resamp-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-04-09 20:47:21.000000 resamp-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:47:25.436391 resamp-1.6.4/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 20:47:21.000000 resamp-1.6.4/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31802 2024-04-09 20:47:21.000000 resamp-1.6.4/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:47:25.436391 resamp-1.6.4/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:47:25.000000 resamp-1.6.4/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:47:25.440391 resamp-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 20:47:21.000000 resamp-1.6.4/setup.py
```

### Comparing `resamp-1.6.3/LICENSE` & `resamp-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.3/PKG-INFO` & `resamp-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.3
+Version: 1.6.4
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.3/README.md` & `resamp-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resamp-1.6.3/resamp/__init__.py` & `resamp-1.6.4/resamp/__init__.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.3/resamp/resamp.py` & `resamp-1.6.4/resamp/resamp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,61 @@
-### ACTIVE FINAL SCRIPT
-##FINAL SCRIPTS VERSION - 4.0 (UPDATED BOOTSRATPPING FUNCTION), OVERRIDE EXPECTED VALUE
-## ALL MODIFICATION ACTIVE
-
 # LS 40 resampling library to complement/combine with Hypothesize
 
 ### ACTIVE FINAL SCRIPT
 
-## NAME: resamp.py
-## VERSION - 1.5
+## VERSION - 1.6.4
 ## STATUS: ALL MODIFICATION ACTIVE AND LIVE IN PYPI (PIP INSTALL STATISTICS_LIBRARY)
-## DATE: 9 MARCH 2024 
+## DATE: 9 APRIL 2024 
 ## AUTHOR: VISHANTH HARI RAJ
-## SUPERVISOR: JANE
+## SUPERVISOR: JANE SHEVTSOV
+
 
 import pandas as pd
 import numpy as np
 from scipy.stats import chi2
 import logging
 import os
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 
-##MAD FUNCTION Mean-Absolute-Deviation
+##MAD FUNCTION Median Absolute Deviation
 
-def mean_absolute_deviation(data):
+def median_absolute_deviation(data):
     """
-    Calculate the Mean Absolute Deviation (MAD) of a 1D dataset.
+    Calculate the Median Absolute Deviation (MAD) of a 1D dataset.
 
     The function accepts either a 1D array-like, a filename of a CSV or an Excel file.
     In case of a file, the function expects it to contain a single column of numbers.
 
     Parameters:
     data (array-like or str): A 1D array or list containing the dataset, or a filename.
 
     Returns:
-    float: The Mean Absolute Deviation of the dataset.
+    float: The Median Absolute Deviation of the dataset.
 
     Example:
-    >>> mean_absolute_deviation([1, 2, 3, 4, 5])
+    >>> median_absolute_deviation([1, 2, 3, 4, 5])
     1.2
 
-    >>> mean_absolute_deviation('data.csv') # Assuming 'data.csv' contains a single column of numbers
+    >>> median_absolute_deviation('data.csv') # Assuming 'data.csv' contains a single column of numbers
     # Returns the MAD of the numbers in 'data.csv'
     """
-#     try:
-#         # Check if data is a filename
-#         if isinstance(data, str):
-#             if data.endswith('.csv'):
-#                 data = pd.read_csv(data).squeeze()  # Assuming a single column
-#             elif data.endswith(('.xls', '.xlsx')):
-#                 data = pd.read_excel(data).squeeze()  # Assuming a single column
-#             else:
-#                 raise ValueError("File format not supported. Please use CSV or Excel files.")
-        
-        # Calculate MAD
-#2-D array (work column by column)
+    # Calculate MAD
+    #2-D array (work column by column)
     try:
         median = np.median(data)
         deviations = np.abs(data - median)
-        mad = np.mean(deviations)
+        mad = np.median(deviations)
         return mad
     except Exception as e:
         return f"An error occurred: {e}"
 
 # test_data = [15, 26, 30, 40, 55]
-# mad = mean_absolute_deviation(test_data)
+# mad = median_absolute_deviation(test_data)
 # print(mad)
 
 ###############################################################################################################################
 
 def read_data(input_data):
     # Function to read data from either a file path or DataFrame
     if isinstance(input_data, pd.DataFrame):
@@ -132,48 +118,14 @@
         chi_abs = calculate_chi_abs(observed_data, expected_data)
         return chi_abs
     except Exception as e:
         logging.error("Error calculating chi absolute: ", exc_info=True)
         return None
 
 
-def calculate_p_value(chi_squared, dof):
-    p_value = chi2.sf(chi_squared, dof)
-    return p_value
-
-
-def chi_squared_stat(observed_data, expected_data):
-    try:
-        observed = read_data(observed_data)
-        expected = read_data(expected_data)
-        compare_dimensions(observed, expected)
-        chi_squared = calculate_chi_squared(observed, expected)
-        return chi_squared
-    except Exception as e:
-        logging.error("Error calculating chi-squared: ", exc_info=True)
-        return None
-
-
-def p_value_stat(observed_data, expected_data):
-    try:
-        observed = read_data(observed_data)
-        expected = read_data(expected_data)
-        compare_dimensions(observed, expected)
-        chi_squared = calculate_chi_squared(observed, expected)
-        dof = (observed.shape[0] - 1) * (observed.shape[1] - 1)
-        return calculate_p_value(chi_squared, dof)
-    except Exception as e:
-        logging.error("Error calculating p-value: ", exc_info=True)
-        return None
-
-
-# Example usage (assuming observed_data and expected_data are numpy arrays):
-# p_value_mean_ratio = calculate_p_value_mean_ratio(observed_data, expected_data, num_simulations=1000, with_replacement=True, sample_size=None)
-# print(f"P-value (Mean Ratio): {p_value_mean_ratio}")
-        
 
 def convert_df_to_numpy(df_observed, df_expected):
     """
     Converts DataFrame data to numpy arrays for use in other functions, 
     particularly for bootstrapping.
 
     Parameters:
@@ -390,15 +342,15 @@
         # Calculate the Risk Ratio (RR) for the current simulated dataset and store it
         simulated_rr[i] = prob_event_treatment1 / prob_event_other_treatment
 
     # Return an array of simulated RR values
     return simulated_rr
 
 
-# Calculate the 95% confidence interval
+# Calculate the 99% confidence interval
 def calculate_confidence_interval(simulated_rr, percentile=99):
     """
     Calculate the confidence interval for the relative risk based on the distribution of simulated relative risks.
 
     Parameters:
         simulated_rr (np.array): Array of simulated relative risks.
         percentile (float, optional): The percentile for the confidence interval. Defaults to 95.
@@ -586,20 +538,60 @@
         print(f"{confidence_interval*100:.0f}% Confidence Interval: ({lower_bound:.3f}, {upper_bound:.3f})")
     except Exception as e:
         print(f"An error occurred: {e}")
 
 
 ###############################################################################################################################
 
-# 1-D Confidence Interval Calculation 
-# Additional this function also do the same job : def calculate_confidence_interval(simulated_rr, percentile=95):
-
+# 1-Sample Tests
 import numpy as np
 
-def cal_ci_onedim(data, confidence_level=99):
+def resample_one_group_count(box, sample_stat, count_what="A", two_tailed=False, sims=10000, proportion=False, return_resamples=False):
+    """
+    Calculate a p-value for a count or proportion. Used to compare a sample to a population/base rate.
+    
+    Parameters:
+        box (np array or list): Box model representing population
+        sample_stat (float): Statistic for the sample
+        count_what (char): What character in the box model should be counted. Default "A".
+        sims (int): How many simulations to run. Default 10,000
+        proportion (boolean): Calculate count or proportion (default count)
+        tails (int): One or two tails
+    
+    Returns:
+        p-value
+        resampling data (if desired)
+    """
+
+    dataArr = np.array(box)  #Converts box model to NumPy array
+
+    #Resampling loop
+    resampleArr = np.zeros(sims)  #Preallocates array to store resampling results
+    for i in range(sims):
+        p_sample = np.random.choice(box, len(box), replace=True)  #Samples from the box model (with replacement)
+        p_count = np.sum(p_sample == count_what)
+        resampleArr[i] = p_count
+    
+    #Compute p-value
+    if proportion == False:
+        observed = np.sum(dataArr == count_what)
+    else:
+        observed = np.mean(dataArr == count_what)
+    p = calculate_p_value_bootstrap(observed_data = sample_stat, simulated_data = resampleArr, two_tailed=two_tailed)
+    
+    #Return results
+    if return_resamples:
+        return p, resampleArr
+    else:
+        return p
+
+
+    
+# Additional this function also do the same job : def calculate_confidence_interval(simulated_rr, percentile=95):
+def cal_ci_one_sample(data, confidence_level=99):
     """
     Calculate a custom confidence interval for a 1-D array based on the specified confidence level.
     
     Parameters:
         data (np.array): The 1-D array of resampled values or any numeric data.
         confidence_level (float): The confidence level expressed as a percentage. Defaults to 99.
     
@@ -622,14 +614,17 @@
     upper_value = data[upper_pos]
     
     return lower_value, upper_value
 
 
 #########################################################################################################################################
 
+#Linear regression, slope/intercept resampling and finding confidence interval
+
+
 import numpy as np
 import pandas as pd
 from scipy.stats import linregress
 
 def bootstrap_confidence_interval(x, y, n_bootstrap=1000, confidence_level=99, return_type='both'):
     slopes = []
     intercepts = []
@@ -704,45 +699,45 @@
     
     plt.xlabel('X')
     plt.ylabel('Y')
     plt.title('Bootstrap Regression Lines')
     plt.legend()
     plt.show()
 
-
 ###################################################################################################################################
 
 ##Power Analysis
 
 import numpy as np
 
 def calculate_statistic(data, stat_type='median'):
     """Calculate either the mean or median of the data, based on stat_type."""
     return np.mean(data) if stat_type == 'mean' else np.median(data)
 
 def power_analysis(obs_diff, group1, group2, num_simulations=1000, alpha=0.01, power_threshold=0.8, factor_limit=10, measure='median', verbose=False):
     """
     Perform a power analysis using resampling methods to determine the sample size required to achieve a desired power level.
     The function stops increasing the sample size once the factor limit is reached.
-    
+
     Parameters:
     obs_diff -- the observed difference in medians or means between the two groups, depending on 'measure'
     group1 -- data for group 1
     group2 -- data for group 2
     num_simulations -- number of simulations to perform
     alpha -- significance level
     power_threshold -- desired power level to achieve
     factor_limit -- the maximum factor by which to increase the sample size
     measure -- 'median' or 'mean', the statistical measure to use for comparison
     verbose -- if True, print intermediate results
-    
+
     Returns:
     required_sample_sizes -- a tuple of the required sample sizes for group 1 and group 2 to achieve the desired power
     achieved_power -- the power that was achieved with the returned sample sizes
-    """    
+    """
+
     factor = 1
     achieved_power = 0
 
     while achieved_power < power_threshold and factor <= factor_limit:
         sample_size_group1 = len(group1) * factor
         sample_size_group2 = len(group2) * factor
         pvals = []
@@ -765,29 +760,15 @@
 
             # Calculate the p-value for this simulation
             pval = (np.sum(null_diffs >= abs(phantom_diff)) + np.sum(null_diffs <= -abs(phantom_diff))) / num_simulations
             pvals.append(pval)
 
         # Calculate the overall power based on the simulations
         achieved_power = np.mean(np.array(pvals) < alpha)
-        
+
         if verbose:
             print(f"Iteration with factor {factor}: Sample size group 1: {sample_size_group1}, Sample size group 2: {sample_size_group2}, Achieved power: {achieved_power}")
 
         factor += 1
 
     required_sample_sizes = (sample_size_group1, sample_size_group2)
     return required_sample_sizes, achieved_power
-
-
-
-# Placeholder for actual calls with real data:
-# required_sample_sizes, achieved_power = power_analysis(
-#     obs_diff, plant_eph, plant_perm,
-#     num_simulations=1000, alpha=0.01, power_threshold=0.8, factor_limit=10,
-#     measure='mean', verbose=True
-# )
-
-
-
-
-
```

### Comparing `resamp-1.6.3/resamp.egg-info/PKG-INFO` & `resamp-1.6.4/resamp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.3
+Version: 1.6.4
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.3/setup.py` & `resamp-1.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.3',
+    version='1.6.4',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
     description='A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
```

