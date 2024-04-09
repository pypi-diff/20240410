# Comparing `tmp/FancySchmancyTestsplit-0.1.0.tar.gz` & `tmp/FancySchmancyTestsplit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FancySchmancyTestsplit-0.1.0.tar", last modified: Tue Apr  9 21:56:17 2024, max compression
+gzip compressed data, was "FancySchmancyTestsplit-0.1.1.tar", last modified: Tue Apr  9 22:19:13 2024, max compression
```

## Comparing `FancySchmancyTestsplit-0.1.0.tar` & `FancySchmancyTestsplit-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 21:56:17.662999 FancySchmancyTestsplit-0.1.0/
--rw-rw-rw-   0        0        0     1998 2024-04-09 21:56:17.661998 FancySchmancyTestsplit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1435 2024-04-09 21:54:56.000000 FancySchmancyTestsplit-0.1.0/README.md
--rw-rw-rw-   0        0        0     1965 2024-04-09 19:13:35.000000 FancySchmancyTestsplit-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 21:56:17.662999 FancySchmancyTestsplit-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 21:56:17.634998 FancySchmancyTestsplit-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:56:17.646000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit/
--rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit/__init__.py
--rw-rw-rw-   0        0        0     3295 2024-04-09 21:52:25.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit/fst.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:56:17.660999 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/
--rw-rw-rw-   0        0        0     1998 2024-04-09 21:56:17.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-09 21:56:17.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 21:56:17.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-09 21:56:17.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-09 21:56:17.000000 FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 21:56:17.658998 FancySchmancyTestsplit-0.1.0/tests/
--rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.0/tests/test_fancy_schmancy_testsplit.py
+drwxrwxrwx   0        0        0        0 2024-04-09 22:19:13.043700 FancySchmancyTestsplit-0.1.1/
+-rw-rw-rw-   0        0        0     2034 2024-04-09 22:19:13.042701 FancySchmancyTestsplit-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1435 2024-04-09 21:54:56.000000 FancySchmancyTestsplit-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1993 2024-04-09 22:18:56.000000 FancySchmancyTestsplit-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 22:19:13.043700 FancySchmancyTestsplit-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 22:19:13.019700 FancySchmancyTestsplit-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 22:19:13.023700 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit/
+-rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit/__init__.py
+-rw-rw-rw-   0        0        0     3295 2024-04-09 21:52:25.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit/fst.py
+drwxrwxrwx   0        0        0        0 2024-04-09 22:19:13.041700 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/
+-rw-rw-rw-   0        0        0     2034 2024-04-09 22:19:12.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-09 22:19:13.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 22:19:13.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-09 22:19:13.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-09 22:19:13.000000 FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 22:19:13.040700 FancySchmancyTestsplit-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.1/tests/test_fancy_schmancy_testsplit.py
```

### Comparing `FancySchmancyTestsplit-0.1.0/PKG-INFO` & `FancySchmancyTestsplit-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.0
+Version: 0.1.1
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.25.2
 Requires-Dist: pandas==2.1.3
+Requires-Dist: scikit-learn==1.3.2
 
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
```

### Comparing `FancySchmancyTestsplit-0.1.0/README.md` & `FancySchmancyTestsplit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.0/pyproject.toml` & `FancySchmancyTestsplit-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,25 @@
 
 # somewhat static info -----------------------------------------------------------------
 name = "FancySchmancyTestsplit"
 description = "a more in-depth testsplit splitting intercategorical"
 keywords = ["test split", "testsplit", "train test split"]
 
 # variable info ------------------------------------------------------------------------
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy==1.25.2",
     "pandas==2.1.3",
+    "scikit-learn==1.3.2",
 ]
 
 [project.optional-dependencies]
 # pdf = ["ReportLab>=1.2", "RXP"]
 # rest = ["docutils>=0.3", "pack ==1.1, ==1.3"]
 
 [project.scripts]
```

### Comparing `FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit/fst.py` & `FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit/fst.py`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.0/src/FancySchmancyTestsplit.egg-info/PKG-INFO` & `FancySchmancyTestsplit-0.1.1/src/FancySchmancyTestsplit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.0
+Version: 0.1.1
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.25.2
 Requires-Dist: pandas==2.1.3
+Requires-Dist: scikit-learn==1.3.2
 
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
 ----
 for reference:
  package | fancy | schmancy | testsplit
  :- | :- | :- | :-
```

### Comparing `FancySchmancyTestsplit-0.1.0/tests/test_fancy_schmancy_testsplit.py` & `FancySchmancyTestsplit-0.1.1/tests/test_fancy_schmancy_testsplit.py`

 * *Files identical despite different names*

