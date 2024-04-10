# Comparing `tmp/fair_trees-2.4.7.tar.gz` & `tmp/fair_trees-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.4.7.tar", last modified: Wed Apr 10 14:13:35 2024, max compression
+gzip compressed data, was "fair_trees-2.4.8.tar", last modified: Wed Apr 10 14:15:57 2024, max compression
```

## Comparing `fair_trees-2.4.7.tar` & `fair_trees-2.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:13:35.636199 fair_trees-2.4.7/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.7/LICENSE
--rw-rw-rw-   0        0        0     5093 2024-04-10 14:13:35.636199 fair_trees-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 14:13:35.620579 fair_trees-2.4.7/fair_trees/
--rw-rw-rw-   0        0        0      106 2024-04-10 14:12:52.000000 fair_trees-2.4.7/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    27353 2024-04-10 14:12:39.000000 fair_trees-2.4.7/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:13:35.636199 fair_trees-2.4.7/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     5093 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 14:13:35.000000 fair_trees-2.4.7/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 14:13:35.636199 fair_trees-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0      775 2024-04-10 14:13:27.000000 fair_trees-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:15:57.168258 fair_trees-2.4.8/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.8/LICENSE
+-rw-rw-rw-   0        0        0     5070 2024-04-10 14:15:57.168258 fair_trees-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4538 2024-04-10 13:25:23.000000 fair_trees-2.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 14:15:57.168258 fair_trees-2.4.8/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-10 14:12:52.000000 fair_trees-2.4.8/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27353 2024-04-10 14:12:39.000000 fair_trees-2.4.8/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:15:57.168258 fair_trees-2.4.8/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     5070 2024-04-10 14:15:57.000000 fair_trees-2.4.8/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-10 14:15:57.000000 fair_trees-2.4.8/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:15:57.000000 fair_trees-2.4.8/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-10 14:15:57.000000 fair_trees-2.4.8/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 14:15:57.000000 fair_trees-2.4.8/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:15:57.168258 fair_trees-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      756 2024-04-10 14:15:40.000000 fair_trees-2.4.8/setup.py
```

### Comparing `fair_trees-2.4.7/LICENSE` & `fair_trees-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.7/PKG-INFO` & `fair_trees-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.7
+Version: 2.4.8
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: urllib
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
 
 # Fair tree classifier using strong demographic parity 
 
 Implementation of the algorithm proposed in:<br>
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.7 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.8 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
-pandas Requires-Dist: urllib Requires-Dist: joblib Requires-Dist: scikit-learn
-# Fair tree classifier using strong demographic parity Implementation of the
-algorithm proposed in:
+pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
+using strong demographic parity Implementation of the algorithm proposed in:
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic
 parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
```

### Comparing `fair_trees-2.4.7/README.md` & `fair_trees-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.7/fair_trees/fair_trees.py` & `fair_trees-2.4.8/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.7/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.8/fair_trees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.7
+Version: 2.4.8
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: urllib
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
 
 # Fair tree classifier using strong demographic parity 
 
 Implementation of the algorithm proposed in:<br>
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic parity_. Machine Learning (2023).
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.7 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.8 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
-pandas Requires-Dist: urllib Requires-Dist: joblib Requires-Dist: scikit-learn
-# Fair tree classifier using strong demographic parity Implementation of the
-algorithm proposed in:
+pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
+using strong demographic parity Implementation of the algorithm proposed in:
 > Pereira Barata, A. et al. _Fair tree classifier using strong demographic
 parity_. Machine Learning (2023). _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
```

### Comparing `fair_trees-2.4.7/setup.py` & `fair_trees-2.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.4.7",
+    version="2.4.8",
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
-        "urllib",
         "joblib",
         "scikit-learn",
     ],
 )
```

