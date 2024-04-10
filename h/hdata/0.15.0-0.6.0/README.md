# Comparing `tmp/hdata-0.15.0.tar.gz` & `tmp/hdata-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdata-0.15.0.tar", max compression
+gzip compressed data, was "hdata-0.6.0.tar", max compression
```

## Comparing `hdata-0.15.0.tar` & `hdata-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0       44 2024-04-10 14:07:29.141106 hdata-0.15.0/README.md
--rw-r--r--   0        0        0      185 2024-04-10 14:07:29.141106 hdata-0.15.0/hdata/__init__.py
--rw-r--r--   0        0        0     7933 2024-04-10 14:07:29.141106 hdata-0.15.0/hdata/force_validation.py
--rw-r--r--   0        0        0     4294 2024-04-10 14:07:29.141106 hdata-0.15.0/hdata/functions.py
--rw-r--r--   0        0        0     2435 2024-04-10 14:07:29.141106 hdata-0.15.0/hdata/models.py
--rw-r--r--   0        0        0     1962 2024-04-10 14:07:29.141106 hdata-0.15.0/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-10 14:07:29.141106 hdata-0.15.0/tests/__init__.py
--rw-r--r--   0        0        0      538 2024-04-10 14:07:29.141106 hdata-0.15.0/tests/test_hdata.py
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 hdata-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-03-18 20:42:22.388270 hdata-0.6.0/README.md
+-rw-r--r--   0        0        0      128 2024-03-18 20:42:22.388270 hdata-0.6.0/hdata/__init__.py
+-rw-r--r--   0        0        0       19 2024-03-18 20:42:22.388270 hdata-0.6.0/hdata/hdata.py
+-rw-r--r--   0        0        0     2601 2024-03-18 20:42:22.388270 hdata-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-03-18 20:42:22.388270 hdata-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      538 2024-03-18 20:42:22.388270 hdata-0.6.0/tests/test_hdata.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 hdata-0.6.0/PKG-INFO
```

### Comparing `hdata-0.15.0/tests/test_hdata.py` & `hdata-0.6.0/tests/test_hdata.py`

 * *Files identical despite different names*

### Comparing `hdata-0.15.0/PKG-INFO` & `hdata-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: hdata
-Version: 0.15.0
+Version: 0.6.0
 Summary: Interacting with the HyperData API.
 Home-page: https://github.com/judahcooper/hdata
 Author: Judah Cooper
 Author-email: judah@hyperdata.network
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: black ; extra == "test"
-Requires-Dist: bump2version ; extra == "dev"
-Requires-Dist: flake8 ; extra == "test"
-Requires-Dist: flake8-docstrings ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: mkdocs ; extra == "doc"
-Requires-Dist: mkdocs-autorefs ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin ; extra == "doc"
-Requires-Dist: mkdocs-material ; extra == "doc"
-Requires-Dist: mkdocs-material-extensions
-Requires-Dist: mkdocstrings (==0.16.0) ; extra == "doc"
-Requires-Dist: mypy ; extra == "test"
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: pip ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: pyarrow
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: requests
-Requires-Dist: toml ; extra == "dev"
-Requires-Dist: tox ; extra == "dev"
-Requires-Dist: twine ; extra == "dev"
-Requires-Dist: virtualenv ; extra == "dev"
+Requires-Dist: black (>=21.5b2,<22.0) ; extra == "test"
+Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
+Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
+Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
+Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=6.1.7,<7.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material-extensions (>=1.0.1,<2.0.0)
+Requires-Dist: mkdocstrings (>=0.15.2,<0.16.0) ; extra == "doc"
+Requires-Dist: mypy (>=0.900,<0.901) ; extra == "test"
+Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra == "dev"
+Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev"
+Requires-Dist: pytest (>=6.2.4,<7.0.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=2.12.0,<3.0.0) ; extra == "test"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
+Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev"
+Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
+Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # hdata
 
 Interacting with the HyperData API
```

