# Comparing `tmp/fair_trees-2.4.4.tar.gz` & `tmp/fair_trees-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.4.4.tar", last modified: Wed Apr 10 13:25:41 2024, max compression
+gzip compressed data, was "fair_trees-2.4.5.tar", last modified: Wed Apr 10 13:44:22 2024, max compression
```

## Comparing `fair_trees-2.4.4.tar` & `fair_trees-2.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:25:41.321960 fair_trees-2.4.4/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.4/LICENSE
--rw-rw-rw-   0        0        0     5070 2024-04-10 13:25:41.321960 fair_trees-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 13:25:41.321960 fair_trees-2.4.4/fair_trees/
--rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.4/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    27223 2024-04-10 13:24:42.000000 fair_trees-2.4.4/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:25:41.321960 fair_trees-2.4.4/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     5070 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 13:25:41.321960 fair_trees-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-04-10 13:25:17.000000 fair_trees-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:44:22.217585 fair_trees-2.4.5/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0     5070 2024-04-10 13:44:22.217585 fair_trees-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 13:44:22.217585 fair_trees-2.4.5/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.5/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27398 2024-04-10 13:43:07.000000 fair_trees-2.4.5/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:44:22.217585 fair_trees-2.4.5/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     5070 2024-04-10 13:44:22.000000 fair_trees-2.4.5/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-10 13:44:22.000000 fair_trees-2.4.5/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:44:22.000000 fair_trees-2.4.5/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-10 13:44:22.000000 fair_trees-2.4.5/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 13:44:22.000000 fair_trees-2.4.5/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 13:44:22.217585 fair_trees-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-04-10 13:43:50.000000 fair_trees-2.4.5/setup.py
```

### Comparing `fair_trees-2.4.4/LICENSE` & `fair_trees-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.4/PKG-INFO` & `fair_trees-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.4
+Version: 2.4.5
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.4 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.5 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
 using strong demographic parity Implementation of the algorithm proposed in:
```

### Comparing `fair_trees-2.4.4/README.md` & `fair_trees-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.4/fair_trees/fair_trees.py` & `fair_trees-2.4.5/fair_trees/fair_trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import joblib
 import warnings
 import numpy as np
 import pandas as pd
+import urllib.request
 from math import sqrt, log2
 from collections import Counter
 from scipy.optimize import minimize
 from joblib import Parallel, delayed
 from sklearn.metrics import roc_auc_score, f1_score
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.preprocessing import OneHotEncoder as OHE, KBinsDiscretizer as KBD
 
 pd.set_option("future.no_silent_downcasting", True)
 warnings.filterwarnings("ignore", category=UserWarning)
 
 def load_datasets():
+    datasets_url = "https://github.com/pereirabarataap/fair_tree_classifier/blob/main/datasets.pkl"
+    urllib.request.urlretrieve(datasets_url, "datasets.pkl");
     return joblib.load("datasets.pkl")
 
 def sdp_score(z_true, y_prob):
     """
     Strong Demographic Parity Score
     Same API as roc_auc_score from sklean.metric
     Returns a value between 0 and 1 in which:
@@ -122,15 +125,14 @@
         self.requires_data_processing = requires_data_processing
         self.generate_prediction_threshold = generate_prediction_threshold
         if isinstance(max_depth, type(None)):
             self.max_depth = np.inf
         else:
             self.max_depth = max_depth
             
-        np.random.seed(self.random_state)
         self.parent_scaff = (1-self.theta)*0.5 - self.theta*0.5
 
     def _get_max_features(self, n_features):
         if self.max_features is None:
             return n_features
         elif isinstance(self.max_features, int):
             return min(self.max_features, n_features)
@@ -365,14 +367,15 @@
         self.n_classes_ = len(np.unique(y))
        
         self.n_sens_groups = z.shape[1]
         self.n_senses_ = {
             sens_group: len(np.unique(z[:, sens_group])) for sens_group in range(self.n_sens_groups)
         }
         
+        np.random.seed(self.random_state)
         self.features_indices = np.random.choice(X.shape[1], self._get_max_features(X.shape[1]), replace=False)
         
         if self.bootstrap:
             resample_idx = np.random.choice(len(y), len(y), replace=True)
             X, y, z = X[resample_idx], y[resample_idx], z[resample_idx]
         
         self.tree_ = self._grow_tree(X, y, z)
@@ -486,15 +489,14 @@
         self.generate_prediction_threshold=generate_prediction_threshold
         if isinstance(max_depth, type(None)):
             self.max_depth = np.inf
         else:
             self.max_depth = max_depth
             
         np.random.seed(self.random_state)
-        
         base_rs = np.random.randint(1, 1e9)
         self.trees = [FairDecisionTreeClassifier(
             theta=self.theta,
             n_bins=self.n_bins,
             random_state=base_rs+i,
             max_depth=self.max_depth,
             bootstrap=self.bootstrap,
```

### Comparing `fair_trees-2.4.4/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.5/fair_trees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.4
+Version: 2.4.5
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.4 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.5 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
 using strong demographic parity Implementation of the algorithm proposed in:
```

### Comparing `fair_trees-2.4.4/setup.py` & `fair_trees-2.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.4.4",
+    version="2.4.5",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

