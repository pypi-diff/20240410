# Comparing `tmp/ex_fuzzy-1.1.1.tar.gz` & `tmp/ex_fuzzy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.1.tar", last modified: Fri Apr  5 15:41:19 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.2.tar", last modified: Wed Apr 10 14:00:24 2024, max compression
```

## Comparing `ex_fuzzy-1.1.1.tar` & `ex_fuzzy-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.197286 ex_fuzzy-1.1.1/
--rw-rw-rw-   0        0        0     3679 2024-04-05 15:41:19.196516 ex_fuzzy-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2801 2024-03-13 11:20:26.000000 ex_fuzzy-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.147572 ex_fuzzy-1.1.1/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.187916 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      255 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    10541 2024-01-31 11:27:43.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2640 2024-04-05 14:46:18.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    42930 2024-04-05 13:22:39.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11458 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    39187 2024-04-05 13:20:29.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.169590 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     3679 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-04-05 15:41:19.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 15:41:19.197286 ex_fuzzy-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-04-05 15:41:14.000000 ex_fuzzy-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.194003 ex_fuzzy-1.1.1/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.657128 ex_fuzzy-1.1.2/
+-rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4327 2024-04-10 14:00:24.653126 ex_fuzzy-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3278 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.527121 ex_fuzzy-1.1.2/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.627124 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    10541 2024-01-31 11:27:43.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2640 2024-04-05 14:46:18.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    43120 2024-04-10 13:41:32.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    39155 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.559122 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     4327 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:00:24.658127 ex_fuzzy-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-04-10 13:55:40.000000 ex_fuzzy-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.650126 ex_fuzzy-1.1.2/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.1/PKG-INFO` & `ex_fuzzy-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex_fuzzy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: networkx
+Requires-Dist: matplotlib
+Requires-Dist: pymoo
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
 
 # Ex-Fuzzy
 ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
 
 Some of the tools available in this library include:
 
 - Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
@@ -65,14 +72,26 @@
 
 ## Installation
 
 You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
 
 `pip install ex-fuzzy`
 
+## Preprint and Citation
 
-## Contributors
-Javier Fumanal Idocin, Javier Andreu-Perez
+You can check our preprint in SSRN in the following link:
+
+https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4766235
 
-All rights reserved, 2021-2024
+To cite the library please use the preprint until the final paper is accepted:
+```
+@article{fumanalex,
+  title={Ex-Fuzzy: A Library for Symbolic Explainable AI Through Fuzzy Logic Programming},
+  author={Fumanal Idocin, Javier and Andreu-Perez, Javier},
+  journal={SSNR}
+}
+```
 
+## Contributors
+Javier Fumanal Idocin, Javier Andreu-Perez
 
+This project is licensed under the terms of the AGLP v3 license, 2021-2024
```

### Comparing `ex_fuzzy-1.1.1/README.md` & `ex_fuzzy-1.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,26 @@
 
 ## Installation
 
 You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
 
 `pip install ex-fuzzy`
 
+## Preprint and Citation
 
-## Contributors
-Javier Fumanal Idocin, Javier Andreu-Perez
+You can check our preprint in SSRN in the following link:
+
+https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4766235
 
-All rights reserved, 2021-2024
+To cite the library please use the preprint until the final paper is accepted:
+```
+@article{fumanalex,
+  title={Ex-Fuzzy: A Library for Symbolic Explainable AI Through Fuzzy Logic Programming},
+  author={Fumanal Idocin, Javier and Andreu-Perez, Javier},
+  journal={SSNR}
+}
+```
 
+## Contributors
+Javier Fumanal Idocin, Javier Andreu-Perez
 
+This project is licensed under the terms of the AGLP v3 license, 2021-2024
```

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 # If Fuzzy variables are already precomputed.
                 problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, n_classes=len(np.unique(y)),
                                     linguistic_variables=self.lvs, domain=self.domain, tolerance=self.tolerance, thread_runner=self.thread_runner,
                                     alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
         else:
             self.fuzzy_type = candidate_rules.fuzzy_type()
             self.n_linguist_variables = candidate_rules.n_linguist_variables()
-            problem = ExploreRuleBases(X, y, n_classes=len(np.unique(y)), cancidate_rules=candidate_rules, thread_runner=self.thread_runner, nRules=self.nRules)
+            problem = ExploreRuleBases(X, y, n_classes=len(np.unique(y)), candidate_rules=candidate_rules, thread_runner=self.thread_runner, nRules=self.nRules)
 
         if self.custom_loss is not None:
             problem.fitness_func = self.custom_loss
 
         if initial_rules is not None:
             rules_gene = problem.encode_rulebase(initial_rules, self.lvs is None)
             rules_gene = (np.ones((pop_size, len(rules_gene))) * rules_gene).astype(int)
@@ -368,15 +368,15 @@
 
 class ExploreRuleBases(Problem):
     '''
     Class to model as pymoo problem the fitting of a rulebase to a set of data given a series of candidate rules for a classification problem using Evolutionary strategies
     Supports type 1 and t2.
     '''
 
-    def __init__(self, X: np.array, y: np.array, nRules: int, n_classes: int, cancidate_rules: rules.MasterRuleBase, thread_runner: StarmapParallelization=None, tolerance:float = 0.01) -> None:
+    def __init__(self, X: np.array, y: np.array, nRules: int, n_classes: int, candidate_rules: rules.MasterRuleBase, thread_runner: StarmapParallelization=None, tolerance:float = 0.01) -> None:
         '''
         Cosntructor method. Initializes the classifier with the number of antecedents, linguist variables and the kind of fuzzy set desired.
 
         :param X: np array or pandas dataframe samples x features.
         :param y: np vector containing the target classes. vector sample
         :param n_class: number of classes in the problem. If None (as default) it will be computed from the data.
         :param cancidate_rules: MasterRuleBase object. If not None, the classifier will use the rules in the object and ignore the conflicting parameters.
@@ -385,20 +385,21 @@
             self.var_names = list(X.columns)
             self.X = X.values
         except AttributeError:
             self.X = X
             self.var_names = [str(ix) for ix in range(X.shape[1])]
 
         self.tolerance = tolerance
-        self.fuzzy_type = cancidate_rules.fuzzy_type()
+        self.fuzzy_type = candidate_rules.fuzzy_type()
         self.y = y
         self.nCons = 1  # This is fixed to MISO rules.
         self.n_classes = n_classes
-        self.candidate_rules = cancidate_rules
+        self.candidate_rules = candidate_rules
         self.nRules = nRules
+        self._precomputed_truth = rules.compute_antecedents_memberships(candidate_rules.get_antecedents(), X)
 
         self.vl_names = self.candidate_rules[0].antecedents[0].linguistic_variable_names()
         self.fuzzy_type = self.candidate_rules[0].antecedents[0].fuzzy_type()
 
         self.min_bounds = np.min(self.X, axis=0)
         self.max_bounds = np.max(self.X, axis=0)
 
@@ -479,32 +480,32 @@
             those features are the parameters to optimize.
 
         :param out: dict where the F field is the fitness. It is used from the outside.
         '''
         try:
             ruleBase = self._construct_ruleBase(x, self.fuzzy_type)
 
-            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, self._precomputed_truth)
+            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, precomputed_truth=self._precomputed_truth)
             
 
             out["F"] = 1 - score
         except rules.RuleError:
             out["F"] = 1
 
     
-    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.95, beta:float=0.025, gamma:float=0.025) -> float:
+    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.95, beta:float=0.025, gamma:float=0.025, precomputed_truth=None) -> float:
         '''
         Fitness function for the optimization problem.
         :param ruleBase: RuleBase object
         :param X: array of train samples. X shape = (n_samples, n_features)
         :param y: array of train labels. y shape = (n_samples,)
         :param tolerance: float. Tolerance for the size evaluation.
         :return: float. Fitness value.
         '''
-        ev_object = evr.evalRuleBase(ruleBase, X, y)
+        ev_object = evr.evalRuleBase(ruleBase, X, y, precomputed_truth=precomputed_truth)
         ev_object.add_rule_weights()
 
         score_acc = ev_object.classification_eval()
         score_rules_size = ev_object.size_antecedents_eval(tolerance)
         score_nrules = ev_object.effective_rulesize_eval(tolerance)
 
         score = score_acc * alpha + (1 - alpha) * (score_rules_size * beta + score_nrules * gamma)
```

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,17 @@
     Computes the apriori algorithm for the given dataframe and threshold the support.
     
     :param data: Dataframe of shape: samples x features
     :param fuzzy variables: dict that maps each feature name with a fuzzy variable.
     :param support_threshold: minimum support to consider frequent an itemset.
     :return: all the frequent itemsets as a list.
     '''
-    n_linguist_variables = len(fuzzy_variables[0])
     list_possible_vars = []
-    for ix in range(len(fuzzy_variables)):
-        list_possible_vars.append([(ix, ax) for ax in range(n_linguist_variables)])
+    for ix, fuzzy_variable in enumerate(fuzzy_variables):
+        list_possible_vars.append([(ix, ax) for ax in range(len(fuzzy_variable))])
 
     memberships = [fuzzy_variables[ix](data.iloc[:, ix].values) for ix in range(data.shape[1])]
     freq_itemsets = []
 
     if max_depth is None:
         max_depth = data.shape[1]
```

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         rules = self.delete_rule_duplicates(rules)
         self.rules = rules
         self.antecedents = antecedents
         self.consequent = consequent
         self.tnorm = tnorm
         self.consequent_centroids = np.zeros(
             (len(consequent.linguistic_variable_names()), 2))
-        for ix, (name, vl_consequent) in enumerate(consequent.linguistic_variables.items()):
+        for ix, vl_consequent in enumerate(consequent.linguistic_variables):
             consequent_domain = vl_consequent.domain
             domain_linspace = np.arange(
                 consequent_domain[0], consequent_domain[1], 0.05)
             consequent_memberships = vl_consequent.membership(domain_linspace)
 
             self.consequent_centroids[ix, :] = centroid.compute_centroid_iv(
                 domain_linspace, consequent_memberships)
@@ -782,15 +782,15 @@
         self.consequent = consequent
         self.tnorm = tnorm
 
         if consequent is not None:
             self.consequent_centroids = np.zeros(
                 (len(consequent.linguistic_variable_names()), ))
 
-            for ix, (name, vl_consequent) in enumerate(consequent.linguistic_variables.items()):
+            for ix, vl_consequent in enumerate(consequent.linguistic_variables):
                 consequent_domain = vl_consequent.domain
                 domain_linspace = np.arange(
                     consequent_domain[0], consequent_domain[1], 0.05)
                 consequent_memberships = vl_consequent.membership(
                     domain_linspace)
 
                 self.consequent_centroids[ix] = centroid.center_of_masses(
```

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.1.2/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex-fuzzy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: networkx
+Requires-Dist: matplotlib
+Requires-Dist: pymoo
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
 
 # Ex-Fuzzy
 ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
 
 Some of the tools available in this library include:
 
 - Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
@@ -65,14 +72,26 @@
 
 ## Installation
 
 You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
 
 `pip install ex-fuzzy`
 
+## Preprint and Citation
 
-## Contributors
-Javier Fumanal Idocin, Javier Andreu-Perez
+You can check our preprint in SSRN in the following link:
+
+https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4766235
 
-All rights reserved, 2021-2024
+To cite the library please use the preprint until the final paper is accepted:
+```
+@article{fumanalex,
+  title={Ex-Fuzzy: A Library for Symbolic Explainable AI Through Fuzzy Logic Programming},
+  author={Fumanal Idocin, Javier and Andreu-Perez, Javier},
+  journal={SSNR}
+}
+```
 
+## Contributors
+Javier Fumanal Idocin, Javier Andreu-Perez
 
+This project is licensed under the terms of the AGLP v3 license, 2021-2024
```

### Comparing `ex_fuzzy-1.1.1/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.2/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 ex_fuzzy.egg-info/PKG-INFO
 ex_fuzzy.egg-info/SOURCES.txt
 ex_fuzzy.egg-info/dependency_links.txt
 ex_fuzzy.egg-info/requires.txt
 ex_fuzzy.egg-info/top_level.txt
```

### Comparing `ex_fuzzy-1.1.1/setup.py` & `ex_fuzzy-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.1/tests/test_centroids.py` & `ex_fuzzy-1.1.2/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/tests/test_classification.py` & `ex_fuzzy-1.1.2/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/tests/test_eval_tools.py` & `ex_fuzzy-1.1.2/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.2/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.1/tests/test_utils.py` & `ex_fuzzy-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

