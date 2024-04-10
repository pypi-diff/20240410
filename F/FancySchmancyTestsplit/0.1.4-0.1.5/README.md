# Comparing `tmp/FancySchmancyTestsplit-0.1.4.tar.gz` & `tmp/FancySchmancyTestsplit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FancySchmancyTestsplit-0.1.4.tar", last modified: Tue Apr  9 23:07:35 2024, max compression
+gzip compressed data, was "FancySchmancyTestsplit-0.1.5.tar", last modified: Wed Apr 10 08:39:38 2024, max compression
```

## Comparing `FancySchmancyTestsplit-0.1.4.tar` & `FancySchmancyTestsplit-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.611934 FancySchmancyTestsplit-0.1.4/
--rw-rw-rw-   0        0        0     2175 2024-04-09 23:07:35.610933 FancySchmancyTestsplit-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1574 2024-04-09 23:07:22.000000 FancySchmancyTestsplit-0.1.4/README.md
--rw-rw-rw-   0        0        0     1993 2024-04-09 23:07:28.000000 FancySchmancyTestsplit-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 23:07:35.611934 FancySchmancyTestsplit-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.587932 FancySchmancyTestsplit-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.592932 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/
--rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/__init__.py
--rw-rw-rw-   0        0        0     3300 2024-04-09 22:38:46.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit/fst.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.609933 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/
--rw-rw-rw-   0        0        0     2175 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-09 23:07:35.000000 FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 23:07:35.608934 FancySchmancyTestsplit-0.1.4/tests/
--rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.4/tests/test_fancy_schmancy_testsplit.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.927991 FancySchmancyTestsplit-0.1.5/
+-rw-rw-rw-   0        0        0     3041 2024-04-10 08:39:38.926992 FancySchmancyTestsplit-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2442 2024-04-10 08:39:22.000000 FancySchmancyTestsplit-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1993 2024-04-10 08:26:18.000000 FancySchmancyTestsplit-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 08:39:38.928991 FancySchmancyTestsplit-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.883991 FancySchmancyTestsplit-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.900992 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/
+-rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/__init__.py
+-rw-rw-rw-   0        0        0     4407 2024-04-10 08:35:10.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/fst.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.926004 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/
+-rw-rw-rw-   0        0        0     3041 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.924993 FancySchmancyTestsplit-0.1.5/tests/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.5/tests/test_fancy_schmancy_testsplit.py
```

### Comparing `FancySchmancyTestsplit-0.1.4/PKG-INFO` & `FancySchmancyTestsplit-0.1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.4
+Version: 0.1.5
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -66,7 +66,43 @@
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
 
 This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
+
+If this was done for "Cat1" and "Cat2", it would look like this:
+
+|| Column B
+:- | -:
+0 | Cat1
+4 | Cat2
+6 | Cat2
+5 | Cat2
+8 | Cat2
+
+To shorten the process, the method fancy_schmancy_testsplit can be used in this way:
+
+```Python
+from FancySchmancyTestsplit.fst import fancy_schmancy_testsplit
+from pandas import DataFrame
+df = DataFrame(data= {"Column A":[10, 14, 12, 13, 9, 5, 13, 16, 18, 4, 12],
+"Column B": ["Cat1", "Cat1", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2"]})
+X_train, X_test, y_train, y_test = \
+    fancy_schmancy_testsplit(data= df,
+                            label_column= "Column B",
+                            test_split= 0.5,
+                            seed= 42
+                            )
+print(y_train)
+```
+|| Column B
+:- | -:
+0 | Cat1
+4 | Cat2
+6 | Cat2
+5 | Cat2
+8 | Cat2
+
+
+
```

### Comparing `FancySchmancyTestsplit-0.1.4/README.md` & `FancySchmancyTestsplit-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -48,8 +48,44 @@
     train_test_split(X, y, test_size = 0.5, random_state = 42)
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
 
-This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
+This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
+
+If this was done for "Cat1" and "Cat2", it would look like this:
+
+|| Column B
+:- | -:
+0 | Cat1
+4 | Cat2
+6 | Cat2
+5 | Cat2
+8 | Cat2
+
+To shorten the process, the method fancy_schmancy_testsplit can be used in this way:
+
+```Python
+from FancySchmancyTestsplit.fst import fancy_schmancy_testsplit
+from pandas import DataFrame
+df = DataFrame(data= {"Column A":[10, 14, 12, 13, 9, 5, 13, 16, 18, 4, 12],
+"Column B": ["Cat1", "Cat1", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2"]})
+X_train, X_test, y_train, y_test = \
+    fancy_schmancy_testsplit(data= df,
+                            label_column= "Column B",
+                            test_split= 0.5,
+                            seed= 42
+                            )
+print(y_train)
+```
+|| Column B
+:- | -:
+0 | Cat1
+4 | Cat2
+6 | Cat2
+5 | Cat2
+8 | Cat2
+
+
+
```

### Comparing `FancySchmancyTestsplit-0.1.4/pyproject.toml` & `FancySchmancyTestsplit-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # somewhat static info -----------------------------------------------------------------
 name = "FancySchmancyTestsplit"
 description = "a more in-depth testsplit splitting intercategorical"
 keywords = ["test split", "testsplit", "train test split"]
 
 # variable info ------------------------------------------------------------------------
-version = "0.1.4"
+version = "0.1.5"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
```

### Comparing `FancySchmancyTestsplit-0.1.4/src/FancySchmancyTestsplit.egg-info/PKG-INFO` & `FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.4
+Version: 0.1.5
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -66,7 +66,43 @@
 print(y_tr)
 ```
 || Column B
 :- | -:
 0 | Cat1
 
 This is done for every unique entry of the given label column, so that a random pick of train and test data is done for every category separately.
+
+If this was done for "Cat1" and "Cat2", it would look like this:
+
+|| Column B
+:- | -:
+0 | Cat1
+4 | Cat2
+6 | Cat2
+5 | Cat2
+8 | Cat2
+
+To shorten the process, the method fancy_schmancy_testsplit can be used in this way:
+
+```Python
+from FancySchmancyTestsplit.fst import fancy_schmancy_testsplit
+from pandas import DataFrame
+df = DataFrame(data= {"Column A":[10, 14, 12, 13, 9, 5, 13, 16, 18, 4, 12],
+"Column B": ["Cat1", "Cat1", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2", "Cat2"]})
+X_train, X_test, y_train, y_test = \
+    fancy_schmancy_testsplit(data= df,
+                            label_column= "Column B",
+                            test_split= 0.5,
+                            seed= 42
+                            )
+print(y_train)
+```
+|| Column B
+:- | -:
+0 | Cat1
+4 | Cat2
+6 | Cat2
+5 | Cat2
+8 | Cat2
+
+
+
```

### Comparing `FancySchmancyTestsplit-0.1.4/tests/test_fancy_schmancy_testsplit.py` & `FancySchmancyTestsplit-0.1.5/tests/test_fancy_schmancy_testsplit.py`

 * *Files identical despite different names*

