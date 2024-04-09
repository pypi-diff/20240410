# Comparing `tmp/FancySchmancyTestsplit-0.1.2.tar.gz` & `tmp/FancySchmancyTestsplit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FancySchmancyTestsplit-0.1.2.tar", last modified: Tue Apr  9 22:53:26 2024, max compression
+gzip compressed data, was "FancySchmancyTestsplit-0.1.3.tar", last modified: Tue Apr  9 23:02:24 2024, max compression
```

## Comparing `FancySchmancyTestsplit-0.1.2.tar` & `FancySchmancyTestsplit-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 22:53:26.874495 FancySchmancyTestsplit-0.1.2/
--rw-rw-rw-   0        0        0     2064 2024-04-09 22:53:26.873497 FancySchmancyTestsplit-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-04-09 22:51:36.000000 FancySchmancyTestsplit-0.1.2/README.md
--rw-rw-rw-   0        0        0     1993 2024-04-09 22:53:19.000000 FancySchmancyTestsplit-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 22:53:26.874495 FancySchmancyTestsplit-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 22:53:26.852495 FancySchmancyTestsplit-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 22:53:26.857496 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit/
--rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit/__init__.py
--rw-rw-rw-   0        0        0     3300 2024-04-09 22:38:46.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit/fst.py
-drwxrwxrwx   0        0        0        0 2024-04-09 22:53:26.871495 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/
--rw-rw-rw-   0        0        0     2064 2024-04-09 22:53:26.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-09 22:53:26.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 22:53:26.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-09 22:53:26.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-09 22:53:26.000000 FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 22:53:26.870495 FancySchmancyTestsplit-0.1.2/tests/
--rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.2/tests/test_fancy_schmancy_testsplit.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.906490 FancySchmancyTestsplit-0.1.3/
+-rw-rw-rw-   0        0        0     2163 2024-04-09 23:02:24.905490 FancySchmancyTestsplit-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1562 2024-04-09 23:02:04.000000 FancySchmancyTestsplit-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1993 2024-04-09 23:02:17.000000 FancySchmancyTestsplit-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 23:02:24.906490 FancySchmancyTestsplit-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.885667 FancySchmancyTestsplit-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.890669 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/
+-rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/__init__.py
+-rw-rw-rw-   0        0        0     3300 2024-04-09 22:38:46.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/fst.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.904490 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/
+-rw-rw-rw-   0        0        0     2163 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.903491 FancySchmancyTestsplit-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.3/tests/test_fancy_schmancy_testsplit.py
```

### Comparing `FancySchmancyTestsplit-0.1.2/PKG-INFO` & `FancySchmancyTestsplit-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.2
+Version: 0.1.3
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -17,21 +17,16 @@
 
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
- sklearn.model_selection | &#10062; | &#10062; | &#9989;
- fancy schmancy testsplit | &#9989; | &#9989; | &#9989;
-
-thumbsup: 
-&#128077;
-thumbsdown:
-&#128078; 
+ sklearn.model_selection | &#128078; | &#128078; | &#128077;
+ fancy schmancy testsplit | &#128077; | &#128077; | &#128077;
 
 a testplit per label category, to ensure that every category is present
         
 ----
 ### Examples
 
 Assume the following DataFrame:
@@ -69,7 +64,9 @@
 X_tr, X_te, y_tr, y_te = \
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
+
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category.
```

### Comparing `FancySchmancyTestsplit-0.1.2/README.md` & `FancySchmancyTestsplit-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
- sklearn.model_selection | &#10062; | &#10062; | &#9989;
- fancy schmancy testsplit | &#9989; | &#9989; | &#9989;
-
-thumbsup: 
-&#128077;
-thumbsdown:
-&#128078; 
+ sklearn.model_selection | &#128078; | &#128078; | &#128077;
+ fancy schmancy testsplit | &#128077; | &#128077; | &#128077;
 
 a testplit per label category, to ensure that every category is present
         
 ----
 ### Examples
 
 Assume the following DataFrame:
@@ -52,7 +47,9 @@
 X_tr, X_te, y_tr, y_te = \
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
+
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category.
```

### Comparing `FancySchmancyTestsplit-0.1.2/pyproject.toml` & `FancySchmancyTestsplit-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # somewhat static info -----------------------------------------------------------------
 name = "FancySchmancyTestsplit"
 description = "a more in-depth testsplit splitting intercategorical"
 keywords = ["test split", "testsplit", "train test split"]
 
 # variable info ------------------------------------------------------------------------
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
```

### Comparing `FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit/fst.py` & `FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/fst.py`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.2/src/FancySchmancyTestsplit.egg-info/PKG-INFO` & `FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.2
+Version: 0.1.3
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -17,21 +17,16 @@
 
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
- sklearn.model_selection | &#10062; | &#10062; | &#9989;
- fancy schmancy testsplit | &#9989; | &#9989; | &#9989;
-
-thumbsup: 
-&#128077;
-thumbsdown:
-&#128078; 
+ sklearn.model_selection | &#128078; | &#128078; | &#128077;
+ fancy schmancy testsplit | &#128077; | &#128077; | &#128077;
 
 a testplit per label category, to ensure that every category is present
         
 ----
 ### Examples
 
 Assume the following DataFrame:
@@ -69,7 +64,9 @@
 X_tr, X_te, y_tr, y_te = \
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
+
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category.
```

### Comparing `FancySchmancyTestsplit-0.1.2/tests/test_fancy_schmancy_testsplit.py` & `FancySchmancyTestsplit-0.1.3/tests/test_fancy_schmancy_testsplit.py`

 * *Files identical despite different names*

