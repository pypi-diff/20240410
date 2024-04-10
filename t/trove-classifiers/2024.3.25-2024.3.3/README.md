# Comparing `tmp/trove-classifiers-2024.3.25.tar.gz` & `tmp/trove-classifiers-2024.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove-classifiers-2024.3.25.tar", last modified: Mon Mar 25 14:58:23 2024, max compression
+gzip compressed data, was "trove-classifiers-2024.3.3.tar", last modified: Sun Mar  3 20:17:28 2024, max compression
```

## Comparing `trove-classifiers-2024.3.25.tar` & `trove-classifiers-2024.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.610387 trove-classifiers-2024.3.25/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-25 14:58:23.610387 trove-classifiers-2024.3.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.606387 trove-classifiers-2024.3.25/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/bin/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.606387 trove-classifiers-2024.3.25/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:58:23.610387 trove-classifiers-2024.3.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.606387 trove-classifiers-2024.3.25/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.606387 trove-classifiers-2024.3.25/src/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (127)    41270 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/src/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/src/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/src/trove_classifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.610387 trove-classifiers-2024.3.25/src/trove_classifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-25 14:58:23.000000 trove-classifiers-2024.3.25/src/trove_classifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-25 14:58:23.000000 trove-classifiers-2024.3.25/src/trove_classifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:58:23.000000 trove-classifiers-2024.3.25/src/trove_classifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 14:58:23.000000 trove-classifiers-2024.3.25/src/trove_classifiers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.606387 trove-classifiers-2024.3.25/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:23.610387 trove-classifiers-2024.3.25/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/tests/lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-25 14:58:00.000000 trove-classifiers-2024.3.25/tests/test_classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/bin/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 20:17:28.001174 trove-classifiers-2024.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/src/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)    41090 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/src/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/src/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/src/trove_classifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/src/trove_classifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-03 20:17:27.000000 trove-classifiers-2024.3.3/src/trove_classifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-03 20:17:27.000000 trove-classifiers-2024.3.3/src/trove_classifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 20:17:27.000000 trove-classifiers-2024.3.3/src/trove_classifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-03 20:17:27.000000 trove-classifiers-2024.3.3/src/trove_classifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:17:27.997174 trove-classifiers-2024.3.3/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/tests/lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-03 20:16:58.000000 trove-classifiers-2024.3.3/tests/test_classifiers.py
```

### Comparing `trove-classifiers-2024.3.25/CONTRIBUTING.md` & `trove-classifiers-2024.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/LICENSE` & `trove-classifiers-2024.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/Makefile` & `trove-classifiers-2024.3.3/Makefile`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/PKG-INFO` & `trove-classifiers-2024.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2024.3.25
+Version: 2024.3.3
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2024.3.25/README.md` & `trove-classifiers-2024.3.3/README.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/bin/sort.py` & `trove-classifiers-2024.3.3/bin/sort.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/setup.py` & `trove-classifiers-2024.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/src/trove_classifiers/__init__.py` & `trove-classifiers-2024.3.3/src/trove_classifiers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,18 +165,14 @@
     "Framework :: Odoo :: 11.0",
     "Framework :: Odoo :: 12.0",
     "Framework :: Odoo :: 13.0",
     "Framework :: Odoo :: 14.0",
     "Framework :: Odoo :: 15.0",
     "Framework :: Odoo :: 16.0",
     "Framework :: Odoo :: 17.0",
-    "Framework :: OpenTelemetry",
-    "Framework :: OpenTelemetry :: Distros",
-    "Framework :: OpenTelemetry :: Exporters",
-    "Framework :: OpenTelemetry :: Instrumentations",
     "Framework :: Opps",
     "Framework :: Paste",
     "Framework :: Pelican",
     "Framework :: Pelican :: Plugins",
     "Framework :: Pelican :: Themes",
     "Framework :: Plone",
     "Framework :: Plone :: 3.2",
```

### Comparing `trove-classifiers-2024.3.25/src/trove_classifiers.egg-info/PKG-INFO` & `trove-classifiers-2024.3.3/src/trove_classifiers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2024.3.25
+Version: 2024.3.3
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2024.3.25/tests/lib/__init__.py` & `trove-classifiers-2024.3.3/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.3.25/tests/test_classifiers.py` & `trove-classifiers-2024.3.3/tests/test_classifiers.py`

 * *Files identical despite different names*

