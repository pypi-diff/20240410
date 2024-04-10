# Comparing `tmp/pystreed-1.2.2.tar.gz` & `tmp/pystreed-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystreed-1.2.2.tar", last modified: Thu Mar 21 10:19:20 2024, max compression
+gzip compressed data, was "pystreed-1.2.3.tar", last modified: Wed Apr 10 13:33:58 2024, max compression
```

## Comparing `pystreed-1.2.2.tar` & `pystreed-1.2.3.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.625261 pystreed-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-21 10:19:11.000000 pystreed-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15671 2024-03-21 10:19:20.625261 pystreed-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-03-21 10:19:11.000000 pystreed-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-21 10:19:15.000000 pystreed-1.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.617261 pystreed-1.2.2/pystreed/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19517 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/cost_sensitive_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/group_fair.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/prescriptive_policy_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/survival_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-21 10:19:15.000000 pystreed-1.2.2/pystreed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.625261 pystreed-1.2.2/pystreed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15671 2024-03-21 10:19:20.000000 pystreed-1.2.2/pystreed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-21 10:19:20.000000 pystreed-1.2.2/pystreed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:19:20.000000 pystreed-1.2.2/pystreed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-21 10:19:20.000000 pystreed-1.2.2/pystreed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-21 10:19:20.000000 pystreed-1.2.2/pystreed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:19:20.625261 pystreed-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-21 10:19:15.000000 pystreed-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.621261 pystreed-1.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.621261 pystreed-1.2.2/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/model/branch.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/model/data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/model/feature_vector.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.621261 pystreed-1.2.2/src/solver/
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/branch_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18849 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/cost_combiner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/cost_storage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/counter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/data_splitter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/dataset_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/define_parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/difference_computer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/feature_selector_gini.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/result.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/similarity_lowerbound.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    45224 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20817 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/solver/terminal_solver.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.625261 pystreed-1.2.2/src/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.625261 pystreed-1.2.2/src/tasks/accuracy/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/accuracy/accuracy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/accuracy/cost_complex_accuracy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/cost_sensitive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/eq_opp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/f1score.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/group_fairness.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/optimization_task.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/prescriptive_policy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/tasks/survival_analysis.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:19:20.625261 pystreed-1.2.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/utils/file_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/utils/key_value_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/utils/parameter_handler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-21 10:19:15.000000 pystreed-1.2.2/src/utils/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-10 13:33:49.000000 pystreed-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-04-10 13:33:58.209267 pystreed-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14005 2024-04-10 13:33:49.000000 pystreed-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 13:33:52.000000 pystreed-1.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.201267 pystreed-1.2.3/pystreed/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19517 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/cost_sensitive_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/group_fair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/instance_cost_sensitive_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/prescriptive_policy_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/survival_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/pystreed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:33:58.209267 pystreed-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-10 13:33:52.000000 pystreed-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.205267 pystreed-1.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.205267 pystreed-1.2.3/src/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/model/branch.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/model/data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/model/feature_vector.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.205267 pystreed-1.2.3/src/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/branch_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/cost_combiner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/cost_storage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/counter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/data_splitter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/dataset_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/define_parameters.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/difference_computer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/feature_selector_gini.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/result.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/similarity_lowerbound.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45271 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20872 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/terminal_solver.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/src/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/src/tasks/accuracy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/accuracy/accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/accuracy/cost_complex_accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/cost_sensitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/eq_opp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/f1score.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/group_fairness.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/instance_cost_sensitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/optimization_task.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/prescriptive_policy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/survival_analysis.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/file_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/key_value_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/parameter_handler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/utils.cpp
```

### Comparing `pystreed-1.2.2/LICENSE` & `pystreed-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/PKG-INFO` & `pystreed-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystreed
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Implementation of STreeD: Dynamic Programming Approach for Optimal Decision Trees with Separable objectives and Constraints
 Author-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>, Emir Demirović <E.Demirovic@tudelft.nl>, "Mathijs M. de Weerdt" <M.M.deWeerdt@tudelft.nl>
 Maintainer-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>
 License: Copyright 2023 Jacobus G. M. van der Linden, Delft University of Technology
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -140,14 +140,21 @@
 
 The costs can be specified with `CostSpecifier` object. This object is either initialized with a file name for the cost specification and the number of classes; or with the misclassification cost matrix, and the cost specifier per feature. When testing a feature in a branch node, the cost for that feature is paid for every instance that passes through it. When another feature from the same group was tested before, the discounted cost is paid. When another feature that is binarized from the same original feature is already tested, the cost is zero.
 
 Note that currently `STreeDCostSensitiveClassifier` does not support automatic binarization.
 
 See [examples/cost_sensitive_example.py](examples/cost_sensitive_example.py) for an example.
 
+### Instance-Cost-Sensitive Classification
+`STreeDInstanceCostSensitiveClassifier` implements an instance-cost-sensitive classifier. Each instance can  have a different misclassification cost per label.
+
+The costs can be specified with a `CostVector` object. For each instance, initialize a `CostVector` object with a list of the costs for each possible label. 
+
+See [examples/instance_cost_sensitive_example.py](examples/instance_cost_sensitive_example.py) for an example.
+
 ### Classification under a Group Fairness constraint
 `STreeDGroupFairnessClassifier` implements a classifier that satisfies a group fairness constraint.
 The maximum amount of discrimination on the training data can be specified by the `discrimination-limit` parameter, e.g., 0.01 for maximum of 1% discrimination.
 
 Currently two fairness constraint optmization tasks are implemented:
 * `group-fairness`: This satisfies a _demographic parity_ constraint. Demographic parity requires that the positive rates for both groups is equal.
 * `equality-of-opportunity`: This satisfies a _equality of opportunity_ constraint. Equality of opportunity requires that the _true_ positive rates for both groups is equal.
```

### Comparing `pystreed-1.2.2/README.md` & `pystreed-1.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -112,14 +112,21 @@
 
 The costs can be specified with `CostSpecifier` object. This object is either initialized with a file name for the cost specification and the number of classes; or with the misclassification cost matrix, and the cost specifier per feature. When testing a feature in a branch node, the cost for that feature is paid for every instance that passes through it. When another feature from the same group was tested before, the discounted cost is paid. When another feature that is binarized from the same original feature is already tested, the cost is zero.
 
 Note that currently `STreeDCostSensitiveClassifier` does not support automatic binarization.
 
 See [examples/cost_sensitive_example.py](examples/cost_sensitive_example.py) for an example.
 
+### Instance-Cost-Sensitive Classification
+`STreeDInstanceCostSensitiveClassifier` implements an instance-cost-sensitive classifier. Each instance can  have a different misclassification cost per label.
+
+The costs can be specified with a `CostVector` object. For each instance, initialize a `CostVector` object with a list of the costs for each possible label. 
+
+See [examples/instance_cost_sensitive_example.py](examples/instance_cost_sensitive_example.py) for an example.
+
 ### Classification under a Group Fairness constraint
 `STreeDGroupFairnessClassifier` implements a classifier that satisfies a group fairness constraint.
 The maximum amount of discrimination on the training data can be specified by the `discrimination-limit` parameter, e.g., 0.01 for maximum of 1% discrimination.
 
 Currently two fairness constraint optmization tasks are implemented:
 * `group-fairness`: This satisfies a _demographic parity_ constraint. Demographic parity requires that the positive rates for both groups is equal.
 * `equality-of-opportunity`: This satisfies a _equality of opportunity_ constraint. Equality of opportunity requires that the _true_ positive rates for both groups is equal.
```

### Comparing `pystreed-1.2.2/pyproject.toml` & `pystreed-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "pybind11>=2.10.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pystreed"
-version = "1.2.2"
+version = "1.2.3"
 requires-python = ">=3.8"						 
 description = "Python Implementation of STreeD: Dynamic Programming Approach for Optimal Decision Trees with Separable objectives and Constraints"
 license=  {file = "LICENSE"}
 readme = "README.md"						
 authors = [
     {name = "Jacobus G. M. van der Linden", email="J.G.M.vanderLinden@tudelft.nl"},
     {name = "Emir Demirović", email="E.Demirovic@tudelft.nl"},
```

### Comparing `pystreed-1.2.2/pystreed/base.py` & `pystreed-1.2.3/pystreed/base.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/binarizer.py` & `pystreed-1.2.3/pystreed/binarizer.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/classification.py` & `pystreed-1.2.3/pystreed/classification.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/cost_sensitive_classification.py` & `pystreed-1.2.3/pystreed/cost_sensitive_classification.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/group_fair.py` & `pystreed-1.2.3/pystreed/group_fair.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/prescriptive_policy_generation.py` & `pystreed-1.2.3/pystreed/prescriptive_policy_generation.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/survival_analysis.py` & `pystreed-1.2.3/pystreed/survival_analysis.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed/utils.py` & `pystreed-1.2.3/pystreed/utils.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/pystreed.egg-info/PKG-INFO` & `pystreed-1.2.3/pystreed.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystreed
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Implementation of STreeD: Dynamic Programming Approach for Optimal Decision Trees with Separable objectives and Constraints
 Author-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>, Emir Demirović <E.Demirovic@tudelft.nl>, "Mathijs M. de Weerdt" <M.M.deWeerdt@tudelft.nl>
 Maintainer-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>
 License: Copyright 2023 Jacobus G. M. van der Linden, Delft University of Technology
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -140,14 +140,21 @@
 
 The costs can be specified with `CostSpecifier` object. This object is either initialized with a file name for the cost specification and the number of classes; or with the misclassification cost matrix, and the cost specifier per feature. When testing a feature in a branch node, the cost for that feature is paid for every instance that passes through it. When another feature from the same group was tested before, the discounted cost is paid. When another feature that is binarized from the same original feature is already tested, the cost is zero.
 
 Note that currently `STreeDCostSensitiveClassifier` does not support automatic binarization.
 
 See [examples/cost_sensitive_example.py](examples/cost_sensitive_example.py) for an example.
 
+### Instance-Cost-Sensitive Classification
+`STreeDInstanceCostSensitiveClassifier` implements an instance-cost-sensitive classifier. Each instance can  have a different misclassification cost per label.
+
+The costs can be specified with a `CostVector` object. For each instance, initialize a `CostVector` object with a list of the costs for each possible label. 
+
+See [examples/instance_cost_sensitive_example.py](examples/instance_cost_sensitive_example.py) for an example.
+
 ### Classification under a Group Fairness constraint
 `STreeDGroupFairnessClassifier` implements a classifier that satisfies a group fairness constraint.
 The maximum amount of discrimination on the training data can be specified by the `discrimination-limit` parameter, e.g., 0.01 for maximum of 1% discrimination.
 
 Currently two fairness constraint optmization tasks are implemented:
 * `group-fairness`: This satisfies a _demographic parity_ constraint. Demographic parity requires that the positive rates for both groups is equal.
 * `equality-of-opportunity`: This satisfies a _equality of opportunity_ constraint. Equality of opportunity requires that the _true_ positive rates for both groups is equal.
```

### Comparing `pystreed-1.2.2/pystreed.egg-info/SOURCES.txt` & `pystreed-1.2.3/pystreed.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pystreed/__init__.py
 pystreed/base.py
 pystreed/binarizer.py
 pystreed/classification.py
 pystreed/cost_sensitive_classification.py
 pystreed/data.py
 pystreed/group_fair.py
+pystreed/instance_cost_sensitive_classification.py
 pystreed/prescriptive_policy_generation.py
 pystreed/survival_analysis.py
 pystreed/utils.py
 pystreed.egg-info/PKG-INFO
 pystreed.egg-info/SOURCES.txt
 pystreed.egg-info/dependency_links.txt
 pystreed.egg-info/requires.txt
@@ -36,14 +37,15 @@
 src/solver/similarity_lowerbound.cpp
 src/solver/solver.cpp
 src/solver/terminal_solver.cpp
 src/tasks/cost_sensitive.cpp
 src/tasks/eq_opp.cpp
 src/tasks/f1score.cpp
 src/tasks/group_fairness.cpp
+src/tasks/instance_cost_sensitive.cpp
 src/tasks/optimization_task.cpp
 src/tasks/prescriptive_policy.cpp
 src/tasks/survival_analysis.cpp
 src/tasks/accuracy/accuracy.cpp
 src/tasks/accuracy/cost_complex_accuracy.cpp
 src/utils/file_reader.cpp
 src/utils/key_value_heap.cpp
```

### Comparing `pystreed-1.2.2/src/bindings.cpp` & `pystreed-1.2.3/src/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 namespace py = pybind11;
 using namespace STreeD;
 
 enum task_type {
     accuracy,
     cost_complex_accuracy,
     cost_sensitive,
+    instance_cost_sensitive,
     f1score,
     group_fairness,
     equality_of_opportunity,
     prescriptive_policy,
     survival_analysis
 };
 
 task_type get_task_type_code(std::string& task) {
     if (task == "accuracy") return accuracy;
     else if (task == "cost-complex-accuracy") return cost_complex_accuracy;
     else if (task == "cost-sensitive") return cost_sensitive;
+    else if (task == "instance-cost-sensitive") return instance_cost_sensitive;
     else if (task == "f1-score") return f1score;
     else if (task == "group-fairness") return group_fairness;
     else if (task == "equality-of-opportunity") return equality_of_opportunity;
     else if (task == "prescriptive-policy") return prescriptive_policy;
     else if (task == "survival-analysis") return survival_analysis;
     else {
         std::cout << "Encountered unknown optimization task: " << task << std::endl;
@@ -255,14 +257,15 @@
     DefineSolver<Accuracy>(m, "Accuracy");
     DefineSolver<CostComplexAccuracy>(m, "CostComplexAccuracy");
     DefineSolver<F1Score>(m, "F1Score");
     DefineSolver<SurvivalAnalysis>(m, "Survival");
     DefineSolver<PrescriptivePolicy>(m, "PrescriptivePolicy");
     DefineSolver<GroupFairness>(m, "GroupFairness");
     DefineSolver<EqOpp>(m, "EqOpp");
+    DefineSolver<InstanceCostSensitive>(m, "InstanceCostSensitive");
     py::class_<Solver<CostSensitive>> cost_sensitive_solver = DefineSolver<CostSensitive>(m, "CostSensitive");
     cost_sensitive_solver.def("specify_costs", [](Solver<CostSensitive>& solver, const CostSpecifier& cost_specifier) {
         solver.GetTask()->UpdateCostSpecifier(cost_specifier);
     });
 
     m.def("initialize_streed_solver", [](ParameterHandler& parameters) {
         py::scoped_ostream_redirect stream(std::cout, py::module_::import("sys").attr("stdout"));
@@ -280,14 +283,15 @@
 
         STreeD::AbstractSolver* solver;
         std::string task = parameters.GetStringParameter("task");
         switch(get_task_type_code(task)) {
             case accuracy: solver = new Solver<Accuracy>(parameters, &rng); break;
             case cost_complex_accuracy: solver = new Solver<CostComplexAccuracy>(parameters, &rng); break;
             case cost_sensitive: solver = new Solver<CostSensitive>(parameters, &rng); break;
+            case instance_cost_sensitive: solver = new Solver<InstanceCostSensitive>(parameters, &rng); break;
             case f1score: solver = new Solver<F1Score>(parameters, &rng); break;
             case group_fairness: solver = new Solver<GroupFairness>(parameters, &rng); break;
             case equality_of_opportunity: solver = new Solver<EqOpp>(parameters, &rng); break;
             case prescriptive_policy: solver = new Solver<PrescriptivePolicy>(parameters, &rng); break;
             case survival_analysis: solver = new Solver<SurvivalAnalysis>(parameters, &rng); break;
         }
         return solver;
@@ -308,15 +312,20 @@
         .def(py::init<>())
         .def_readonly("historic_treatment", &PPGData::k)
         .def_readonly("historic_outcome", &PPGData::y)
         .def_readonly("propensity_score", &PPGData::mu)
         .def_readonly("predicted_outcome", &PPGData::yhat)
         .def_readonly("optimal_treatment", &PPGData::k_opt)
         .def_readonly("counterfactual_outcome", &PPGData::cf_y);
-        
+       
+    py::class_<InstanceCostSensitiveData>(m, "CostVector")
+        .def(py::init<std::vector<double>&>())
+        .def(py::init<>())
+        .def_readonly("costs", &InstanceCostSensitiveData::costs);
+
     /*************************************
            Label
      ************************************/
     py::class_<FeatureCostSpecifier>(m, "FeatureCostSpecifier")
         .def(py::init<double, double, const std::string&, int, int>())
         .def_readonly("feature_cost", &FeatureCostSpecifier::feature_cost)
         .def_readonly("discount_cost", &FeatureCostSpecifier::discount_cost)
```

### Comparing `pystreed-1.2.2/src/main.cpp` & `pystreed-1.2.3/src/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 		STreeD::FileReader::ReadData<STreeD::Accuracy>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "cost-complex-accuracy") {
 		solver =  new STreeD::Solver<STreeD::CostComplexAccuracy>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::CostComplexAccuracy>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "cost-sensitive") {
 		solver =  new STreeD::Solver<STreeD::CostSensitive>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::CostSensitive>(parameters, data, train_data, test_data, &rng);
+	} else if (task == "instance-cost-sensitive") {
+		solver = new STreeD::Solver<STreeD::InstanceCostSensitive>(parameters, &rng);
+		STreeD::FileReader::ReadData<STreeD::InstanceCostSensitive>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "f1-score") {
 		solver =  new STreeD::Solver<STreeD::F1Score>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::F1Score>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "group-fairness") {
 		solver =  new STreeD::Solver<STreeD::GroupFairness>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::GroupFairness>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "equality-of-opportunity") {
```

### Comparing `pystreed-1.2.2/src/model/branch.cpp` & `pystreed-1.2.3/src/model/branch.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/model/data.cpp` & `pystreed-1.2.3/src/model/data.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/model/feature_vector.cpp` & `pystreed-1.2.3/src/model/feature_vector.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/solver/branch_cache.cpp` & `pystreed-1.2.3/src/solver/branch_cache.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
 		return int(count);
 	}
 
 	template class BranchCache<Accuracy>;
 	template class BranchCache<CostComplexAccuracy>;
 	
 	template class BranchCache<CostSensitive>;
+	template class BranchCache<InstanceCostSensitive>;
 	template class BranchCache<F1Score>;
 	template class BranchCache<GroupFairness>;
 	template class BranchCache<EqOpp>;
 	template class BranchCache<PrescriptivePolicy>;
 	template class BranchCache<SurvivalAnalysis>;
 
 }
```

### Comparing `pystreed-1.2.2/src/solver/cache.cpp` & `pystreed-1.2.3/src/solver/cache.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 		// Dataset caching do not need to transfer equivalent branches
 	}
 
 	template class Cache<Accuracy>;
 	template class Cache<CostComplexAccuracy>;
 
 	template class Cache<CostSensitive>;
+	template class Cache<InstanceCostSensitive>;
 	template class Cache<F1Score>;
 	template class Cache<GroupFairness>;
 	template class Cache<EqOpp>;
 	template class Cache<PrescriptivePolicy>;
 	template class Cache<SurvivalAnalysis>;
 
 }
```

### Comparing `pystreed-1.2.2/src/solver/cost_combiner.cpp` & `pystreed-1.2.3/src/solver/cost_combiner.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -472,14 +472,15 @@
 		}
 	}
 
 	template class CostCalculator<Accuracy>;
 	template class CostCalculator<CostComplexAccuracy>;
 
 	template class CostCalculator<CostSensitive>;
+	template class CostCalculator<InstanceCostSensitive>;
 	template class CostCalculator<F1Score>;
 	template class CostCalculator<GroupFairness>;
 
 	template class CostCalculator<EqOpp>;
 	template class CostCalculator<PrescriptivePolicy>;
 	template class CostCalculator<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.2/src/solver/cost_storage.cpp` & `pystreed-1.2.3/src/solver/cost_storage.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 		return num_features * index_row - index_row * (index_row + 1) / 2;
 	}
 
 	template class CostStorage<Accuracy>;
 	template class CostStorage<CostComplexAccuracy>;
 
 	template class CostStorage<CostSensitive>;
+	template class CostStorage<InstanceCostSensitive>;
 	template class CostStorage<F1Score>;
 	template class CostStorage<GroupFairness>;
 	template class CostStorage<EqOpp>;
 	template class CostStorage<PrescriptivePolicy>;
 	template class CostStorage<SurvivalAnalysis>;
 
 }
```

### Comparing `pystreed-1.2.2/src/solver/counter.cpp` & `pystreed-1.2.3/src/solver/counter.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/solver/data_splitter.cpp` & `pystreed-1.2.3/src/solver/data_splitter.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/solver/dataset_cache.cpp` & `pystreed-1.2.3/src/solver/dataset_cache.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
 		return iter;
 	}
 
 	template class DatasetCache<Accuracy>;
 	template class DatasetCache<CostComplexAccuracy>;
 
 	template class DatasetCache<CostSensitive>;
+	template class DatasetCache<InstanceCostSensitive>;
 	template class DatasetCache<F1Score>;
 	template class DatasetCache<GroupFairness>;
 	template class DatasetCache<EqOpp>;
 	template class DatasetCache<PrescriptivePolicy>;
 	template class DatasetCache<SurvivalAnalysis>;
 
 }
```

### Comparing `pystreed-1.2.2/src/solver/define_parameters.cpp` & `pystreed-1.2.3/src/solver/define_parameters.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		parameters.DefineStringParameter
 		(
 			"task",
 			"Task to optimize.",
 			"accuracy",
 			"Main Parameters",
 			{"accuracy", "cost-complex-accuracy", "f1-score", "group-fairness", "survival-analysis",
-			"equality-of-opportunity", "cost-sensitive", "prescriptive-policy" }
+			"equality-of-opportunity", "cost-sensitive", "prescriptive-policy", "instance-cost-sensitive"}
 		);
 
 		parameters.DefineBooleanParameter
 		(
 			"hyper-tune",
 			"Enable/disable hyper-tuning.",
 			false,
```

### Comparing `pystreed-1.2.2/src/solver/difference_computer.cpp` & `pystreed-1.2.3/src/solver/difference_computer.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/solver/feature_selector_gini.cpp` & `pystreed-1.2.3/src/solver/feature_selector_gini.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/solver/similarity_lowerbound.cpp` & `pystreed-1.2.3/src/solver/similarity_lowerbound.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -135,12 +135,13 @@
 	}
 
 
 	template class SimilarityLowerBoundComputer<Accuracy>;
 	template class SimilarityLowerBoundComputer<CostComplexAccuracy>;
 
 	template class SimilarityLowerBoundComputer<CostSensitive>;
+	template class SimilarityLowerBoundComputer<InstanceCostSensitive>;
 	template class SimilarityLowerBoundComputer<F1Score>;
 	template class SimilarityLowerBoundComputer<GroupFairness>;
 	template class SimilarityLowerBoundComputer<EqOpp>;
 	template class SimilarityLowerBoundComputer<PrescriptivePolicy>;
 }
```

### Comparing `pystreed-1.2.2/src/solver/solver.cpp` & `pystreed-1.2.3/src/solver/solver.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1010,14 +1010,15 @@
 		return labels;
 	}
 
 	template class Solver<Accuracy>;
 	template class Solver<CostComplexAccuracy>;
 
 	template class Solver<CostSensitive>;
+	template class Solver<InstanceCostSensitive>;
 	template class Solver<F1Score>;
 	template class Solver<GroupFairness>;
 	template class Solver<EqOpp>;
 	template class Solver<PrescriptivePolicy>;
 	template class Solver<SurvivalAnalysis>;
 }
```

### Comparing `pystreed-1.2.2/src/solver/terminal_solver.cpp` & `pystreed-1.2.3/src/solver/terminal_solver.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -449,14 +449,15 @@
 		}
 	}
 
 	template class TerminalSolver<Accuracy>;
 	template class TerminalSolver<CostComplexAccuracy>;
 
 	template class TerminalSolver<CostSensitive>;
+	template class TerminalSolver<InstanceCostSensitive>;
 	template class TerminalSolver<F1Score>;
 	template class TerminalSolver<GroupFairness>;
 	template class TerminalSolver<EqOpp>;
 	template class TerminalSolver<PrescriptivePolicy>;
 	template class TerminalSolver<SurvivalAnalysis>;
 
 }
```

### Comparing `pystreed-1.2.2/src/tasks/accuracy/cost_complex_accuracy.cpp` & `pystreed-1.2.3/src/tasks/accuracy/cost_complex_accuracy.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/cost_sensitive.cpp` & `pystreed-1.2.3/src/tasks/cost_sensitive.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/eq_opp.cpp` & `pystreed-1.2.3/src/tasks/eq_opp.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/f1score.cpp` & `pystreed-1.2.3/src/tasks/f1score.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/group_fairness.cpp` & `pystreed-1.2.3/src/tasks/group_fairness.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/optimization_task.cpp` & `pystreed-1.2.3/src/tasks/optimization_task.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/prescriptive_policy.cpp` & `pystreed-1.2.3/src/tasks/prescriptive_policy.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/tasks/survival_analysis.cpp` & `pystreed-1.2.3/src/tasks/survival_analysis.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/utils/file_reader.cpp` & `pystreed-1.2.3/src/utils/file_reader.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 	}
 
 
 	template void FileReader::ReadData<Accuracy>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<CostComplexAccuracy>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 
 	template void FileReader::ReadData<CostSensitive>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
+	template void FileReader::ReadData<InstanceCostSensitive>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<F1Score>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<GroupFairness>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<EqOpp>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<PrescriptivePolicy>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<SurvivalAnalysis>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 
 }
```

### Comparing `pystreed-1.2.2/src/utils/key_value_heap.cpp` & `pystreed-1.2.3/src/utils/key_value_heap.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.2/src/utils/parameter_handler.cpp` & `pystreed-1.2.3/src/utils/parameter_handler.cpp`

 * *Files identical despite different names*

