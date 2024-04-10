# Comparing `tmp/pygrype-0.2.0.tar.gz` & `tmp/pygrype-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrype-0.2.0.tar", last modified: Wed Aug 16 14:22:24 2023, max compression
+gzip compressed data, was "pygrype-0.2.1.tar", last modified: Tue Apr  9 14:51:48 2024, max compression
```

## Comparing `pygrype-0.2.0.tar` & `pygrype-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.259917 pygrype-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.251917 pygrype-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-16 14:22:14.000000 pygrype-0.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-16 14:22:14.000000 pygrype-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-16 14:22:14.000000 pygrype-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-16 14:22:14.000000 pygrype-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-16 14:22:24.255917 pygrype-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-16 14:22:14.000000 pygrype-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/pygrype/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/pygrype/core/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/grype_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/pygrype/core/list/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/list/db_meta_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/pygrype/core/scan/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/cvss.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/cvss_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/distro.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/match_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/match_details_found.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/match_details_searched_by.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/scan_source.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/searched_by_distro.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/target.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/vulnerability.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/core/scan/vulnerability_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/grype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-16 14:22:14.000000 pygrype-0.2.0/pygrype/grype_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/pygrype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-16 14:22:24.000000 pygrype-0.2.0/pygrype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-16 14:22:24.000000 pygrype-0.2.0/pygrype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 14:22:24.000000 pygrype-0.2.0/pygrype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-16 14:22:24.000000 pygrype-0.2.0/pygrype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-16 14:22:14.000000 pygrype-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-16 14:22:14.000000 pygrype-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-16 14:22:24.259917 pygrype-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 14:22:24.255917 pygrype-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-16 14:22:14.000000 pygrype-0.2.0/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.658586 pygrype-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 14:51:43.000000 pygrype-0.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 14:51:43.000000 pygrype-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 14:51:43.000000 pygrype-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 14:51:43.000000 pygrype-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 14:51:48.666586 pygrype-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 14:51:43.000000 pygrype-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/pygrype/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/pygrype/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/grype_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/pygrype/core/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/list/db_meta_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/pygrype/core/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/cvss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/cvss_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match_details_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match_details_searched_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/scan_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/searched_by_distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/vulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/vulnerability_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/grype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/grype_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/pygrype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 14:51:43.000000 pygrype-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 14:51:43.000000 pygrype-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:51:48.666586 pygrype-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 14:51:43.000000 pygrype-0.2.1/test/test_version.py
```

### Comparing `pygrype-0.2.0/.github/workflows/python-package.yml` & `pygrype-0.2.1/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `pygrype-0.2.0/.github/workflows/python-publish.yml` & `pygrype-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.0/.gitignore` & `pygrype-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.0/LICENSE` & `pygrype-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.0/PKG-INFO` & `pygrype-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrype
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for Grype
 Author-email: Albert Simon <simon.albert75@gmail.com>
 License: MIT License
 Keywords: anchore,grype,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
@@ -13,18 +13,20 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dacite>=1.8.1
 
 # PyGrype
 
 ![PyPI](https://img.shields.io/pypi/v/pygrype)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pygrype)
 ![PyPI - License](https://img.shields.io/pypi/l/pygrype)
```

### Comparing `pygrype-0.2.0/README.md` & `pygrype-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.0/pygrype/grype.py` & `pygrype-0.2.1/pygrype/grype.py`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.0/pygrype/grype_db.py` & `pygrype-0.2.1/pygrype/grype_db.py`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.0/pygrype.egg-info/PKG-INFO` & `pygrype-0.2.1/pygrype.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrype
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for Grype
 Author-email: Albert Simon <simon.albert75@gmail.com>
 License: MIT License
 Keywords: anchore,grype,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
@@ -13,18 +13,20 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dacite>=1.8.1
 
 # PyGrype
 
 ![PyPI](https://img.shields.io/pypi/v/pygrype)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pygrype)
 ![PyPI - License](https://img.shields.io/pypi/l/pygrype)
```

### Comparing `pygrype-0.2.0/pygrype.egg-info/SOURCES.txt` & `pygrype-0.2.1/pygrype.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 .github/workflows/python-publish.yml
 pygrype/__init__.py
 pygrype/grype.py
 pygrype/grype_db.py
 pygrype.egg-info/PKG-INFO
 pygrype.egg-info/SOURCES.txt
 pygrype.egg-info/dependency_links.txt
+pygrype.egg-info/requires.txt
 pygrype.egg-info/top_level.txt
 pygrype/core/grype_version.py
 pygrype/core/list/db_meta_data.py
 pygrype/core/scan/artifact.py
 pygrype/core/scan/cvss.py
 pygrype/core/scan/cvss_metrics.py
 pygrype/core/scan/distro.py
```

### Comparing `pygrype-0.2.0/pyproject.toml` & `pygrype-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 [project]
 name = "pygrype"
 authors = [
     {name = "Albert Simon", email = "simon.albert75@gmail.com"}
 ]
 description = "Python wrapper for Grype"
+dependencies = [
+    "dacite>=1.8.1"
+]
 license = { text = "MIT License" }
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: IPython",
     "Intended Audience :: Developers",
@@ -23,12 +26,13 @@
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 requires-python = ">=3.7"
 keywords = ["anchore", "grype", "security"]
 dynamic = ["version"]
```

