# Comparing `tmp/adaptive-1.1.0.tar.gz` & `tmp/adaptive-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive-1.1.0.tar", last modified: Mon Aug 14 18:53:55 2023, max compression
+gzip compressed data, was "adaptive-1.2.0.tar", last modified: Wed Apr 10 07:51:04 2024, max compression
```

## Comparing `adaptive-1.1.0.tar` & `adaptive-1.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 josephweston  (1000) josephweston  (1000)        0 2023-08-14 18:53:55.975729 adaptive-1.1.0/
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1227 2023-07-17 23:14:54.000000 adaptive-1.1.0/AUTHORS.md
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1521 2023-07-17 23:14:54.000000 adaptive-1.1.0/LICENSE
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)       16 2023-07-17 23:14:15.000000 adaptive-1.1.0/MANIFEST.in
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    11551 2023-08-14 18:53:55.975729 adaptive-1.1.0/PKG-INFO
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    10733 2023-07-17 23:14:54.000000 adaptive-1.1.0/README.md
-drwxr-xr-x   0 josephweston  (1000) josephweston  (1000)        0 2023-08-14 18:53:55.985729 adaptive-1.1.0/adaptive/
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1274 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/__init__.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)      110 2023-08-14 18:53:55.985729 adaptive-1.1.0/adaptive/_version.py
-drwxr-xr-x   0 josephweston  (1000) josephweston  (1000)        0 2023-08-14 18:53:55.975729 adaptive-1.1.0/adaptive/learner/
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1052 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/__init__.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     8700 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/average_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    26147 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/average_learner1D.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    21987 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/balancing_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     7642 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/base_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     7534 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/data_saver.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     6671 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/integrator_coeffs.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    23367 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/integrator_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    33332 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/learner1D.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    31038 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/learner2D.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    45314 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/learnerND.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     9773 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/sequence_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     6005 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/skopt_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    24593 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/learner/triangulation.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     8854 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/notebook_integration.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    43879 2023-08-01 20:34:58.000000 adaptive-1.1.0/adaptive/runner.py
-drwxr-xr-x   0 josephweston  (1000) josephweston  (1000)        0 2023-08-14 18:53:55.975729 adaptive-1.1.0/adaptive/tests/
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)        0 2023-07-17 23:14:15.000000 adaptive-1.1.0/adaptive/tests/__init__.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    19299 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/algorithm_4.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     2187 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_average_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     2166 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_average_learner1d.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     2201 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_balancing_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     8704 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_cquad.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    12699 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_learner1d.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1669 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_learnernd.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    24883 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_learners.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1034 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_notebook_integration.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     2793 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_pickling.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     5876 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_runner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1707 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_sequence_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1452 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_skopt_learner.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    10004 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/test_triangulation.py
-drwxr-xr-x   0 josephweston  (1000) josephweston  (1000)        0 2023-08-14 18:53:55.975729 adaptive-1.1.0/adaptive/tests/unit/
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)        0 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/unit/__init__.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1318 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/unit/test_learnernd.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1843 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/unit/test_learnernd_integration.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     3338 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/tests/unit/test_triangulation.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)      374 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/types.py
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     6076 2023-07-17 23:14:54.000000 adaptive-1.1.0/adaptive/utils.py
-drwxr-xr-x   0 josephweston  (1000) josephweston  (1000)        0 2023-08-14 18:53:55.975729 adaptive-1.1.0/adaptive.egg-info/
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)    11551 2023-08-14 18:53:55.000000 adaptive-1.1.0/adaptive.egg-info/PKG-INFO
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     1518 2023-08-14 18:53:55.000000 adaptive-1.1.0/adaptive.egg-info/SOURCES.txt
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)        1 2023-08-14 18:53:55.000000 adaptive-1.1.0/adaptive.egg-info/dependency_links.txt
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)      484 2023-08-14 18:53:55.000000 adaptive-1.1.0/adaptive.egg-info/requires.txt
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)        9 2023-08-14 18:53:55.000000 adaptive-1.1.0/adaptive.egg-info/top_level.txt
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)     3521 2023-07-17 23:14:54.000000 adaptive-1.1.0/pyproject.toml
--rw-r--r--   0 josephweston  (1000) josephweston  (1000)      141 2023-08-14 18:53:55.975729 adaptive-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.332553 adaptive-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-10 07:50:51.000000 adaptive-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-10 07:50:51.000000 adaptive-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 07:50:51.000000 adaptive-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-10 07:51:04.332553 adaptive-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10733 2024-04-10 07:50:51.000000 adaptive-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.336553 adaptive-1.2.0/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 07:51:04.336553 adaptive-1.2.0/adaptive/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.328553 adaptive-1.2.0/adaptive/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/average_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/average_learner1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21987 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/balancing_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/base_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/data_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/integrator_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/integrator_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33353 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/learner1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31038 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/learner2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45362 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/learnerND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/skopt_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24593 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/learner/triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/notebook_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47162 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.328553 adaptive-1.2.0/adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/algorithm_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_average_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_average_learner1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_balancing_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_cquad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_learner1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_learnernd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24883 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_learners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_notebook_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_skopt_learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/test_triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.332553 adaptive-1.2.0/adaptive/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/test_learnernd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/test_learnernd_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/tests/unit/test_triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-10 07:50:51.000000 adaptive-1.2.0/adaptive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:51:04.332553 adaptive-1.2.0/adaptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 07:51:04.000000 adaptive-1.2.0/adaptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-10 07:50:51.000000 adaptive-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 07:51:04.332553 adaptive-1.2.0/setup.cfg
```

### Comparing `adaptive-1.1.0/AUTHORS.md` & `adaptive-1.2.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/LICENSE` & `adaptive-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/PKG-INFO` & `adaptive-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: adaptive
-Version: 1.1.0
-Summary: Parallel active learning of mathematical functions
-Maintainer: Adaptive authors
-License: BSD
-Project-URL: homepage, https://adaptive.readthedocs.io/
-Project-URL: documentation, https://adaptive.readthedocs.io/
-Project-URL: repository, https://github.com/python-adaptive/adaptive
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: other
-Provides-Extra: notebook
-Provides-Extra: testing
-License-File: LICENSE
-License-File: AUTHORS.md
-
 
 # ![logo](https://adaptive.readthedocs.io/en/latest/_static/logo.png) *Adaptive*: Parallel Active Learning of Mathematical Functions :brain::1234:
 <!-- badges-start -->
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/python-adaptive/adaptive/main?filepath=example-notebook.ipynb)
 [![Conda](https://img.shields.io/badge/install%20with-conda-green.svg)](https://anaconda.org/conda-forge/adaptive)
 [![Coverage](https://img.shields.io/codecov/c/github/python-adaptive/adaptive)](https://codecov.io/gh/python-adaptive/adaptive)
```

### Comparing `adaptive-1.1.0/README.md` & `adaptive-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,61 @@
+Metadata-Version: 2.1
+Name: adaptive
+Version: 1.2.0
+Summary: Parallel active learning of mathematical functions
+Maintainer: Adaptive authors
+License: BSD
+Project-URL: homepage, https://adaptive.readthedocs.io/
+Project-URL: documentation, https://adaptive.readthedocs.io/
+Project-URL: repository, https://github.com/python-adaptive/adaptive
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: scipy
+Requires-Dist: sortedcollections>=1.1
+Requires-Dist: sortedcontainers>=2.0
+Requires-Dist: cloudpickle
+Requires-Dist: loky>=2.9
+Requires-Dist: typing_extensions; python_version < "3.10"
+Requires-Dist: versioningit
+Provides-Extra: other
+Requires-Dist: dill; extra == "other"
+Requires-Dist: distributed; extra == "other"
+Requires-Dist: ipyparallel>=6.2.5; extra == "other"
+Requires-Dist: scikit-optimize>=0.8.1; extra == "other"
+Requires-Dist: scikit-learn; extra == "other"
+Requires-Dist: wexpect; os_name == "nt" and extra == "other"
+Requires-Dist: pexpect; os_name != "nt" and extra == "other"
+Provides-Extra: notebook
+Requires-Dist: ipython; extra == "notebook"
+Requires-Dist: ipykernel>=4.8.0; extra == "notebook"
+Requires-Dist: jupyter_client>=5.2.2; extra == "notebook"
+Requires-Dist: holoviews>=1.9.1; extra == "notebook"
+Requires-Dist: ipywidgets; extra == "notebook"
+Requires-Dist: bokeh; extra == "notebook"
+Requires-Dist: pandas; extra == "notebook"
+Requires-Dist: matplotlib; extra == "notebook"
+Requires-Dist: plotly; extra == "notebook"
+Provides-Extra: testing
+Requires-Dist: flaky; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-randomly; extra == "testing"
+Requires-Dist: pytest-timeout; extra == "testing"
+Requires-Dist: pre_commit; extra == "testing"
+Requires-Dist: typeguard; extra == "testing"
+
 
 # ![logo](https://adaptive.readthedocs.io/en/latest/_static/logo.png) *Adaptive*: Parallel Active Learning of Mathematical Functions :brain::1234:
 <!-- badges-start -->
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/python-adaptive/adaptive/main?filepath=example-notebook.ipynb)
 [![Conda](https://img.shields.io/badge/install%20with-conda-green.svg)](https://anaconda.org/conda-forge/adaptive)
 [![Coverage](https://img.shields.io/codecov/c/github/python-adaptive/adaptive)](https://codecov.io/gh/python-adaptive/adaptive)
```

### Comparing `adaptive-1.1.0/adaptive/__init__.py` & `adaptive-1.2.0/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/__init__.py` & `adaptive-1.2.0/adaptive/learner/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/average_learner.py` & `adaptive-1.2.0/adaptive/learner/average_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/average_learner1D.py` & `adaptive-1.2.0/adaptive/learner/average_learner1D.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         return points, loss_improvements
 
     def _ask_for_new_point(self, n: int) -> tuple[Points, list[float]]:
         """When asking for n new points, the learner returns n times a single
         new point, since in general n << min_samples and this point will need
         to be resampled many more times"""
         points, (loss_improvement,) = self._ask_points_without_adding(1)
-        seed_points = [(seed, x) for seed, x in zip(range(n), n * points)]
+        seed_points = list(zip(range(n), n * points))
         loss_improvements = [loss_improvement / n] * n
         return seed_points, loss_improvements  # type: ignore[return-value]
 
     def tell_pending(self, seed_x: Point) -> None:  # type: ignore[override]
         _, x = seed_x
         self.pending_points.add(seed_x)
         if x not in self.data:
```

### Comparing `adaptive-1.1.0/adaptive/learner/balancing_learner.py` & `adaptive-1.2.0/adaptive/learner/balancing_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/base_learner.py` & `adaptive-1.2.0/adaptive/learner/base_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/data_saver.py` & `adaptive-1.2.0/adaptive/learner/data_saver.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/integrator_coeffs.py` & `adaptive-1.2.0/adaptive/learner/integrator_coeffs.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/integrator_learner.py` & `adaptive-1.2.0/adaptive/learner/integrator_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
 
 class DivergentIntegralError(ValueError):
     pass
 
 
 class _Interval:
-
     """
     Attributes
     ----------
     (a, b) : (float, float)
         The left and right boundary of the interval.
     c : numpy array of shape (4, 33)
         Coefficients of the fit.
```

### Comparing `adaptive-1.1.0/adaptive/learner/learner1D.py` & `adaptive-1.2.0/adaptive/learner/learner1D.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         return xs[1] - xs[0]  # type: ignore[operator]
 
     N = len(xs) - 2  # number of constructed triangles
     if isinstance(ys[0], collections.abc.Iterable):
         pts = [(x, *y) for x, y in zip(xs, ys)]  # type: ignore[misc]
         vol = simplex_volume_in_embedding
     else:
-        pts = [(x, y) for x, y in zip(xs, ys)]
+        pts = list(zip(xs, ys))
         vol = volume
     return sum(vol(pts[i : i + 3]) for i in range(N)) / N
 
 
 def resolution_loss_function(
     min_length: Real = 0, max_length: Real = 1
 ) -> Callable[[XsType0, YsType0], Float]:
@@ -629,18 +629,20 @@
         self.pending_points.add(x)
         self._update_neighbors(x, self.neighbors_combined)
         self._update_losses(x, real=False)
 
     def tell_many(
         self,
         xs: Sequence[Float] | np.ndarray,
-        ys: Sequence[Float]
-        | Sequence[Sequence[Float]]
-        | Sequence[np.ndarray]
-        | np.ndarray,
+        ys: (
+            Sequence[Float]
+            | Sequence[Sequence[Float]]
+            | Sequence[np.ndarray]
+            | np.ndarray
+        ),
         *,
         force: bool = False,
     ) -> None:
         if not force and not (len(xs) > 0.5 * len(self.data) and len(xs) > 2):
             # Only run this more efficient method if there are
             # at least 2 points and the amount of points added are
             # at least half of the number of points already in 'data'.
```

### Comparing `adaptive-1.1.0/adaptive/learner/learner2D.py` & `adaptive-1.2.0/adaptive/learner/learner2D.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/learnerND.py` & `adaptive-1.2.0/adaptive/learner/learnerND.py`

 * *Files 0% similar despite different names*

```diff
@@ -983,17 +983,19 @@
                 scale_factor = np.product(np.diag(self._transform))
                 a_sq = np.sqrt(np.min(self.tri.volumes()) * scale_factor)
                 n = max(10, int(0.658 / a_sq))
 
             xs = ys = np.linspace(0, 1, n)
             xys = [xs[:, None], ys[None, :]]
             values = [
-                cut_mapping[i]
-                if i in cut_mapping
-                else xys.pop(0) * (b[1] - b[0]) + b[0]
+                (
+                    cut_mapping[i]
+                    if i in cut_mapping
+                    else xys.pop(0) * (b[1] - b[0]) + b[0]
+                )
                 for i, b in enumerate(self._bbox)
             ]
 
             lbrt = [b for i, b in enumerate(self._bbox) if i not in cut_mapping]
             lbrt = np.reshape(lbrt, (2, 2)).T.flatten().tolist()
 
             if len(self.data) >= 4:
```

### Comparing `adaptive-1.1.0/adaptive/learner/sequence_learner.py` & `adaptive-1.2.0/adaptive/learner/sequence_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/skopt_learner.py` & `adaptive-1.2.0/adaptive/learner/skopt_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/learner/triangulation.py` & `adaptive-1.2.0/adaptive/learner/triangulation.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/notebook_integration.py` & `adaptive-1.2.0/adaptive/notebook_integration.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/runner.py` & `adaptive-1.2.0/adaptive/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,15 +466,15 @@
         learner: LearnerType,
         goal: Callable[[LearnerType], bool] | None = None,
         *,
         loss_goal: float | None = None,
         npoints_goal: int | None = None,
         end_time_goal: datetime | None = None,
         duration_goal: timedelta | int | float | None = None,
-        executor: (ExecutorTypes | None) = None,
+        executor: ExecutorTypes | None = None,
         ntasks: int | None = None,
         log: bool = False,
         shutdown_executor: bool = False,
         retries: int = 0,
         raise_if_retries_exceeded: bool = True,
     ) -> None:
         if inspect.iscoroutinefunction(learner.function):
@@ -625,15 +625,15 @@
         learner: LearnerType,
         goal: Callable[[LearnerType], bool] | None = None,
         *,
         loss_goal: float | None = None,
         npoints_goal: int | None = None,
         end_time_goal: datetime | None = None,
         duration_goal: timedelta | int | float | None = None,
-        executor: (ExecutorTypes | None) = None,
+        executor: ExecutorTypes | None = None,
         ntasks: int | None = None,
         log: bool = False,
         shutdown_executor: bool = False,
         ioloop=None,
         retries: int = 0,
         raise_if_retries_exceeded: bool = True,
     ) -> None:
@@ -718,14 +718,22 @@
     def cancel(self) -> None:
         """Cancel the runner.
 
         This is equivalent to calling ``runner.task.cancel()``.
         """
         self.task.cancel()
 
+    def block_until_done(self) -> None:
+        if in_ipynb():
+            raise RuntimeError(
+                "Cannot block the event loop when running in a Jupyter notebook."
+                " Use `await runner.task` instead."
+            )
+        self.ioloop.run_until_complete(self.task)
+
     def live_plot(
         self,
         *,
         plotter: Callable[[LearnerType], holoviews.Element] | None = None,
         update_interval: float = 2.0,
         name: str | None = None,
         normalize: bool = True,
@@ -764,14 +772,64 @@
         """Display live information about the runner.
 
         Returns an interactive ipywidget that can be
         visualized in a Jupyter notebook.
         """
         return live_info(self, update_interval=update_interval)
 
+    def live_info_terminal(
+        self, *, update_interval: float = 0.5, overwrite_previous: bool = True
+    ) -> asyncio.Task:
+        """
+        Display live information about the runner in the terminal.
+
+        This function provides a live update of the runner's status in the terminal.
+        The update can either overwrite the previous status or be printed on a new line.
+
+        Parameters
+        ----------
+        update_interval : float, optional
+            The time interval (in seconds) at which the runner's status is updated
+            in the terminal. Default is 0.5 seconds.
+        overwrite_previous : bool, optional
+            If True, each update will overwrite the previous status in the terminal.
+            If False, each update will be printed on a new line.
+            Default is True.
+
+        Returns
+        -------
+        asyncio.Task
+            The asynchronous task responsible for updating the runner's status in
+            the terminal.
+
+        Examples
+        --------
+        >>> runner = AsyncRunner(...)
+        >>> runner.live_info_terminal(update_interval=1.0, overwrite_previous=False)
+
+        Notes
+        -----
+        This function uses ANSI escape sequences to control the terminal's cursor
+        position. It might not work as expected on all terminal emulators.
+        """
+
+        async def _update(runner: AsyncRunner) -> None:
+            try:
+                while not runner.task.done():
+                    if overwrite_previous:
+                        # Clear the terminal
+                        print("\033[H\033[J", end="")
+                    print(_info_text(runner, separator="\t"))
+                    await asyncio.sleep(update_interval)
+
+            except asyncio.CancelledError:
+                print("Live info display cancelled.")
+
+        return self.ioloop.create_task(_update(self))
+
     async def _run(self) -> None:
         first_completed = asyncio.FIRST_COMPLETED
 
         if self._get_max_tasks() < 1:
             raise RuntimeError("Executor has no workers")
 
         try:
@@ -843,14 +901,51 @@
                 await asyncio.wait([self.task], timeout=interval)
             method(self.learner)  # one last time
 
         self.saving_task = self.ioloop.create_task(_saver())
         return self.saving_task
 
 
+def _info_text(runner, separator: str = "\n"):
+    status = runner.status()
+
+    color_map = {
+        "cancelled": "\033[33m",  # Yellow
+        "failed": "\033[31m",  # Red
+        "running": "\033[34m",  # Blue
+        "finished": "\033[32m",  # Green
+    }
+
+    overhead = runner.overhead()
+    if overhead < 50:
+        overhead_color = "\033[32m"  # Green
+    else:
+        overhead_color = "\033[31m"  # Red
+
+    info = [
+        ("time", str(datetime.now())),
+        ("status", f"{color_map[status]}{status}\033[0m"),
+        ("elapsed time", str(timedelta(seconds=runner.elapsed_time()))),
+        ("overhead", f"{overhead_color}{overhead:.2f}%\033[0m"),
+    ]
+
+    with suppress(Exception):
+        info.append(("# of points", runner.learner.npoints))
+
+    with suppress(Exception):
+        info.append(("# of samples", runner.learner.nsamples))
+
+    with suppress(Exception):
+        info.append(("latest loss", f'{runner.learner._cache["loss"]:.3f}'))
+
+    width = 30
+    formatted_info = [f"{k}: {v}".ljust(width) for i, (k, v) in enumerate(info)]
+    return separator.join(formatted_info)
+
+
 # Default runner
 Runner = AsyncRunner
 
 
 def simple(
     learner: LearnerType,
     goal: Callable[[LearnerType], bool] | None = None,
@@ -952,15 +1047,15 @@
             # TODO: check if this is correct. Isn't MPI,loky supported?
             "Only a concurrent.futures.Executor, distributed.Client,"
             " or ipyparallel.Client can be used."
         )
 
 
 def _get_ncores(
-    ex: (ExecutorTypes),
+    ex: ExecutorTypes,
 ) -> int:
     """Return the maximum  number of cores that an executor can use."""
     if with_ipyparallel:
         import ipyparallel
     if with_distributed:
         import distributed
     if with_mpi4py:
@@ -1091,15 +1186,16 @@
                 end_time=end_time,
                 duration=duration,
                 allow_running_forever=allow_running_forever,
             )
             for lrn in learner.learners
         ]
         return lambda learner: all(
-            goal(lrn) for lrn, goal in zip(learner.learners, goals)  # type: ignore[attr-defined]
+            goal(lrn)
+            for lrn, goal in zip(learner.learners, goals)  # type: ignore[attr-defined]
         )
     if npoints is not None:
         return lambda learner: learner.npoints >= npoints  # type: ignore[operator]
     if end_time is not None:
         return _TimeGoal(end_time)
     if duration is not None:
         return _TimeGoal(duration)
```

### Comparing `adaptive-1.1.0/adaptive/tests/algorithm_4.py` & `adaptive-1.2.0/adaptive/tests/algorithm_4.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,19 @@
         fx[1 : n[depth] - 1 : 2] = f(points[1 : n[depth] - 1 : 2])
         self.fx = fx
         split = self.calc_igral_and_err(self.c) > hint * norm(self.c)
         return points, split, n[depth] - n[depth - 1]
 
 
 def algorithm_4(
-    f: Callable, a: int, b: int, tol: float, N_loops: int = int(1e9)  # noqa: B008
+    f: Callable,
+    a: int,
+    b: int,
+    tol: float,
+    N_loops: int = int(1e9),  # noqa: B008
 ) -> tuple[float, float, int, list[_Interval]]:
     """ALGORITHM_4 evaluates an integral using adaptive quadrature. The
     algorithm uses Clenshaw-Curtis quadrature rules of increasing
     degree in each interval and bisects the interval if either the
     function does not appear to be smooth or a rule of maximum degree
     has been reached. The error estimate is computed from the L2-norm
     of the difference between two successive interpolations of the
```

### Comparing `adaptive-1.1.0/adaptive/tests/test_average_learner.py` & `adaptive-1.2.0/adaptive/tests/test_average_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_average_learner1d.py` & `adaptive-1.2.0/adaptive/tests/test_average_learner1d.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_balancing_learner.py` & `adaptive-1.2.0/adaptive/tests/test_balancing_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_cquad.py` & `adaptive-1.2.0/adaptive/tests/test_cquad.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_learner1d.py` & `adaptive-1.2.0/adaptive/tests/test_learner1d.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_learnernd.py` & `adaptive-1.2.0/adaptive/tests/test_learnernd.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_learners.py` & `adaptive-1.2.0/adaptive/tests/test_learners.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_notebook_integration.py` & `adaptive-1.2.0/adaptive/tests/test_notebook_integration.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_pickling.py` & `adaptive-1.2.0/adaptive/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_runner.py` & `adaptive-1.2.0/adaptive/tests/test_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import platform
 import sys
 import time
 
 import numpy as np
 import pytest
 
@@ -30,15 +29,15 @@
 
 def blocking_runner(learner, **kw):
     BlockingRunner(learner, executor=SequentialExecutor(), **kw)
 
 
 def async_runner(learner, **kw):
     runner = AsyncRunner(learner, executor=SequentialExecutor(), **kw)
-    asyncio.get_event_loop().run_until_complete(runner.task)
+    runner.block_until_done()
 
 
 runners = [simple, blocking_runner, async_runner]
 
 
 @pytest.mark.parametrize("runner", runners)
 def test_simple(runner):
@@ -67,15 +66,15 @@
 
 def test_aync_def_function():
     async def f(x):
         return x
 
     learner = Learner1D(f, (-1, 1))
     runner = AsyncRunner(learner, npoints_goal=10)
-    asyncio.get_event_loop().run_until_complete(runner.task)
+    runner.block_until_done()
 
 
 # --- Test with different executors
 
 
 @pytest.fixture(scope="session")
 def loky_executor():
@@ -154,15 +153,15 @@
     )
     assert learner.npoints > 0
 
 
 def test_default_executor():
     learner = Learner1D(linear, (-1, 1))
     runner = AsyncRunner(learner, npoints_goal=10)
-    asyncio.get_event_loop().run_until_complete(runner.task)
+    runner.block_until_done()
 
 
 def test_auto_goal():
     learner = Learner1D(linear, (-1, 1))
     simple(learner, auto_goal(npoints=4))
     assert learner.npoints == 4
```

### Comparing `adaptive-1.1.0/adaptive/tests/test_sequence_learner.py` & `adaptive-1.2.0/adaptive/tests/test_sequence_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_skopt_learner.py` & `adaptive-1.2.0/adaptive/tests/test_skopt_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/test_triangulation.py` & `adaptive-1.2.0/adaptive/tests/test_triangulation.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/unit/test_learnernd.py` & `adaptive-1.2.0/adaptive/tests/unit/test_learnernd.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/unit/test_learnernd_integration.py` & `adaptive-1.2.0/adaptive/tests/unit/test_learnernd_integration.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/tests/unit/test_triangulation.py` & `adaptive-1.2.0/adaptive/tests/unit/test_triangulation.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive/utils.py` & `adaptive-1.2.0/adaptive/utils.py`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/adaptive.egg-info/PKG-INFO` & `adaptive-1.2.0/adaptive.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,60 @@
 Metadata-Version: 2.1
 Name: adaptive
-Version: 1.1.0
+Version: 1.2.0
 Summary: Parallel active learning of mathematical functions
 Maintainer: Adaptive authors
 License: BSD
 Project-URL: homepage, https://adaptive.readthedocs.io/
 Project-URL: documentation, https://adaptive.readthedocs.io/
 Project-URL: repository, https://github.com/python-adaptive/adaptive
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: scipy
+Requires-Dist: sortedcollections>=1.1
+Requires-Dist: sortedcontainers>=2.0
+Requires-Dist: cloudpickle
+Requires-Dist: loky>=2.9
+Requires-Dist: typing_extensions; python_version < "3.10"
+Requires-Dist: versioningit
 Provides-Extra: other
+Requires-Dist: dill; extra == "other"
+Requires-Dist: distributed; extra == "other"
+Requires-Dist: ipyparallel>=6.2.5; extra == "other"
+Requires-Dist: scikit-optimize>=0.8.1; extra == "other"
+Requires-Dist: scikit-learn; extra == "other"
+Requires-Dist: wexpect; os_name == "nt" and extra == "other"
+Requires-Dist: pexpect; os_name != "nt" and extra == "other"
 Provides-Extra: notebook
+Requires-Dist: ipython; extra == "notebook"
+Requires-Dist: ipykernel>=4.8.0; extra == "notebook"
+Requires-Dist: jupyter_client>=5.2.2; extra == "notebook"
+Requires-Dist: holoviews>=1.9.1; extra == "notebook"
+Requires-Dist: ipywidgets; extra == "notebook"
+Requires-Dist: bokeh; extra == "notebook"
+Requires-Dist: pandas; extra == "notebook"
+Requires-Dist: matplotlib; extra == "notebook"
+Requires-Dist: plotly; extra == "notebook"
 Provides-Extra: testing
-License-File: LICENSE
-License-File: AUTHORS.md
+Requires-Dist: flaky; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-randomly; extra == "testing"
+Requires-Dist: pytest-timeout; extra == "testing"
+Requires-Dist: pre_commit; extra == "testing"
+Requires-Dist: typeguard; extra == "testing"
 
 
 # ![logo](https://adaptive.readthedocs.io/en/latest/_static/logo.png) *Adaptive*: Parallel Active Learning of Mathematical Functions :brain::1234:
 <!-- badges-start -->
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/python-adaptive/adaptive/main?filepath=example-notebook.ipynb)
 [![Conda](https://img.shields.io/badge/install%20with-conda-green.svg)](https://anaconda.org/conda-forge/adaptive)
```

### Comparing `adaptive-1.1.0/adaptive.egg-info/SOURCES.txt` & `adaptive-1.2.0/adaptive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive-1.1.0/pyproject.toml` & `adaptive-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools ~= 65.0.0", "versioningit ~= 2.2.0", "wheel"]
+requires = ["setuptools ~= 69.0.0", "versioningit ~= 3.0.0", "wheel"]
 
 [project]
 name = "adaptive"
 dynamic = ["version"]
 description = "Parallel active learning of mathematical functions"
 maintainers = [{ name = "Adaptive authors" }]
 license = { text = "BSD" }
@@ -12,14 +12,15 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "scipy",
     "sortedcollections >= 1.1",
     "sortedcontainers >= 2.0",
     "cloudpickle",
     "loky >= 2.9",
@@ -91,36 +92,39 @@
 output = ".coverage.xml"
 
 [tool.mypy]
 ignore_missing_imports = true
 python_version = "3.9"
 
 [tool.ruff]
-line-length = 150
+line-length = 88
 target-version = "py39"
+
+[tool.ruff.lint]
 select = ["B", "C", "E", "F", "W", "T", "B9", "I", "UP"]
 ignore = [
     "T20",     # flake8-print
     "ANN101",  # Missing type annotation for {name} in method
     "S101",    # Use of assert detected
     "PD901",   # df is a bad variable name. Be kinder to your future self.
     "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in {name}
     "D402",    # First line should not be the function's signature
     "PLW0603", # Using the global statement to update `X` is discouraged
     "D401",    # First line of docstring should be in imperative mood
+    "E501",    # Line too long
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.mccabe]
+max-complexity = 18
+
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["SLF001"]
 "ci/*" = ["INP001"]
 "tests/test_examples.py" = ["E501"]
 
-[tool.ruff.mccabe]
-max-complexity = 18
-
 [tool.versioningit]
 
 [tool.versioningit.vcs]
 method = "git"
 match = ["v*"]
 default-tag = "0.0.0"
```

