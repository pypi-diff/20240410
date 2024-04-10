# Comparing `tmp/featuristic-1.0.1.tar.gz` & `tmp/featuristic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuristic-1.0.1.tar", last modified: Thu Apr  4 19:22:44 2024, max compression
+gzip compressed data, was "featuristic-1.1.0.tar", last modified: Wed Apr 10 14:39:26 2024, max compression
```

## Comparing `featuristic-1.0.1.tar` & `featuristic-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.911091 featuristic-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-04 19:22:41.000000 featuristic-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-04 19:22:44.911091 featuristic-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-04 19:22:41.000000 featuristic-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-04-04 19:22:41.000000 featuristic-1.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:22:44.911091 featuristic-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.903092 featuristic-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/datasets/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/selection/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/selection/genetic_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/selection/population.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.907091 featuristic-1.0.1/src/featuristic/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/fitness.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/genetic_feature_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/mrmr.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/program.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/synthesis/symbolic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 19:22:41.000000 featuristic-1.0.1/src/featuristic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.911091 featuristic-1.0.1/src/featuristic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 19:22:44.000000 featuristic-1.0.1/src/featuristic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:22:44.911091 featuristic-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_fitness.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_genetic_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_genetic_feature_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-04 19:22:41.000000 featuristic-1.0.1/tests/test_symbolic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.877311 featuristic-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-10 14:39:23.000000 featuristic-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-10 14:39:26.877311 featuristic-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-10 14:39:23.000000 featuristic-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10956 2024-04-10 14:39:23.000000 featuristic-1.1.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:39:26.877311 featuristic-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.869311 featuristic-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.869311 featuristic-1.1.0/src/featuristic/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.873311 featuristic-1.1.0/src/featuristic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/datasets/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.873311 featuristic-1.1.0/src/featuristic/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/selection/genetic_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/selection/population.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.873311 featuristic-1.1.0/src/featuristic/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/genetic_feature_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/mrmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/synthesis/symbolic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 14:39:23.000000 featuristic-1.1.0/src/featuristic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.873311 featuristic-1.1.0/src/featuristic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-10 14:39:26.000000 featuristic-1.1.0/src/featuristic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 14:39:26.000000 featuristic-1.1.0/src/featuristic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:39:26.000000 featuristic-1.1.0/src/featuristic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-10 14:39:26.000000 featuristic-1.1.0/src/featuristic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 14:39:26.000000 featuristic-1.1.0/src/featuristic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:39:26.873311 featuristic-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_genetic_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_genetic_feature_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-10 14:39:23.000000 featuristic-1.1.0/tests/test_symbolic_functions.py
```

### Comparing `featuristic-1.0.1/LICENSE.txt` & `featuristic-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/PKG-INFO` & `featuristic-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuristic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Genetic algorithms for automated feature engineering and feature selection
 License: Copyright 2024 Martin Eastwood
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files
         (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge,
         publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished
         to do so, subject to the following conditions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: featuristic Version: 1.0.1 Summary: Genetic
+Metadata-Version: 2.1 Name: featuristic Version: 1.1.0 Summary: Genetic
 algorithms for automated feature engineering and feature selection License:
 Copyright 2024 Martin Eastwood Permission is hereby granted, free of charge, to
 any person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `featuristic-1.0.1/pyproject.toml` & `featuristic-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "featuristic"
 
 # Versions should comply with PEP 440
-version = "1.0.1"
+version = "1.1.0"
 
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Genetic algorithms for automated feature engineering and feature selection"
```

### Comparing `featuristic-1.0.1/readme.md` & `featuristic-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/datasets/fetch.py` & `featuristic-1.1.0/src/featuristic/datasets/fetch.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/selection/genetic_feature_selection.py` & `featuristic-1.1.0/src/featuristic/selection/genetic_feature_selection.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/selection/population.py` & `featuristic-1.1.0/src/featuristic/selection/population.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/synthesis/fitness.py` & `featuristic-1.1.0/src/featuristic/synthesis/fitness.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/synthesis/genetic_feature_synthesis.py` & `featuristic-1.1.0/src/featuristic/synthesis/genetic_feature_synthesis.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,55 +9,52 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from tqdm import tqdm
 
 from .fitness import fitness_pearson
 from .mrmr import MaxRelevanceMinRedundancy
 from .population import ParallelPopulation, SerialPopulation
 from .program import render_prog
-from .symbolic_functions import SymbolicFunction, operations
+from .symbolic_functions import CustomSymbolicFunction, operations
 from .preprocess import preprocess_data
 
 
 class GeneticFeatureSynthesis(BaseEstimator, TransformerMixin):
     """
     The Genetic Feature Synthesis class uses genetic programming to generate new
     features using a technique based on Symbolic Regression. This is done by initially
     building a population of naive random formulas that represent transformations of
     the input features. The population is then evolved over a number of generations
-    using genetic operators such as mutation and crossover to find the best programs
+    using genetic functions such as mutation and crossover to find the best programs
     that minimize a given fitness function. The best features are then identified using
     a Maximum Relevance Minimum Redundancy (mRMR) algorithm to find those features
     that are most correlated with the target variable while being least correlated with
     each other.
     """
 
     def __init__(
         self,
-        functions: Union[List[SymbolicFunction] | None] = None,
         num_features: int = 10,
         population_size: int = 100,
         max_generations: int = 25,
         tournament_size: int = 10,
         crossover_proba: float = 0.85,
         parsimony_coefficient: float = 0.001,
         early_termination_iters: int = 15,
+        functions: Union[List[str] | None] = None,
+        custom_functions: Union[List[CustomSymbolicFunction] | None] = None,
         return_all_features: bool = True,
         n_jobs: int = -1,
         pbar: bool = True,
         verbose: bool = False,
     ):
         """
         Initialize the Symbolic Feature Generator.
 
         Args
         ----
-        functions : list
-            The list of functions to use in the programs. If `None` then all the
-            built-in functions are used.
-
         num_features : int
             The number of best features to generate. Internally, `3 * num_features`
             programs are generated and the
             best `num_features` are selected via Maximum Relevance Minimum Redundancy
             (mRMR).
 
         population_size : int
@@ -85,14 +82,23 @@
             increases computation complexity and reduces the interpretability of the
             features.
 
         early_termination_iters : int
             If the best score does not improve for this number of generations, then the
             algorithm will terminate early.
 
+        functions : list
+            The list of functions to use in the programs. If `None` then all the
+            built-in functions are used. The functions must be the names of the
+            functions returned by the `list_symbolic_functions` method.
+
+        custom_functions : list
+            A list of custom functions to use in the programs. Each custom function
+            must be an instance of the `CustomSymbolicFunction` class.
+
         return_all_features : bool
             Whether to return all the features generated or just the best features.
 
         n_jobs : int
             The number of parallel jobs to run. If `-1`, use all available cores else
             uses n_jobs. If `n_jobs=1`, then the computation is done in serial.
 
@@ -101,15 +107,30 @@
 
         verbose : bool
             Whether to print out aditional information
         """
         if functions is None:
             self.functions = operations
         else:
-            self.functions = functions
+            self.functions = []
+            for func in functions:
+                found = False
+                for op in operations:
+                    if op().name == func:
+                        self.functions.append(op)
+                        found = True
+                        break
+                if not found:
+                    raise ValueError(
+                        f"Function '{func}' not found in symbolic operations"
+                    )
+
+        if custom_functions is not None:
+            for func in custom_functions:
+                self.functions.append(func)
 
         self.population_size = population_size
         self.max_generations = max_generations
         self.tournament_size = tournament_size
         self.crossover_proba = crossover_proba
         self.num_features = num_features
         self.parsimony_coefficient = parsimony_coefficient
```

### Comparing `featuristic-1.0.1/src/featuristic/synthesis/mrmr.py` & `featuristic-1.1.0/src/featuristic/synthesis/mrmr.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/synthesis/population.py` & `featuristic-1.1.0/src/featuristic/synthesis/population.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 from typing import Callable, List, Self
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, cpu_count, delayed
 
 from .program import random_prog, select_random_node, node_count
-from .symbolic_functions import SymbolicFunction
 
 
 class BasePopulation:
     """
     A class to represent the population of symbolic programs in the
     genetic programming algorithm.
     """
 
     def __init__(
         self,
         population_size: int,
-        operations: List[SymbolicFunction],
+        operations: List,
         tournament_size: int = 3,
         crossover_prob: float = 0.75,
     ):
         """
         Initialize the population.
 
         Args
@@ -241,15 +240,15 @@
     A class to represent the population of programs in the genetic programming algorithm where
     the programs are evaluated serially.
     """
 
     def __init__(
         self,
         population_size: int,
-        operations: List[SymbolicFunction],
+        operations: List,
         tournament_size: int = 3,
         crossover_prob: float = 0.75,
     ):
         """
         Initialize the population class.
 
         Args
@@ -341,15 +340,15 @@
     A class to represent the population of programs in the genetic programming algorithm where
     the programs are evaluated in parallel via joblib.
     """
 
     def __init__(
         self,
         population_size: int,
-        operations: List[SymbolicFunction],
+        operations: List,
         tournament_size: int = 3,
         crossover_prob: float = 0.75,
         n_jobs: int = -1,
     ):
         """
         Initialize the population class.
```

### Comparing `featuristic-1.0.1/src/featuristic/synthesis/preprocess.py` & `featuristic-1.1.0/src/featuristic/synthesis/preprocess.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/src/featuristic/synthesis/program.py` & `featuristic-1.1.0/src/featuristic/synthesis/program.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Functions for manipulating the symbolic programs."""
 
 from typing import List
 
 import numpy as np
 import pandas as pd
 
-from .symbolic_functions import SymbolicFunction
+from .symbolic_functions import CustomSymbolicFunction
 
 
-def random_prog(depth: int, X: pd.DataFrame, operations: List[SymbolicFunction]):
+def random_prog(depth: int, X: pd.DataFrame, operations: List):
     """
     Generate a random program for symbolic regression.
 
     Parameters
     ----------
     depth : int
         The depth of the program.
@@ -20,15 +20,18 @@
     X : pd.DataFrame
         The input data.
 
     operations : list
         The list of operations to use.
     """
     if np.random.randint(0, 10) >= depth * 2:
-        op = operations[np.random.randint(0, len(operations) - 1)]()
+        op = operations[np.random.randint(0, len(operations) - 1)]
+        if not isinstance(op, CustomSymbolicFunction):
+            op = op()
+
         return {
             "func": op,
             "children": [
                 random_prog(depth + 1, X, operations) for _ in range(op.arg_count)
             ],
             "format_str": op.format_str,
         }
```

### Comparing `featuristic-1.0.1/src/featuristic.egg-info/PKG-INFO` & `featuristic-1.1.0/src/featuristic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuristic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Genetic algorithms for automated feature engineering and feature selection
 License: Copyright 2024 Martin Eastwood
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files
         (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge,
         publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished
         to do so, subject to the following conditions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: featuristic Version: 1.0.1 Summary: Genetic
+Metadata-Version: 2.1 Name: featuristic Version: 1.1.0 Summary: Genetic
 algorithms for automated feature engineering and feature selection License:
 Copyright 2024 Martin Eastwood Permission is hereby granted, free of charge, to
 any person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `featuristic-1.0.1/src/featuristic.egg-info/SOURCES.txt` & `featuristic-1.1.0/src/featuristic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/tests/test_fitness.py` & `featuristic-1.1.0/tests/test_fitness.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     b = pd.Series([1, 1, 1])
     c = ft.synthesis.fitness.fitness_pearson({}, 1, a, b)
     assert c == sys.maxsize
 
     a = pd.Series([1, 2, 3, 4, 5])
     b = pd.Series([1, 2, 3, 4, 5])
     c = ft.synthesis.fitness.fitness_pearson({}, 0.001, a, b)
-    assert c == approx(1.0)
+    assert c == approx(-1.0)
```

### Comparing `featuristic-1.0.1/tests/test_genetic_feature_selection.py` & `featuristic-1.1.0/tests/test_genetic_feature_selection.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/tests/test_genetic_feature_synthesis.py` & `featuristic-1.1.0/tests/test_genetic_feature_synthesis.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/tests/test_programs.py` & `featuristic-1.1.0/tests/test_programs.py`

 * *Files identical despite different names*

### Comparing `featuristic-1.0.1/tests/test_symbolic_functions.py` & `featuristic-1.1.0/tests/test_symbolic_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,11 +230,11 @@
             approx(1.0),
         ]
     )
     assert (func(a) == b).all()
 
 
 def test_list_operations():
-    ops = ft.synthesis.symbolic_functions.list_operations()
+    ops = ft.synthesis.symbolic_functions.list_functions()
 
     assert len(ops) > 0
     assert all(isinstance(op, str) for op in ops)
```

