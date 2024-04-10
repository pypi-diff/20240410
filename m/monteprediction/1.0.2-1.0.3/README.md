# Comparing `tmp/monteprediction-1.0.2.tar.gz` & `tmp/monteprediction-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monteprediction-1.0.2.tar", last modified: Fri Mar  1 03:24:49 2024, max compression
+gzip compressed data, was "monteprediction-1.0.3.tar", last modified: Wed Apr 10 03:36:47 2024, max compression
```

## Comparing `monteprediction-1.0.2.tar` & `monteprediction-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:24:49.382925 monteprediction-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-01 03:24:37.000000 monteprediction-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-01 03:24:49.382925 monteprediction-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-01 03:24:37.000000 monteprediction-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:24:49.378925 monteprediction-1.0.2/monteprediction/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-01 03:24:37.000000 monteprediction-1.0.2/monteprediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-01 03:24:37.000000 monteprediction-1.0.2/monteprediction/calendarutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-01 03:24:37.000000 monteprediction-1.0.2/monteprediction/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-01 03:24:37.000000 monteprediction-1.0.2/monteprediction/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-01 03:24:37.000000 monteprediction-1.0.2/monteprediction/truth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:24:49.382925 monteprediction-1.0.2/monteprediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-01 03:24:49.000000 monteprediction-1.0.2/monteprediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-01 03:24:49.000000 monteprediction-1.0.2/monteprediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 03:24:49.000000 monteprediction-1.0.2/monteprediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-01 03:24:49.000000 monteprediction-1.0.2/monteprediction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 03:24:49.000000 monteprediction-1.0.2/monteprediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-01 03:24:49.000000 monteprediction-1.0.2/monteprediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 03:24:49.382925 monteprediction-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-01 03:24:37.000000 monteprediction-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:24:49.378925 monteprediction-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-01 03:24:37.000000 monteprediction-1.0.2/tests/test_calendarutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.065123 monteprediction-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 03:36:36.000000 monteprediction-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 03:36:47.065123 monteprediction-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 03:36:36.000000 monteprediction-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.061123 monteprediction-1.0.3/monteprediction/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/calendarutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.065123 monteprediction-1.0.3/monteprediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:36:47.065123 monteprediction-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 03:36:36.000000 monteprediction-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.065123 monteprediction-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-10 03:36:36.000000 monteprediction-1.0.3/tests/test_calendarutil.py
```

### Comparing `monteprediction-1.0.2/LICENSE` & `monteprediction-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.2/PKG-INFO` & `monteprediction-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monteprediction-1.0.2/monteprediction/submission.py` & `monteprediction-1.0.3/monteprediction/submission.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.2/monteprediction/truth.py` & `monteprediction-1.0.3/monteprediction/truth.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.2/monteprediction.egg-info/PKG-INFO` & `monteprediction-1.0.3/monteprediction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monteprediction-1.0.2/setup.py` & `monteprediction-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="monteprediction",
-    version="1.0.2",
+    version="1.0.3",
     description="A Weekly Monte Carlo Game",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/microprediction/monteprediction",
     author="microprediction",
     author_email="peter.cotton@microprediction.com",
     license="MIT",
```

### Comparing `monteprediction-1.0.2/tests/test_calendarutil.py` & `monteprediction-1.0.3/tests/test_calendarutil.py`

 * *Files identical despite different names*

