# Comparing `tmp/qtsit-0.0.1.dev20240123003738.tar.gz` & `tmp/qtsit-0.0.1.dev20240410133333.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtsit-0.0.1.dev20240123003738.tar", last modified: Mon Jan 22 19:07:38 2024, max compression
+gzip compressed data, was "qtsit-0.0.1.dev20240410133333.tar", last modified: Wed Apr 10 13:33:33 2024, max compression
```

## Comparing `qtsit-0.0.1.dev20240123003738.tar` & `qtsit-0.0.1.dev20240410133333.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shreyasv   (501) staff       (20)        0 2024-01-22 19:07:38.878036 qtsit-0.0.1.dev20240123003738/
--rw-r--r--   0 shreyasv   (501) staff       (20)     1062 2024-01-21 15:32:37.000000 qtsit-0.0.1.dev20240123003738/LICENSE
--rw-r--r--   0 shreyasv   (501) staff       (20)      899 2024-01-22 19:07:38.878110 qtsit-0.0.1.dev20240123003738/PKG-INFO
--rw-r--r--   0 shreyasv   (501) staff       (20)      783 2024-01-22 18:40:26.000000 qtsit-0.0.1.dev20240123003738/README.md
-drwxr-xr-x   0 shreyasv   (501) staff       (20)        0 2024-01-22 19:07:38.876178 qtsit-0.0.1.dev20240123003738/qtsit/
--rw-r--r--   0 shreyasv   (501) staff       (20)      126 2024-01-22 16:18:28.000000 qtsit-0.0.1.dev20240123003738/qtsit/__init__.py
--rw-r--r--   0 shreyasv   (501) staff       (20)      136 2024-01-21 15:23:54.000000 qtsit-0.0.1.dev20240123003738/qtsit/__main__.py
-drwxr-xr-x   0 shreyasv   (501) staff       (20)        0 2024-01-22 19:07:38.877792 qtsit-0.0.1.dev20240123003738/qtsit/algorithms/
--rw-r--r--   0 shreyasv   (501) staff       (20)       79 2024-01-22 16:22:15.000000 qtsit-0.0.1.dev20240123003738/qtsit/algorithms/__init__.py
--rw-r--r--   0 shreyasv   (501) staff       (20)      185 2024-01-22 16:20:51.000000 qtsit-0.0.1.dev20240123003738/qtsit/algorithms/randomwalk.py
--rw-r--r--   0 shreyasv   (501) staff       (20)      317 2024-01-21 15:23:54.000000 qtsit-0.0.1.dev20240123003738/qtsit/base.py
--rw-r--r--   0 shreyasv   (501) staff       (20)      734 2024-01-21 15:23:54.000000 qtsit-0.0.1.dev20240123003738/qtsit/cli.py
-drwxr-xr-x   0 shreyasv   (501) staff       (20)        0 2024-01-22 19:07:38.877388 qtsit-0.0.1.dev20240123003738/qtsit.egg-info/
--rw-r--r--   0 shreyasv   (501) staff       (20)      899 2024-01-22 19:07:38.000000 qtsit-0.0.1.dev20240123003738/qtsit.egg-info/PKG-INFO
--rw-r--r--   0 shreyasv   (501) staff       (20)      303 2024-01-22 19:07:38.000000 qtsit-0.0.1.dev20240123003738/qtsit.egg-info/SOURCES.txt
--rw-r--r--   0 shreyasv   (501) staff       (20)        1 2024-01-22 19:07:38.000000 qtsit-0.0.1.dev20240123003738/qtsit.egg-info/dependency_links.txt
--rw-r--r--   0 shreyasv   (501) staff       (20)       13 2024-01-22 19:07:38.000000 qtsit-0.0.1.dev20240123003738/qtsit.egg-info/requires.txt
--rw-r--r--   0 shreyasv   (501) staff       (20)        6 2024-01-22 19:07:38.000000 qtsit-0.0.1.dev20240123003738/qtsit.egg-info/top_level.txt
--rw-r--r--   0 shreyasv   (501) staff       (20)      701 2024-01-22 19:07:38.878405 qtsit-0.0.1.dev20240123003738/setup.cfg
--rw-r--r--   0 shreyasv   (501) staff       (20)     2178 2024-01-22 19:07:28.000000 qtsit-0.0.1.dev20240123003738/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:33.488473 qtsit-0.0.1.dev20240410133333/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 13:33:33.488473 qtsit-0.0.1.dev20240410133333/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:33.488473 qtsit-0.0.1.dev20240410133333/qtsit/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/qtsit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/qtsit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:33.488473 qtsit-0.0.1.dev20240410133333/qtsit/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/qtsit/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/qtsit/algorithms/randomwalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/qtsit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/qtsit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:33.488473 qtsit-0.0.1.dev20240410133333/qtsit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 13:33:33.000000 qtsit-0.0.1.dev20240410133333/qtsit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 13:33:33.000000 qtsit-0.0.1.dev20240410133333/qtsit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:33:33.000000 qtsit-0.0.1.dev20240410133333/qtsit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 13:33:33.000000 qtsit-0.0.1.dev20240410133333/qtsit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 13:33:33.000000 qtsit-0.0.1.dev20240410133333/qtsit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 13:33:33.492473 qtsit-0.0.1.dev20240410133333/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-10 13:33:23.000000 qtsit-0.0.1.dev20240410133333/setup.py
```

### Comparing `qtsit-0.0.1.dev20240123003738/LICENSE` & `qtsit-0.0.1.dev20240410133333/LICENSE`

 * *Files identical despite different names*

### Comparing `qtsit-0.0.1.dev20240123003738/PKG-INFO` & `qtsit-0.0.1.dev20240410133333/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: qtsit
-Version: 0.0.1.dev20240123003738
+Version: 0.0.1.dev20240410133333
 Summary: QTSIT: Quantum Technologies for Industry Transformation Toolkit
 Home-page: https://github.com/qtsit/qtsit
 Maintainer: QTSIT contributors
 License: MIT
 Project-URL: Documentation, https://qtsit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/QTSIT/qtsit
 Keywords: qtsit,quantum-chemistry,quantum-computing,quantum-ml,quantum-ai
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9,<3.12
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `qtsit-0.0.1.dev20240123003738/README.md` & `qtsit-0.0.1.dev20240410133333/README.md`

 * *Files identical despite different names*

### Comparing `qtsit-0.0.1.dev20240123003738/qtsit/cli.py` & `qtsit-0.0.1.dev20240410133333/qtsit/cli.py`

 * *Files identical despite different names*

### Comparing `qtsit-0.0.1.dev20240123003738/qtsit.egg-info/PKG-INFO` & `qtsit-0.0.1.dev20240410133333/qtsit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: qtsit
-Version: 0.0.1.dev20240123003738
+Version: 0.0.1.dev20240410133333
 Summary: QTSIT: Quantum Technologies for Industry Transformation Toolkit
 Home-page: https://github.com/qtsit/qtsit
 Maintainer: QTSIT contributors
 License: MIT
 Project-URL: Documentation, https://qtsit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/QTSIT/qtsit
 Keywords: qtsit,quantum-chemistry,quantum-computing,quantum-ml,quantum-ai
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9,<3.12
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `qtsit-0.0.1.dev20240123003738/setup.py` & `qtsit-0.0.1.dev20240410133333/setup.py`

 * *Files identical despite different names*

