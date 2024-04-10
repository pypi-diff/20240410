# Comparing `tmp/qtsit-0.0.1.dev20240410135159.tar.gz` & `tmp/qtsit-0.0.1.dev20240410142259.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtsit-0.0.1.dev20240410135159.tar", last modified: Wed Apr 10 13:51:59 2024, max compression
+gzip compressed data, was "qtsit-0.0.1.dev20240410142259.tar", last modified: Wed Apr 10 14:23:00 2024, max compression
```

## Comparing `qtsit-0.0.1.dev20240410135159.tar` & `qtsit-0.0.1.dev20240410142259.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:59.787579 qtsit-0.0.1.dev20240410135159/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 13:51:59.787579 qtsit-0.0.1.dev20240410135159/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:59.783579 qtsit-0.0.1.dev20240410135159/qtsit/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/qtsit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/qtsit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:59.787579 qtsit-0.0.1.dev20240410135159/qtsit/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/qtsit/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/qtsit/algorithms/randomwalk.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/qtsit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/qtsit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:59.787579 qtsit-0.0.1.dev20240410135159/qtsit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 13:51:59.000000 qtsit-0.0.1.dev20240410135159/qtsit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 13:51:59.000000 qtsit-0.0.1.dev20240410135159/qtsit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:51:59.000000 qtsit-0.0.1.dev20240410135159/qtsit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 13:51:59.000000 qtsit-0.0.1.dev20240410135159/qtsit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 13:51:59.000000 qtsit-0.0.1.dev20240410135159/qtsit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 13:51:59.787579 qtsit-0.0.1.dev20240410135159/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-10 13:51:49.000000 qtsit-0.0.1.dev20240410135159/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:00.263507 qtsit-0.0.1.dev20240410142259/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 14:23:00.263507 qtsit-0.0.1.dev20240410142259/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:00.263507 qtsit-0.0.1.dev20240410142259/qtsit/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/qtsit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/qtsit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:00.263507 qtsit-0.0.1.dev20240410142259/qtsit/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/qtsit/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/qtsit/algorithms/randomwalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/qtsit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/qtsit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:00.263507 qtsit-0.0.1.dev20240410142259/qtsit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 14:23:00.000000 qtsit-0.0.1.dev20240410142259/qtsit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 14:23:00.000000 qtsit-0.0.1.dev20240410142259/qtsit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:23:00.000000 qtsit-0.0.1.dev20240410142259/qtsit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 14:23:00.000000 qtsit-0.0.1.dev20240410142259/qtsit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 14:23:00.000000 qtsit-0.0.1.dev20240410142259/qtsit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 14:23:00.263507 qtsit-0.0.1.dev20240410142259/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-10 14:22:48.000000 qtsit-0.0.1.dev20240410142259/setup.py
```

### Comparing `qtsit-0.0.1.dev20240410135159/LICENSE` & `qtsit-0.0.1.dev20240410142259/LICENSE`

 * *Files identical despite different names*

### Comparing `qtsit-0.0.1.dev20240410135159/PKG-INFO` & `qtsit-0.0.1.dev20240410142259/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtsit
-Version: 0.0.1.dev20240410135159
+Version: 0.0.1.dev20240410142259
 Summary: QTSIT: Quantum Technologies for Industry Transformation Toolkit
 Home-page: https://github.com/qtsit/qtsit
 Maintainer: QTSIT contributors
 License: MIT
 Project-URL: Documentation, https://qtsit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/QTSIT/qtsit
 Keywords: qtsit,quantum-chemistry,quantum-computing,quantum-ml,quantum-ai
```

### Comparing `qtsit-0.0.1.dev20240410135159/README.md` & `qtsit-0.0.1.dev20240410142259/README.md`

 * *Files identical despite different names*

### Comparing `qtsit-0.0.1.dev20240410135159/qtsit/cli.py` & `qtsit-0.0.1.dev20240410142259/qtsit/cli.py`

 * *Files identical despite different names*

### Comparing `qtsit-0.0.1.dev20240410135159/qtsit.egg-info/PKG-INFO` & `qtsit-0.0.1.dev20240410142259/qtsit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtsit
-Version: 0.0.1.dev20240410135159
+Version: 0.0.1.dev20240410142259
 Summary: QTSIT: Quantum Technologies for Industry Transformation Toolkit
 Home-page: https://github.com/qtsit/qtsit
 Maintainer: QTSIT contributors
 License: MIT
 Project-URL: Documentation, https://qtsit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/QTSIT/qtsit
 Keywords: qtsit,quantum-chemistry,quantum-computing,quantum-ml,quantum-ai
```

### Comparing `qtsit-0.0.1.dev20240410135159/setup.py` & `qtsit-0.0.1.dev20240410142259/setup.py`

 * *Files identical despite different names*

