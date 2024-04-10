# Comparing `tmp/in-silico-fate-mapping-0.1.1.tar.gz` & `tmp/in-silico-fate-mapping-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-silico-fate-mapping-0.1.1.tar", last modified: Tue Apr 18 16:13:53 2023, max compression
+gzip compressed data, was "in-silico-fate-mapping-0.1.2.tar", last modified: Wed Apr 10 17:04:59 2024, max compression
```

## Comparing `in-silico-fate-mapping-0.1.1.tar` & `in-silico-fate-mapping-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.581357 in-silico-fate-mapping-0.1.1/.github/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/.github/workflows/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2810 2022-07-19 16:25:03.000000 in-silico-fate-mapping-0.1.1/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      992 2022-07-19 16:25:03.000000 in-silico-fate-mapping-0.1.1/.gitignore
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/.napari/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4201 2022-07-19 16:25:03.000000 in-silico-fate-mapping-0.1.1/.napari/DESCRIPTION.md
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1199 2022-07-19 18:21:12.000000 in-silico-fate-mapping-0.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      761 2023-03-10 23:09:37.000000 in-silico-fate-mapping-0.1.1/CITATION.cff
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1498 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/LICENSE
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       96 2022-07-19 16:25:03.000000 in-silico-fate-mapping-0.1.1/MANIFEST.in
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6153 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4889 2023-04-10 18:23:31.000000 in-silico-fate-mapping-0.1.1/README.md
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      272 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/pyproject.toml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1824 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/setup.cfg
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.581357 in-silico-fate-mapping-0.1.1/src/
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      220 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1170 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_reader.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2927 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_divergence.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2070 2023-03-10 22:26:50.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_fate_mapping.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2556 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_io.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2103 2023-03-10 22:26:50.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_widget.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      160 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_version.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5549 2023-03-10 22:26:50.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_widget.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      388 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_writer.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/cli/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/cli/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3077 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/cli/divergence_cli.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      955 2023-03-10 22:26:50.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/conftest.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3130 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/divergence.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3675 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/fast_radius_regression.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    13398 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/fate_mapping.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      893 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/napari.yaml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      373 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/widget_utils.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-18 16:13:53.585357 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6153 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1263 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/SOURCES.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/dependency_links.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      149 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/entry_points.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      107 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/requires.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       23 2023-04-18 16:13:53.000000 in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/top_level.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      621 2023-02-02 23:57:27.000000 in-silico-fate-mapping-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.995345 in-silico-fate-mapping-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.987345 in-silico-fate-mapping-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.991345 in-silico-fate-mapping-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.991345 in-silico-fate-mapping-0.1.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-10 17:04:58.995345 in-silico-fate-mapping-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-10 17:04:58.999345 in-silico-fate-mapping-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.991345 in-silico-fate-mapping-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.995345 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.995345 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.995345 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/cli/divergence_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/fast_radius_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/widget_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:04:58.995345 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 17:04:58.000000 in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-10 17:04:46.000000 in-silico-fate-mapping-0.1.2/tox.ini
```

### Comparing `in-silico-fate-mapping-0.1.1/.github/workflows/test_and_deploy.yml` & `in-silico-fate-mapping-0.1.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/.gitignore` & `in-silico-fate-mapping-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/.napari/DESCRIPTION.md` & `in-silico-fate-mapping-0.1.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/.pre-commit-config.yaml` & `in-silico-fate-mapping-0.1.2/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # make every import absolute
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.0
     hooks:
       - id: absolufy-imports
 # sorting imports
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 # automatic upgrade to newer python versions syntax
   - repo: https://github.com/asottile/pyupgrade
     rev: v2.30.0
     hooks:
       - id: pyupgrade
```

### Comparing `in-silico-fate-mapping-0.1.1/CITATION.cff` & `in-silico-fate-mapping-0.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/LICENSE` & `in-silico-fate-mapping-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/PKG-INFO` & `in-silico-fate-mapping-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: in-silico-fate-mapping
-Version: 0.1.1
-Summary: TODO
-Home-page: https://github.com/royerlab/in-silico-fate-mapping
-Author: Jordao Bragantini
-Author-email: jordao.bragantini@czbiohub.org
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/royerlab/in-silico-fate-mapping/issues
-Project-URL: Documentation, https://github.com/royerlab/in-silico-fate-mapping#README.md
-Project-URL: Source Code, https://github.com/royerlab/in-silico-fate-mapping
-Project-URL: User Support, https://github.com/royerlab/in-silico-fate-mapping/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # in silico fate mapping
 
 [![License BSD-3](https://img.shields.io/pypi/l/in-silico-fate-mapping.svg?color=green)](https://github.com/royerlab/in-silico-fate-mapping/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/in-silico-fate-mapping.svg?color=green)](https://pypi.org/project/in-silico-fate-mapping)
 [![Python Version](https://img.shields.io/pypi/pyversions/in-silico-fate-mapping.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/in-silico-fate-mapping/workflows/tests/badge.svg)](https://github.com/royerlab/in-silico-fate-mapping/actions)
 [![codecov](https://codecov.io/gh/royerlab/in-silico-fate-mapping/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/in-silico-fate-mapping)
@@ -43,18 +14,23 @@
 
 Video example below:
 
 https://user-images.githubusercontent.com/21022743/216478216-89c1c35f-2ce4-44e8-adb8-9aeea75b5833.mp4
 
 ## Installation
 
-You can install `in-silico-fate-mapping` via [pip]:
+We suggest you create a fresh conda environment to avoid conflicts with your existing package.
+To do this, you need to:
+
+    conda create -n fatemap python=3.11
+    conda activate fatemap
 
-    pip install in-silico-fate-mapping
+And then, you can install `in-silico-fate-mapping` via [pip] and other additional useful packages:
 
+    pip install ultrack napari-ome-zarr napari[all] in-silicio-fate-mapping
 
 To install the latest development version :
 
     pip install git+https://github.com/royerlab/in-silico-fate-mapping.git
 
 
 ## IO file format
@@ -107,15 +83,15 @@
 viewer = napari.Viewer()
 viewer.window.add_dock_widget(FateMappingWidget(viewer))
 
 viewer.open(image_path, plugin="napari-ome-zarr")
 
 tracks = pd.read_csv(tracks_path)
 viewer.add_tracks(tracks[["TrackID", "t", "z", "y", "x"]])
-viewer.add_points(name="Markers")
+viewer.add_points(name="Markers", ndim=4)
 
 napari.run()
 ```
 
 ## Citing
 
 If used please cite:
```

### Comparing `in-silico-fate-mapping-0.1.1/setup.cfg` & `in-silico-fate-mapping-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_reader.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
-TRACKS_HEADER = ("TrackID", "t", "z", "y", "x")
+TRACKS_HEADER = (
+    ("track_id", "TrackID"),
+    ("t", "T"),
+    ("z", "Z"),
+    ("y", "Z"),
+    ("x", "X"),
+)
 
 
 def napari_get_reader(path):
     if isinstance(path, list):
         path = path[0]
 
     if isinstance(path, str):
         path = Path(path)
 
     if not path.name.endswith(".csv") or not path.exists():
         return None
 
     header = pd.read_csv(path, nrows=0).columns.tolist()
-    for colname in TRACKS_HEADER:
-        if colname != "z" and colname not in header:
+    for colnames in TRACKS_HEADER:
+        if all(c not in header for c in colnames) and colnames[0] != "z":
             return None
 
     return reader_function
 
 
 def read_csv(path: str):
     df = pd.read_csv(path)
 
     data = []
-    for colname in TRACKS_HEADER:
-        try:
-            data.append(df[colname])
-        except KeyError:
-            if colname != "z":
-                raise KeyError(f"{colname} not found in .csv header.")
+    for colnames in TRACKS_HEADER:
+        found = False
+        for c in colnames:
+            if c in df.columns:
+                data.append(df[c])
+                found = True
+                break
+        if not found and colnames[0] != "z":
+            raise KeyError(f"{colnames[0]} not found in .csv header.")
 
     data = np.stack(data).T
 
     props = {
         colname: df[colname]
         for colname in df.columns
         if colname not in TRACKS_HEADER
```

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_divergence.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_divergence.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_fate_mapping.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_fate_mapping.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_io.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,31 +21,35 @@
     tracks_data[n_nodes // 2 :, 0] = 2
     tracks_data[: n_nodes // 2, 1] = np.arange(n_nodes // 2)
     tracks_data[n_nodes // 2 :, 1] = np.arange(n_nodes - n_nodes // 2)
 
     return pd.DataFrame(tracks_data, columns=["TrackID", "t", "z", "y", "x"])
 
 
-def test_get_reader(tmp_path: Path, tracks: pd.DataFrame) -> None:
+@pytest.mark.parametrize("track_id_col", ["TrackID", "track_id"])
+def test_get_reader(
+    tmp_path: Path, tracks: pd.DataFrame, track_id_col: str
+) -> None:
     path = tmp_path / "good_tracks.csv"
     tracks["NodeID"] = np.arange(len(tracks)) + 1
     tracks["Labels"] = np.random.randint(2, size=len(tracks))
+    tracks.rename(columns={"TrackID": track_id_col}, inplace=True)
     tracks.to_csv(path, index=False)
 
     reader = napari_get_reader(path)
     assert callable(reader)
 
     data, kwargs, type = reader(path)[0]
     assert type == "tracks"
 
     props = kwargs["properties"]
 
     assert np.allclose(props["NodeID"], tracks["NodeID"])
     assert np.allclose(props["Labels"], tracks["Labels"])
-    assert np.allclose(data, tracks[["TrackID", "t", "z", "y", "x"]])
+    assert np.allclose(data, tracks[[track_id_col, "t", "z", "y", "x"]])
 
 
 def test_napari_read(
     make_napari_viewer: ViewerMaker,
     tmp_path: Path,
     tracks: pd.DataFrame,
 ) -> None:
```

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_tests/test_widget.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/_widget.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/_widget.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/cli/divergence_cli.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/cli/divergence_cli.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/conftest.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/conftest.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/divergence.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/divergence.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/fast_radius_regression.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/fate_mapping.py` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping/napari.yaml` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping/napari.yaml`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/PKG-INFO` & `in-silico-fate-mapping-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-silico-fate-mapping
-Version: 0.1.1
+Version: 0.1.2
 Summary: TODO
 Home-page: https://github.com/royerlab/in-silico-fate-mapping
 Author: Jordao Bragantini
 Author-email: jordao.bragantini@czbiohub.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/in-silico-fate-mapping/issues
 Project-URL: Documentation, https://github.com/royerlab/in-silico-fate-mapping#README.md
@@ -20,16 +20,29 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: zarr
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: napari
+Requires-Dist: click
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
 
 # in silico fate mapping
 
 [![License BSD-3](https://img.shields.io/pypi/l/in-silico-fate-mapping.svg?color=green)](https://github.com/royerlab/in-silico-fate-mapping/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/in-silico-fate-mapping.svg?color=green)](https://pypi.org/project/in-silico-fate-mapping)
 [![Python Version](https://img.shields.io/pypi/pyversions/in-silico-fate-mapping.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/in-silico-fate-mapping/workflows/tests/badge.svg)](https://github.com/royerlab/in-silico-fate-mapping/actions)
@@ -43,18 +56,23 @@
 
 Video example below:
 
 https://user-images.githubusercontent.com/21022743/216478216-89c1c35f-2ce4-44e8-adb8-9aeea75b5833.mp4
 
 ## Installation
 
-You can install `in-silico-fate-mapping` via [pip]:
+We suggest you create a fresh conda environment to avoid conflicts with your existing package.
+To do this, you need to:
+
+    conda create -n fatemap python=3.11
+    conda activate fatemap
 
-    pip install in-silico-fate-mapping
+And then, you can install `in-silico-fate-mapping` via [pip] and other additional useful packages:
 
+    pip install ultrack napari-ome-zarr napari[all] in-silicio-fate-mapping
 
 To install the latest development version :
 
     pip install git+https://github.com/royerlab/in-silico-fate-mapping.git
 
 
 ## IO file format
@@ -107,15 +125,15 @@
 viewer = napari.Viewer()
 viewer.window.add_dock_widget(FateMappingWidget(viewer))
 
 viewer.open(image_path, plugin="napari-ome-zarr")
 
 tracks = pd.read_csv(tracks_path)
 viewer.add_tracks(tracks[["TrackID", "t", "z", "y", "x"]])
-viewer.add_points(name="Markers")
+viewer.add_points(name="Markers", ndim=4)
 
 napari.run()
 ```
 
 ## Citing
 
 If used please cite:
```

### Comparing `in-silico-fate-mapping-0.1.1/src/in_silico_fate_mapping.egg-info/SOURCES.txt` & `in-silico-fate-mapping-0.1.2/src/in_silico_fate_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-silico-fate-mapping-0.1.1/tox.ini` & `in-silico-fate-mapping-0.1.2/tox.ini`

 * *Files identical despite different names*

