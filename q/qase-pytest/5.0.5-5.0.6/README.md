# Comparing `tmp/qase-pytest-5.0.5.tar.gz` & `tmp/qase-pytest-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-pytest-5.0.5.tar", last modified: Wed Mar 13 09:09:43 2024, max compression
+gzip compressed data, was "qase-pytest-5.0.6.tar", last modified: Wed Apr 10 14:45:12 2024, max compression
```

## Comparing `qase-pytest-5.0.5.tar` & `qase-pytest-5.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.408844 qase-pytest-5.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/CONFIGURATION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-13 09:09:43.408844 qase-pytest-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/UPGRADE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.404844 qase-pytest-5.0.5/example/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/example/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-13 09:09:43.408844 qase-pytest-5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.404844 qase-pytest-5.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.408844 qase-pytest-5.0.5/src/qase_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 09:09:43.000000 qase-pytest-5.0.5/src/qase_pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.404844 qase-pytest-5.0.5/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.408844 qase-pytest-5.0.5/src/qaseio/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/src/qaseio/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/src/qaseio/pytest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/src/qaseio/pytest/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/src/qaseio/pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:43.408844 qase-pytest-5.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-13 09:09:40.000000 qase-pytest-5.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/CONFIGURATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/UPGRADE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/example/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.857262 qase-pytest-5.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/src/qase_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.857262 qase-pytest-5.0.6/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/src/qaseio/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tox.ini
```

### Comparing `qase-pytest-5.0.5/.coveragerc` & `qase-pytest-5.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/.gitignore` & `qase-pytest-5.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/.pre-commit-config.yaml` & `qase-pytest-5.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/CONFIGURATION.md` & `qase-pytest-5.0.6/CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/LICENSE.txt` & `qase-pytest-5.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/PKG-INFO` & `qase-pytest-5.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.5
+Version: 5.0.6
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-pytest-5.0.5/README.md` & `qase-pytest-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/UPGRADE.md` & `qase-pytest-5.0.6/UPGRADE.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/pyproject.toml` & `qase-pytest-5.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [build-system]
-requires = ["setuptools>=69", "wheel"]
+requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-pytest"
-version = "5.0.5"
+version = "5.0.6"
 description = "Qase Pytest Plugin for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Pytest",
     "Programming Language :: Python",
 ]
 urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-pytest"}
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 dependencies = [
-    "qase-python-commons>=2.0.9,<2.1.0",
-    "pytest>=8.0.0",
-    "filelock~=3.13.1",
+    "qase-python-commons>=2.0.11,<2.1.0",
+    "pytest>=7.4.4",
+    "filelock~=3.12.2",
     "more_itertools",
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-minversion = 3.8
-envlist = py{38,39,310,311}
+minversion = 3.7
+envlist = py{37,38,39,310,311}
 
 [testenv]
 deps =
     pytest
     pytest-cov
 passenv =
     HOME
```

### Comparing `qase-pytest-5.0.5/setup.cfg` & `qase-pytest-5.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/setup.py` & `qase-pytest-5.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/src/qase_pytest.egg-info/PKG-INFO` & `qase-pytest-5.0.6/src/qase_pytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.5
+Version: 5.0.6
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-pytest-5.0.5/src/qase_pytest.egg-info/SOURCES.txt` & `qase-pytest-5.0.6/src/qase_pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/src/qaseio/pytest/__init__.py` & `qase-pytest-5.0.6/src/qaseio/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/src/qaseio/pytest/conftest.py` & `qase-pytest-5.0.6/src/qaseio/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/src/qaseio/pytest/options.py` & `qase-pytest-5.0.6/src/qaseio/pytest/options.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.5/src/qaseio/pytest/plugin.py` & `qase-pytest-5.0.6/src/qaseio/pytest/plugin.py`

 * *Files identical despite different names*

