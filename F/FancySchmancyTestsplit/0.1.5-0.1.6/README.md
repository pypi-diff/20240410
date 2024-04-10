# Comparing `tmp/FancySchmancyTestsplit-0.1.5.tar.gz` & `tmp/FancySchmancyTestsplit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FancySchmancyTestsplit-0.1.5.tar", last modified: Wed Apr 10 08:39:38 2024, max compression
+gzip compressed data, was "FancySchmancyTestsplit-0.1.6.tar", last modified: Wed Apr 10 08:52:06 2024, max compression
```

## Comparing `FancySchmancyTestsplit-0.1.5.tar` & `FancySchmancyTestsplit-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.927991 FancySchmancyTestsplit-0.1.5/
--rw-rw-rw-   0        0        0     3041 2024-04-10 08:39:38.926992 FancySchmancyTestsplit-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2442 2024-04-10 08:39:22.000000 FancySchmancyTestsplit-0.1.5/README.md
--rw-rw-rw-   0        0        0     1993 2024-04-10 08:26:18.000000 FancySchmancyTestsplit-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 08:39:38.928991 FancySchmancyTestsplit-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.883991 FancySchmancyTestsplit-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.900992 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/
--rw-rw-rw-   0        0        0      128 2024-04-09 20:35:46.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/__init__.py
--rw-rw-rw-   0        0        0     4407 2024-04-10 08:35:10.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/fst.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.926004 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/
--rw-rw-rw-   0        0        0     3041 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-10 08:39:38.000000 FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 08:39:38.924993 FancySchmancyTestsplit-0.1.5/tests/
--rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.5/tests/test_fancy_schmancy_testsplit.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:52:06.458226 FancySchmancyTestsplit-0.1.6/
+-rw-rw-rw-   0        0        0     3041 2024-04-10 08:52:06.457225 FancySchmancyTestsplit-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2442 2024-04-10 08:39:22.000000 FancySchmancyTestsplit-0.1.6/README.md
+-rw-rw-rw-   0        0        0     1993 2024-04-10 08:50:13.000000 FancySchmancyTestsplit-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 08:52:06.458226 FancySchmancyTestsplit-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 08:52:06.430192 FancySchmancyTestsplit-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 08:52:06.439202 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit/
+-rw-rw-rw-   0        0        0     3101 2024-04-10 08:49:53.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit/__init__.py
+-rw-rw-rw-   0        0        0     4407 2024-04-10 08:35:10.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit/fst.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:52:06.456227 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/
+-rw-rw-rw-   0        0        0     3041 2024-04-10 08:52:06.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-10 08:52:06.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:52:06.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-10 08:52:06.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-10 08:52:06.000000 FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 08:52:06.455227 FancySchmancyTestsplit-0.1.6/tests/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.6/tests/test_fancy_schmancy_testsplit.py
```

### Comparing `FancySchmancyTestsplit-0.1.5/PKG-INFO` & `FancySchmancyTestsplit-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.5
+Version: 0.1.6
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `FancySchmancyTestsplit-0.1.5/README.md` & `FancySchmancyTestsplit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.5/pyproject.toml` & `FancySchmancyTestsplit-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # somewhat static info -----------------------------------------------------------------
 name = "FancySchmancyTestsplit"
 description = "a more in-depth testsplit splitting intercategorical"
 keywords = ["test split", "testsplit", "train test split"]
 
 # variable info ------------------------------------------------------------------------
-version = "0.1.5"
+version = "0.1.6"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
```

### Comparing `FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit/fst.py` & `FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit/fst.py`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.5/src/FancySchmancyTestsplit.egg-info/PKG-INFO` & `FancySchmancyTestsplit-0.1.6/src/FancySchmancyTestsplit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.5
+Version: 0.1.6
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `FancySchmancyTestsplit-0.1.5/tests/test_fancy_schmancy_testsplit.py` & `FancySchmancyTestsplit-0.1.6/tests/test_fancy_schmancy_testsplit.py`

 * *Files identical despite different names*

