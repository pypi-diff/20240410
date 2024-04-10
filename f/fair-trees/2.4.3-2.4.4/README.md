# Comparing `tmp/fair_trees-2.4.3.tar.gz` & `tmp/fair_trees-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.4.3.tar", last modified: Tue Apr  9 17:32:09 2024, max compression
+gzip compressed data, was "fair_trees-2.4.4.tar", last modified: Wed Apr 10 13:25:41 2024, max compression
```

## Comparing `fair_trees-2.4.3.tar` & `fair_trees-2.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 17:32:09.850113 fair_trees-2.4.3/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.3/LICENSE
--rw-rw-rw-   0        0        0     4906 2024-04-09 17:32:09.850113 fair_trees-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4374 2024-04-09 17:32:02.000000 fair_trees-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 17:32:09.845103 fair_trees-2.4.3/fair_trees/
--rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.3/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    27184 2024-04-09 16:55:06.000000 fair_trees-2.4.3/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 17:32:09.849113 fair_trees-2.4.3/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4906 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 17:32:09.000000 fair_trees-2.4.3/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 17:32:09.851113 fair_trees-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-04-09 17:31:46.000000 fair_trees-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:25:41.321960 fair_trees-2.4.4/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.4/LICENSE
+-rw-rw-rw-   0        0        0     5070 2024-04-10 13:25:41.321960 fair_trees-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 13:25:41.321960 fair_trees-2.4.4/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.4/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27223 2024-04-10 13:24:42.000000 fair_trees-2.4.4/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:25:41.321960 fair_trees-2.4.4/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     5070 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 13:25:41.000000 fair_trees-2.4.4/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 13:25:41.321960 fair_trees-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-04-10 13:25:17.000000 fair_trees-2.4.4/setup.py
```

### Comparing `fair_trees-2.4.3/LICENSE` & `fair_trees-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.3/PKG-INFO` & `fair_trees-2.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.3
+Version: 2.4.4
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
 
-# Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
+# Fair tree classifier using strong demographic parity 
+
+Implementation of the algorithm proposed in:<br>
+> Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
+<a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines, use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
 ## Installation
 A)<br>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.3 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.4 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
-using strong demographic parity _[_>_>_] This package learns fair decision tree
+using strong demographic parity Implementation of the algorithm proposed in:
+> Pereira Barata, A. et al. _Fair tree classifier using strong demographic
+parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
```

### Comparing `fair_trees-2.4.3/README.md` & `fair_trees-2.4.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
+# Fair tree classifier using strong demographic parity 
+
+Implementation of the algorithm proposed in:<br>
+> Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
+<a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines, use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
 ## Installation
 A)<br>
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-# Fair tree classifier using strong demographic parity _[_>_>_] This package learns
-fair decision tree classifiers which can then be bagged into fair random
-forests, following the scikit-learn API standards. When incorporating
-FairDecisionTreeClassifier or FairRandomForestClassifier objects into scikit-
-learn pipelines, use the fit_params={"z": z} parameter to pass the sensitive
-attribute(s) z ## Installation A)
+# Fair tree classifier using strong demographic parity Implementation of the
+algorithm proposed in:
+> Pereira Barata, A. et al. _Fair tree classifier using strong demographic
+parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
+classifiers which can then be bagged into fair random forests, following the
+scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
+FairRandomForestClassifier objects into scikit-learn pipelines, use the
+fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
+Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python from fair_trees import
 FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
 clf.predict_proba(X)[:,1] print(sdp_score(z, y_prob)) ``` ## Example ```python
```

### Comparing `fair_trees-2.4.3/fair_trees/fair_trees.py` & `fair_trees-2.4.4/fair_trees/fair_trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,16 +536,17 @@
         # concatenating X into numpy array
         X = np.concatenate(X_concat_list, axis=1)
         
         pre_vars = [y, z]
         for i in range(len(pre_vars)):
             pre_vars[i] = pd.DataFrame(pre_vars[i])
             for column in pre_vars[i].columns:
+                unique_values = sorted(pre_vars[i][column].unique())
                 pre_vars[i][column] = pre_vars[i][column].replace(
-                    {pre_vars[i][column].unique()[j]: j for j in range(len(pre_vars[i][column].unique()))}
+                    {unique_values[j]: j for j in range(len(unique_values))}
                 )
             pre_vars[i] = pre_vars[i].values.astype(int)
         y, z = pre_vars
         
         return X, y.ravel(), z
     
     def _prepare_input_predict(self, X):
```

### Comparing `fair_trees-2.4.3/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.4/fair_trees.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.3
+Version: 2.4.4
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
 
-# Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
+# Fair tree classifier using strong demographic parity 
+
+Implementation of the algorithm proposed in:<br>
+> Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
+<a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines, use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
 ## Installation
 A)<br>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.3 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.4 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
-using strong demographic parity _[_>_>_] This package learns fair decision tree
+using strong demographic parity Implementation of the algorithm proposed in:
+> Pereira Barata, A. et al. _Fair tree classifier using strong demographic
+parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
```

### Comparing `fair_trees-2.4.3/setup.py` & `fair_trees-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.4.3",
+    version="2.4.4",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

