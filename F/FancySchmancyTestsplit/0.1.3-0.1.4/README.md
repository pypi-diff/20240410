# Comparing `tmp/FancySchmancyTestsplit-0.1.3.tar.gz` & `tmp/FancySchmancyTestsplit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FancySchmancyTestsplit-0.1.3.tar", last modified: Tue Apr  9 23:02:24 2024, max compression
+gzip compressed data, was "FancySchmancyTestsplit-0.1.4.tar", last modified: Tue Apr  9 23:07:35 2024, max compression
```

## Comparing `FancySchmancyTestsplit-0.1.3.tar` & `FancySchmancyTestsplit-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.906490 FancySchmancyTestsplit-0.1.3/
--rw-rw-rw-   0        0        0     2163 2024-04-09 23:02:24.905490 FancySchmancyTestsplit-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1562 2024-04-09 23:02:04.000000 FancySchmancyTestsplit-0.1.3/README.md
--rw-rw-rw-   0        0        0     1993 2024-04-09 23:02:17.000000 FancySchmancyTestsplit-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 23:02:24.906490 FancySchmancyTestsplit-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.885667 FancySchmancyTestsplit-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.890669 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/
--rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/__init__.py
--rw-rw-rw-   0        0        0     3300 2024-04-09 22:38:46.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/fst.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.904490 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/
--rw-rw-rw-   0        0        0     2163 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-09 23:02:24.000000 FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 23:02:24.903491 FancySchmancyTestsplit-0.1.3/tests/
--rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.3/tests/test_fancy_schmancy_testsplit.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.611934 FancySchmancyTestsplit-0.1.4/
+-rw-rw-rw-   0        0        0     2175 2024-04-09 23:07:35.610933 FancySchmancyTestsplit-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1574 2024-04-09 23:07:22.000000 FancySchmancyTestsplit-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1993 2024-04-09 23:07:28.000000 FancySchmancyTestsplit-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 23:07:35.611934 FancySchmancyTestsplit-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.587932 FancySchmancyTestsplit-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.592932 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/
+-rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/__init__.py
+-rw-rw-rw-   0        0        0     3300 2024-04-09 22:38:46.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/fst.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.609933 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/
+-rw-rw-rw-   0        0        0     2175 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.608934 FancySchmancyTestsplit-0.1.4/tests/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.4/tests/test_fancy_schmancy_testsplit.py
```

### Comparing `FancySchmancyTestsplit-0.1.3/PKG-INFO` & `FancySchmancyTestsplit-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.3
+Version: 0.1.4
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -20,15 +20,15 @@
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
  sklearn.model_selection | &#128078; | &#128078; | &#128077;
  fancy schmancy testsplit | &#128077; | &#128077; | &#128077;
 
-a testplit per label category, to ensure that every category is present
+a testsplit per label category, to ensure that every category is present
         
 ----
 ### Examples
 
 Assume the following DataFrame:
 ```Python
 df = DataFrame(data= {"Column A":[10, 14, 12, 13, 9, 5, 13, 16, 18, 4, 12],
@@ -65,8 +65,8 @@
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
 
-This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category.
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
```

### Comparing `FancySchmancyTestsplit-0.1.3/README.md` & `FancySchmancyTestsplit-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
  sklearn.model_selection | &#128078; | &#128078; | &#128077;
  fancy schmancy testsplit | &#128077; | &#128077; | &#128077;
 
-a testplit per label category, to ensure that every category is present
+a testsplit per label category, to ensure that every category is present
         
 ----
 ### Examples
 
 Assume the following DataFrame:
 ```Python
 df = DataFrame(data= {"Column A":[10, 14, 12, 13, 9, 5, 13, 16, 18, 4, 12],
@@ -48,8 +48,8 @@
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
 
-This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category.
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
```

### Comparing `FancySchmancyTestsplit-0.1.3/pyproject.toml` & `FancySchmancyTestsplit-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # somewhat static info -----------------------------------------------------------------
 name = "FancySchmancyTestsplit"
 description = "a more in-depth testsplit splitting intercategorical"
 keywords = ["test split", "testsplit", "train test split"]
 
 # variable info ------------------------------------------------------------------------
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
```

### Comparing `FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit/fst.py` & `FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/fst.py`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.3/src/FancySchmancyTestsplit.egg-info/PKG-INFO` & `FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.3
+Version: 0.1.4
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -20,15 +20,15 @@
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
  sklearn.model_selection | &#128078; | &#128078; | &#128077;
  fancy schmancy testsplit | &#128077; | &#128077; | &#128077;
 
-a testplit per label category, to ensure that every category is present
+a testsplit per label category, to ensure that every category is present
         
 ----
 ### Examples
 
 Assume the following DataFrame:
 ```Python
 df = DataFrame(data= {"Column A":[10, 14, 12, 13, 9, 5, 13, 16, 18, 4, 12],
@@ -65,8 +65,8 @@
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
 
-This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category.
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
```

### Comparing `FancySchmancyTestsplit-0.1.3/tests/test_fancy_schmancy_testsplit.py` & `FancySchmancyTestsplit-0.1.4/tests/test_fancy_schmancy_testsplit.py`

 * *Files identical despite different names*

