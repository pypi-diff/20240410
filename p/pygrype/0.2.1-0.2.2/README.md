# Comparing `tmp/pygrype-0.2.1.tar.gz` & `tmp/pygrype-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrype-0.2.1.tar", last modified: Tue Apr  9 14:51:48 2024, max compression
+gzip compressed data, was "pygrype-0.2.2.tar", last modified: Wed Apr 10 10:27:35 2024, max compression
```

## Comparing `pygrype-0.2.1.tar` & `pygrype-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.658586 pygrype-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 14:51:43.000000 pygrype-0.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 14:51:43.000000 pygrype-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 14:51:43.000000 pygrype-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 14:51:43.000000 pygrype-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 14:51:48.666586 pygrype-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 14:51:43.000000 pygrype-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/pygrype/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/pygrype/core/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/grype_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.662586 pygrype-0.2.1/pygrype/core/list/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/list/db_meta_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/pygrype/core/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/cvss.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/cvss_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/distro.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match_details_found.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/match_details_searched_by.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/scan_source.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/searched_by_distro.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/target.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/vulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/core/scan/vulnerability_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/grype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 14:51:43.000000 pygrype-0.2.1/pygrype/grype_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/pygrype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 14:51:48.000000 pygrype-0.2.1/pygrype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 14:51:43.000000 pygrype-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 14:51:43.000000 pygrype-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:51:48.666586 pygrype-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:51:48.666586 pygrype-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 14:51:43.000000 pygrype-0.2.1/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.698110 pygrype-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.690110 pygrype-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.694110 pygrype-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-10 10:27:30.000000 pygrype-0.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 10:27:30.000000 pygrype-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 10:27:30.000000 pygrype-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 10:27:30.000000 pygrype-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 10:27:35.698110 pygrype-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-10 10:27:30.000000 pygrype-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.694110 pygrype-0.2.2/pygrype/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.694110 pygrype-0.2.2/pygrype/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/grype_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.694110 pygrype-0.2.2/pygrype/core/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/list/db_meta_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.698110 pygrype-0.2.2/pygrype/core/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/cvss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/cvss_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/match_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/match_details_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/match_details_searched_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/scan_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/searched_by_distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/vulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/core/scan/vulnerability_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/grype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 10:27:30.000000 pygrype-0.2.2/pygrype/grype_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.698110 pygrype-0.2.2/pygrype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 10:27:35.000000 pygrype-0.2.2/pygrype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-10 10:27:35.000000 pygrype-0.2.2/pygrype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:27:35.000000 pygrype-0.2.2/pygrype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 10:27:35.000000 pygrype-0.2.2/pygrype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 10:27:35.000000 pygrype-0.2.2/pygrype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 10:27:30.000000 pygrype-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 10:27:30.000000 pygrype-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:27:35.698110 pygrype-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:27:35.698110 pygrype-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 10:27:30.000000 pygrype-0.2.2/test/test_version.py
```

### Comparing `pygrype-0.2.1/.github/workflows/python-package.yml` & `pygrype-0.2.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/.github/workflows/python-publish.yml` & `pygrype-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/.gitignore` & `pygrype-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/LICENSE` & `pygrype-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/PKG-INFO` & `pygrype-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrype
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for Grype
 Author-email: Albert Simon <simon.albert75@gmail.com>
 License: MIT License
 Keywords: anchore,grype,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
```

### Comparing `pygrype-0.2.1/README.md` & `pygrype-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/pygrype/grype.py` & `pygrype-0.2.2/pygrype/grype.py`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/pygrype/grype_db.py` & `pygrype-0.2.2/pygrype/grype_db.py`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/pygrype.egg-info/PKG-INFO` & `pygrype-0.2.2/pygrype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrype
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for Grype
 Author-email: Albert Simon <simon.albert75@gmail.com>
 License: MIT License
 Keywords: anchore,grype,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
```

### Comparing `pygrype-0.2.1/pygrype.egg-info/SOURCES.txt` & `pygrype-0.2.2/pygrype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygrype-0.2.1/pyproject.toml` & `pygrype-0.2.2/pyproject.toml`

 * *Files identical despite different names*

