# Comparing `tmp/vf_portalytics-1.1.1.tar.gz` & `tmp/vf_portalytics-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vf_portalytics-1.1.1.tar", last modified: Tue Mar 26 07:52:27 2024, max compression
+gzip compressed data, was "dist/vf_portalytics-1.1.2.tar", last modified: Wed Apr 10 07:56:50 2024, max compression
```

## Comparing `vf_portalytics-1.1.1.tar` & `vf_portalytics-1.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/.circleci/
--rw-r--r--   0 root         (0) root         (0)     2045 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/.codacy.yml
--rw-r--r--   0 root         (0) root         (0)      884 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     8332 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    35141 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      192 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3603 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/example_notebooks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/example_notebooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39193 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/example_notebooks/example.ipynb
--rw-r--r--   0 root         (0) root         (0)    35263 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/example_notebooks/feature_subset_example.ipynb
--rw-r--r--   0 root         (0) root         (0)    20806 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/example_notebooks/multimodel_example.ipynb
--rw-r--r--   0 root         (0) root         (0)     1147 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      458 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1719 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1437 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_account_cluster_transformer.py
--rw-r--r--   0 root         (0) root         (0)     5926 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     1436 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_custom_cluster_transformer.py
--rw-r--r--   0 root         (0) root         (0)     5596 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_feature_subset.py
--rw-r--r--   0 root         (0) root         (0)     6262 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_lw_cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     1471 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_ml_helpers.py
--rw-r--r--   0 root         (0) root         (0)     5488 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_multi_model.py
--rw-r--r--   0 root         (0) root         (0)     3483 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_multi_transformer.py
--rw-r--r--   0 root         (0) root         (0)      877 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_phasing_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2244 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_prediction_model.py
--rw-r--r--   0 root         (0) root         (0)     4637 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_preprocessing.py
--rw-r--r--   0 root         (0) root         (0)      707 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/tests/test_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics/
--rw-r--r--   0 root         (0) root         (0)      167 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13085 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     1258 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4864 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/feature_subset.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/lw_cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     7390 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/ml_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6939 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/model.py
--rw-r--r--   0 root         (0) root         (0)    12096 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/multi_model.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/tool.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-03-26 07:50:23.000000 vf_portalytics-1.1.1/vf_portalytics/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3603 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1209 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 07:50:28.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      721 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-26 07:52:27.000000 vf_portalytics-1.1.1/vf_portalytics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/.codacy.yml
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     8383 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    35141 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3581 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/example_notebooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39193 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/example.ipynb
+-rw-r--r--   0 root         (0) root         (0)    35263 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/feature_subset_example.ipynb
+-rw-r--r--   0 root         (0) root         (0)    20806 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/multimodel_example.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_account_cluster_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_custom_cluster_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_feature_subset.py
+-rw-r--r--   0 root         (0) root         (0)     6262 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_lw_cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_ml_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5577 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_multi_model.py
+-rw-r--r--   0 root         (0) root         (0)     3483 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_multi_transformer.py
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_phasing_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_prediction_model.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics/
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13085 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/feature_subset.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/lw_cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     7390 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/ml_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/model.py
+-rw-r--r--   0 root         (0) root         (0)    12096 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/multi_model.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3581 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/top_level.txt
```

### Comparing `vf_portalytics-1.1.1/.circleci/config.yml` & `vf_portalytics-1.1.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/AUTHORS` & `vf_portalytics-1.1.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/ChangeLog` & `vf_portalytics-1.1.2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.1.2
+-----
+
+* Depreciate xgboost
+* Speedup tests
+
 1.1.1
 -----
 
 * Speedup tests
 * Sudo
 * Use api token to connect to pypi
```

### Comparing `vf_portalytics-1.1.1/LICENSE` & `vf_portalytics-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/PKG-INFO` & `vf_portalytics-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf_portalytics
-Version: 1.1.1
+Version: 1.1.2
 Summary: A consistent interface for creating Machine Learning Models compatible with VisualFabriq environment
 Home-page: https://github.com/visualfabriq/portalytics
 Author: Carst Vaartjes
 Author-email: cvaartjes@visualfabriq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=2.7
 License-File: LICENSE
-License-File: AUTHORS
 
 # portalytics
 Portable Jupyter Setup for Machine Learning.
 
 A consistent interface for creating Machine Learning Models compatible with VisualFabriq environment.
 
 Build models using our portalytics module.
```

### Comparing `vf_portalytics-1.1.1/README.md` & `vf_portalytics-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/example_notebooks/example.ipynb` & `vf_portalytics-1.1.2/example_notebooks/example.ipynb`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/example_notebooks/feature_subset_example.ipynb` & `vf_portalytics-1.1.2/example_notebooks/feature_subset_example.ipynb`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/example_notebooks/multimodel_example.ipynb` & `vf_portalytics-1.1.2/example_notebooks/multimodel_example.ipynb`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/requirements.txt` & `vf_portalytics-1.1.2/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 seaborn==0.9.1; python_version <= "2.7"
 seaborn>=0.10.1; python_version > "3.3"
 # the prediction libraries;
 # sklearn is pinned because if a user pickles a model with a different version, the unpickling creates issues
 scikit-learn==0.20.4; python_version < "3.10"
 scikit-learn==1.1.3; python_version >= "3.10"
 xgboost==0.82; python_version <= "2.7"
-xgboost==1.5.2; python_version > "3.3"
+xgboost==0.82; python_version > "3.3"
 statsmodels==0.10.2; python_version <= "2.7"
 statsmodels>=0.12.0; python_version > "3.3"
 pytest>=5.3.5; python_version > '3.3'
 pytest==4.6.9; python_version <= '2.7'
 pytest-cov==2.8.1
```

### Comparing `vf_portalytics-1.1.1/setup.cfg` & `vf_portalytics-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/helpers.py` & `vf_portalytics-1.1.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_account_cluster_transformer.py` & `vf_portalytics-1.1.2/tests/test_account_cluster_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_cluster_model.py` & `vf_portalytics-1.1.2/tests/test_cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_custom_cluster_transformer.py` & `vf_portalytics-1.1.2/tests/test_custom_cluster_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_feature_subset.py` & `vf_portalytics-1.1.2/tests/test_feature_subset.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_lw_cluster_model.py` & `vf_portalytics-1.1.2/tests/test_lw_cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_ml_helpers.py` & `vf_portalytics-1.1.2/tests/test_ml_helpers.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_multi_model.py` & `vf_portalytics-1.1.2/tests/test_multi_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     ordinal_features = ['feature_1']
 
     # imitate params given from hyper optimization tuning
     params = {
         'A': {
             'model_name': 'XGBRegressor',
             'transformer_nominal': 'TargetEncoder',
+            'n_estimators': 3,
             'transformer_ordinal': 'OrdinalEncoder'
         },
         'B': {
             'model_name': 'XGBRegressor',
+            'n_estimators': 3,
             'transformer_nominal': 'TargetEncoder',
             'transformer_ordinal': 'OrdinalEncoder'
         }
     }
 
     # Initialize model
     model = MultiModel(group_col=cat_feature, clusters=clusters, params=params,
@@ -76,14 +78,15 @@
     nominal_features = ['feature_0']
     ordinal_features = ['feature_1']
 
     # imitate params given from hyper optimization tuning
     params = {
         'group_0': {
             'model_name': 'XGBRegressor',
+            'n_estimators': 5,
             'transformer_nominal': 'TargetEncoder',
             'transformer_ordinal': 'OrdinalEncoder'},
     }
 
 
     # Initiliaze model
     model = MultiModel(group_col=cat_feature, clusters=clusters, params=params,
@@ -124,31 +127,31 @@
     params = {
         'A': {
             'model_name': 'XGBRegressorChain',
             'order': [0, 1],
             'max_depth': 2,
             'min_samples_leaf': 400,
             'min_samples_split': 400,
-            'n_estimators': 11,
+            'n_estimators': 6,
             'transformer_nominal': 'TargetEncoder',
             'transformer_ordinal': 'OrdinalEncoder'
         },
         'B': {
             'model_name': 'ExtraTreesRegressor',
             'max_depth': 2,
             'min_samples_leaf': 400,
             'min_samples_split': 400,
-            'n_estimators': 10,
+            'n_estimators': 5,
             'transformer_nominal': 'TargetEncoder',
             'transformer_ordinal': 'OrdinalEncoder'
         }
     }
 
     # Initiliaze model
     model = MultiModel(group_col=cat_feature, clusters=clusters, params=params,
                        selected_features=selected_features, nominals=nominal_features, ordinals=ordinal_features)
     model.fit(train_x, train_y)
     pred_test_y = model.predict(test_x)
 
     assert pred_test_y.shape[1] == 2
-    assert model.sub_models['B'].n_estimators == 10
-    assert model.sub_models['A'].base_estimator.n_estimators == 11
+    assert model.sub_models['B'].n_estimators == 5
+    assert model.sub_models['A'].base_estimator.n_estimators == 6
```

### Comparing `vf_portalytics-1.1.1/tests/test_multi_transformer.py` & `vf_portalytics-1.1.2/tests/test_multi_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_phasing_transformer.py` & `vf_portalytics-1.1.2/tests/test_phasing_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_prediction_model.py` & `vf_portalytics-1.1.2/tests/test_prediction_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_preprocessing.py` & `vf_portalytics-1.1.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/tests/test_tool.py` & `vf_portalytics-1.1.2/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/cluster_model.py` & `vf_portalytics-1.1.2/vf_portalytics/cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/dataset.py` & `vf_portalytics-1.1.2/vf_portalytics/dataset.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/feature_subset.py` & `vf_portalytics-1.1.2/vf_portalytics/feature_subset.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/lw_cluster_model.py` & `vf_portalytics-1.1.2/vf_portalytics/lw_cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/ml_helpers.py` & `vf_portalytics-1.1.2/vf_portalytics/ml_helpers.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/model.py` & `vf_portalytics-1.1.2/vf_portalytics/model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/multi_model.py` & `vf_portalytics-1.1.2/vf_portalytics/multi_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/tool.py` & `vf_portalytics-1.1.2/vf_portalytics/tool.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics/viz.py` & `vf_portalytics-1.1.2/vf_portalytics/viz.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics.egg-info/PKG-INFO` & `vf_portalytics-1.1.2/vf_portalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf-portalytics
-Version: 1.1.1
+Version: 1.1.2
 Summary: A consistent interface for creating Machine Learning Models compatible with VisualFabriq environment
 Home-page: https://github.com/visualfabriq/portalytics
 Author: Carst Vaartjes
 Author-email: cvaartjes@visualfabriq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=2.7
 License-File: LICENSE
-License-File: AUTHORS
 
 # portalytics
 Portable Jupyter Setup for Machine Learning.
 
 A consistent interface for creating Machine Learning Models compatible with VisualFabriq environment.
 
 Build models using our portalytics module.
```

### Comparing `vf_portalytics-1.1.1/vf_portalytics.egg-info/SOURCES.txt` & `vf_portalytics-1.1.2/vf_portalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.1/vf_portalytics.egg-info/requires.txt` & `vf_portalytics-1.1.2/vf_portalytics.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 numpy>=1.19.1
 
 [:(python_version > "3.3")]
 pandas~=1.1
 numexpr>=2.7.1
 matplotlib>=3.1.2
 seaborn>=0.10.1
-xgboost==1.5.2
+xgboost==0.82
 statsmodels>=0.12.0
 
 [:(python_version > '3.3')]
 pytest>=5.3.5
 
 [:(python_version >= "3")]
 joblib~=1.2.0
```

