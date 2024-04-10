# Comparing `tmp/resamp-1.6.7.2.tar.gz` & `tmp/resamp-1.6.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.7.2.tar", last modified: Wed Apr 10 06:22:57 2024, max compression
+gzip compressed data, was "resamp-1.6.7.3.tar", last modified: Wed Apr 10 06:44:18 2024, max compression
```

## Comparing `resamp-1.6.7.2.tar` & `resamp-1.6.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:22:57.796556 resamp-1.6.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 06:22:53.000000 resamp-1.6.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-10 06:22:57.796556 resamp-1.6.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-10 06:22:53.000000 resamp-1.6.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:22:57.796556 resamp-1.6.7.2/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 06:22:53.000000 resamp-1.6.7.2/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-04-10 06:22:53.000000 resamp-1.6.7.2/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:22:57.796556 resamp-1.6.7.2/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-10 06:22:57.000000 resamp-1.6.7.2/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 06:22:57.000000 resamp-1.6.7.2/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:22:57.000000 resamp-1.6.7.2/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 06:22:57.000000 resamp-1.6.7.2/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 06:22:57.000000 resamp-1.6.7.2/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:22:57.796556 resamp-1.6.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-10 06:22:53.000000 resamp-1.6.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:44:18.535586 resamp-1.6.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 06:44:14.000000 resamp-1.6.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-10 06:44:18.535586 resamp-1.6.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-10 06:44:14.000000 resamp-1.6.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:44:18.531587 resamp-1.6.7.3/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-10 06:44:14.000000 resamp-1.6.7.3/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-04-10 06:44:14.000000 resamp-1.6.7.3/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:44:18.531587 resamp-1.6.7.3/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-10 06:44:18.000000 resamp-1.6.7.3/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 06:44:18.000000 resamp-1.6.7.3/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:44:18.000000 resamp-1.6.7.3/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 06:44:18.000000 resamp-1.6.7.3/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 06:44:18.000000 resamp-1.6.7.3/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:44:18.535586 resamp-1.6.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-10 06:44:14.000000 resamp-1.6.7.3/setup.py
```

### Comparing `resamp-1.6.7.2/LICENSE` & `resamp-1.6.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.7.2/PKG-INFO` & `resamp-1.6.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.7.2
+Version: 1.6.7.3
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.7.2/README.md` & `resamp-1.6.7.3/README.md`

 * *Files identical despite different names*

### Comparing `resamp-1.6.7.2/resamp/__init__.py` & `resamp-1.6.7.3/resamp/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     read_data,
     compare_dimensions,
     calculate_chi_squared,
     calculate_expected,
     calculate_chi_abs,
     chi_abs_stat,
     calculate_p_value,
-    chi_squared_stat,
-    p_value_stat,
     convert_df_to_numpy,
     bootstrap_chi_abs,
     calculate_p_value_bootstrap,
     plot_chi_abs_distribution,
     calculate_relative_risk_two_treatments,
     resample_and_calculate_rr,
     calculate_confidence_interval,
@@ -35,36 +33,36 @@
     bootstrap_confidence_interval,
     plot_bootstrap_lines,
     calculate_statistic,
     power_analysis,
 )
 
 __all__ = [
-    "mean_absolute_deviation",
+    "median_absolute_deviation",
     "read_data",
     "compare_dimensions",
     "calculate_chi_squared",
     "calculate_expected",
     "calculate_chi_abs",
     "chi_abs_stat",
     "calculate_p_value",
-    "chi_squared_stat",
     "p_value_stat",
     "convert_df_to_numpy",
     "bootstrap_chi_abs",
     "calculate_p_value_bootstrap",
     "plot_chi_abs_distribution",
     "calculate_relative_risk_two_treatments",
     "resample_and_calculate_rr",
     "calculate_confidence_interval",
     "calculate_probabilities_for_each_treatment",
     "plot_relative_risk_distribution",
     "calculate_p_value",
     "plot_null_distribution",
     "permute_correlation",
     "compute_correlation_ci",
+    "resample_one_group_count",
     "cal_ci_onedim",
     "bootstrap_confidence_interval",
     "plot_bootstrap_lines",
     "calculate_statistic",
     "power_analysis",
 ]
```

### Comparing `resamp-1.6.7.2/resamp/resamp.py` & `resamp-1.6.7.3/resamp/resamp.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.7.2/resamp.egg-info/PKG-INFO` & `resamp-1.6.7.3/resamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.7.2
+Version: 1.6.7.3
 Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.7.2/setup.py` & `resamp-1.6.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.7.2',
+    version='1.6.7.3',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
     description='A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
```

