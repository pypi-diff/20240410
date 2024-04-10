# Comparing `tmp/target-ports-2.0.tar.gz` & `tmp/target-ports-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-2.0.tar", last modified: Wed Apr  3 23:40:05 2024, max compression
+gzip compressed data, was "target-ports-2.1.tar", last modified: Wed Apr 10 10:08:06 2024, max compression
```

## Comparing `target-ports-2.0.tar` & `target-ports-2.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.359513 target-ports-2.0/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-2.0/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 23:40:05.358899 target-ports-2.0/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-2.0/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-03 23:39:44.000000 target-ports-2.0/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 23:40:05.359604 target-ports-2.0/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.345551 target-ports-2.0/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.348823 target-ports-2.0/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-2.0/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     6599 2024-04-03 23:39:39.000000 target-ports-2.0/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.358284 target-ports-2.0/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 10:08:06.123653 target-ports-2.1/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-2.1/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4368 2024-04-10 10:08:06.123213 target-ports-2.1/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-2.1/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1187 2024-04-10 10:07:35.000000 target-ports-2.1/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-10 10:08:06.123718 target-ports-2.1/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 10:08:06.115215 target-ports-2.1/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 10:08:06.118226 target-ports-2.1/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-2.1/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6599 2024-04-03 23:39:39.000000 target-ports-2.1/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 10:08:06.122635 target-ports-2.1/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4368 2024-04-10 10:08:06.000000 target-ports-2.1/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      356 2024-04-10 10:08:06.000000 target-ports-2.1/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-10 10:08:06.000000 target-ports-2.1/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-10 10:08:06.000000 target-ports-2.1/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-10 10:08:06.000000 target-ports-2.1/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-10 10:08:06.000000 target-ports-2.1/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 10:08:06.121957 target-ports-2.1/tests/
+-rw-r--r--   0 d33pster   (501) staff       (20)      176 2024-04-10 09:46:22.000000 target-ports-2.1/tests/test_ports.py
```

### Comparing `target-ports-2.0/LICENSE` & `target-ports-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-2.0/PKG-INFO` & `target-ports-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 2.0
+Version: 2.1
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -33,20 +33,19 @@
 Project-URL: GitHub, https://github.com/d33pster/target-ports
 Project-URL: Issues, https://github.com/d33pster/target-ports/issues
 Project-URL: Documentation, https://d33pster.github.io/target-ports/
 Keywords: d33pster,port scanner,port,scanner,recon,portscanner,target-ports,targetports
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
 Requires-Dist: optioner>=1.4.5
 
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
```

### Comparing `target-ports-2.0/README.md` & `target-ports-2.1/README.md`

 * *Files identical despite different names*

### Comparing `target-ports-2.0/pyproject.toml` & `target-ports-2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "2.0"
+version = "2.1"
 description = "Scan ports of a target"
-requires-python = ">=3.9"
+requires-python = ">3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'termcolor',
```

### Comparing `target-ports-2.0/src/target_ports/target_ports.py` & `target-ports-2.1/src/target_ports/target_ports.py`

 * *Files identical despite different names*

### Comparing `target-ports-2.0/src/target_ports.egg-info/PKG-INFO` & `target-ports-2.1/src/target_ports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 2.0
+Version: 2.1
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -33,20 +33,19 @@
 Project-URL: GitHub, https://github.com/d33pster/target-ports
 Project-URL: Issues, https://github.com/d33pster/target-ports/issues
 Project-URL: Documentation, https://d33pster.github.io/target-ports/
 Keywords: d33pster,port scanner,port,scanner,recon,portscanner,target-ports,targetports
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
 Requires-Dist: optioner>=1.4.5
 
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
```

