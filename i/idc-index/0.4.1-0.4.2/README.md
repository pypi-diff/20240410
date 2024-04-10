# Comparing `tmp/idc_index-0.4.1.tar.gz` & `tmp/idc_index-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  9 14:00:47 2024, max compression
+gzip compressed data, last modified: Wed Apr 10 02:39:09 2024, max compression
```

## Comparing `idc_index-0.4.1.tar` & `idc_index-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      125 2024-04-09 14:00:47.000000 idc_index-0.4.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-09 14:00:47.000000 idc_index-0.4.1/.gitattributes
--rw-r--r--   0        0        0     2357 2024-04-09 14:00:47.000000 idc_index-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-09 14:00:47.000000 idc_index-0.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-04-09 14:00:47.000000 idc_index-0.4.1/noxfile.py
--rw-r--r--   0        0        0     2394 2024-04-09 14:00:47.000000 idc_index-0.4.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-09 14:00:47.000000 idc_index-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-09 14:00:47.000000 idc_index-0.4.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-04-09 14:00:47.000000 idc_index-0.4.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1581 2024-04-09 14:00:47.000000 idc_index-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-04-09 14:00:47.000000 idc_index-0.4.1/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-04-09 14:00:47.000000 idc_index-0.4.1/docs/conf.py
--rw-r--r--   0        0        0      196 2024-04-09 14:00:47.000000 idc_index-0.4.1/docs/index.md
--rw-r--r--   0        0        0      263 2024-04-09 14:00:47.000000 idc_index-0.4.1/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-04-09 14:00:47.000000 idc_index-0.4.1/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-04-09 14:00:47.000000 idc_index-0.4.1/idc_index/_version.pyi
--rw-r--r--   0        0        0    25055 2024-04-09 14:00:47.000000 idc_index-0.4.1/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-04-09 14:00:47.000000 idc_index-0.4.1/idc_index/py.typed
--rw-r--r--   0        0        0     1383 2024-04-09 14:00:47.000000 idc_index-0.4.1/queries/idc_index.sql
--rw-r--r--   0        0        0        0 2024-04-09 14:00:47.000000 idc_index-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     3595 2024-04-09 14:00:47.000000 idc_index-0.4.1/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-04-09 14:00:47.000000 idc_index-0.4.1/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2024-04-09 14:00:47.000000 idc_index-0.4.1/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-04-09 14:00:47.000000 idc_index-0.4.1/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-04-09 14:00:47.000000 idc_index-0.4.1/.gitignore
--rw-r--r--   0        0        0     1077 2024-04-09 14:00:47.000000 idc_index-0.4.1/LICENSE
--rw-r--r--   0        0        0     4290 2024-04-09 14:00:47.000000 idc_index-0.4.1/README.md
--rw-r--r--   0        0        0     6146 2024-04-09 14:00:47.000000 idc_index-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7569 2024-04-09 14:00:47.000000 idc_index-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-10 02:39:09.000000 idc_index-0.4.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-10 02:39:09.000000 idc_index-0.4.2/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-04-10 02:39:09.000000 idc_index-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-10 02:39:09.000000 idc_index-0.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-04-10 02:39:09.000000 idc_index-0.4.2/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1581 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-04-10 02:39:09.000000 idc_index-0.4.2/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-04-10 02:39:09.000000 idc_index-0.4.2/docs/index.md
+-rw-r--r--   0        0        0      263 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/_version.pyi
+-rw-r--r--   0        0        0    25026 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/py.typed
+-rw-r--r--   0        0        0     1383 2024-04-10 02:39:09.000000 idc_index-0.4.2/queries/idc_index.sql
+-rw-r--r--   0        0        0        0 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     3595 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      437 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-04-10 02:39:09.000000 idc_index-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1077 2024-04-10 02:39:09.000000 idc_index-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4290 2024-04-10 02:39:09.000000 idc_index-0.4.2/README.md
+-rw-r--r--   0        0        0     6159 2024-04-10 02:39:09.000000 idc_index-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7592 2024-04-10 02:39:09.000000 idc_index-0.4.2/PKG-INFO
```

### Comparing `idc_index-0.4.1/.pre-commit-config.yaml` & `idc_index-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/noxfile.py` & `idc_index-0.4.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/.github/CONTRIBUTING.md` & `idc_index-0.4.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/.github/matchers/pylint.json` & `idc_index-0.4.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/.github/workflows/cd.yml` & `idc_index-0.4.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/.github/workflows/ci.yml` & `idc_index-0.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/docs/conf.py` & `idc_index-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/idc_index/index.py` & `idc_index-0.4.2/idc_index/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 aws_endpoint_url = "https://s3.amazonaws.com"
 gcp_endpoint_url = "https://storage.googleapis.com"
 
 
 class IDCClient:
     def __init__(self):
-        file_path = idc_index_data.IDC_INDEX_CSV_ARCHIVE_FILEPATH
+        file_path = idc_index_data.IDC_INDEX_PARQUET_FILEPATH
 
         # Read index file
         logger.debug(f"Reading index file v{idc_index_data.__version__}")
-        self.index = pd.read_csv(file_path, dtype=str, encoding="utf-8")
+        self.index = pd.read_parquet(file_path)
         self.index = self.index.astype(str).replace("nan", "")
         self.index["series_size_MB"] = self.index["series_size_MB"].astype(float)
         self.collection_summary = self.index.groupby("collection_id").agg(
             {"Modality": pd.Series.unique, "series_size_MB": "sum"}
         )
 
         # Lookup s5cmd
```

### Comparing `idc_index-0.4.1/queries/idc_index.sql` & `idc_index-0.4.2/queries/idc_index.sql`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/tests/idcindex.py` & `idc_index-0.4.2/tests/idcindex.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/.gitignore` & `idc_index-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/LICENSE` & `idc_index-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/README.md` & `idc_index-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.1/pyproject.toml` & `idc_index-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,18 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   'duckdb>=0.10.0',
-  "idc-index-data==17.0.0",
+  "idc-index-data==17.0.2",
   "pandas<2.2",
   "psutil",
+  "pyarrow",
   "s5cmd",
 ]
 
 [project.optional-dependencies]
 test = [
   "importlib_metadata>=2.0; python_version<'3.10'",
   "pytest >=6",
```

### Comparing `idc_index-0.4.1/PKG-INFO` & `idc_index-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -42,17 +42,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: duckdb>=0.10.0
-Requires-Dist: idc-index-data==17.0.0
+Requires-Dist: idc-index-data==17.0.2
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
+Requires-Dist: pyarrow
 Requires-Dist: s5cmd
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
```

