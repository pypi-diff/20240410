# Comparing `tmp/fair_trees-2.4.2.tar.gz` & `tmp/fair_trees-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.4.2.tar", last modified: Tue Apr  9 17:26:55 2024, max compression
+gzip compressed data, was "fair_trees-2.4.3.tar", last modified: Tue Apr  9 17:32:09 2024, max compression
```

## Comparing `fair_trees-2.4.2.tar` & `fair_trees-2.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 17:26:55.776878 fair_trees-2.4.2/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.2/LICENSE
--rw-rw-rw-   0        0        0     4900 2024-04-09 17:26:55.775827 fair_trees-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4368 2024-04-09 17:26:21.000000 fair_trees-2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 17:26:55.769837 fair_trees-2.4.2/fair_trees/
--rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.2/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    27184 2024-04-09 16:55:06.000000 fair_trees-2.4.2/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 17:26:55.775827 fair_trees-2.4.2/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4900 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 17:26:55.776878 fair_trees-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-04-09 17:26:48.000000 fair_trees-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:32:09.850113 fair_trees-2.4.3/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.3/LICENSE
+-rw-rw-rw-   0        0        0     4906 2024-04-09 17:32:09.850113 fair_trees-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4374 2024-04-09 17:32:02.000000 fair_trees-2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 17:32:09.845103 fair_trees-2.4.3/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.3/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27184 2024-04-09 16:55:06.000000 fair_trees-2.4.3/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:32:09.849113 fair_trees-2.4.3/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4906 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:32:09.851113 fair_trees-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-04-09 17:31:46.000000 fair_trees-2.4.3/setup.py
```

### Comparing `fair_trees-2.4.2/LICENSE` & `fair_trees-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.2/PKG-INFO` & `fair_trees-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.2
+Version: 2.4.3
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -34,16 +34,16 @@
 
 datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
-y_prob = clf.predict_proba(X)
-print(sdp_sore(z, y_prob))
+y_prob = clf.predict_proba(X)[:,1]
+print(sdp_score(z, y_prob))
 ```
 ## Example
 ```python
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.2 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.3 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
 using strong demographic parity _[_>_>_] This package learns fair decision tree
@@ -13,17 +13,17 @@
 Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python from fair_trees import
 FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
-clf.predict_proba(X) print(sdp_sore(z, y_prob)) ``` ## Example ```python import
-numpy as np import pandas as pd import seaborn as sb from tqdm.notebook import
-tqdm from matplotlib import pyplot as plt from sklearn.metrics import
+clf.predict_proba(X)[:,1] print(sdp_score(z, y_prob)) ``` ## Example ```python
+import numpy as np import pandas as pd import seaborn as sb from tqdm.notebook
+import tqdm from matplotlib import pyplot as plt from sklearn.metrics import
 roc_auc_score from sklearn.model_selection import StratifiedKFold as SKF from
 fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
 datasets = load_datasets() results_data = [] for dataset in tqdm(datasets): X =
 datasets[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"]
 fold = 0 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring
 stratified kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype
 (str).apply( lambda row: row[y.name] + "".join([row[col] for col in
```

### Comparing `fair_trees-2.4.2/README.md` & `fair_trees-2.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
-y_prob = clf.predict_proba(X)
-print(sdp_sore(z, y_prob))
+y_prob = clf.predict_proba(X)[:,1]
+print(sdp_score(z, y_prob))
 ```
 ## Example
 ```python
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 attribute(s) z ## Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python from fair_trees import
 FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
-clf.predict_proba(X) print(sdp_sore(z, y_prob)) ``` ## Example ```python import
-numpy as np import pandas as pd import seaborn as sb from tqdm.notebook import
-tqdm from matplotlib import pyplot as plt from sklearn.metrics import
+clf.predict_proba(X)[:,1] print(sdp_score(z, y_prob)) ``` ## Example ```python
+import numpy as np import pandas as pd import seaborn as sb from tqdm.notebook
+import tqdm from matplotlib import pyplot as plt from sklearn.metrics import
 roc_auc_score from sklearn.model_selection import StratifiedKFold as SKF from
 fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
 datasets = load_datasets() results_data = [] for dataset in tqdm(datasets): X =
 datasets[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"]
 fold = 0 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring
 stratified kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype
 (str).apply( lambda row: row[y.name] + "".join([row[col] for col in
```

### Comparing `fair_trees-2.4.2/fair_trees/fair_trees.py` & `fair_trees-2.4.3/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.2/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.3/fair_trees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.2
+Version: 2.4.3
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -34,16 +34,16 @@
 
 datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
-y_prob = clf.predict_proba(X)
-print(sdp_sore(z, y_prob))
+y_prob = clf.predict_proba(X)[:,1]
+print(sdp_score(z, y_prob))
 ```
 ## Example
 ```python
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.2 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.3 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
 using strong demographic parity _[_>_>_] This package learns fair decision tree
@@ -13,17 +13,17 @@
 Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python from fair_trees import
 FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
-clf.predict_proba(X) print(sdp_sore(z, y_prob)) ``` ## Example ```python import
-numpy as np import pandas as pd import seaborn as sb from tqdm.notebook import
-tqdm from matplotlib import pyplot as plt from sklearn.metrics import
+clf.predict_proba(X)[:,1] print(sdp_score(z, y_prob)) ``` ## Example ```python
+import numpy as np import pandas as pd import seaborn as sb from tqdm.notebook
+import tqdm from matplotlib import pyplot as plt from sklearn.metrics import
 roc_auc_score from sklearn.model_selection import StratifiedKFold as SKF from
 fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
 datasets = load_datasets() results_data = [] for dataset in tqdm(datasets): X =
 datasets[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"]
 fold = 0 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring
 stratified kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype
 (str).apply( lambda row: row[y.name] + "".join([row[col] for col in
```

### Comparing `fair_trees-2.4.2/setup.py` & `fair_trees-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.4.2",
+    version="2.4.3",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

