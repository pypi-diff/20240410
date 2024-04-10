# Comparing `tmp/open-radar-data-0.1.0.tar.gz` & `tmp/open-radar-data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-radar-data-0.1.0.tar", last modified: Mon Mar 11 21:15:02 2024, max compression
+gzip compressed data, was "open-radar-data-0.1.1.tar", last modified: Wed Apr 10 14:14:18 2024, max compression
```

## Comparing `open-radar-data-0.1.0.tar` & `open-radar-data-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-11 21:14:35.000000 open-radar-data-0.1.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/make_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/open_radar_data/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/open_radar_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/open_radar_data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/open_radar_data/registry.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/open_radar_data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/open_radar_data/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-11 21:14:59.000000 open-radar-data-0.1.0/open_radar_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/open_radar_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-11 21:14:59.000000 open-radar-data-0.1.0/open_radar_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-11 21:15:02.000000 open-radar-data-0.1.0/open_radar_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 21:14:59.000000 open-radar-data-0.1.0/open_radar_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 21:14:59.000000 open-radar-data-0.1.0/open_radar_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 21:14:59.000000 open-radar-data-0.1.0/open_radar_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 21:14:39.000000 open-radar-data-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 21:15:02.837148 open-radar-data-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:14:18.285858 open-radar-data-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:14:18.281858 open-radar-data-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:14:18.281858 open-radar-data-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-10 14:14:18.285858 open-radar-data-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-10 14:13:51.000000 open-radar-data-0.1.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/make_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:14:18.281858 open-radar-data-0.1.1/open_radar_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/open_radar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/open_radar_data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/open_radar_data/registry.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:14:18.281858 open-radar-data-0.1.1/open_radar_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/open_radar_data/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 14:14:14.000000 open-radar-data-0.1.1/open_radar_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:14:18.281858 open-radar-data-0.1.1/open_radar_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-10 14:14:14.000000 open-radar-data-0.1.1/open_radar_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-10 14:14:18.000000 open-radar-data-0.1.1/open_radar_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:14:14.000000 open-radar-data-0.1.1/open_radar_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 14:14:14.000000 open-radar-data-0.1.1/open_radar_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 14:14:14.000000 open-radar-data-0.1.1/open_radar_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 14:13:55.000000 open-radar-data-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:14:18.285858 open-radar-data-0.1.1/setup.cfg
```

### Comparing `open-radar-data-0.1.0/.github/workflows/ci.yaml` & `open-radar-data-0.1.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/.github/workflows/pypi-release.yml` & `open-radar-data-0.1.1/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/.gitignore` & `open-radar-data-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/.pre-commit-config.yaml` & `open-radar-data-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/LICENSE` & `open-radar-data-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/PKG-INFO` & `open-radar-data-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-radar-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provides utility functions for accessing data repository for openradar examples/notebooks
 Author: Open Radar Team
 License: MIT License
         
         Copyright (c) 2022-2023 openradar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `open-radar-data-0.1.0/README.md` & `open-radar-data-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/open_radar_data/dataset.py` & `open-radar-data-0.1.1/open_radar_data/dataset.py`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/open_radar_data/registry.txt` & `open-radar-data-0.1.1/open_radar_data/registry.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 0080_20210730_160000_01_02.scn.gz f9c0599c323169413a938054712ea4bfb82bce8ba0f511d9e74edf605857593a
+0308.ave.gz 44c5d237923039a9d13be5b8e98a4a495f528b69e949c4efe29c967be1d931d9
+0308.pro.gz a825894d03c283d55add9793d93b14911c4ba972943b798d9633aa86ee296f9c
+0308.raw.gz a4d448a0d2d6467bdf45c756e8af991fbc97662d7ebde886542fcbe46360da1b
 2006_20220324_000000_000.scnx.gz 425b09551860400b1945891d43dcecf841fcca14530c4e70ef1a2eae08af641a
 2013051000000600dBZ.vol 48bc61eebe4c3799e03d2ce219e27f17ab721178251009b41af095ed4f61e4ee
 20220628072500_savevol_COSMO_LOOKUP_TEMP.nc 8f1785c25d1c535615b5ef5ae672ee0a07d8259ff72d396b84ec88e9fcdff63b
 71_20181220_060628.pvol.h5 5289ab5efaf5780b1d420633ceead02af329ad9ae55ef34d3759fecc108f26d5
 DWD-Vol-2_99999_20180601054047_00.h5 9879ff9e79eaebb7e1a8972fb4126c09537cdc21f6941510322658b263b9bcfc
 KATX20130717_195021_V06 10824fb0b296ae27035ee848bfc17d3c5ad53a116bd4667f09a9c5cd28f1c5a3
 KLBB20160601_150025_V06 b5b8639605a0c88be1ed1f1941333304e559fcf31f8ca3c98aac1520c9896914
```

### Comparing `open-radar-data-0.1.0/open_radar_data.egg-info/PKG-INFO` & `open-radar-data-0.1.1/open_radar_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-radar-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provides utility functions for accessing data repository for openradar examples/notebooks
 Author: Open Radar Team
 License: MIT License
         
         Copyright (c) 2022-2023 openradar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `open-radar-data-0.1.0/open_radar_data.egg-info/SOURCES.txt` & `open-radar-data-0.1.1/open_radar_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-radar-data-0.1.0/pyproject.toml` & `open-radar-data-0.1.1/pyproject.toml`

 * *Files identical despite different names*

