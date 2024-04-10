# Comparing `tmp/fair_trees-2.4.6.tar.gz` & `tmp/fair_trees-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.4.6.tar", last modified: Wed Apr 10 14:05:30 2024, max compression
+gzip compressed data, was "fair_trees-2.4.7.tar", last modified: Wed Apr 10 14:13:35 2024, max compression
```

## Comparing `fair_trees-2.4.6.tar` & `fair_trees-2.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:05:30.642836 fair_trees-2.4.6/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.6/LICENSE
--rw-rw-rw-   0        0        0     5070 2024-04-10 14:05:30.642836 fair_trees-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 14:05:30.642836 fair_trees-2.4.6/fair_trees/
--rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.6/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    27397 2024-04-10 14:04:49.000000 fair_trees-2.4.6/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:05:30.642836 fair_trees-2.4.6/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     5070 2024-04-10 14:05:30.000000 fair_trees-2.4.6/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-10 14:05:30.000000 fair_trees-2.4.6/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:05:30.000000 fair_trees-2.4.6/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-10 14:05:30.000000 fair_trees-2.4.6/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 14:05:30.000000 fair_trees-2.4.6/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 14:05:30.642836 fair_trees-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-04-10 14:05:19.000000 fair_trees-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:13:35.636199 fair_trees-2.4.7/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0     5093 2024-04-10 14:13:35.636199 fair_trees-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 14:13:35.620579 fair_trees-2.4.7/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-10 14:12:52.000000 fair_trees-2.4.7/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27353 2024-04-10 14:12:39.000000 fair_trees-2.4.7/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:13:35.636199 fair_trees-2.4.7/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     5093 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:13:35.636199 fair_trees-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      775 2024-04-10 14:13:27.000000 fair_trees-2.4.7/setup.py
```

### Comparing `fair_trees-2.4.6/LICENSE` & `fair_trees-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.6/PKG-INFO` & `fair_trees-2.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.6
+Version: 2.4.7
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: urllib
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
 
 # Fair tree classifier using strong demographic parity 
 
 Implementation of the algorithm proposed in:<br>
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.6 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.7 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
-pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
-using strong demographic parity Implementation of the algorithm proposed in:
+pandas Requires-Dist: urllib Requires-Dist: joblib Requires-Dist: scikit-learn
+# Fair tree classifier using strong demographic parity Implementation of the
+algorithm proposed in:
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic
 parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
```

### Comparing `fair_trees-2.4.6/README.md` & `fair_trees-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.6/fair_trees/fair_trees.py` & `fair_trees-2.4.7/fair_trees/fair_trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
+import urllib
 import joblib
 import warnings
 import numpy as np
 import pandas as pd
-import urllib.request
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
-    datasets_url = "https://github.com/pereirabarataap/fair_tree_classifier/raw/main/datasets.pkl"
-    urllib.request.urlretrieve(datasets_url, "datasets.pkl");
-    return joblib.load("datasets.pkl")
+    datasets_url = "https://github.com/pereirabarataap/fair_tree_classifier/raw/main/datasets.pkl"    
+    return joblib.load(urllib.request.urlopen(datasets_url))
 
 def sdp_score(z_true, y_prob):
     """
     Strong Demographic Parity Score
     Same API as roc_auc_score from sklean.metric
     Returns a value between 0 and 1 in which:
         0 indicates complete algorithmic bias,
```

### Comparing `fair_trees-2.4.6/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.7/fair_trees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.6
+Version: 2.4.7
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: urllib
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
 
 # Fair tree classifier using strong demographic parity 
 
 Implementation of the algorithm proposed in:<br>
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.6 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.7 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
-pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
-using strong demographic parity Implementation of the algorithm proposed in:
+pandas Requires-Dist: urllib Requires-Dist: joblib Requires-Dist: scikit-learn
+# Fair tree classifier using strong demographic parity Implementation of the
+algorithm proposed in:
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic
 parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
```

### Comparing `fair_trees-2.4.6/setup.py` & `fair_trees-2.4.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.4.6",
+    version="2.4.7",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
     install_requires=[
         "scipy",
         "numpy",
         "pandas",
+        "urllib",
         "joblib",
-        "scikit-learn"
+        "scikit-learn",
     ],
 )
```

