# Comparing `tmp/mlflow-cratedb-2.8.1.tar.gz` & `tmp/mlflow-cratedb-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-cratedb-2.8.1.tar", last modified: Fri Nov 24 22:45:30 2023, max compression
+gzip compressed data, was "mlflow-cratedb-2.9.2.tar", last modified: Thu Jan 25 04:05:35 2024, max compression
```

## Comparing `mlflow-cratedb-2.8.1.tar` & `mlflow-cratedb-2.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.711789 mlflow-cratedb-2.8.1/
--rw-r--r--   0 amo        (501) staff       (20)     2600 2023-11-24 22:44:24.000000 mlflow-cratedb-2.8.1/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)    10175 2023-09-06 18:13:26.000000 mlflow-cratedb-2.8.1/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      230 2023-09-13 11:08:00.000000 mlflow-cratedb-2.8.1/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     7892 2023-11-24 22:45:30.711389 mlflow-cratedb-2.8.1/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     4596 2023-11-24 13:51:59.000000 mlflow-cratedb-2.8.1/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.691534 mlflow-cratedb-2.8.1/docs/
--rw-r--r--   0 amo        (501) staff       (20)     2930 2023-10-11 18:54:59.000000 mlflow-cratedb-2.8.1/docs/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)     3813 2023-10-11 18:54:59.000000 mlflow-cratedb-2.8.1/docs/container.md
--rw-r--r--   0 amo        (501) staff       (20)     1576 2023-09-13 11:08:00.000000 mlflow-cratedb-2.8.1/docs/development.md
--rw-r--r--   0 amo        (501) staff       (20)     4059 2023-10-11 18:54:59.000000 mlflow-cratedb-2.8.1/docs/handbook.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.693403 mlflow-cratedb-2.8.1/mlflow_cratedb/
--rw-r--r--   0 amo        (501) staff       (20)      170 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.700060 mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.701063 mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/ddl/
--rw-r--r--   0 amo        (501) staff       (20)     3793 2023-11-24 13:51:59.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/ddl/cratedb.sql
--rw-r--r--   0 amo        (501) staff       (20)      554 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/ddl/drop.sql
--rw-r--r--   0 amo        (501) staff       (20)     1116 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/setup_db.py
--rw-r--r--   0 amo        (501) staff       (20)      425 2023-10-10 21:46:52.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/boot.py
--rw-r--r--   0 amo        (501) staff       (20)      282 2023-09-12 12:06:41.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/cli.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.701661 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.705166 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/
--rw-r--r--   0 amo        (501) staff       (20)      793 2023-10-10 21:34:03.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      475 2023-09-12 12:32:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/db_types.py
--rw-r--r--   0 amo        (501) staff       (20)      714 2023-10-10 21:46:52.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/db_utils.py
--rw-r--r--   0 amo        (501) staff       (20)     2534 2023-11-24 13:51:59.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/model.py
--rw-r--r--   0 amo        (501) staff       (20)     1013 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/search_utils.py
--rw-r--r--   0 amo        (501) staff       (20)     1146 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/server.py
--rw-r--r--   0 amo        (501) staff       (20)      359 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/settings.py
--rw-r--r--   0 amo        (501) staff       (20)     5419 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/tracking.py
--rw-r--r--   0 amo        (501) staff       (20)      159 2023-10-10 21:46:52.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/patch/sqlalchemy.py
--rw-r--r--   0 amo        (501) staff       (20)       94 2023-09-12 10:35:18.000000 mlflow-cratedb-2.8.1/mlflow_cratedb/server.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.709324 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     7892 2023-11-24 22:45:30.000000 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     1129 2023-11-24 22:45:30.000000 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-11-24 22:45:30.000000 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)      115 2023-11-24 22:45:30.000000 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      391 2023-11-24 22:45:30.000000 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       15 2023-11-24 22:45:30.000000 mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     3442 2023-09-10 16:29:13.000000 mlflow-cratedb-2.8.1/new.md
--rw-r--r--   0 amo        (501) staff       (20)     5576 2023-11-24 22:43:47.000000 mlflow-cratedb-2.8.1/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-11-24 22:45:30.711869 mlflow-cratedb-2.8.1/setup.cfg
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-11-24 22:45:30.708786 mlflow-cratedb-2.8.1/tests/
--rw-r--r--   0 amo        (501) staff       (20)     2189 2023-10-11 18:54:59.000000 mlflow-cratedb-2.8.1/tests/test_adapter.py
--rw-r--r--   0 amo        (501) staff       (20)      667 2023-09-12 12:06:41.000000 mlflow-cratedb-2.8.1/tests/test_cli.py
--rw-r--r--   0 amo        (501) staff       (20)     7446 2023-11-24 13:51:59.000000 mlflow-cratedb-2.8.1/tests/test_examples.py
--rw-r--r--   0 amo        (501) staff       (20)      492 2023-09-12 12:32:18.000000 mlflow-cratedb-2.8.1/tests/test_mlflow.py
--rw-r--r--   0 amo        (501) staff       (20)   145027 2023-11-24 13:51:59.000000 mlflow-cratedb-2.8.1/tests/test_tracking.py
--rw-r--r--   0 amo        (501) staff       (20)     1824 2023-11-01 10:44:45.000000 mlflow-cratedb-2.8.1/tests/test_tracking_issues.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.082177 mlflow-cratedb-2.9.2/
+-rw-r--r--   0 amo        (501) staff       (20)     2744 2024-01-25 04:04:14.000000 mlflow-cratedb-2.9.2/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)    10175 2023-09-06 18:13:26.000000 mlflow-cratedb-2.9.2/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      230 2023-09-13 11:08:00.000000 mlflow-cratedb-2.9.2/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     7895 2024-01-25 04:05:35.081769 mlflow-cratedb-2.9.2/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     4596 2023-11-24 13:51:59.000000 mlflow-cratedb-2.9.2/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.064384 mlflow-cratedb-2.9.2/docs/
+-rw-r--r--   0 amo        (501) staff       (20)     2930 2023-10-11 18:54:59.000000 mlflow-cratedb-2.9.2/docs/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)     3813 2023-10-11 18:54:59.000000 mlflow-cratedb-2.9.2/docs/container.md
+-rw-r--r--   0 amo        (501) staff       (20)     1576 2023-09-13 11:08:00.000000 mlflow-cratedb-2.9.2/docs/development.md
+-rw-r--r--   0 amo        (501) staff       (20)     4059 2023-10-11 18:54:59.000000 mlflow-cratedb-2.9.2/docs/handbook.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.066837 mlflow-cratedb-2.9.2/mlflow_cratedb/
+-rw-r--r--   0 amo        (501) staff       (20)      170 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.069163 mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.070300 mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/ddl/
+-rw-r--r--   0 amo        (501) staff       (20)     3793 2023-11-24 13:51:59.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/ddl/cratedb.sql
+-rw-r--r--   0 amo        (501) staff       (20)      554 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/ddl/drop.sql
+-rw-r--r--   0 amo        (501) staff       (20)     1116 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/setup_db.py
+-rw-r--r--   0 amo        (501) staff       (20)      425 2023-10-10 21:46:52.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/boot.py
+-rw-r--r--   0 amo        (501) staff       (20)      282 2023-09-12 12:06:41.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/cli.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.071035 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.074936 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/
+-rw-r--r--   0 amo        (501) staff       (20)      793 2023-10-10 21:34:03.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      475 2023-09-12 12:32:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/db_types.py
+-rw-r--r--   0 amo        (501) staff       (20)      714 2023-10-10 21:46:52.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/db_utils.py
+-rw-r--r--   0 amo        (501) staff       (20)     2534 2023-11-24 13:51:59.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/model.py
+-rw-r--r--   0 amo        (501) staff       (20)     1013 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/search_utils.py
+-rw-r--r--   0 amo        (501) staff       (20)     1146 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/server.py
+-rw-r--r--   0 amo        (501) staff       (20)      359 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/settings.py
+-rw-r--r--   0 amo        (501) staff       (20)     5419 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/tracking.py
+-rw-r--r--   0 amo        (501) staff       (20)      159 2023-10-10 21:46:52.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/patch/sqlalchemy.py
+-rw-r--r--   0 amo        (501) staff       (20)       94 2023-09-12 10:35:18.000000 mlflow-cratedb-2.9.2/mlflow_cratedb/server.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.079723 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     7895 2024-01-25 04:05:35.000000 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     1129 2024-01-25 04:05:35.000000 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-01-25 04:05:35.000000 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)      115 2024-01-25 04:05:35.000000 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      394 2024-01-25 04:05:35.000000 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       15 2024-01-25 04:05:35.000000 mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     3442 2023-09-10 16:29:13.000000 mlflow-cratedb-2.9.2/new.md
+-rw-r--r--   0 amo        (501) staff       (20)     5529 2024-01-25 04:03:25.000000 mlflow-cratedb-2.9.2/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-01-25 04:05:35.082255 mlflow-cratedb-2.9.2/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-01-25 04:05:35.079078 mlflow-cratedb-2.9.2/tests/
+-rw-r--r--   0 amo        (501) staff       (20)     2189 2023-10-11 18:54:59.000000 mlflow-cratedb-2.9.2/tests/test_adapter.py
+-rw-r--r--   0 amo        (501) staff       (20)      667 2023-09-12 12:06:41.000000 mlflow-cratedb-2.9.2/tests/test_cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     7446 2023-11-24 13:51:59.000000 mlflow-cratedb-2.9.2/tests/test_examples.py
+-rw-r--r--   0 amo        (501) staff       (20)      492 2023-09-12 12:32:18.000000 mlflow-cratedb-2.9.2/tests/test_mlflow.py
+-rw-r--r--   0 amo        (501) staff       (20)   145027 2023-11-24 13:51:59.000000 mlflow-cratedb-2.9.2/tests/test_tracking.py
+-rw-r--r--   0 amo        (501) staff       (20)     1824 2023-11-01 10:44:45.000000 mlflow-cratedb-2.9.2/tests/test_tracking_issues.py
```

### Comparing `mlflow-cratedb-2.8.1/CHANGES.md` & `mlflow-cratedb-2.9.2/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 
 ## in progress
 
+## 2024-01-25 v2.9.2
+- Update to [MLflow 2.9.2](https://github.com/mlflow/mlflow/releases/tag/v2.9.2)
+- Update to Python 3.11 across the board
+
 ## 2023-11-24 v2.8.1
 - Update to [MLflow 2.8.1](https://github.com/mlflow/mlflow/releases/tag/v2.8.1)
 
 ## 2023-11-24 v2.8.0
 - Update to [MLflow 2.8.0](https://github.com/mlflow/mlflow/releases/tag/v2.8.0)
 
   Attention: Please note when updating from a previous version:
```

### Comparing `mlflow-cratedb-2.8.1/LICENSE` & `mlflow-cratedb-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/PKG-INFO` & `mlflow-cratedb-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-cratedb
-Version: 2.8.1
+Version: 2.9.2
 Summary: MLflow adapter for CrateDB
 Author-email: Andreas Motl <andreas.motl@crate.io>
 License: Apache License 2.0
 Project-URL: changelog, https://github.com/crate-workbench/mlflow-cratedb/blob/main/CHANGES.md
 Project-URL: documentation, https://github.com/crate-workbench/mlflow-cratedb
 Project-URL: homepage, https://github.com/crate-workbench/mlflow-cratedb
 Project-URL: repository, https://github.com/crate-workbench/mlflow-cratedb
@@ -43,33 +43,33 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crash
 Requires-Dist: crate[sqlalchemy]>=0.34
-Requires-Dist: cratedb-toolkit==0.0.2
-Requires-Dist: mlflow==2.8.1
+Requires-Dist: cratedb-toolkit==0.0.3
+Requires-Dist: mlflow==2.9.2
 Requires-Dist: sqlparse<0.5
 Provides-Extra: develop
 Requires-Dist: black<24; extra == "develop"
-Requires-Dist: mypy==1.7; extra == "develop"
+Requires-Dist: mypy==1.8.0; extra == "develop"
 Requires-Dist: poethepoet<1; extra == "develop"
-Requires-Dist: pyproject-fmt<1.6; extra == "develop"
-Requires-Dist: ruff==0.1.6; extra == "develop"
+Requires-Dist: pyproject-fmt<1.7; extra == "develop"
+Requires-Dist: ruff==0.1.14; extra == "develop"
 Requires-Dist: validate-pyproject<0.16; extra == "develop"
 Provides-Extra: examples
 Requires-Dist: pycaret[analysis,models,parallel,test,tuner]==3.2; platform_machine != "aarch64" and extra == "examples"
 Requires-Dist: salesforce-merlion<2.1; extra == "examples"
 Requires-Dist: werkzeug==2.2.3; extra == "examples"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: twine<5; extra == "release"
 Provides-Extra: test
-Requires-Dist: psutil==5.9.2; extra == "test"
+Requires-Dist: psutil==5.9.8; extra == "test"
 Requires-Dist: pytest<8; extra == "test"
 Requires-Dist: pytest-cov<5; extra == "test"
 
 # MLflow adapter for CrateDB
 
 [![Tests](https://github.com/crate-workbench/mlflow-cratedb/actions/workflows/main.yml/badge.svg)](https://github.com/crate-workbench/mlflow-cratedb/actions/workflows/main.yml)
 [![Test coverage](https://img.shields.io/codecov/c/gh/crate-workbench/mlflow-cratedb.svg)](https://codecov.io/gh/crate-workbench/mlflow-cratedb/)
```

### Comparing `mlflow-cratedb-2.8.1/README.md` & `mlflow-cratedb-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/docs/backlog.md` & `mlflow-cratedb-2.9.2/docs/backlog.md`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/docs/container.md` & `mlflow-cratedb-2.9.2/docs/container.md`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/docs/development.md` & `mlflow-cratedb-2.9.2/docs/development.md`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/docs/handbook.md` & `mlflow-cratedb-2.9.2/docs/handbook.md`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/ddl/cratedb.sql` & `mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/ddl/cratedb.sql`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/ddl/drop.sql` & `mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/ddl/drop.sql`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/adapter/setup_db.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/adapter/setup_db.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/__init__.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/db_utils.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/db_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/model.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/search_utils.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/search_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/server.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/server.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb/patch/mlflow/tracking.py` & `mlflow-cratedb-2.9.2/mlflow_cratedb/patch/mlflow/tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/PKG-INFO` & `mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-cratedb
-Version: 2.8.1
+Version: 2.9.2
 Summary: MLflow adapter for CrateDB
 Author-email: Andreas Motl <andreas.motl@crate.io>
 License: Apache License 2.0
 Project-URL: changelog, https://github.com/crate-workbench/mlflow-cratedb/blob/main/CHANGES.md
 Project-URL: documentation, https://github.com/crate-workbench/mlflow-cratedb
 Project-URL: homepage, https://github.com/crate-workbench/mlflow-cratedb
 Project-URL: repository, https://github.com/crate-workbench/mlflow-cratedb
@@ -43,33 +43,33 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crash
 Requires-Dist: crate[sqlalchemy]>=0.34
-Requires-Dist: cratedb-toolkit==0.0.2
-Requires-Dist: mlflow==2.8.1
+Requires-Dist: cratedb-toolkit==0.0.3
+Requires-Dist: mlflow==2.9.2
 Requires-Dist: sqlparse<0.5
 Provides-Extra: develop
 Requires-Dist: black<24; extra == "develop"
-Requires-Dist: mypy==1.7; extra == "develop"
+Requires-Dist: mypy==1.8.0; extra == "develop"
 Requires-Dist: poethepoet<1; extra == "develop"
-Requires-Dist: pyproject-fmt<1.6; extra == "develop"
-Requires-Dist: ruff==0.1.6; extra == "develop"
+Requires-Dist: pyproject-fmt<1.7; extra == "develop"
+Requires-Dist: ruff==0.1.14; extra == "develop"
 Requires-Dist: validate-pyproject<0.16; extra == "develop"
 Provides-Extra: examples
 Requires-Dist: pycaret[analysis,models,parallel,test,tuner]==3.2; platform_machine != "aarch64" and extra == "examples"
 Requires-Dist: salesforce-merlion<2.1; extra == "examples"
 Requires-Dist: werkzeug==2.2.3; extra == "examples"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: twine<5; extra == "release"
 Provides-Extra: test
-Requires-Dist: psutil==5.9.2; extra == "test"
+Requires-Dist: psutil==5.9.8; extra == "test"
 Requires-Dist: pytest<8; extra == "test"
 Requires-Dist: pytest-cov<5; extra == "test"
 
 # MLflow adapter for CrateDB
 
 [![Tests](https://github.com/crate-workbench/mlflow-cratedb/actions/workflows/main.yml/badge.svg)](https://github.com/crate-workbench/mlflow-cratedb/actions/workflows/main.yml)
 [![Test coverage](https://img.shields.io/codecov/c/gh/crate-workbench/mlflow-cratedb.svg)](https://codecov.io/gh/crate-workbench/mlflow-cratedb/)
```

### Comparing `mlflow-cratedb-2.8.1/mlflow_cratedb.egg-info/SOURCES.txt` & `mlflow-cratedb-2.9.2/mlflow_cratedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/new.md` & `mlflow-cratedb-2.9.2/new.md`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/pyproject.toml` & `mlflow-cratedb-2.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -74,39 +74,39 @@
 dynamic = [
   "version",
 ]
 
 dependencies = [
   "crash",
   "crate[sqlalchemy]>=0.34",
-  "cratedb-toolkit==0.0.2",
-  "mlflow==2.8.1",
+  "cratedb-toolkit==0.0.3",
+  "mlflow==2.9.2",
   "sqlparse<0.5",
 ]
 
 [project.optional-dependencies]
 develop = [
   "black<24",
-  "mypy==1.7",
+  "mypy==1.8.0",
   "poethepoet<1",
-  "pyproject-fmt<1.6",
-  "ruff==0.1.6",
+  "pyproject-fmt<1.7",
+  "ruff==0.1.14",
   "validate-pyproject<0.16",
 ]
 examples = [
   'pycaret[analysis,models,parallel,test,tuner]==3.2; platform_machine != "aarch64"',
   "salesforce-merlion<2.1",
   "werkzeug==2.2.3",
 ]
 release = [
   "build<2",
   "twine<5",
 ]
 test = [
-  "psutil==5.9.2", # This version has binary wheels for Python 3.10.
+  "psutil==5.9.8",
   "pytest<8",
   "pytest-cov<5",
 ]
 [project.scripts]
 mlflow-cratedb = "mlflow_cratedb.cli:cli"
 [project.entry-points."mlflow.app"]
 mlflow-cratedb = "mlflow_cratedb.server:app"
```

### Comparing `mlflow-cratedb-2.8.1/tests/test_adapter.py` & `mlflow-cratedb-2.9.2/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/tests/test_cli.py` & `mlflow-cratedb-2.9.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/tests/test_examples.py` & `mlflow-cratedb-2.9.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/tests/test_tracking.py` & `mlflow-cratedb-2.9.2/tests/test_tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow-cratedb-2.8.1/tests/test_tracking_issues.py` & `mlflow-cratedb-2.9.2/tests/test_tracking_issues.py`

 * *Files identical despite different names*

