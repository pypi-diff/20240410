# Comparing `tmp/pytruncreg-0.1.tar.gz` & `tmp/pytruncreg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytruncreg-0.1.tar", last modified: Wed Apr 10 03:03:53 2024, max compression
+gzip compressed data, was "pytruncreg-0.1.1.tar", last modified: Wed Apr 10 03:12:50 2024, max compression
```

## Comparing `pytruncreg-0.1.tar` & `pytruncreg-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 03:03:53.808208 pytruncreg-0.1/
--rw-r--r--   0 ryo766     (503) staff       (20)     1065 2024-04-10 02:46:05.000000 pytruncreg-0.1/LICENSE
--rw-r--r--   0 ryo766     (503) staff       (20)     2927 2024-04-10 03:03:53.808035 pytruncreg-0.1/PKG-INFO
--rw-r--r--   0 ryo766     (503) staff       (20)     2592 2024-04-10 02:46:05.000000 pytruncreg-0.1/README.md
-drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 03:03:53.806822 pytruncreg-0.1/pytruncreg/
--rw-r--r--   0 ryo766     (503) staff       (20)       60 2024-04-10 02:46:05.000000 pytruncreg-0.1/pytruncreg/__init__.py
--rw-r--r--   0 ryo766     (503) staff       (20)     5709 2024-04-10 02:46:05.000000 pytruncreg-0.1/pytruncreg/truncreg.py
-drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 03:03:53.807845 pytruncreg-0.1/pytruncreg.egg-info/
--rw-r--r--   0 ryo766     (503) staff       (20)     2927 2024-04-10 03:03:53.000000 pytruncreg-0.1/pytruncreg.egg-info/PKG-INFO
--rw-r--r--   0 ryo766     (503) staff       (20)      241 2024-04-10 03:03:53.000000 pytruncreg-0.1/pytruncreg.egg-info/SOURCES.txt
--rw-r--r--   0 ryo766     (503) staff       (20)        1 2024-04-10 03:03:53.000000 pytruncreg-0.1/pytruncreg.egg-info/dependency_links.txt
--rw-r--r--   0 ryo766     (503) staff       (20)       19 2024-04-10 03:03:53.000000 pytruncreg-0.1/pytruncreg.egg-info/requires.txt
--rw-r--r--   0 ryo766     (503) staff       (20)       11 2024-04-10 03:03:53.000000 pytruncreg-0.1/pytruncreg.egg-info/top_level.txt
--rw-r--r--   0 ryo766     (503) staff       (20)       38 2024-04-10 03:03:53.808251 pytruncreg-0.1/setup.cfg
--rw-r--r--   0 ryo766     (503) staff       (20)      482 2024-04-10 02:46:05.000000 pytruncreg-0.1/setup.py
+drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 03:12:50.651330 pytruncreg-0.1.1/
+-rw-r--r--   0 ryo766     (503) staff       (20)     1065 2024-04-10 02:46:05.000000 pytruncreg-0.1.1/LICENSE
+-rw-r--r--   0 ryo766     (503) staff       (20)     2934 2024-04-10 03:12:50.651132 pytruncreg-0.1.1/PKG-INFO
+-rw-r--r--   0 ryo766     (503) staff       (20)     2592 2024-04-10 02:46:05.000000 pytruncreg-0.1.1/README.md
+drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 03:12:50.649733 pytruncreg-0.1.1/pytruncreg/
+-rw-r--r--   0 ryo766     (503) staff       (20)       60 2024-04-10 02:46:05.000000 pytruncreg-0.1.1/pytruncreg/__init__.py
+-rw-r--r--   0 ryo766     (503) staff       (20)     5709 2024-04-10 02:46:05.000000 pytruncreg-0.1.1/pytruncreg/truncreg.py
+drwxr-xr-x   0 ryo766     (503) staff       (20)        0 2024-04-10 03:12:50.650877 pytruncreg-0.1.1/pytruncreg.egg-info/
+-rw-r--r--   0 ryo766     (503) staff       (20)     2934 2024-04-10 03:12:50.000000 pytruncreg-0.1.1/pytruncreg.egg-info/PKG-INFO
+-rw-r--r--   0 ryo766     (503) staff       (20)      241 2024-04-10 03:12:50.000000 pytruncreg-0.1.1/pytruncreg.egg-info/SOURCES.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)        1 2024-04-10 03:12:50.000000 pytruncreg-0.1.1/pytruncreg.egg-info/dependency_links.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)       19 2024-04-10 03:12:50.000000 pytruncreg-0.1.1/pytruncreg.egg-info/requires.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)       11 2024-04-10 03:12:50.000000 pytruncreg-0.1.1/pytruncreg.egg-info/top_level.txt
+-rw-r--r--   0 ryo766     (503) staff       (20)       38 2024-04-10 03:12:50.651378 pytruncreg-0.1.1/setup.cfg
+-rw-r--r--   0 ryo766     (503) staff       (20)      489 2024-04-10 03:12:23.000000 pytruncreg-0.1.1/setup.py
```

### Comparing `pytruncreg-0.1/LICENSE` & `pytruncreg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytruncreg-0.1/PKG-INFO` & `pytruncreg-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytruncreg
-Version: 0.1
+Version: 0.1.1
 Summary: Truncated Gaussian Regression Models
-Home-page: https://github.com/ryan-odea/pytruncreg/
+Home-page: https://github.com/CausalInference/pytruncreg
 Author: Ryan ODea
 Author-email: ryanodea@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
```

### Comparing `pytruncreg-0.1/README.md` & `pytruncreg-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytruncreg-0.1/pytruncreg/truncreg.py` & `pytruncreg-0.1.1/pytruncreg/truncreg.py`

 * *Files identical despite different names*

### Comparing `pytruncreg-0.1/pytruncreg.egg-info/PKG-INFO` & `pytruncreg-0.1.1/pytruncreg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytruncreg
-Version: 0.1
+Version: 0.1.1
 Summary: Truncated Gaussian Regression Models
-Home-page: https://github.com/ryan-odea/pytruncreg/
+Home-page: https://github.com/CausalInference/pytruncreg
 Author: Ryan ODea
 Author-email: ryanodea@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
```

