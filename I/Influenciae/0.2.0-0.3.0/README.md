# Comparing `tmp/Influenciae-0.2.0.tar.gz` & `tmp/Influenciae-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Influenciae-0.2.0.tar", last modified: Wed Feb 22 14:57:30 2023, max compression
+gzip compressed data, was "Influenciae-0.3.0.tar", last modified: Wed Apr 10 08:58:19 2024, max compression
```

## Comparing `Influenciae-0.2.0.tar` & `Influenciae-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/Influenciae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-02-22 14:57:30.000000 Influenciae-0.2.0/Influenciae.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-22 14:57:30.000000 Influenciae-0.2.0/Influenciae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 14:57:30.000000 Influenciae-0.2.0/Influenciae.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-22 14:57:30.000000 Influenciae-0.2.0/Influenciae.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 14:57:30.000000 Influenciae-0.2.0/Influenciae.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-02-22 14:57:21.000000 Influenciae-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-02-22 14:57:30.135035 Influenciae-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-02-22 14:57:21.000000 Influenciae-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.131035 Influenciae-0.2.0/deel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/benchmark/base_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/benchmark/cifar10_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/benchmark/influence_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/benchmark/model_resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/boundary_based/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/boundary_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/boundary_based/sample_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/boundary_based/weights_boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/common/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/common/base_influence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/common/ihvp_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31065 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/common/inverse_hessian_vector_product.py
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/common/model_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/influence/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/influence/arnoldi_influence_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/influence/base_group_influence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/influence/first_order_influence_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/influence/second_order_influence_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/plots/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/plots/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/rps/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/rps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/rps/rps_l2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/rps/rps_lje.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/trac_in/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/trac_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/trac_in/tracin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/types/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:57:30.135035 Influenciae-0.2.0/deel/influenciae/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/utils/backtracking_line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/utils/conjugate_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/utils/nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/utils/sorted_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-02-22 14:57:21.000000 Influenciae-0.2.0/deel/influenciae/utils/tf_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 14:57:30.135035 Influenciae-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-02-22 14:57:21.000000 Influenciae-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.465691 Influenciae-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/Influenciae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17641 2024-04-10 08:58:19.000000 Influenciae-0.3.0/Influenciae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-10 08:58:19.000000 Influenciae-0.3.0/Influenciae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:58:19.000000 Influenciae-0.3.0/Influenciae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 08:58:19.000000 Influenciae-0.3.0/Influenciae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 08:58:19.000000 Influenciae-0.3.0/Influenciae.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-10 08:58:07.000000 Influenciae-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17641 2024-04-10 08:58:19.465691 Influenciae-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-04-10 08:58:07.000000 Influenciae-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.453691 Influenciae-0.3.0/deel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.457691 Influenciae-0.3.0/deel/influenciae/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.457691 Influenciae-0.3.0/deel/influenciae/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19551 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/benchmark/base_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/benchmark/cifar10_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19977 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/benchmark/influence_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19105 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/benchmark/model_resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.457691 Influenciae-0.3.0/deel/influenciae/boundary_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/boundary_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/boundary_based/sample_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/boundary_based/weights_boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.457691 Influenciae-0.3.0/deel/influenciae/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/common/base_influence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/common/ihvp_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31065 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/common/inverse_hessian_vector_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/common/model_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/deel/influenciae/influence/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/influence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/influence/arnoldi_influence_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/influence/base_group_influence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/influence/first_order_influence_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/influence/second_order_influence_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/deel/influenciae/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/plots/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/plots/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/deel/influenciae/rps/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/rps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/rps/base_representer_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/rps/rps_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/rps/rps_lje.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/deel/influenciae/trac_in/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/trac_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/trac_in/tracin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/deel/influenciae/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:58:19.461691 Influenciae-0.3.0/deel/influenciae/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/utils/backtracking_line_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/utils/conjugate_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/utils/nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/utils/sorted_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-04-10 08:58:07.000000 Influenciae-0.3.0/deel/influenciae/utils/tf_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:58:19.465691 Influenciae-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-10 08:58:07.000000 Influenciae-0.3.0/setup.py
```

### Comparing `Influenciae-0.2.0/Influenciae.egg-info/PKG-INFO` & `Influenciae-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,193 +1,196 @@
-Metadata-Version: 2.1
-Name: Influenciae
-Version: 0.2.0
-Summary: A Tensorflow Toolbox for Influence Functions
-Author: DEEL Core Team
-Author-email: agustin-martin.picard@irt-saintexupery.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
-<div align="center">
-    <img src="docs/assets/banner2.png" width="75%" alt="Influenciae" align="center" />
-</div>
-<br>
-
-<div align="center">
-    <a href="#">
-        <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9, 3.10-efefef">
-    </a>
-    <a href="#tf">
-        <img src="https://img.shields.io/badge/TensorFlow-2.7, 2.8, 2.9-00458A">
-    </a>
-    <a href="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml">
-        <img alt="PyLint" src="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml/badge.svg">
-    </a>
-    <a href="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml">
-        <img alt="Tox" src="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml/badge.svg">
-    </a>
-    <a href="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml">
-        <img alt="Pypi" src="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml/badge.svg">
-    </a>
-    <a href="#">
-        <img src="https://img.shields.io/badge/License-MIT-efefef">
-    </a>
-    <br>
-    <a href="https://deel-ai.github.io/influenciae/"><strong>Explore Influenciae docs »</strong></a>
-</div>
-<br>
-
-Influenciae is a Python toolkit dedicated to computing influence values for the discovery of potentially problematic samples in a dataset and the generation of data-centric explanations for deep learning models. In this library based on Tensorflow, we gather state-of-the-art methods for estimating the importance of training samples and their influence on test data-points for validating the quality of datasets and of the models trained on them.
-
-## 🔥 Tutorials
-
-We propose some hands-on tutorials to get familiar with the library and it's API:
-
-- [**Getting Started**](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
-- [**Benchmarking with Mislabeled sample detection**](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) </sub>
-- [**Using the first order influence calculator**](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) </sub>
-- [**Using the second order influence calculator**](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) </sub>
-- [**Using TracIn**](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) </sub>
-- [**Using Representer Point Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) </sub>
-- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) </sub>
-
-## 🚀 Quick Start
-
-Influenciae requires a version of python 3.7 or higher and several libraries, including Tensorflow and Numpy. Installation can be done using Pypi:
-
-```python
-pip install influenciae
-```
-
-Once Influenciae is installed, there are two major applications for the different modules (that all follow the same API).
-So, except for group-specific functions that are only available on the `influence` module, all the classes are able to compute self-influence values, the influence with one point wrt another, as well as find the top-k samples for both of these situations.
-
-### Discovering influential examples
-
-Particularly useful when validating datasets, influence functions (and related notions) allow for gaining an insight into what samples the models thinks to be "important". For this, the training dataset and a trained model are needed.
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import FirstOrderInfluenceCalculator
-from deel.influenciae.utils import ORDER
-
-# load the model, the training loss (without reduction) and the training data (with the labels and in a batched TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-data_and_influence_dataset = influence_calculator.compute_influence_values(train_dataset)
-# or influence_calculator.compute_top_k_from_training_dataset(train_dataset, k_samples, ORDER.DESCENDING) when the
-# dataset is too large
-```
-
-This is also explained more in depth in the [Getting Started tutotial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
-
-### Explaining neural networks through their training data
-
-Another application is to explain some model's predictions by looking on which training samples they are based on. Again, the training dataset, the model and the samples we wish to explain are needed.
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import FirstOrderInfluenceCalculator
-from deel.influenciae.utils import ORDER
-
-# load the model, the training loss (without reduction), the training data and
-# the data to explain (with the labels and in batched a TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-data_and_influence_dataset = influence_calculator.estimate_influence_values_in_batches(samples_to_explain, train_dataset)
-# or influence_calculator.top_k(samples_to_explain, train_dataset, k_samples, ORDER.DESCENDING) when the
-# dataset is too large
-```
-
-This is also explained more in depth in the [Getting Started tutorial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
-
-### Determining the influence of groups of samples
-
-The previous examples use notions of influence that are applied individually to each data-point, but it is possible to extend this to groups. That is, answer the question of what would a model look like if it hadn't seen a whole group of data-points during training, for example. This can be computed namely using the `FirstOrderInfluenceCalculator` and `SecondOrderInfluenceCalculator`, for implementations where pairwise interactions between each of the data-points are not taken into account and do, respectively.
-
-For obtaining the groups' influence:
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import SecondOrderInfluenceCalculator
-
-# load the model, the training loss (without reduction), the training data and
-# the data to explain (with the labels and in a batched TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
-data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train, groups_to_explain)
-```
-
-For the data-centric explanations:
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import SecondOrderInfluenceCalculator
-
-# load the model, the training loss (without reduction), the training data and
-# the data to explain (with the labels and in a batched TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
-data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train)
-```
-
-## 📦 What's Included
-
-All the influence calculation methods work on Tensorflow models trained for any sort of task and on any type of data. Visualization functionality is implemented for image datasets only (for the moment).
-
-| **Influence Method**                                    | Source                                                                                             |                                                                              Tutorial                                                                               |
-|:--------------------------------------------------------|:---------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-| Influence Functions                                     | [Paper](https://arxiv.org/abs/1703.04730)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
-| RelatIF                                                 | [Paper](https://arxiv.org/pdf/2003.11630.pdf)                                                      | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
-| Influence Functions  (first order, groups)              | [Paper](https://arxiv.org/abs/1905.13289)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
-| Influence Functions  (second order, groups)             | [Paper](https://arxiv.org/abs/1911.00418)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) |
-| Arnoldi (Scaling Up Influence Functions)                | [Paper](https://arxiv.org/abs/2112.03052)                                                          |                                                                                 WIP                                                                                 |
-| Representer Point Selection  (L2)                       | [Paper](https://arxiv.org/abs/1811.09720)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) |
-| Representer Point Selection  (Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) |
-| Trac-In                                                 | [Paper](https://arxiv.org/abs/2002.08484)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) |
-| Boundary-based influence                                | --                                                                                                 |                                                                                 WIP                                                                                 |
-
-## 👀 See Also
-
-This library proposes implementations of some of the different popular ways of calculating the influence of data-points on TF, but there are also other ones using other frameworks. 
-
-Some other tools for efficiently computing influence functions.
-
-- [Scaling Up Influence Functions](https://github.com/google-research/jax-influence) a Python library using JAX implementing a scalable algorithm for computing influence functions.
-- [FastIF: Scalable Influence Functions for Efficient Model Interpretation and Debugging](https://github.com/salesforce/fast-influence-functions) a Python library using PyTorch implementing another scalable algorithm for computing influence functions.
-
-More from the DEEL project:
-
-- [Xplique](https://github.com/deel-ai/xplique) a Python library exclusively dedicated to explaining neural networks.
-- [deel-lip](https://github.com/deel-ai/deel-lip) a Python library for training k-Lipschitz neural networks on TF.
-- [deel-torchlip](https://github.com/deel-ai/deel-torchlip) a Python library for training k-Lipschitz neural networks on PyTorch.
-- [DEEL White paper](https://arxiv.org/abs/2103.10529) a summary of the DEEL team on the challenges of certifiable AI and the role of data quality, representativity and explainability for this purpose.
-
-## 🙏 Acknowledgments
-
-<img align="right" src="https://www.deel.ai/wp-content/uploads/2021/05/logo-DEEL.png" width="25%">
-This project received funding from the French ”Investing for the Future – PIA3” program within the Artificial and Natural Intelligence Toulouse Institute (ANITI). The authors gratefully acknowledge the support of the <a href="https://www.deel.ai/"> DEEL </a> project.
-
-## 👨‍🎓 Creators
-
-This library was first created as a research tool by [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in the context of the DEEL project with the help of [David Vigouroux](mailto:david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr). Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to transform the code base as a practical user-(almost)-friendly and efficient tool.
-
-## 📝 License
-
-The package is released under <a href="https://choosealicense.com/licenses/mit"> MIT license</a>.
+<div align="center">
+    <img src="docs/assets/banner2.png" width="75%" alt="Influenciae" align="center" />
+</div>
+<br>
+
+<div align="center">
+    <a href="#">
+        <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9, 3.10-efefef">
+    </a>
+    <a href="#tf">
+        <img src="https://img.shields.io/badge/TensorFlow-2.7, 2.8, 2.9-00458A">
+    </a>
+    <a href="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml">
+        <img alt="PyLint" src="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml/badge.svg">
+    </a>
+    <a href="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml">
+        <img alt="Tox" src="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml/badge.svg">
+    </a>
+    <a href="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml">
+        <img alt="Pypi" src="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml/badge.svg">
+    </a>
+    <a href="#">
+        <img src="https://img.shields.io/badge/License-MIT-efefef">
+    </a>
+    <br>
+    <a href="https://deel-ai.github.io/influenciae/"><strong>Explore Influenciae docs »</strong></a>
+</div>
+<br>
+
+Influenciae is a Python toolkit dedicated to computing influence values for the discovery of potentially problematic samples in a dataset and the generation of data-centric explanations for deep learning models. In this library based on Tensorflow, we gather state-of-the-art methods for estimating the importance of training samples and their influence on test data-points for validating the quality of datasets and of the models trained on them.
+
+## 🔥 Tutorials
+
+We propose some hands-on tutorials to get familiar with the library and it's API:
+
+- [**Getting Started**](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
+- [**Benchmarking with Mislabeled sample detection**](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) </sub>
+- [**Using the first order influence calculator**](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) </sub>
+- [**Using the second order influence calculator**](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) </sub>
+- [**Using Arnoldi Influence Calculator**](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) </sub>
+- [**Using TracIn**](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) </sub>
+- [**Using Representer Point Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) </sub>
+- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) </sub>
+- [**Using Boundary-based Influence**](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) </sub>
+
+## 🚀 Quick Start
+
+Influenciae requires a version of python 3.7 or higher and several libraries, including Tensorflow and Numpy. Installation can be done using Pypi:
+
+```python
+pip install influenciae
+```
+
+Once Influenciae is installed, there are two major applications for the different modules (that all follow the same API).
+So, except for group-specific functions that are only available on the `influence` module, all the classes are able to compute self-influence values, the influence with one point wrt another, as well as find the top-k samples for both of these situations.
+
+### Discovering influential examples
+
+Particularly useful when validating datasets, influence functions (and related notions) allow for gaining an insight into what samples the models thinks to be "important". For this, the training dataset and a trained model are needed.
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import FirstOrderInfluenceCalculator
+from deel.influenciae.utils import ORDER
+
+# load the model, the training loss (without reduction) and the training data (with the labels and in a batched TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset = influence_calculator.compute_influence_values(train_dataset)
+# or influence_calculator.compute_top_k_from_training_dataset(train_dataset, k_samples, ORDER.DESCENDING) when the
+# dataset is too large
+```
+
+This is also explained more in depth in the [Getting Started tutotial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
+
+### Explaining neural networks through their training data
+
+Another application is to explain some model's predictions by looking on which training samples they are based on. Again, the training dataset, the model and the samples we wish to explain are needed.
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import FirstOrderInfluenceCalculator
+from deel.influenciae.utils import ORDER
+
+# load the model, the training loss (without reduction), the training data and
+# the data to explain (with the labels and in batched a TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset = influence_calculator.estimate_influence_values_in_batches(samples_to_explain, train_dataset)
+# or influence_calculator.top_k(samples_to_explain, train_dataset, k_samples, ORDER.DESCENDING) when the
+# dataset is too large
+```
+
+This is also explained more in depth in the [Getting Started tutorial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
+
+### Determining the influence of groups of samples
+
+The previous examples use notions of influence that are applied individually to each data-point, but it is possible to extend this to groups. That is, answer the question of what would a model look like if it hadn't seen a whole group of data-points during training, for example. This can be computed namely using the `FirstOrderInfluenceCalculator` and `SecondOrderInfluenceCalculator`, for implementations where pairwise interactions between each of the data-points are not taken into account and do, respectively.
+
+For obtaining the groups' influence:
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import SecondOrderInfluenceCalculator
+
+# load the model, the training loss (without reduction), the training data and
+# the data to explain (with the labels and in a batched TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
+data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train, groups_to_explain)
+```
+
+For the data-centric explanations:
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import SecondOrderInfluenceCalculator
+
+# load the model, the training loss (without reduction), the training data and
+# the data to explain (with the labels and in a batched TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
+data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train)
+```
+
+## 📦 What's Included
+
+All the influence calculation methods work on Tensorflow models trained for any sort of task and on any type of data. Visualization functionality is implemented for image datasets only (for the moment).
+
+| **Influence Method**                                    | Source                                                                                             |                                                                              Tutorial                                                                               |
+|:--------------------------------------------------------|:---------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Influence Functions                                     | [Paper](https://arxiv.org/abs/1703.04730)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
+| RelatIF                                                 | [Paper](https://arxiv.org/pdf/2003.11630.pdf)                                                      | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
+| Influence Functions  (first order, groups)              | [Paper](https://arxiv.org/abs/1905.13289)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
+| Influence Functions  (second order, groups)             | [Paper](https://arxiv.org/abs/1911.00418)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) |
+| Arnoldi iteration (Scaling Up Influence Functions)      | [Paper](https://arxiv.org/abs/2112.03052)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)  |
+| Trac-In                                                 | [Paper](https://arxiv.org/abs/2002.08484)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) |
+| Representer Point Selection  (L2)                       | [Paper](https://arxiv.org/abs/1811.09720)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) |
+| Representer Point Selection  (Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) |
+| Boundary-based influence                                | --                                                                                                 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) |
+
+## 👀 See Also
+
+This library proposes implementations of some of the different popular ways of calculating the influence of data-points on TF, but there are also other ones using other frameworks. 
+
+Some other tools for efficiently computing influence functions.
+
+- [Scaling Up Influence Functions](https://github.com/google-research/jax-influence) a Python library using JAX implementing a scalable algorithm for computing influence functions.
+- [FastIF: Scalable Influence Functions for Efficient Model Interpretation and Debugging](https://github.com/salesforce/fast-influence-functions) a Python library using PyTorch implementing another scalable algorithm for computing influence functions.
+
+More from the DEEL project:
+
+- [Xplique](https://github.com/deel-ai/xplique) a Python library exclusively dedicated to explaining neural networks.
+- [deel-lip](https://github.com/deel-ai/deel-lip) a Python library for training k-Lipschitz neural networks on TF.
+- [deel-torchlip](https://github.com/deel-ai/deel-torchlip) a Python library for training k-Lipschitz neural networks on PyTorch.
+- [DEEL White paper](https://arxiv.org/abs/2103.10529) a summary of the DEEL team on the challenges of certifiable AI and the role of data quality, representativity and explainability for this purpose.
+
+## 🙏 Acknowledgments
+
+<img align="right" src="https://www.deel.ai/wp-content/uploads/2021/05/logo-DEEL.png" width="25%">
+This project received funding from the French ”Investing for the Future – PIA3” program within the Artificial and Natural Intelligence Toulouse Institute (ANITI). The authors gratefully acknowledge the support of the <a href="https://www.deel.ai/"> DEEL </a> project.
+
+## 👨‍🎓 Creators
+
+This library was first created as a research tool by [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in the context of the DEEL project with the help of [David Vigouroux](mailto:david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr). Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to transform the code base as a practical user-(almost)-friendly and efficient tool.
+
+## 🗞️ Citation
+
+If you use Influenciae as part of your workflow in a scientific publication, please consider citing the 🗞️ [official paper](https://hal.science/hal-04284178/):
+
+```
+@unpublished{picard:hal-04284178,
+  TITLE = {{Influenci{\ae}: A library for tracing the influence back to the data-points}},
+  AUTHOR = {Picard, Agustin Martin and Hervier, Lucas and Fel, Thomas and Vigouroux, David},
+  URL = {https://hal.science/hal-04284178},
+  NOTE = {working paper or preprint},
+  YEAR = {2023},
+  MONTH = Nov,
+  KEYWORDS = {Data-centric ai ; XAI ; Explainability ; Influence Functions ; Open-source toolbox},
+  PDF = {https://hal.science/hal-04284178/file/ms.pdf},
+  HAL_ID = {hal-04284178},
+  HAL_VERSION = {v1},
+}
+```
+
+## 📝 License
+
+The package is released under <a href="https://choosealicense.com/licenses/mit"> MIT license</a>.
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: Influenciae Version: 0.2.0 Summary: A Tensorflow
-Toolbox for Influence Functions Author: DEEL Core Team Author-email: agustin-
-martin.picard@irt-saintexupery.com License: MIT Classifier: Development Status
-:: 4 - Beta Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
-docs License-File: LICENSE
                                  [Influenciae]
 
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._7_,_ _3_._8_,_ _3_._9_,_ _3_._1_0_-_e_f_e_f_e_f_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_e_n_s_o_r_F_l_o_w_-_2_._7_,_ _2_._8_,_ _2_._9_-_0_0_4_5_8_A_]_[_P_y_L_i_n_t_]_[_T_o_x_]_[_P_y_p_i_]_[_h_t_t_p_s_:
                   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_e_f_e_f_e_f_]
                           _EE_xx_pp_ll_oo_rr_ee_ _II_nn_ff_ll_uu_ee_nn_cc_ii_aa_ee_ _dd_oo_cc_ss_ _?Â_?»
 
@@ -33,28 +25,37 @@
 1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing)
 - [**Using the second order influence calculator**](https://
 colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/1qNvKiU3-
-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) - [**Using TracIn**](https://
+aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) - [**Using Arnoldi Influence
+Calculator**](https://colab.research.google.com/drive/
+1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)
+- [**Using TracIn**](https://colab.research.google.com/drive/
+1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing)
+- [**Using Representer Point Selection - L2 (RPS_L2)**](https://
+colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
-1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) - [**Using Representer Point
-Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/
-17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
-- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**]
+17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) - [**Using Representer Point
+Selection - Local Jacobian Expansion (RPS_LJE)**](https://
+colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/14e7wwFRQJhY-
-huVYmJ7ri355kfLJgAPA?usp=sharing) [![Open In Colab](https://
+huVYmJ7ri355kfLJgAPA?usp=sharing) - [**Using Boundary-based Influence**](https:
+//colab.research.google.com/drive/
+1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing)
 ## ð Quick Start Influenciae requires a version of python 3.7 or higher and
 several libraries, including Tensorflow and Numpy. Installation can be done
 using Pypi: ```python pip install influenciae ``` Once Influenciae is
 installed, there are two major applications for the different modules (that all
 follow the same API). So, except for group-specific functions that are only
 available on the `influence` module, all the classes are able to compute self-
 influence values, the influence with one point wrt another, as well as find the
@@ -62,18 +63,18 @@
 examples Particularly useful when validating datasets, influence functions (and
 related notions) allow for gaining an insight into what samples the models
 thinks to be "important". For this, the training dataset and a trained model
 are needed. ```python from deel.influenciae.common import InfluenceModel,
 ExactIHVP from deel.influenciae.influence import FirstOrderInfluenceCalculator
 from deel.influenciae.utils import ORDER # load the model, the training loss
 (without reduction) and the training data (with the labels and in a batched TF
-dataset) influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model,
-train_dataset, ihvp_calculator) data_and_influence_dataset =
+dataset) influence_model = InfluenceModel(model, start_layer=target_layer,
+loss_function=loss_function) ihvp_calculator = ExactIHVP(influence_model,
+train_dataset) influence_calculator = FirstOrderInfluenceCalculator
+(influence_model, train_dataset, ihvp_calculator) data_and_influence_dataset =
 influence_calculator.compute_influence_values(train_dataset) # or
 influence_calculator.compute_top_k_from_training_dataset(train_dataset,
 k_samples, ORDER.DESCENDING) when the # dataset is too large ``` This is also
 explained more in depth in the [Getting Started tutotial](https://
 colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
@@ -82,17 +83,18 @@
 predictions by looking on which training samples they are based on. Again, the
 training dataset, the model and the samples we wish to explain are needed.
 ```python from deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import FirstOrderInfluenceCalculator from
 deel.influenciae.utils import ORDER # load the model, the training loss
 (without reduction), the training data and # the data to explain (with the
 labels and in batched a TF dataset) influence_model = InfluenceModel(model,
-target_layer, loss_function) ihvp_calculator = ExactIHVP(influence_model,
-train_dataset) influence_calculator = FirstOrderInfluenceCalculator
-(influence_model, train_dataset, ihvp_calculator) data_and_influence_dataset =
+start_layer=target_layer, loss_function=loss_function) ihvp_calculator =
+ExactIHVP(influence_model, train_dataset) influence_calculator =
+FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_in_batches(samples_to_explain,
 train_dataset) # or influence_calculator.top_k(samples_to_explain,
 train_dataset, k_samples, ORDER.DESCENDING) when the # dataset is too large ```
 This is also explained more in depth in the [Getting Started tutorial](https://
 colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
@@ -105,28 +107,30 @@
 `SecondOrderInfluenceCalculator`, for implementations where pairwise
 interactions between each of the data-points are not taken into account and do,
 respectively. For obtaining the groups' influence: ```python from
 deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import SecondOrderInfluenceCalculator # load the
 model, the training loss (without reduction), the training data and # the data
 to explain (with the labels and in a batched TF dataset) influence_model =
-InfluenceModel(model, target_layer, loss_function) ihvp_calculator = ExactIHVP
-(influence_model, train_dataset) influence_calculator =
-SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-# or FirstOrderInfluenceCalculator data_and_influence_dataset =
+InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model,
+train_dataset, ihvp_calculator) # or FirstOrderInfluenceCalculator
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_group(groups_train,
 groups_to_explain) ``` For the data-centric explanations: ```python from
 deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import SecondOrderInfluenceCalculator # load the
 model, the training loss (without reduction), the training data and # the data
 to explain (with the labels and in a batched TF dataset) influence_model =
-InfluenceModel(model, target_layer, loss_function) ihvp_calculator = ExactIHVP
-(influence_model, train_dataset) influence_calculator =
-SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-# or FirstOrderInfluenceCalculator data_and_influence_dataset =
+InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model,
+train_dataset, ihvp_calculator) # or FirstOrderInfluenceCalculator
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_group(groups_train) ``` ## ð¦
 What's Included All the influence calculation methods work on Tensorflow models
 trained for any sort of task and on any type of data. Visualization
 functionality is implemented for image datasets only (for the moment). |
 **Influence Method** | Source | Tutorial | |:----------------------------------
 ----------------------|:-------------------------------------------------------
 --------------------------------------------|:---------------------------------
@@ -141,28 +145,33 @@
 | | Influence Functions (first order, groups) | [Paper](https://arxiv.org/abs/
 1905.13289) | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) | | Influence Functions (second
 order, groups) | [Paper](https://arxiv.org/abs/1911.00418) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing)
-| | Arnoldi (Scaling Up Influence Functions) | [Paper](https://arxiv.org/abs/
-2112.03052) | WIP | | Representer Point Selection (L2) | [Paper](https://
-arxiv.org/abs/1811.09720) | [![Open In Colab](https://
+| | Arnoldi iteration (Scaling Up Influence Functions) | [Paper](https://
+arxiv.org/abs/2112.03052) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
-| | Representer Point Selection (Local Jacobian Expansion) | [Paper](https://
-proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-
-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-
-huVYmJ7ri355kfLJgAPA?usp=sharing) | | Trac-In | [Paper](https://arxiv.org/abs/
-2002.08484) | [![Open In Colab](https://colab.research.google.com/assets/colab-
+colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)
+| | Trac-In | [Paper](https://arxiv.org/abs/2002.08484) | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing)
+| | Representer Point Selection (L2) | [Paper](https://arxiv.org/abs/
+1811.09720) | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) | | Boundary-based influence | -
-- | WIP | ## ð See Also This library proposes implementations of some of the
+17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) | | Representer Point Selection
+(Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/
+file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+| | Boundary-based influence | -- | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing)
+| ## ð See Also This library proposes implementations of some of the
 different popular ways of calculating the influence of data-points on TF, but
 there are also other ones using other frameworks. Some other tools for
 efficiently computing influence functions. - [Scaling Up Influence Functions]
 (https://github.com/google-research/jax-influence) a Python library using JAX
 implementing a scalable algorithm for computing influence functions. - [FastIF:
 Scalable Influence Functions for Efficient Model Interpretation and Debugging]
 (https://github.com/salesforce/fast-influence-functions) a Python library using
@@ -181,8 +190,18 @@
 (ANITI). The authors gratefully acknowledge the support of the _D_E_E_L_ project. ##
 ð¨âð Creators This library was first created as a research tool by
 [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in
 the context of the DEEL project with the help of [David Vigouroux](mailto:
 david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr).
 Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to
 transform the code base as a practical user-(almost)-friendly and efficient
-tool. ## ð License The package is released under _M_I_T_ _l_i_c_e_n_s_e.
+tool. ## ðï¸ Citation If you use Influenciae as part of your workflow in a
+scientific publication, please consider citing the ðï¸ [official paper]
+(https://hal.science/hal-04284178/): ``` @unpublished{picard:hal-04284178,
+TITLE = {{Influenci{\ae}: A library for tracing the influence back to the data-
+points}}, AUTHOR = {Picard, Agustin Martin and Hervier, Lucas and Fel, Thomas
+and Vigouroux, David}, URL = {https://hal.science/hal-04284178}, NOTE =
+{working paper or preprint}, YEAR = {2023}, MONTH = Nov, KEYWORDS = {Data-
+centric ai ; XAI ; Explainability ; Influence Functions ; Open-source toolbox},
+PDF = {https://hal.science/hal-04284178/file/ms.pdf}, HAL_ID = {hal-04284178},
+HAL_VERSION = {v1}, } ``` ## ð License The package is released under _M_I_T
+_l_i_c_e_n_s_e.
```

### Comparing `Influenciae-0.2.0/Influenciae.egg-info/SOURCES.txt` & `Influenciae-0.3.0/Influenciae.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 deel/influenciae/influence/base_group_influence.py
 deel/influenciae/influence/first_order_influence_calculator.py
 deel/influenciae/influence/second_order_influence_calculator.py
 deel/influenciae/plots/__init__.py
 deel/influenciae/plots/benchmark.py
 deel/influenciae/plots/image.py
 deel/influenciae/rps/__init__.py
+deel/influenciae/rps/base_representer_point.py
 deel/influenciae/rps/rps_l2.py
 deel/influenciae/rps/rps_lje.py
 deel/influenciae/trac_in/__init__.py
 deel/influenciae/trac_in/tracin.py
 deel/influenciae/types/__init__.py
 deel/influenciae/utils/__init__.py
 deel/influenciae/utils/backtracking_line_search.py
```

### Comparing `Influenciae-0.2.0/LICENSE` & `Influenciae-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/PKG-INFO` & `Influenciae-0.3.0/Influenciae.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: Influenciae
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Tensorflow Toolbox for Influence Functions
 Author: DEEL Core Team
 Author-email: agustin-martin.picard@irt-saintexupery.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tensorflow<2.10.0,>=2.7.0
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pylint; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: numkdoc; extra == "docs"
 
 <div align="center">
     <img src="docs/assets/banner2.png" width="75%" alt="Influenciae" align="center" />
 </div>
 <br>
 
 <div align="center">
@@ -51,17 +59,19 @@
 
 We propose some hands-on tutorials to get familiar with the library and it's API:
 
 - [**Getting Started**](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
 - [**Benchmarking with Mislabeled sample detection**](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) </sub>
 - [**Using the first order influence calculator**](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) </sub>
 - [**Using the second order influence calculator**](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) </sub>
+- [**Using Arnoldi Influence Calculator**](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) </sub>
 - [**Using TracIn**](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) </sub>
 - [**Using Representer Point Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) </sub>
 - [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) </sub>
+- [**Using Boundary-based Influence**](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) </sub>
 
 ## 🚀 Quick Start
 
 Influenciae requires a version of python 3.7 or higher and several libraries, including Tensorflow and Numpy. Installation can be done using Pypi:
 
 ```python
 pip install influenciae
@@ -77,15 +87,15 @@
 ```python
 from deel.influenciae.common import InfluenceModel, ExactIHVP
 from deel.influenciae.influence import FirstOrderInfluenceCalculator
 from deel.influenciae.utils import ORDER
 
 # load the model, the training loss (without reduction) and the training data (with the labels and in a batched TF dataset)
 
-influence_model = InfluenceModel(model, target_layer, loss_function)
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
 ihvp_calculator = ExactIHVP(influence_model, train_dataset)
 influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
 data_and_influence_dataset = influence_calculator.compute_influence_values(train_dataset)
 # or influence_calculator.compute_top_k_from_training_dataset(train_dataset, k_samples, ORDER.DESCENDING) when the
 # dataset is too large
 ```
 
@@ -99,15 +109,15 @@
 from deel.influenciae.common import InfluenceModel, ExactIHVP
 from deel.influenciae.influence import FirstOrderInfluenceCalculator
 from deel.influenciae.utils import ORDER
 
 # load the model, the training loss (without reduction), the training data and
 # the data to explain (with the labels and in batched a TF dataset)
 
-influence_model = InfluenceModel(model, target_layer, loss_function)
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
 ihvp_calculator = ExactIHVP(influence_model, train_dataset)
 influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
 data_and_influence_dataset = influence_calculator.estimate_influence_values_in_batches(samples_to_explain, train_dataset)
 # or influence_calculator.top_k(samples_to_explain, train_dataset, k_samples, ORDER.DESCENDING) when the
 # dataset is too large
 ```
 
@@ -122,30 +132,30 @@
 ```python
 from deel.influenciae.common import InfluenceModel, ExactIHVP
 from deel.influenciae.influence import SecondOrderInfluenceCalculator
 
 # load the model, the training loss (without reduction), the training data and
 # the data to explain (with the labels and in a batched TF dataset)
 
-influence_model = InfluenceModel(model, target_layer, loss_function)
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
 ihvp_calculator = ExactIHVP(influence_model, train_dataset)
 influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
 data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train, groups_to_explain)
 ```
 
 For the data-centric explanations:
 
 ```python
 from deel.influenciae.common import InfluenceModel, ExactIHVP
 from deel.influenciae.influence import SecondOrderInfluenceCalculator
 
 # load the model, the training loss (without reduction), the training data and
 # the data to explain (with the labels and in a batched TF dataset)
 
-influence_model = InfluenceModel(model, target_layer, loss_function)
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
 ihvp_calculator = ExactIHVP(influence_model, train_dataset)
 influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
 data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train)
 ```
 
 ## 📦 What's Included
 
@@ -153,19 +163,19 @@
 
 | **Influence Method**                                    | Source                                                                                             |                                                                              Tutorial                                                                               |
 |:--------------------------------------------------------|:---------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
 | Influence Functions                                     | [Paper](https://arxiv.org/abs/1703.04730)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
 | RelatIF                                                 | [Paper](https://arxiv.org/pdf/2003.11630.pdf)                                                      | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
 | Influence Functions  (first order, groups)              | [Paper](https://arxiv.org/abs/1905.13289)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
 | Influence Functions  (second order, groups)             | [Paper](https://arxiv.org/abs/1911.00418)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) |
-| Arnoldi (Scaling Up Influence Functions)                | [Paper](https://arxiv.org/abs/2112.03052)                                                          |                                                                                 WIP                                                                                 |
+| Arnoldi iteration (Scaling Up Influence Functions)      | [Paper](https://arxiv.org/abs/2112.03052)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)  |
+| Trac-In                                                 | [Paper](https://arxiv.org/abs/2002.08484)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) |
 | Representer Point Selection  (L2)                       | [Paper](https://arxiv.org/abs/1811.09720)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) |
 | Representer Point Selection  (Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) |
-| Trac-In                                                 | [Paper](https://arxiv.org/abs/2002.08484)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) |
-| Boundary-based influence                                | --                                                                                                 |                                                                                 WIP                                                                                 |
+| Boundary-based influence                                | --                                                                                                 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) |
 
 ## 👀 See Also
 
 This library proposes implementations of some of the different popular ways of calculating the influence of data-points on TF, but there are also other ones using other frameworks. 
 
 Some other tools for efficiently computing influence functions.
 
@@ -184,10 +194,29 @@
 <img align="right" src="https://www.deel.ai/wp-content/uploads/2021/05/logo-DEEL.png" width="25%">
 This project received funding from the French ”Investing for the Future – PIA3” program within the Artificial and Natural Intelligence Toulouse Institute (ANITI). The authors gratefully acknowledge the support of the <a href="https://www.deel.ai/"> DEEL </a> project.
 
 ## 👨‍🎓 Creators
 
 This library was first created as a research tool by [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in the context of the DEEL project with the help of [David Vigouroux](mailto:david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr). Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to transform the code base as a practical user-(almost)-friendly and efficient tool.
 
+## 🗞️ Citation
+
+If you use Influenciae as part of your workflow in a scientific publication, please consider citing the 🗞️ [official paper](https://hal.science/hal-04284178/):
+
+```
+@unpublished{picard:hal-04284178,
+  TITLE = {{Influenci{\ae}: A library for tracing the influence back to the data-points}},
+  AUTHOR = {Picard, Agustin Martin and Hervier, Lucas and Fel, Thomas and Vigouroux, David},
+  URL = {https://hal.science/hal-04284178},
+  NOTE = {working paper or preprint},
+  YEAR = {2023},
+  MONTH = Nov,
+  KEYWORDS = {Data-centric ai ; XAI ; Explainability ; Influence Functions ; Open-source toolbox},
+  PDF = {https://hal.science/hal-04284178/file/ms.pdf},
+  HAL_ID = {hal-04284178},
+  HAL_VERSION = {v1},
+}
+```
+
 ## 📝 License
 
 The package is released under <a href="https://choosealicense.com/licenses/mit"> MIT license</a>.
```

#### html2text {}

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 2.1 Name: Influenciae Version: 0.2.0 Summary: A Tensorflow
+Metadata-Version: 2.1 Name: Influenciae Version: 0.3.0 Summary: A Tensorflow
 Toolbox for Influence Functions Author: DEEL Core Team Author-email: agustin-
 martin.picard@irt-saintexupery.com License: MIT Classifier: Development Status
 :: 4 - Beta Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
-docs License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+tensorflow<2.10.0,>=2.7.0 Requires-Dist: numpy Requires-Dist: matplotlib
+Provides-Extra: tests Requires-Dist: pytest; extra == "tests" Requires-Dist:
+pylint; extra == "tests" Provides-Extra: docs Requires-Dist: mkdocs; extra ==
+"docs" Requires-Dist: mkdocs-material; extra == "docs" Requires-Dist: numkdoc;
+extra == "docs"
                                  [Influenciae]
 
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._7_,_ _3_._8_,_ _3_._9_,_ _3_._1_0_-_e_f_e_f_e_f_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_e_n_s_o_r_F_l_o_w_-_2_._7_,_ _2_._8_,_ _2_._9_-_0_0_4_5_8_A_]_[_P_y_L_i_n_t_]_[_T_o_x_]_[_P_y_p_i_]_[_h_t_t_p_s_:
                   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_e_f_e_f_e_f_]
                           _EE_xx_pp_ll_oo_rr_ee_ _II_nn_ff_ll_uu_ee_nn_cc_ii_aa_ee_ _dd_oo_cc_ss_ _?Â_?»
 
@@ -33,28 +37,37 @@
 1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing)
 - [**Using the second order influence calculator**](https://
 colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/1qNvKiU3-
-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) - [**Using TracIn**](https://
+aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) - [**Using Arnoldi Influence
+Calculator**](https://colab.research.google.com/drive/
+1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)
+- [**Using TracIn**](https://colab.research.google.com/drive/
+1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing)
+- [**Using Representer Point Selection - L2 (RPS_L2)**](https://
+colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
-1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) - [**Using Representer Point
-Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/
-17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
-- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**]
+17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) - [**Using Representer Point
+Selection - Local Jacobian Expansion (RPS_LJE)**](https://
+colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/14e7wwFRQJhY-
-huVYmJ7ri355kfLJgAPA?usp=sharing) [![Open In Colab](https://
+huVYmJ7ri355kfLJgAPA?usp=sharing) - [**Using Boundary-based Influence**](https:
+//colab.research.google.com/drive/
+1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing)
 ## ð Quick Start Influenciae requires a version of python 3.7 or higher and
 several libraries, including Tensorflow and Numpy. Installation can be done
 using Pypi: ```python pip install influenciae ``` Once Influenciae is
 installed, there are two major applications for the different modules (that all
 follow the same API). So, except for group-specific functions that are only
 available on the `influence` module, all the classes are able to compute self-
 influence values, the influence with one point wrt another, as well as find the
@@ -62,18 +75,18 @@
 examples Particularly useful when validating datasets, influence functions (and
 related notions) allow for gaining an insight into what samples the models
 thinks to be "important". For this, the training dataset and a trained model
 are needed. ```python from deel.influenciae.common import InfluenceModel,
 ExactIHVP from deel.influenciae.influence import FirstOrderInfluenceCalculator
 from deel.influenciae.utils import ORDER # load the model, the training loss
 (without reduction) and the training data (with the labels and in a batched TF
-dataset) influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model,
-train_dataset, ihvp_calculator) data_and_influence_dataset =
+dataset) influence_model = InfluenceModel(model, start_layer=target_layer,
+loss_function=loss_function) ihvp_calculator = ExactIHVP(influence_model,
+train_dataset) influence_calculator = FirstOrderInfluenceCalculator
+(influence_model, train_dataset, ihvp_calculator) data_and_influence_dataset =
 influence_calculator.compute_influence_values(train_dataset) # or
 influence_calculator.compute_top_k_from_training_dataset(train_dataset,
 k_samples, ORDER.DESCENDING) when the # dataset is too large ``` This is also
 explained more in depth in the [Getting Started tutotial](https://
 colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
@@ -82,17 +95,18 @@
 predictions by looking on which training samples they are based on. Again, the
 training dataset, the model and the samples we wish to explain are needed.
 ```python from deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import FirstOrderInfluenceCalculator from
 deel.influenciae.utils import ORDER # load the model, the training loss
 (without reduction), the training data and # the data to explain (with the
 labels and in batched a TF dataset) influence_model = InfluenceModel(model,
-target_layer, loss_function) ihvp_calculator = ExactIHVP(influence_model,
-train_dataset) influence_calculator = FirstOrderInfluenceCalculator
-(influence_model, train_dataset, ihvp_calculator) data_and_influence_dataset =
+start_layer=target_layer, loss_function=loss_function) ihvp_calculator =
+ExactIHVP(influence_model, train_dataset) influence_calculator =
+FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_in_batches(samples_to_explain,
 train_dataset) # or influence_calculator.top_k(samples_to_explain,
 train_dataset, k_samples, ORDER.DESCENDING) when the # dataset is too large ```
 This is also explained more in depth in the [Getting Started tutorial](https://
 colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
@@ -105,28 +119,30 @@
 `SecondOrderInfluenceCalculator`, for implementations where pairwise
 interactions between each of the data-points are not taken into account and do,
 respectively. For obtaining the groups' influence: ```python from
 deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import SecondOrderInfluenceCalculator # load the
 model, the training loss (without reduction), the training data and # the data
 to explain (with the labels and in a batched TF dataset) influence_model =
-InfluenceModel(model, target_layer, loss_function) ihvp_calculator = ExactIHVP
-(influence_model, train_dataset) influence_calculator =
-SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-# or FirstOrderInfluenceCalculator data_and_influence_dataset =
+InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model,
+train_dataset, ihvp_calculator) # or FirstOrderInfluenceCalculator
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_group(groups_train,
 groups_to_explain) ``` For the data-centric explanations: ```python from
 deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import SecondOrderInfluenceCalculator # load the
 model, the training loss (without reduction), the training data and # the data
 to explain (with the labels and in a batched TF dataset) influence_model =
-InfluenceModel(model, target_layer, loss_function) ihvp_calculator = ExactIHVP
-(influence_model, train_dataset) influence_calculator =
-SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-# or FirstOrderInfluenceCalculator data_and_influence_dataset =
+InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model,
+train_dataset, ihvp_calculator) # or FirstOrderInfluenceCalculator
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_group(groups_train) ``` ## ð¦
 What's Included All the influence calculation methods work on Tensorflow models
 trained for any sort of task and on any type of data. Visualization
 functionality is implemented for image datasets only (for the moment). |
 **Influence Method** | Source | Tutorial | |:----------------------------------
 ----------------------|:-------------------------------------------------------
 --------------------------------------------|:---------------------------------
@@ -141,28 +157,33 @@
 | | Influence Functions (first order, groups) | [Paper](https://arxiv.org/abs/
 1905.13289) | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) | | Influence Functions (second
 order, groups) | [Paper](https://arxiv.org/abs/1911.00418) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing)
-| | Arnoldi (Scaling Up Influence Functions) | [Paper](https://arxiv.org/abs/
-2112.03052) | WIP | | Representer Point Selection (L2) | [Paper](https://
-arxiv.org/abs/1811.09720) | [![Open In Colab](https://
+| | Arnoldi iteration (Scaling Up Influence Functions) | [Paper](https://
+arxiv.org/abs/2112.03052) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
-| | Representer Point Selection (Local Jacobian Expansion) | [Paper](https://
-proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-
-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-
-huVYmJ7ri355kfLJgAPA?usp=sharing) | | Trac-In | [Paper](https://arxiv.org/abs/
-2002.08484) | [![Open In Colab](https://colab.research.google.com/assets/colab-
+colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)
+| | Trac-In | [Paper](https://arxiv.org/abs/2002.08484) | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing)
+| | Representer Point Selection (L2) | [Paper](https://arxiv.org/abs/
+1811.09720) | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) | | Boundary-based influence | -
-- | WIP | ## ð See Also This library proposes implementations of some of the
+17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) | | Representer Point Selection
+(Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/
+file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+| | Boundary-based influence | -- | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing)
+| ## ð See Also This library proposes implementations of some of the
 different popular ways of calculating the influence of data-points on TF, but
 there are also other ones using other frameworks. Some other tools for
 efficiently computing influence functions. - [Scaling Up Influence Functions]
 (https://github.com/google-research/jax-influence) a Python library using JAX
 implementing a scalable algorithm for computing influence functions. - [FastIF:
 Scalable Influence Functions for Efficient Model Interpretation and Debugging]
 (https://github.com/salesforce/fast-influence-functions) a Python library using
@@ -181,8 +202,18 @@
 (ANITI). The authors gratefully acknowledge the support of the _D_E_E_L_ project. ##
 ð¨âð Creators This library was first created as a research tool by
 [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in
 the context of the DEEL project with the help of [David Vigouroux](mailto:
 david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr).
 Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to
 transform the code base as a practical user-(almost)-friendly and efficient
-tool. ## ð License The package is released under _M_I_T_ _l_i_c_e_n_s_e.
+tool. ## ðï¸ Citation If you use Influenciae as part of your workflow in a
+scientific publication, please consider citing the ðï¸ [official paper]
+(https://hal.science/hal-04284178/): ``` @unpublished{picard:hal-04284178,
+TITLE = {{Influenci{\ae}: A library for tracing the influence back to the data-
+points}}, AUTHOR = {Picard, Agustin Martin and Hervier, Lucas and Fel, Thomas
+and Vigouroux, David}, URL = {https://hal.science/hal-04284178}, NOTE =
+{working paper or preprint}, YEAR = {2023}, MONTH = Nov, KEYWORDS = {Data-
+centric ai ; XAI ; Explainability ; Influence Functions ; Open-source toolbox},
+PDF = {https://hal.science/hal-04284178/file/ms.pdf}, HAL_ID = {hal-04284178},
+HAL_VERSION = {v1}, } ``` ## ð License The package is released under _M_I_T
+_l_i_c_e_n_s_e.
```

### Comparing `Influenciae-0.2.0/README.md` & `Influenciae-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,175 +1,222 @@
-<div align="center">
-    <img src="docs/assets/banner2.png" width="75%" alt="Influenciae" align="center" />
-</div>
-<br>
-
-<div align="center">
-    <a href="#">
-        <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9, 3.10-efefef">
-    </a>
-    <a href="#tf">
-        <img src="https://img.shields.io/badge/TensorFlow-2.7, 2.8, 2.9-00458A">
-    </a>
-    <a href="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml">
-        <img alt="PyLint" src="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml/badge.svg">
-    </a>
-    <a href="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml">
-        <img alt="Tox" src="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml/badge.svg">
-    </a>
-    <a href="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml">
-        <img alt="Pypi" src="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml/badge.svg">
-    </a>
-    <a href="#">
-        <img src="https://img.shields.io/badge/License-MIT-efefef">
-    </a>
-    <br>
-    <a href="https://deel-ai.github.io/influenciae/"><strong>Explore Influenciae docs »</strong></a>
-</div>
-<br>
-
-Influenciae is a Python toolkit dedicated to computing influence values for the discovery of potentially problematic samples in a dataset and the generation of data-centric explanations for deep learning models. In this library based on Tensorflow, we gather state-of-the-art methods for estimating the importance of training samples and their influence on test data-points for validating the quality of datasets and of the models trained on them.
-
-## 🔥 Tutorials
-
-We propose some hands-on tutorials to get familiar with the library and it's API:
-
-- [**Getting Started**](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
-- [**Benchmarking with Mislabeled sample detection**](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) </sub>
-- [**Using the first order influence calculator**](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) </sub>
-- [**Using the second order influence calculator**](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) </sub>
-- [**Using TracIn**](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) </sub>
-- [**Using Representer Point Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) </sub>
-- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) </sub>
-
-## 🚀 Quick Start
-
-Influenciae requires a version of python 3.7 or higher and several libraries, including Tensorflow and Numpy. Installation can be done using Pypi:
-
-```python
-pip install influenciae
-```
-
-Once Influenciae is installed, there are two major applications for the different modules (that all follow the same API).
-So, except for group-specific functions that are only available on the `influence` module, all the classes are able to compute self-influence values, the influence with one point wrt another, as well as find the top-k samples for both of these situations.
-
-### Discovering influential examples
-
-Particularly useful when validating datasets, influence functions (and related notions) allow for gaining an insight into what samples the models thinks to be "important". For this, the training dataset and a trained model are needed.
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import FirstOrderInfluenceCalculator
-from deel.influenciae.utils import ORDER
-
-# load the model, the training loss (without reduction) and the training data (with the labels and in a batched TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-data_and_influence_dataset = influence_calculator.compute_influence_values(train_dataset)
-# or influence_calculator.compute_top_k_from_training_dataset(train_dataset, k_samples, ORDER.DESCENDING) when the
-# dataset is too large
-```
-
-This is also explained more in depth in the [Getting Started tutotial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
-
-### Explaining neural networks through their training data
-
-Another application is to explain some model's predictions by looking on which training samples they are based on. Again, the training dataset, the model and the samples we wish to explain are needed.
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import FirstOrderInfluenceCalculator
-from deel.influenciae.utils import ORDER
-
-# load the model, the training loss (without reduction), the training data and
-# the data to explain (with the labels and in batched a TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-data_and_influence_dataset = influence_calculator.estimate_influence_values_in_batches(samples_to_explain, train_dataset)
-# or influence_calculator.top_k(samples_to_explain, train_dataset, k_samples, ORDER.DESCENDING) when the
-# dataset is too large
-```
-
-This is also explained more in depth in the [Getting Started tutorial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
-
-### Determining the influence of groups of samples
-
-The previous examples use notions of influence that are applied individually to each data-point, but it is possible to extend this to groups. That is, answer the question of what would a model look like if it hadn't seen a whole group of data-points during training, for example. This can be computed namely using the `FirstOrderInfluenceCalculator` and `SecondOrderInfluenceCalculator`, for implementations where pairwise interactions between each of the data-points are not taken into account and do, respectively.
-
-For obtaining the groups' influence:
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import SecondOrderInfluenceCalculator
-
-# load the model, the training loss (without reduction), the training data and
-# the data to explain (with the labels and in a batched TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
-data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train, groups_to_explain)
-```
-
-For the data-centric explanations:
-
-```python
-from deel.influenciae.common import InfluenceModel, ExactIHVP
-from deel.influenciae.influence import SecondOrderInfluenceCalculator
-
-# load the model, the training loss (without reduction), the training data and
-# the data to explain (with the labels and in a batched TF dataset)
-
-influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
-data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train)
-```
-
-## 📦 What's Included
-
-All the influence calculation methods work on Tensorflow models trained for any sort of task and on any type of data. Visualization functionality is implemented for image datasets only (for the moment).
-
-| **Influence Method**                                    | Source                                                                                             |                                                                              Tutorial                                                                               |
-|:--------------------------------------------------------|:---------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-| Influence Functions                                     | [Paper](https://arxiv.org/abs/1703.04730)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
-| RelatIF                                                 | [Paper](https://arxiv.org/pdf/2003.11630.pdf)                                                      | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
-| Influence Functions  (first order, groups)              | [Paper](https://arxiv.org/abs/1905.13289)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
-| Influence Functions  (second order, groups)             | [Paper](https://arxiv.org/abs/1911.00418)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) |
-| Arnoldi (Scaling Up Influence Functions)                | [Paper](https://arxiv.org/abs/2112.03052)                                                          |                                                                                 WIP                                                                                 |
-| Representer Point Selection  (L2)                       | [Paper](https://arxiv.org/abs/1811.09720)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) |
-| Representer Point Selection  (Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) |
-| Trac-In                                                 | [Paper](https://arxiv.org/abs/2002.08484)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) |
-| Boundary-based influence                                | --                                                                                                 |                                                                                 WIP                                                                                 |
-
-## 👀 See Also
-
-This library proposes implementations of some of the different popular ways of calculating the influence of data-points on TF, but there are also other ones using other frameworks. 
-
-Some other tools for efficiently computing influence functions.
-
-- [Scaling Up Influence Functions](https://github.com/google-research/jax-influence) a Python library using JAX implementing a scalable algorithm for computing influence functions.
-- [FastIF: Scalable Influence Functions for Efficient Model Interpretation and Debugging](https://github.com/salesforce/fast-influence-functions) a Python library using PyTorch implementing another scalable algorithm for computing influence functions.
-
-More from the DEEL project:
-
-- [Xplique](https://github.com/deel-ai/xplique) a Python library exclusively dedicated to explaining neural networks.
-- [deel-lip](https://github.com/deel-ai/deel-lip) a Python library for training k-Lipschitz neural networks on TF.
-- [deel-torchlip](https://github.com/deel-ai/deel-torchlip) a Python library for training k-Lipschitz neural networks on PyTorch.
-- [DEEL White paper](https://arxiv.org/abs/2103.10529) a summary of the DEEL team on the challenges of certifiable AI and the role of data quality, representativity and explainability for this purpose.
-
-## 🙏 Acknowledgments
-
-<img align="right" src="https://www.deel.ai/wp-content/uploads/2021/05/logo-DEEL.png" width="25%">
-This project received funding from the French ”Investing for the Future – PIA3” program within the Artificial and Natural Intelligence Toulouse Institute (ANITI). The authors gratefully acknowledge the support of the <a href="https://www.deel.ai/"> DEEL </a> project.
-
-## 👨‍🎓 Creators
-
-This library was first created as a research tool by [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in the context of the DEEL project with the help of [David Vigouroux](mailto:david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr). Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to transform the code base as a practical user-(almost)-friendly and efficient tool.
-
-## 📝 License
-
-The package is released under <a href="https://choosealicense.com/licenses/mit"> MIT license</a>.
+Metadata-Version: 2.1
+Name: Influenciae
+Version: 0.3.0
+Summary: A Tensorflow Toolbox for Influence Functions
+Author: DEEL Core Team
+Author-email: agustin-martin.picard@irt-saintexupery.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tensorflow<2.10.0,>=2.7.0
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pylint; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: numkdoc; extra == "docs"
+
+<div align="center">
+    <img src="docs/assets/banner2.png" width="75%" alt="Influenciae" align="center" />
+</div>
+<br>
+
+<div align="center">
+    <a href="#">
+        <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9, 3.10-efefef">
+    </a>
+    <a href="#tf">
+        <img src="https://img.shields.io/badge/TensorFlow-2.7, 2.8, 2.9-00458A">
+    </a>
+    <a href="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml">
+        <img alt="PyLint" src="https://github.com/deel-ai/influenciae/actions/workflows/linter.yml/badge.svg">
+    </a>
+    <a href="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml">
+        <img alt="Tox" src="https://github.com/deel-ai/influenciae/actions/workflows/tests.yml/badge.svg">
+    </a>
+    <a href="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml">
+        <img alt="Pypi" src="https://github.com/deel-ai/influenciae/actions/workflows/publish.yml/badge.svg">
+    </a>
+    <a href="#">
+        <img src="https://img.shields.io/badge/License-MIT-efefef">
+    </a>
+    <br>
+    <a href="https://deel-ai.github.io/influenciae/"><strong>Explore Influenciae docs »</strong></a>
+</div>
+<br>
+
+Influenciae is a Python toolkit dedicated to computing influence values for the discovery of potentially problematic samples in a dataset and the generation of data-centric explanations for deep learning models. In this library based on Tensorflow, we gather state-of-the-art methods for estimating the importance of training samples and their influence on test data-points for validating the quality of datasets and of the models trained on them.
+
+## 🔥 Tutorials
+
+We propose some hands-on tutorials to get familiar with the library and it's API:
+
+- [**Getting Started**](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
+- [**Benchmarking with Mislabeled sample detection**](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_5-RC_YBHptVCElBbjxWfWQ1LMU20vOp?usp=sharing) </sub>
+- [**Using the first order influence calculator**](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) </sub>
+- [**Using the second order influence calculator**](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) </sub>
+- [**Using Arnoldi Influence Calculator**](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) </sub>
+- [**Using TracIn**](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) </sub>
+- [**Using Representer Point Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) </sub>
+- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) </sub>
+- [**Using Boundary-based Influence**](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) </sub>
+
+## 🚀 Quick Start
+
+Influenciae requires a version of python 3.7 or higher and several libraries, including Tensorflow and Numpy. Installation can be done using Pypi:
+
+```python
+pip install influenciae
+```
+
+Once Influenciae is installed, there are two major applications for the different modules (that all follow the same API).
+So, except for group-specific functions that are only available on the `influence` module, all the classes are able to compute self-influence values, the influence with one point wrt another, as well as find the top-k samples for both of these situations.
+
+### Discovering influential examples
+
+Particularly useful when validating datasets, influence functions (and related notions) allow for gaining an insight into what samples the models thinks to be "important". For this, the training dataset and a trained model are needed.
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import FirstOrderInfluenceCalculator
+from deel.influenciae.utils import ORDER
+
+# load the model, the training loss (without reduction) and the training data (with the labels and in a batched TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset = influence_calculator.compute_influence_values(train_dataset)
+# or influence_calculator.compute_top_k_from_training_dataset(train_dataset, k_samples, ORDER.DESCENDING) when the
+# dataset is too large
+```
+
+This is also explained more in depth in the [Getting Started tutotial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
+
+### Explaining neural networks through their training data
+
+Another application is to explain some model's predictions by looking on which training samples they are based on. Again, the training dataset, the model and the samples we wish to explain are needed.
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import FirstOrderInfluenceCalculator
+from deel.influenciae.utils import ORDER
+
+# load the model, the training loss (without reduction), the training data and
+# the data to explain (with the labels and in batched a TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset = influence_calculator.estimate_influence_values_in_batches(samples_to_explain, train_dataset)
+# or influence_calculator.top_k(samples_to_explain, train_dataset, k_samples, ORDER.DESCENDING) when the
+# dataset is too large
+```
+
+This is also explained more in depth in the [Getting Started tutorial](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing) </sub>
+
+### Determining the influence of groups of samples
+
+The previous examples use notions of influence that are applied individually to each data-point, but it is possible to extend this to groups. That is, answer the question of what would a model look like if it hadn't seen a whole group of data-points during training, for example. This can be computed namely using the `FirstOrderInfluenceCalculator` and `SecondOrderInfluenceCalculator`, for implementations where pairwise interactions between each of the data-points are not taken into account and do, respectively.
+
+For obtaining the groups' influence:
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import SecondOrderInfluenceCalculator
+
+# load the model, the training loss (without reduction), the training data and
+# the data to explain (with the labels and in a batched TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
+data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train, groups_to_explain)
+```
+
+For the data-centric explanations:
+
+```python
+from deel.influenciae.common import InfluenceModel, ExactIHVP
+from deel.influenciae.influence import SecondOrderInfluenceCalculator
+
+# load the model, the training loss (without reduction), the training data and
+# the data to explain (with the labels and in a batched TF dataset)
+
+influence_model = InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)  # or FirstOrderInfluenceCalculator
+data_and_influence_dataset = influence_calculator.estimate_influence_values_group(groups_train)
+```
+
+## 📦 What's Included
+
+All the influence calculation methods work on Tensorflow models trained for any sort of task and on any type of data. Visualization functionality is implemented for image datasets only (for the moment).
+
+| **Influence Method**                                    | Source                                                                                             |                                                                              Tutorial                                                                               |
+|:--------------------------------------------------------|:---------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Influence Functions                                     | [Paper](https://arxiv.org/abs/1703.04730)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
+| RelatIF                                                 | [Paper](https://arxiv.org/pdf/2003.11630.pdf)                                                      | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
+| Influence Functions  (first order, groups)              | [Paper](https://arxiv.org/abs/1905.13289)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) |
+| Influence Functions  (second order, groups)             | [Paper](https://arxiv.org/abs/1911.00418)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) |
+| Arnoldi iteration (Scaling Up Influence Functions)      | [Paper](https://arxiv.org/abs/2112.03052)  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)  |
+| Trac-In                                                 | [Paper](https://arxiv.org/abs/2002.08484)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) |
+| Representer Point Selection  (L2)                       | [Paper](https://arxiv.org/abs/1811.09720)                                                          | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) |
+| Representer Point Selection  (Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing) |
+| Boundary-based influence                                | --                                                                                                 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) |
+
+## 👀 See Also
+
+This library proposes implementations of some of the different popular ways of calculating the influence of data-points on TF, but there are also other ones using other frameworks. 
+
+Some other tools for efficiently computing influence functions.
+
+- [Scaling Up Influence Functions](https://github.com/google-research/jax-influence) a Python library using JAX implementing a scalable algorithm for computing influence functions.
+- [FastIF: Scalable Influence Functions for Efficient Model Interpretation and Debugging](https://github.com/salesforce/fast-influence-functions) a Python library using PyTorch implementing another scalable algorithm for computing influence functions.
+
+More from the DEEL project:
+
+- [Xplique](https://github.com/deel-ai/xplique) a Python library exclusively dedicated to explaining neural networks.
+- [deel-lip](https://github.com/deel-ai/deel-lip) a Python library for training k-Lipschitz neural networks on TF.
+- [deel-torchlip](https://github.com/deel-ai/deel-torchlip) a Python library for training k-Lipschitz neural networks on PyTorch.
+- [DEEL White paper](https://arxiv.org/abs/2103.10529) a summary of the DEEL team on the challenges of certifiable AI and the role of data quality, representativity and explainability for this purpose.
+
+## 🙏 Acknowledgments
+
+<img align="right" src="https://www.deel.ai/wp-content/uploads/2021/05/logo-DEEL.png" width="25%">
+This project received funding from the French ”Investing for the Future – PIA3” program within the Artificial and Natural Intelligence Toulouse Institute (ANITI). The authors gratefully acknowledge the support of the <a href="https://www.deel.ai/"> DEEL </a> project.
+
+## 👨‍🎓 Creators
+
+This library was first created as a research tool by [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in the context of the DEEL project with the help of [David Vigouroux](mailto:david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr). Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to transform the code base as a practical user-(almost)-friendly and efficient tool.
+
+## 🗞️ Citation
+
+If you use Influenciae as part of your workflow in a scientific publication, please consider citing the 🗞️ [official paper](https://hal.science/hal-04284178/):
+
+```
+@unpublished{picard:hal-04284178,
+  TITLE = {{Influenci{\ae}: A library for tracing the influence back to the data-points}},
+  AUTHOR = {Picard, Agustin Martin and Hervier, Lucas and Fel, Thomas and Vigouroux, David},
+  URL = {https://hal.science/hal-04284178},
+  NOTE = {working paper or preprint},
+  YEAR = {2023},
+  MONTH = Nov,
+  KEYWORDS = {Data-centric ai ; XAI ; Explainability ; Influence Functions ; Open-source toolbox},
+  PDF = {https://hal.science/hal-04284178/file/ms.pdf},
+  HAL_ID = {hal-04284178},
+  HAL_VERSION = {v1},
+}
+```
+
+## 📝 License
+
+The package is released under <a href="https://choosealicense.com/licenses/mit"> MIT license</a>.
```

#### html2text {}

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1 Name: Influenciae Version: 0.3.0 Summary: A Tensorflow
+Toolbox for Influence Functions Author: DEEL Core Team Author-email: agustin-
+martin.picard@irt-saintexupery.com License: MIT Classifier: Development Status
+:: 4 - Beta Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+tensorflow<2.10.0,>=2.7.0 Requires-Dist: numpy Requires-Dist: matplotlib
+Provides-Extra: tests Requires-Dist: pytest; extra == "tests" Requires-Dist:
+pylint; extra == "tests" Provides-Extra: docs Requires-Dist: mkdocs; extra ==
+"docs" Requires-Dist: mkdocs-material; extra == "docs" Requires-Dist: numkdoc;
+extra == "docs"
                                  [Influenciae]
 
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._7_,_ _3_._8_,_ _3_._9_,_ _3_._1_0_-_e_f_e_f_e_f_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_e_n_s_o_r_F_l_o_w_-_2_._7_,_ _2_._8_,_ _2_._9_-_0_0_4_5_8_A_]_[_P_y_L_i_n_t_]_[_T_o_x_]_[_P_y_p_i_]_[_h_t_t_p_s_:
                   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_e_f_e_f_e_f_]
                           _EE_xx_pp_ll_oo_rr_ee_ _II_nn_ff_ll_uu_ee_nn_cc_ii_aa_ee_ _dd_oo_cc_ss_ _?Â_?»
 
@@ -25,28 +37,37 @@
 1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing)
 - [**Using the second order influence calculator**](https://
 colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/1qNvKiU3-
-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) - [**Using TracIn**](https://
+aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing) - [**Using Arnoldi Influence
+Calculator**](https://colab.research.google.com/drive/
+1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)
+- [**Using TracIn**](https://colab.research.google.com/drive/
+1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing)
+- [**Using Representer Point Selection - L2 (RPS_L2)**](https://
+colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
-1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) - [**Using Representer Point
-Selection - L2 (RPS_L2)**](https://colab.research.google.com/drive/
-17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
-- [**Using Representer Point Selection - Local Jacobian Expansion (RPS_LJE)**]
+17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) - [**Using Representer Point
+Selection - Local Jacobian Expansion (RPS_LJE)**](https://
+colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/14e7wwFRQJhY-
-huVYmJ7ri355kfLJgAPA?usp=sharing) [![Open In Colab](https://
+huVYmJ7ri355kfLJgAPA?usp=sharing) - [**Using Boundary-based Influence**](https:
+//colab.research.google.com/drive/
+1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing)
 ## ð Quick Start Influenciae requires a version of python 3.7 or higher and
 several libraries, including Tensorflow and Numpy. Installation can be done
 using Pypi: ```python pip install influenciae ``` Once Influenciae is
 installed, there are two major applications for the different modules (that all
 follow the same API). So, except for group-specific functions that are only
 available on the `influence` module, all the classes are able to compute self-
 influence values, the influence with one point wrt another, as well as find the
@@ -54,18 +75,18 @@
 examples Particularly useful when validating datasets, influence functions (and
 related notions) allow for gaining an insight into what samples the models
 thinks to be "important". For this, the training dataset and a trained model
 are needed. ```python from deel.influenciae.common import InfluenceModel,
 ExactIHVP from deel.influenciae.influence import FirstOrderInfluenceCalculator
 from deel.influenciae.utils import ORDER # load the model, the training loss
 (without reduction) and the training data (with the labels and in a batched TF
-dataset) influence_model = InfluenceModel(model, target_layer, loss_function)
-ihvp_calculator = ExactIHVP(influence_model, train_dataset)
-influence_calculator = FirstOrderInfluenceCalculator(influence_model,
-train_dataset, ihvp_calculator) data_and_influence_dataset =
+dataset) influence_model = InfluenceModel(model, start_layer=target_layer,
+loss_function=loss_function) ihvp_calculator = ExactIHVP(influence_model,
+train_dataset) influence_calculator = FirstOrderInfluenceCalculator
+(influence_model, train_dataset, ihvp_calculator) data_and_influence_dataset =
 influence_calculator.compute_influence_values(train_dataset) # or
 influence_calculator.compute_top_k_from_training_dataset(train_dataset,
 k_samples, ORDER.DESCENDING) when the # dataset is too large ``` This is also
 explained more in depth in the [Getting Started tutotial](https://
 colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
@@ -74,17 +95,18 @@
 predictions by looking on which training samples they are based on. Again, the
 training dataset, the model and the samples we wish to explain are needed.
 ```python from deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import FirstOrderInfluenceCalculator from
 deel.influenciae.utils import ORDER # load the model, the training loss
 (without reduction), the training data and # the data to explain (with the
 labels and in batched a TF dataset) influence_model = InfluenceModel(model,
-target_layer, loss_function) ihvp_calculator = ExactIHVP(influence_model,
-train_dataset) influence_calculator = FirstOrderInfluenceCalculator
-(influence_model, train_dataset, ihvp_calculator) data_and_influence_dataset =
+start_layer=target_layer, loss_function=loss_function) ihvp_calculator =
+ExactIHVP(influence_model, train_dataset) influence_calculator =
+FirstOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_in_batches(samples_to_explain,
 train_dataset) # or influence_calculator.top_k(samples_to_explain,
 train_dataset, k_samples, ORDER.DESCENDING) when the # dataset is too large ```
 This is also explained more in depth in the [Getting Started tutorial](https://
 colab.research.google.com/drive/1vQ6seX6KOr48zx4nLELoy9j1X4jzQv1p?usp=sharing)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
@@ -97,28 +119,30 @@
 `SecondOrderInfluenceCalculator`, for implementations where pairwise
 interactions between each of the data-points are not taken into account and do,
 respectively. For obtaining the groups' influence: ```python from
 deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import SecondOrderInfluenceCalculator # load the
 model, the training loss (without reduction), the training data and # the data
 to explain (with the labels and in a batched TF dataset) influence_model =
-InfluenceModel(model, target_layer, loss_function) ihvp_calculator = ExactIHVP
-(influence_model, train_dataset) influence_calculator =
-SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-# or FirstOrderInfluenceCalculator data_and_influence_dataset =
+InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model,
+train_dataset, ihvp_calculator) # or FirstOrderInfluenceCalculator
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_group(groups_train,
 groups_to_explain) ``` For the data-centric explanations: ```python from
 deel.influenciae.common import InfluenceModel, ExactIHVP from
 deel.influenciae.influence import SecondOrderInfluenceCalculator # load the
 model, the training loss (without reduction), the training data and # the data
 to explain (with the labels and in a batched TF dataset) influence_model =
-InfluenceModel(model, target_layer, loss_function) ihvp_calculator = ExactIHVP
-(influence_model, train_dataset) influence_calculator =
-SecondOrderInfluenceCalculator(influence_model, train_dataset, ihvp_calculator)
-# or FirstOrderInfluenceCalculator data_and_influence_dataset =
+InfluenceModel(model, start_layer=target_layer, loss_function=loss_function)
+ihvp_calculator = ExactIHVP(influence_model, train_dataset)
+influence_calculator = SecondOrderInfluenceCalculator(influence_model,
+train_dataset, ihvp_calculator) # or FirstOrderInfluenceCalculator
+data_and_influence_dataset =
 influence_calculator.estimate_influence_values_group(groups_train) ``` ## ð¦
 What's Included All the influence calculation methods work on Tensorflow models
 trained for any sort of task and on any type of data. Visualization
 functionality is implemented for image datasets only (for the moment). |
 **Influence Method** | Source | Tutorial | |:----------------------------------
 ----------------------|:-------------------------------------------------------
 --------------------------------------------|:---------------------------------
@@ -133,28 +157,33 @@
 | | Influence Functions (first order, groups) | [Paper](https://arxiv.org/abs/
 1905.13289) | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1WlYcQNu5obhVjhonN2QYi8ybKyZJl4iY?usp=sharing) | | Influence Functions (second
 order, groups) | [Paper](https://arxiv.org/abs/1911.00418) | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1qNvKiU3-aZWhRA0rxS6X3ebeNkoznJJe?usp=sharing)
-| | Arnoldi (Scaling Up Influence Functions) | [Paper](https://arxiv.org/abs/
-2112.03052) | WIP | | Representer Point Selection (L2) | [Paper](https://
-arxiv.org/abs/1811.09720) | [![Open In Colab](https://
+| | Arnoldi iteration (Scaling Up Influence Functions) | [Paper](https://
+arxiv.org/abs/2112.03052) | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing)
-| | Representer Point Selection (Local Jacobian Expansion) | [Paper](https://
-proceedings.neurips.cc/paper/2021/file/c460dc0f18fc309ac07306a4a55d2fd6-
-Paper.pdf) | [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://colab.research.google.com/drive/14e7wwFRQJhY-
-huVYmJ7ri355kfLJgAPA?usp=sharing) | | Trac-In | [Paper](https://arxiv.org/abs/
-2002.08484) | [![Open In Colab](https://colab.research.google.com/assets/colab-
+colab.research.google.com/drive/1rQU33sbD0YW1cZMRlJmS15EW5O16yoDE?usp=sharing)
+| | Trac-In | [Paper](https://arxiv.org/abs/2002.08484) | [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing)
+| | Representer Point Selection (L2) | [Paper](https://arxiv.org/abs/
+1811.09720) | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1E94cGF46SUQXcCTNwQ4VGSjXEKm7g21c?usp=sharing) | | Boundary-based influence | -
-- | WIP | ## ð See Also This library proposes implementations of some of the
+17W5s30LbxABbDd8hbdwYE56abyWjSC4u?usp=sharing) | | Representer Point Selection
+(Local Jacobian Expansion) | [Paper](https://proceedings.neurips.cc/paper/2021/
+file/c460dc0f18fc309ac07306a4a55d2fd6-Paper.pdf) | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/14e7wwFRQJhY-huVYmJ7ri355kfLJgAPA?usp=sharing)
+| | Boundary-based influence | -- | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1785eHgT91FfqG1f25s7ovqd6JhP5uklh?usp=sharing)
+| ## ð See Also This library proposes implementations of some of the
 different popular ways of calculating the influence of data-points on TF, but
 there are also other ones using other frameworks. Some other tools for
 efficiently computing influence functions. - [Scaling Up Influence Functions]
 (https://github.com/google-research/jax-influence) a Python library using JAX
 implementing a scalable algorithm for computing influence functions. - [FastIF:
 Scalable Influence Functions for Efficient Model Interpretation and Debugging]
 (https://github.com/salesforce/fast-influence-functions) a Python library using
@@ -173,8 +202,18 @@
 (ANITI). The authors gratefully acknowledge the support of the _D_E_E_L_ project. ##
 ð¨âð Creators This library was first created as a research tool by
 [Agustin Martin PICARD](mailto:agustin-martin.picard@irt-saintexupery.com) in
 the context of the DEEL project with the help of [David Vigouroux](mailto:
 david.vigouroux@irt-saintexupery.com) and [Thomas FEL](http://thomasfel.fr).
 Later on, [Lucas Hervier](https://github.com/lucashervier) joined the team to
 transform the code base as a practical user-(almost)-friendly and efficient
-tool. ## ð License The package is released under _M_I_T_ _l_i_c_e_n_s_e.
+tool. ## ðï¸ Citation If you use Influenciae as part of your workflow in a
+scientific publication, please consider citing the ðï¸ [official paper]
+(https://hal.science/hal-04284178/): ``` @unpublished{picard:hal-04284178,
+TITLE = {{Influenci{\ae}: A library for tracing the influence back to the data-
+points}}, AUTHOR = {Picard, Agustin Martin and Hervier, Lucas and Fel, Thomas
+and Vigouroux, David}, URL = {https://hal.science/hal-04284178}, NOTE =
+{working paper or preprint}, YEAR = {2023}, MONTH = Nov, KEYWORDS = {Data-
+centric ai ; XAI ; Explainability ; Influence Functions ; Open-source toolbox},
+PDF = {https://hal.science/hal-04284178/file/ms.pdf}, HAL_ID = {hal-04284178},
+HAL_VERSION = {v1}, } ``` ## ð License The package is released under _M_I_T
+_l_i_c_e_n_s_e.
```

### Comparing `Influenciae-0.2.0/deel/influenciae/__init__.py` & `Influenciae-0.3.0/deel/influenciae/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Influenciae
 -------
 
 The goal of Influenciae is to provide a simple interface to the various influence functions
 techniques
 """
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 from . import influence
 from . import common
 from . import rps
 from . import trac_in
 from . import benchmark
 from . import plots
```

### Comparing `Influenciae-0.2.0/deel/influenciae/benchmark/base_benchmark.py` & `Influenciae-0.3.0/deel/influenciae/benchmark/base_benchmark.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/benchmark/cifar10_benchmark.py` & `Influenciae-0.3.0/deel/influenciae/benchmark/cifar10_benchmark.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ----------
     model
         Either a string for the base model ('resnet', 'efficient_net' or 'vgg19'), or a TF
         base model itself.
     use_regularization
         A boolean indicating whether to add regularization on the final model's last layer.
     """
-    def __init__(self, model: Union[str, Model], use_regularization: bool = True, **kwargs):
+    def __init__(self, model: Union[str, Model], use_regularization: bool = True, use_bias: bool = True, **kwargs):
         super().__init__(**kwargs)
         if isinstance(model, Model):
             base_model = model
         else:
             if model == 'resnet':
                 base_model = ResNet(input_shape=(32, 32, 3), include_top=False, block='basic_block',
                                     residual_unit='v1',
@@ -69,17 +69,22 @@
             dense_1 = Dense(128)
         self.add(dense_1)
 
         self.add(Dropout(0.4))
         self.add(tf.keras.layers.LeakyReLU())
 
         if use_regularization:
-            dense_2 = Dense(10, kernel_regularizer=L1L2(l1=1e-4, l2=1e-4), kernel_initializer="he_normal")
+            dense_2 = Dense(
+                10,
+                kernel_regularizer=L1L2(l1=1e-4, l2=1e-4),
+                kernel_initializer="he_normal",
+                use_bias=use_bias
+            )
         else:
-            dense_2 = Dense(10)
+            dense_2 = Dense(10, use_bias=use_bias)
 
         self.add(dense_2)
 
 
 class Cifar10TrainingProcedure(BaseTrainingProcedure):
     """
     A class for streamlining the process of training models on the CIFAR-10 dataset.
@@ -88,14 +93,16 @@
     ----------
     epochs
         An integer indicating for how long the model should be trained
     model_type
         A string with the type of model to use. Either 'resnet', 'efficient_net' or 'vgg19'.
     use_regu
         A boolean indicating whether L1L2 regularization should be used on the last layer.
+    use_bias
+        A boolean for adding a bias to the last layer.
     force_overfit
         A boolean for if the training schedule to be used should try to overfit the model or not.
     epochs_to_save
         A list of integers for the eventual saving of the model's checkpoints and training information.
         Useful for computing influence-related quantities using TracIn.
     verbose
         A boolean indicating whether to print the progress to stdout.
@@ -103,22 +110,24 @@
         A boolean indicating the use of tensorboard for logging.
     """
     def __init__(
             self,
             epochs: int = 60,
             model_type: str = 'resnet',
             use_regu: bool = True,
+            use_bias: bool = True,
             force_overfit: bool = False,
             epochs_to_save: Optional[List[int]] = None,
             verbose: bool = True,
             use_tensorboard: bool = False
     ):
         self.epochs = epochs
         self.model_type = model_type
         self.use_regu = use_regu
+        self.use_bias = use_bias
         self.force_overfit = force_overfit
         self.epochs_to_save = epochs_to_save
         self.verbose = verbose
         self.use_tensorboard = use_tensorboard
         # first order
         self.schedule = [(10, 0.5), (20, 0.5), (30, 0.5), (40, 0.5), (50, 0.5)]
         self.learning_rate = 1E-3
@@ -167,15 +176,15 @@
 
         training_dataset = training_dataset.shuffle(1000).batch(train_batch_size)
         training_dataset_augment = training_dataset.map(lambda x, y: (preprocess(x), y))
         training_dataset_augment = training_dataset_augment.prefetch(100)
 
         test_dataset = test_dataset.batch(test_batch_size).prefetch(100)
 
-        model = ConvNetCIFAR(self.model_type, self.use_regu)
+        model = ConvNetCIFAR(self.model_type, self.use_regu, self.use_bias)
 
         loss = CategoricalCrossentropy(from_logits=True)
 
         if self.force_overfit:
             def LearningRateSchedulerMaxMin(lr_start=0.01, lr_end=0.0001, epochs=100):
                 lr_decay = (lr_end / lr_start) ** (1. / epochs)
                 return tf.keras.callbacks.LearningRateScheduler(lambda e: lr_start * lr_decay ** e)
@@ -262,14 +271,15 @@
     """
     def __init__(
             self,
             epochs: int = 60,
             model_type: str = 'resnet',
             mislabeling_ratio: float = 0.0005,
             use_regu: bool = True,
+            use_bias: bool = True,
             force_overfit: bool = False,
             train_batch_size: int = 128,
             test_batch_size: int = 128,
             influence_batch_size: Optional[int] = None,
             epochs_to_save: Optional[List[int]] = None,
             take_batch: Optional[int] = None,
             verbose_training: bool = True,
@@ -277,14 +287,15 @@
         ): # pylint: disable=R0913
 
         config = {
             "epochs": epochs,
             "model_type": model_type,
             "mislabeling_ratio": mislabeling_ratio,
             "use_regularization": use_regu,
+            "use_bias": use_bias,
             "optimizer": 'sgd' if force_overfit else 'adam',
             "train_batch_size": train_batch_size,
             "test_batch_size": test_batch_size,
             "epochs_to_save": epochs_to_save if epochs_to_save is not None else [],
             "samples_to_take": take_batch if take_batch is not None else -1,
         }
 
@@ -297,15 +308,15 @@
 
         training_dataset = tf.data.Dataset.from_tensor_slices((x_train, y_train))
         test_dataset = tf.data.Dataset.from_tensor_slices((x_test, y_test))
 
         if take_batch is not None:
             training_dataset = training_dataset.take(take_batch)
             test_dataset = test_dataset.take(take_batch)
-        training_procedure = Cifar10TrainingProcedure(epochs, model_type, use_regu, force_overfit, epochs_to_save,
-                                                      verbose_training, use_tensorboard)
+        training_procedure = Cifar10TrainingProcedure(epochs, model_type, use_regu, use_bias, force_overfit,
+                                                      epochs_to_save, verbose_training, use_tensorboard)
         super().__init__(training_dataset, test_dataset, training_procedure,
                          nb_classes=10, mislabeling_ratio=mislabeling_ratio,
                          train_batch_size=train_batch_size,
                          test_batch_size=test_batch_size,
                          influence_batch_size=influence_batch_size,
                          config=config)
```

### Comparing `Influenciae-0.2.0/deel/influenciae/benchmark/influence_factory.py` & `Influenciae-0.3.0/deel/influenciae/benchmark/influence_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,17 +198,15 @@
         """
         influence_model = InfluenceModel(model, start_layer=self.start_layer, loss_function=self.loss_function)
 
         if self.dataset_hessian_size is None or self.dataset_hessian_size < 0:
             dataset_hessian = training_dataset
         else:
             batch_size = training_dataset._batch_size.numpy()  # pylint: disable=W0212
-            take_size = int(
-                np.ceil(float(self.dataset_hessian_size) / batch_size)) * batch_size
-            dataset_hessian = training_dataset.take(take_size)
+            dataset_hessian = training_dataset.unbatch().take(self.dataset_hessian_size).batch(batch_size)
 
         if self.ihvp_mode == 'exact':
             ihvp_calculator_factory = ExactIHVPFactory()
         elif self.ihvp_mode == 'cgd':
             ihvp_calculator_factory = CGDIHVPFactory(self.feature_extractor, self.n_opt_iters)
         elif self.ihvp_mode == 'lissa':
             ihvp_calculator_factory = LissaIHVPFactory(self.feature_extractor, self.n_opt_iters, damping=1e-4, scale=5.)
```

### Comparing `Influenciae-0.2.0/deel/influenciae/benchmark/model_resnet.py` & `Influenciae-0.3.0/deel/influenciae/benchmark/model_resnet.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/boundary_based/__init__.py` & `Influenciae-0.3.0/deel/influenciae/boundary_based/__init__.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/boundary_based/sample_boundary.py` & `Influenciae-0.3.0/deel/influenciae/boundary_based/sample_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         x2 = tf.gather(x, tf.expand_dims(indexes_2, axis=1), batch_dims=1)
 
         delta_x = x1 - tf.repeat(x2, tf.shape(x1)[1], axis=1)
 
         return delta_x
 
     @tf.function
-    def __step(self, x: tf.Tensor, y_pred: tf.Tensor) -> Tuple[tf.Tensor, tf.Tensor, tf.Tensor]:
+    def _step(self, x: tf.Tensor, y_pred: tf.Tensor) -> Tuple[tf.Tensor, tf.Tensor, tf.Tensor]:
         """
         The optimization step to find the distance between the boundary and a given sample x.
 
         Notes
         -----
         To see more details about the optimization procedure for multi-class classifier, please
         refer to [https://arxiv.org/abs/1511.04599]
@@ -159,15 +159,15 @@
         score
             The influence score of the sample.
         """
         x = tf.expand_dims(x, axis=0)
         y_pred = self.model(x)
 
         def body(index, x_current):
-            computation, _, x_new = self.__step(x_current, y_pred)
+            computation, _, x_new = self._step(x_current, y_pred)
             return computation, index + 1, x_new
 
         _, _, x_adversarial = tf.while_loop(
             lambda cond, index, x_current: tf.logical_and(cond, index < self.step_nbr),
             lambda cond, index, x_current: body(index, x_current),
             [tf.constant(True), tf.constant(0, dtype=tf.int32), x])
```

### Comparing `Influenciae-0.2.0/deel/influenciae/boundary_based/weights_boundary.py` & `Influenciae-0.3.0/deel/influenciae/boundary_based/weights_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         x2 = tf.gather(x, tf.expand_dims(indexes_2, axis=1), batch_dims=1)
 
         delta_x = x1 - tf.repeat(x2, tf.shape(x1)[1], axis=1)
 
         return delta_x
 
     @tf.function
-    def __step(self, x: tf.Tensor, y_pred: tf.Tensor) -> Tuple[tf.Tensor, tf.Tensor]:
+    def _step(self, x: tf.Tensor, y_pred: tf.Tensor) -> Tuple[tf.Tensor, tf.Tensor]:
         """
         The optimization step to find the distance between the boundary and a given sample x.
         To see more details about the optimization procedure for multi-class classifiers,
         please refer to [https://arxiv.org/abs/1511.04599]
 
         Notes
         -----
@@ -207,15 +207,15 @@
             The influence score of the sample.
         """
 
         x = tf.expand_dims(x, axis=0)
         y_pred = self.model(x)
 
         tf.while_loop(lambda cond, index: tf.logical_and(cond, index < self.step_nbr),
-                      lambda cond, index: (self.__step(x, y_pred)[0], index + 1),
+                      lambda cond, index: (self._step(x, y_pred)[0], index + 1),
                       [tf.constant(True), tf.constant(0, dtype=tf.int32)])
 
         score = self.__delta_weights()
 
         self.__reset_weights()
 
         return score
```

### Comparing `Influenciae-0.2.0/deel/influenciae/common/__init__.py` & `Influenciae-0.3.0/deel/influenciae/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/common/base_influence.py` & `Influenciae-0.3.0/deel/influenciae/common/base_influence.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,38 +265,14 @@
         inf_vect_ds = map_to_device(train_set, lambda *batch: (batch, self._compute_influence_vector(batch)), device)
         if save_influence_vector_ds_path is not None:
             inf_vect = inf_vect_ds.map(lambda *batch: batch[-1])
             self._save_dataset(inf_vect.unbatch(), save_influence_vector_ds_path)
 
         return inf_vect_ds
 
-    @abstractmethod
-    def _estimate_individual_influence_values_from_batch(
-            self,
-            train_samples: Tuple[tf.Tensor, ...],
-            samples_to_evaluate: Tuple[tf.Tensor, ...]
-    ) -> tf.Tensor:
-        """
-        Estimate the (individual) influence scores of a single batch of samples with respect to
-        a batch of samples belonging to the model's training dataset.
-
-        Parameters
-        ----------
-        train_samples
-            A single batch of training samples (and their target values).
-        samples_to_evaluate
-            A single batch of samples of which we wish to compute the influence of removing the training
-            samples.
-
-        Returns
-        -------
-        A tensor containing the individual influence scores.
-        """
-        raise NotImplementedError()
-
     def estimate_influence_values_in_batches(
             self,
             dataset_to_evaluate: tf.data.Dataset,
             train_set: tf.data.Dataset,
             influence_vector_in_cache: CACHE = CACHE.MEMORY,
             load_influence_vector_path: Optional[str] = None,
             save_influence_vector_path: Optional[str] = None,
```

### Comparing `Influenciae-0.2.0/deel/influenciae/common/ihvp_factory.py` & `Influenciae-0.3.0/deel/influenciae/common/ihvp_factory.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/common/inverse_hessian_vector_product.py` & `Influenciae-0.3.0/deel/influenciae/common/inverse_hessian_vector_product.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/common/model_wrappers.py` & `Influenciae-0.3.0/deel/influenciae/common/model_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
     def __init__(self,
                  model: tf.keras.Model,
                  start_layer: Optional[Union[str, int]] = None,
                  last_layer: Optional[Union[str, int]] = None,
                  loss_function: Callable = tf.keras.losses.CategoricalCrossentropy(
                      from_logits=False, reduction=Reduction.NONE),
                  process_batch_for_loss_fn: ProcessBatchTypeAlias = default_process_batch):
-
+        self.start_layer = start_layer
         weights_to_watch = InfluenceModel._get_weights_of_interest(model, start_layer, last_layer)
         super().__init__(model, weights_to_watch, loss_function, process_batch_for_loss_fn, weights_processed=True)
 
     @staticmethod
     def _get_weights_of_interest(model: tf.keras.Model,
                                  start_layer: Optional[Union[str, int]],
                                  last_layer: Optional[Union[str, int]]) -> list:
```

### Comparing `Influenciae-0.2.0/deel/influenciae/influence/__init__.py` & `Influenciae-0.3.0/deel/influenciae/influence/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 # =====================================================================================
 """
 Influence function module
 """
 from .first_order_influence_calculator import FirstOrderInfluenceCalculator
 from .second_order_influence_calculator import SecondOrderInfluenceCalculator
 from .arnoldi_influence_calculator import ArnoldiInfluenceCalculator
+from .base_group_influence import BaseGroupInfluenceCalculator
```

### Comparing `Influenciae-0.2.0/deel/influenciae/influence/arnoldi_influence_calculator.py` & `Influenciae-0.3.0/deel/influenciae/influence/arnoldi_influence_calculator.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/influence/base_group_influence.py` & `Influenciae-0.3.0/deel/influenciae/influence/base_group_influence.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,19 @@
             dataset_to_estimate_hessian = dataset.unbatch().shuffle(shuffle_buffer_size)\
                 .take(n_samples_for_hessian).batch(dataset._batch_size)
 
         self.train_set = dataset_to_estimate_hessian
 
         # load ivhp calculator from str, IHVPcalculator enum or InverseHessianVectorProduct object
         if isinstance(ihvp_calculator, str):
-            self.ihvp_calculator = IHVPCalculator.from_string(ihvp_calculator).value(self.model,
-                                                                                     self.train_set)
+            self.ihvp_calculator = IHVPCalculator.from_string(ihvp_calculator).value(self.model, self.train_set) if \
+                ihvp_calculator == 'exact' else \
+                IHVPCalculator.from_string(ihvp_calculator).value(self.model,
+                                                                  self.model.start_layer,
+                                                                  self.train_set)
         elif isinstance(ihvp_calculator, IHVPCalculator):
             self.ihvp_calculator = ihvp_calculator.value(self.model, self.train_set)
         elif isinstance(ihvp_calculator, InverseHessianVectorProduct):
             self.ihvp_calculator = ihvp_calculator
 
     @abstractmethod
     def compute_influence_vector_group(
```

### Comparing `Influenciae-0.2.0/deel/influenciae/influence/first_order_influence_calculator.py` & `Influenciae-0.3.0/deel/influenciae/influence/first_order_influence_calculator.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/influence/second_order_influence_calculator.py` & `Influenciae-0.3.0/deel/influenciae/influence/second_order_influence_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,13 +203,15 @@
             measure the influence of removing the training points.
 
         Returns
         -------
         influence_values_group
             A tensor containing one influence value for the whole group.
         """
+        if group_to_evaluate is None:
+            group_to_evaluate = group_train
         ds_size = self.assert_compatible_datasets(group_train, group_to_evaluate)
         influence = tf.transpose(self.compute_influence_vector_group(group_train))
         reduced_grads = tf.reduce_sum(tf.reshape(self.model.batch_jacobian(group_to_evaluate),
                                                  (ds_size, -1)), axis=0, keepdims=True)
 
         return tf.matmul(reduced_grads, influence)
```

### Comparing `Influenciae-0.2.0/deel/influenciae/plots/benchmark.py` & `Influenciae-0.3.0/deel/influenciae/plots/benchmark.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/plots/image.py` & `Influenciae-0.3.0/deel/influenciae/plots/image.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/trac_in/tracin.py` & `Influenciae-0.3.0/deel/influenciae/trac_in/tracin.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/utils/__init__.py` & `Influenciae-0.3.0/deel/influenciae/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,11 +12,12 @@
      from_layer_name_to_layer_idx,
      is_dataset_batched,
      assert_batched_dataset,
      dataset_size,
      default_process_batch,
      dataset_to_tensor,
      array_to_dataset,
-     map_to_device
+     map_to_device,
+     split_model,
 )
 from .sorted_dict import BatchSort, ORDER
 from .nearest_neighbors import BaseNearestNeighbors, LinearNearestNeighbors
```

### Comparing `Influenciae-0.2.0/deel/influenciae/utils/backtracking_line_search.py` & `Influenciae-0.3.0/deel/influenciae/utils/backtracking_line_search.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/utils/conjugate_gradients.py` & `Influenciae-0.3.0/deel/influenciae/utils/conjugate_gradients.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/utils/nearest_neighbors.py` & `Influenciae-0.3.0/deel/influenciae/utils/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/utils/sorted_dict.py` & `Influenciae-0.3.0/deel/influenciae/utils/sorted_dict.py`

 * *Files identical despite different names*

### Comparing `Influenciae-0.2.0/deel/influenciae/utils/tf_operations.py` & `Influenciae-0.3.0/deel/influenciae/utils/tf_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,14 +53,41 @@
     """
     for layer_idx, layer in enumerate(model.layers):
         if layer.name == layer_name:
             return layer_idx
     raise ValueError(f'No such layer: {layer_name}. Existing layers are: '
                      f'{list(layer.name for layer in model.layers)}.')
 
+def split_model(model: tf.keras.Model, target_layer: Union[str, int]) -> Tuple[tf.keras.Model, tf.keras.Model]:
+    """
+    Splits a model into two sub-models, one containing the layers up to the target layer, and the other containing
+    the layers from the target layer onwards.
+
+    Parameters
+    ----------
+    model
+        Model to split
+    target_layer
+        Layer name or layer index
+
+    Returns
+    -------
+    model_1
+        Model containing the layers up to the target layer
+    model_2
+        Model containing the layers from the target layer onwards
+    """
+    cloned_model = tf.keras.models.clone_model(model)
+    cloned_model.set_weights(model.get_weights())
+    cut_layer = find_layer(cloned_model, target_layer)
+    model_1 = tf.keras.Model(inputs=cloned_model.inputs, outputs=cut_layer.input)
+    model_2 = tf.keras.Model(inputs=tf.keras.Input(tensor=cut_layer.input), outputs=cloned_model.outputs)
+
+    return model_1, model_2
+
 
 def is_dataset_batched(dataset: tf.data.Dataset) -> Union[int, bool]:
     """
     Ensure the dataset is batched, if true return the batch_size else false.
 
     Parameters
     ----------
```

### Comparing `Influenciae-0.2.0/setup.py` & `Influenciae-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as fh:
     README = fh.read()
 
 setup(
     name="Influenciae",
-    version="0.2.0",
+    version="0.3.0",
     description="A Tensorflow Toolbox for Influence Functions",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DEEL Core Team",
     author_email="agustin-martin.picard@irt-saintexupery.com",
     license="MIT",
     install_requires=['tensorflow >=2.7.0, <2.10.0', 'numpy', 'matplotlib'],
```

