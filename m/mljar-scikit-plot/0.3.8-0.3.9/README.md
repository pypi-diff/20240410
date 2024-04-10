# Comparing `tmp/mljar-scikit-plot-0.3.8.tar.gz` & `tmp/mljar-scikit-plot-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mljar-scikit-plot-0.3.8.tar", last modified: Wed Apr 10 12:29:01 2024, max compression
+gzip compressed data, was "mljar-scikit-plot-0.3.9.tar", last modified: Wed Apr 10 13:13:21 2024, max compression
```

## Comparing `mljar-scikit-plot-0.3.8.tar` & `mljar-scikit-plot-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:29:01.914232 mljar-scikit-plot-0.3.8/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1076 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       58 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      968 2024-04-10 12:29:01.914232 mljar-scikit-plot-0.3.8/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       83 2024-04-10 12:28:56.000000 mljar-scikit-plot-0.3.8/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:29:01.910232 mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      968 2024-04-10 12:29:01.000000 mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      475 2024-04-10 12:29:01.000000 mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-04-10 12:29:01.000000 mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       83 2024-04-10 12:29:01.000000 mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-04-10 12:29:01.000000 mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       61 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:29:01.914232 mljar-scikit-plot-0.3.8/scikitplot/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      272 2024-04-10 12:23:41.000000 mljar-scikit-plot-0.3.8/scikitplot/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    25058 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/classifiers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4865 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/cluster.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1735 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/clustering.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8079 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/decomposition.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9921 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/estimators.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7732 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/helpers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    47342 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    44073 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.8/scikitplot/plotters.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-04-10 12:29:01.914232 mljar-scikit-plot-0.3.8/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2152 2024-04-10 12:23:23.000000 mljar-scikit-plot-0.3.8/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 13:13:21.507231 mljar-scikit-plot-0.3.9/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1076 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       58 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      968 2024-04-10 13:13:21.507231 mljar-scikit-plot-0.3.9/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       83 2024-04-10 12:28:56.000000 mljar-scikit-plot-0.3.9/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 13:13:21.507231 mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      968 2024-04-10 13:13:21.000000 mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      475 2024-04-10 13:13:21.000000 mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-04-10 13:13:21.000000 mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       83 2024-04-10 13:13:21.000000 mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-04-10 13:13:21.000000 mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       65 2024-04-10 13:12:39.000000 mljar-scikit-plot-0.3.9/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 13:13:21.507231 mljar-scikit-plot-0.3.9/scikitplot/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      272 2024-04-10 13:13:05.000000 mljar-scikit-plot-0.3.9/scikitplot/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    25058 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/classifiers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4865 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/cluster.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1735 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/clustering.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8079 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/decomposition.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9921 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/estimators.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7732 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/helpers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    47342 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    44073 2024-04-10 12:20:08.000000 mljar-scikit-plot-0.3.9/scikitplot/plotters.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-04-10 13:13:21.507231 mljar-scikit-plot-0.3.9/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2152 2024-04-10 13:13:00.000000 mljar-scikit-plot-0.3.9/setup.py
```

### Comparing `mljar-scikit-plot-0.3.8/LICENSE` & `mljar-scikit-plot-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/PKG-INFO` & `mljar-scikit-plot-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-scikit-plot
-Version: 0.3.8
+Version: 0.3.9
 Summary: An intuitive library to add plotting functionality to scikit-learn objects.
 Home-page: https://github.com/mljar/mljar-scikit-plot
 Author: MLJAR Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mljar-scikit-plot-0.3.8/mljar_scikit_plot.egg-info/PKG-INFO` & `mljar-scikit-plot-0.3.9/mljar_scikit_plot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-scikit-plot
-Version: 0.3.8
+Version: 0.3.9
 Summary: An intuitive library to add plotting functionality to scikit-learn objects.
 Home-page: https://github.com/mljar/mljar-scikit-plot
 Author: MLJAR Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/classifiers.py` & `mljar-scikit-plot-0.3.9/scikitplot/classifiers.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/cluster.py` & `mljar-scikit-plot-0.3.9/scikitplot/cluster.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/clustering.py` & `mljar-scikit-plot-0.3.9/scikitplot/clustering.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/decomposition.py` & `mljar-scikit-plot-0.3.9/scikitplot/decomposition.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/estimators.py` & `mljar-scikit-plot-0.3.9/scikitplot/estimators.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/helpers.py` & `mljar-scikit-plot-0.3.9/scikitplot/helpers.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/metrics.py` & `mljar-scikit-plot-0.3.9/scikitplot/metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/scikitplot/plotters.py` & `mljar-scikit-plot-0.3.9/scikitplot/plotters.py`

 * *Files identical despite different names*

### Comparing `mljar-scikit-plot-0.3.8/setup.py` & `mljar-scikit-plot-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def run_tests(self):
         import pytest
         errcode = pytest.main(self.test_args)
         sys.exit(errcode)
 
 setup(
     name='mljar-scikit-plot',
-    version='0.3.8',
+    version='0.3.9',
     url='https://github.com/mljar/mljar-scikit-plot',
     license='MIT License',
     author='MLJAR Sp. z o.o.',
     tests_require=['pytest'],
     install_requires=[
         'matplotlib>=1.4.0',
         'scikit-learn>=1.1.0',
```

