# Comparing `tmp/segmentation_skeleton_metrics-4.1.1.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.1.1.tar", last modified: Tue Apr  9 21:41:13 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.2.tar", last modified: Tue Apr  9 23:01:43 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.1.1.tar` & `segmentation_skeleton_metrics-4.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.166676 segmentation_skeleton_metrics-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.130677 segmentation_skeleton_metrics-4.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 21:41:13.166676 segmentation_skeleton_metrics-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.138677 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.150677 segmentation_skeleton_metrics-4.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:41:13.166676 segmentation_skeleton_metrics-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/merge_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    28098 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.267871 segmentation_skeleton_metrics-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.235872 segmentation_skeleton_metrics-4.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.239872 segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.239872 segmentation_skeleton_metrics-4.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 23:01:43.267871 segmentation_skeleton_metrics-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.239872 segmentation_skeleton_metrics-4.1.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.239872 segmentation_skeleton_metrics-4.1.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.239872 segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.251872 segmentation_skeleton_metrics-4.1.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.263872 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:01:43.267871 segmentation_skeleton_metrics-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.239872 segmentation_skeleton_metrics-4.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.267871 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/merge_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28403 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.267871 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 23:01:43.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-09 23:01:43.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:01:43.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 23:01:43.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 23:01:43.000000 segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:01:43.267871 segmentation_skeleton_metrics-4.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 23:01:33.000000 segmentation_skeleton_metrics-4.1.2/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.2/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.2/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/.gitignore` & `segmentation_skeleton_metrics-4.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/LICENSE` & `segmentation_skeleton_metrics-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/PKG-INFO` & `segmentation_skeleton_metrics-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.1
+Version: 4.1.2
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.1/README.md` & `segmentation_skeleton_metrics-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/pyproject.toml` & `segmentation_skeleton_metrics-4.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.2/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.2/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.2/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.2/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.2/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.2/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.2/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.2/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/merge_detection.py` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/merge_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,21 +99,21 @@
         Distance between xyz coordinates in "xyz_pair".
 
     """
     min_dist = np.inf
     xyz_pair = list()
     for i in merged_1:
         for j in merged_2:
-            xyz_1 = graph_1.nodes[i]["xyz"]
-            xyz_2 = graph_2.nodes[j]["xyz"]
-            if utils.dist(xyz_1, xyz_2) < min_dist:
-                min_dist = utils.dist(xyz_1, xyz_2)
-                xyz_pair = [xyz_1, xyz_2]
+            xyz_i = graph_1.nodes[i]["xyz"]
+            xyz_j = graph_2.nodes[j]["xyz"]
+            if utils.dist(xyz_i, xyz_j) < min_dist:
+                min_dist = utils.dist(xyz_i, xyz_j)
+                xyz_pair = [xyz_i, xyz_j]
                 if min_dist < dist_threshold:
-                    return xyz_pair, min_dist
+                    return merge_id, xyz_pair, min_dist
     return merge_id, xyz_pair, min_dist
 
 
 def label_intersections(get_projection, xyz_list, xyz_to_id, dist_threshold):
     """
     Projects coordinates in "xyz_list" onto ground truth graphs, then stores
     the correspond label in "hit_ids" if the projection distance is less than
```

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     merge_detection,
     split_detection,
     swc_utils,
     utils,
 )
 from segmentation_skeleton_metrics.swc_utils import save, to_graph
 
-CLOSE_DIST_THRESHOLD = 5
+CLOSE_DIST_THRESHOLD = 3.5
 INTERSECTION_THRESHOLD = 16
-MERGE_DIST_THRESHOLD = 30
+MERGE_DIST_THRESHOLD = 25
 
 
 class SkeletonMetric:
     """
     Class that evaluates the quality of a predicted segmentation by comparing
     the ground truth skeletons to the predicted segmentation mask. The
     accuracy is then quantified by detecting splits and merges, then computing
@@ -162,16 +162,16 @@
         Returns
         -------
         None
 
         """
         graphs = dict()
         for path in paths:
-            swc_id = os.path.basename(path).replace(".swc", "")
-            graphs[swc_id] = to_graph(path, anisotropy=anisotropy)
+            id = utils.get_id(path)
+            graphs[id] = to_graph(path, anisotropy=anisotropy)
         return graphs
 
     def init_labeled_graphs(self):
         """
         Initializes "self.labeled_graphs" by copying each graph in
         "self.graphs", then labels each node with the label in
         "self.label_mask" that coincides with it.
@@ -184,59 +184,59 @@
         -------
         None
 
         """
         print("Labelling Graphs...")
         t0 = time()
         self.labeled_graphs = dict()
-        self.id_to_label_nodes = dict()  # {graph_id: {label: nodes}}
-        for cnt, (graph_id, graph) in enumerate(self.graphs.items()):
+        self.id_to_label_nodes = dict()  # {id: {label: nodes}}
+        for cnt, (id, graph) in enumerate(self.graphs.items()):
             utils.progress_bar(cnt + 1, len(self.graphs))
             labeled_graph, id_to_label_nodes = self.label_graph(graph)
-            self.labeled_graphs[graph_id] = labeled_graph
-            self.id_to_label_nodes[graph_id] = id_to_label_nodes
+            self.labeled_graphs[id] = labeled_graph
+            self.id_to_label_nodes[id] = id_to_label_nodes
 
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
 
-    def label_graph(self, target_graph):
+    def label_graph(self, graph):
         """
-        Iterates over nodes in "target_graph" and stores the label in the
+        Iterates over nodes in "graph" and stores the label in the
         predicted segmentation mask (i.e. "self.label_mask") which coincides
         with each node as a node-level attribute called "label".
 
         Parameters
         ----------
-        target_graph : networkx.Graph
+        graph : networkx.Graph
             Graph that represents a neuron from the ground truth.
 
         Returns
         -------
-        target_graph : networkx.Graph
+        graph : networkx.Graph
             Updated graph with node-level attributes called "label".
 
         """
-        labeled_target_graph = nx.Graph(target_graph)
+        labeled_graph = nx.Graph(graph)
         id_to_label_nodes = dict()
         with ThreadPoolExecutor() as executor:
             # Assign threads
             threads = []
-            for i in labeled_target_graph.nodes:
-                img_coord = gutils.get_coord(labeled_target_graph, i)
+            for i in labeled_graph.nodes:
+                img_coord = gutils.get_coord(labeled_graph, i)
                 threads.append(executor.submit(self.get_label, img_coord, i))
 
             # Store results
             for thread in as_completed(threads):
                 i, label = thread.result()
-                labeled_target_graph.nodes[i].update({"label": label})
+                labeled_graph.nodes[i].update({"label": label})
                 if label in id_to_label_nodes.keys():
                     id_to_label_nodes[label].add(i)
                 else:
                     id_to_label_nodes[label] = set([i])
-        return labeled_target_graph, id_to_label_nodes
+        return labeled_graph, id_to_label_nodes
 
     def get_label(self, img_coord, return_node=False):
         """
         Gets label of voxel at "img_coord".
 
         Parameters
         ----------
@@ -281,14 +281,28 @@
         # Read image label
         if type(self.label_mask) == ts.TensorStore:
             return int(self.label_mask[coord].read().result())
         else:
             return self.label_mask[coord]
 
     def equivalent_label(self, label):
+        """
+        Gets the equivalence class label corresponding to "label".
+
+        Parameters
+        ----------
+        label : int
+            Label to be checked.
+
+        Returns
+        -------
+        label
+            Equivalence class label.
+
+        """
         if self.equiv_labels_map:
             if label in self.equiv_labels_map.keys():
                 return self.equiv_labels_map[label]
             else:
                 return 0
         else:
             return label
@@ -314,37 +328,66 @@
         if self.valid_labels:
             return 0 if label not in self.valid_labels.keys() else label
         else:
             return label
 
     def init_xyz_to_id_node(self):
         self.xyz_to_id_node = dict()
-        for graph_id, graph in self.graphs.items():
+        for id, graph in self.graphs.items():
             for i in graph.nodes:
                 xyz = tuple(graph.nodes[i]["xyz"])
                 if xyz in self.xyz_to_id_node.keys():
-                    self.xyz_to_id_node[xyz][graph_id] = i
+                    self.xyz_to_id_node[xyz][id] = i
                 else:
-                    self.xyz_to_id_node[xyz] = {graph_id: i}
+                    self.xyz_to_id_node[xyz] = {id: i}
 
     def get_pred_coords(self, label):
         if label in self.valid_labels.keys():
             return self.valid_labels[label]
         else:
             return []
 
     # -- Final Constructor Routines --
     def init_kdtree(self):
+        """
+        Builds a KD-Tree from the xyz coordinates from all nodes across all
+        graphs contained in "self.graphs".
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+
+        """
         xyz_list = []
         for _, graph in self.graphs.items():
             for i in graph.nodes:
                 xyz_list.append(graph.nodes[i]["xyz"])
         self.graphs_kdtree = KDTree(xyz_list)
 
     def get_projection(self, xyz):
+        """
+        Gets the xyz coordinates of the nearest neighbor of "xyz".
+
+        Parameters
+        ----------
+        xyz : tuple
+            xyz coordinate to be queried.
+
+        Returns
+        -------
+        tuple
+            xyz coordinate of the nearest neighbor of "xyz".
+        d : float
+            Projection distance.
+
+        """
         d, idx = self.graphs_kdtree.query(xyz, k=1)
         return tuple(self.graphs_kdtree.data[idx]), d
 
     def init_black_holes(self, black_holes):
         if black_holes:
             black_holes_xyz = [bh_dict["xyz"] for bh_dict in black_holes]
             black_holes_id = [bh_dict["swc_id"] for bh_dict in black_holes]
@@ -390,53 +433,53 @@
 
         # Compute metrics
         full_results, avg_results = self.compile_results()
         return full_results, avg_results
 
     def get_all_labels(self):
         labels = set()
-        for graph_id in self.graphs.keys():
-            labels = labels.union(self.get_labels(graph_id))
+        for id in self.graphs.keys():
+            labels = labels.union(self.get_labels(id))
         labels.discard(0)
         return labels
 
-    def get_labels(self, graph_id):
+    def get_labels(self, id):
         """
         Gets the predicted label ids that intersect with the target graph
-        corresponding to "graph_id".
+        corresponding to "id".
 
         Parameters
         ----------
-        graph_id : str
+        id : str
 
         """
-        return set(self.id_to_label_nodes[graph_id].keys())
+        return set(self.id_to_label_nodes[id].keys())
 
-    def zero_nodes(self, graph_id, label):
+    def zero_nodes(self, id, label):
         """
-        Zeros out nodes in "self.labeled_target_graph[graph_id" in the sense
-        the label of nodes with "label" is updated to zero.
+        Zeros out nodes in "self.labeled_graph[id]" in the sense that
+        nodes with "label" are updated to zero.
 
         Parameters
         ----------
-        graph_id : str
+        id : str
             ID of ground truth graph to be updated.
         label : int
             Label that identifies which nodes to have their label updated to
             zero.
 
         Returns
         -------
         None
 
         """
-        if label in self.id_to_label_nodes[graph_id].keys():
-            for i in self.id_to_label_nodes[graph_id][label]:
-                self.labeled_graphs[graph_id].nodes[i]["label"] = 0
-            self.id_to_label_nodes[graph_id][label] = set()
+        if label in self.id_to_label_nodes[id].keys():
+            for i in self.id_to_label_nodes[id][label]:
+                self.labeled_graphs[id].nodes[i]["label"] = 0
+            self.id_to_label_nodes[id][label] = set()
 
     def detect_splits(self):
         """
         Detects splits in the predicted segmentation, then deletes node and
         edges in "self.labeled_graphs" that correspond to a split.
 
         Parameters
@@ -445,26 +488,24 @@
 
         Returns
         -------
         None
 
         """
         t0 = time()
-        for cnt, (graph_id, target_graph) in enumerate(self.graphs.items()):
+        for cnt, (id, graph) in enumerate(self.graphs.items()):
             # Detection
             utils.progress_bar(cnt + 1, len(self.graphs))
-            labeled_graph = self.labeled_graphs[graph_id]
-            labeled_graph = split_detection.run(target_graph, labeled_graph)
+            labeled_graph = self.labeled_graphs[id]
+            labeled_graph = split_detection.run(graph, labeled_graph)
 
             # Update predicted graph
             labeled_graph = gutils.delete_nodes(labeled_graph, 0)
-            labeled_graph = gutils.delete_nodes(labeled_graph, -1)
-            id_to_label_nodes = gutils.store_labels(labeled_graph)
-            self.labeled_graphs[graph_id] = labeled_graph
-            self.id_to_label_nodes[graph_id] = id_to_label_nodes
+            self.labeled_graphs[id] = gutils.delete_nodes(labeled_graph, -1)
+            self.id_to_label_nodes[id] = gutils.store_labels(labeled_graph)
 
         # Report runtime
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
 
     def quantify_splits(self):
         """
@@ -479,22 +520,21 @@
         -------
         None
 
         """
         self.split_cnts = dict()
         self.omit_cnts = dict()
         self.omit_percents = dict()
-        for graph_id in self.graphs.keys():
-            n_splits = gutils.count_splits(self.labeled_graphs[graph_id])
-            n_pred_edges = self.labeled_graphs[graph_id].number_of_edges()
-            n_target_edges = self.graphs[graph_id].number_of_edges()
-
-            self.split_cnts[graph_id] = n_splits
-            self.omit_cnts[graph_id] = n_target_edges - n_pred_edges
-            self.omit_percents[graph_id] = 1 - n_pred_edges / n_target_edges
+        for id in self.graphs.keys():
+            n_pred_edges = self.labeled_graphs[id].number_of_edges()
+            n_target_edges = self.graphs[id].number_of_edges()
+
+            self.split_cnts[id] = gutils.count_splits(self.labeled_graphs[id])
+            self.omit_cnts[id] = n_target_edges - n_pred_edges
+            self.omit_percents[id] = 1 - n_pred_edges / n_target_edges
 
     def detect_merges(self):
         """
         Detects merges in the predicted segmentation, then deletes node and
         edges in "self.labeled_graphs" that correspond to a merge.
 
         Parameters
@@ -534,14 +574,15 @@
             cnt = 1
             chunk_size = int(len(processes) * 0.02)
             detected_merges = set()
             for i, process in enumerate(as_completed(processes)):
                 # Check site
                 merge_id, site, d = process.result()
                 if d < MERGE_DIST_THRESHOLD:
+                    print(merge_id, d)
                     detected_merges.add(merge_id)
                     if self.save:
                         self.save_swc(site[0], site[1], "merge")
 
                 # Report process
                 if i > cnt * chunk_size:
                     utils.progress_bar(i + 1, len(processes))
@@ -565,22 +606,35 @@
                 self.get_projection,
                 self.get_pred_coords(label),
                 self.xyz_to_id_node,
                 CLOSE_DIST_THRESHOLD,
             )
 
             # Remove spurious intersections
-            for graph_id in self.graphs.keys():
-                if graph_id in hit_ids.keys():
-                    if len(hit_ids[graph_id]) < INTERSECTION_THRESHOLD:
-                        self.zero_nodes(graph_id, label)
-                elif label in self.id_to_label_nodes[graph_id]:
-                    self.zero_nodes(graph_id, label)
+            for id in self.graphs.keys():
+                if id in hit_ids.keys():
+                    if len(hit_ids[id]) < INTERSECTION_THRESHOLD:
+                        self.zero_nodes(id, label)
 
     def detect_potential_merges(self):
+        """
+        Detects merges between ground truth graphs which are considered to be
+        potential merge sites.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        set
+            Set of tuples containing a tuple of graph ids and common label
+            between the graphs.
+
+        """
         return merge_detection.detect_potentials(
             self.labeled_graphs, self.get_labels
         )
 
     def near_bdd(self, xyz):
         """
         Determines whether "xyz" is near the boundary of the image.
@@ -626,122 +680,122 @@
 
     def init_tracker(self):
         tracker = dict()
         for label in self.labeled_graphs.keys():
             tracker[label] = set()
         return tracker
 
-    def process_merge(self, graph_id, label):
+    def process_merge(self, id, label):
         """
-        Once a merge has been detected that corresponds to "graph_id", every
-        node in "self.labeled_graph[graph_id]" with that "label" is
+        Once a merge has been detected that corresponds to "id", every
+        node in "self.labeled_graph[id]" with that "label" is
         deleted.
 
         Parameters
         ----------
-        graph_id : str
+        id : str
             Key associated with the labeled_graph to be searched.
         label : int
             Label in prediction that is assocatied with a merge.
 
         Returns
         -------
         None
 
         """
-        graph = self.labeled_graphs[graph_id].copy()
+        graph = self.labeled_graphs[id].copy()
         graph, merged_cnt = gutils.delete_nodes(graph, label, return_cnt=True)
-        self.labeled_graphs[graph_id] = graph
-        self.merged_cnts[graph_id] += merged_cnt
+        self.labeled_graphs[id] = graph
+        self.merged_cnts[id] += merged_cnt
 
     def quantify_merges(self):
         """
-        Computes the percentage of merged edges for each labeled_target_graph.
+        Computes the percentage of merged edges for each labeled_graph.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
         self.merged_percents = dict()
-        for graph_id in self.graphs.keys():
-            n_edges = self.graphs[graph_id].number_of_edges()
-            percent = self.merged_cnts[graph_id] / n_edges
-            self.merged_percents[graph_id] = percent
+        for id in self.graphs.keys():
+            n_edges = self.graphs[id].number_of_edges()
+            percent = self.merged_cnts[id] / n_edges
+            self.merged_percents[id] = percent
 
     def compile_results(self):
         """
         Compiles a dictionary containing the metrics computed by this module.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         full_results : dict
-            Dictionary where the keys are graph_ids and the values are the
+            Dictionary where the keys are ids and the values are the
             result of computing each metric for the corresponding graphs.
         avg_result : dict
             Dictionary where the keys are names of metrics computed by this
-            module and values are the averaged result over all graph_ids.
+            module and values are the averaged result over all ids.
 
         """
         # Compute remaining metrics
         self.compute_edge_accuracy()
         self.compute_erl()
 
         # Summarize results
-        graph_ids, results = self.generate_full_results()
+        ids, results = self.generate_full_results()
         avg_results = self.generate_avg_results()
 
         # Reformat full results
         full_results = dict()
-        for i, graph_id in enumerate(graph_ids):
-            full_results[graph_id] = dict(
-                [(key, results[key][i]) for key in results.keys()]
+        for i, id in enumerate(ids):
+            full_results[id] = dict(
+            [(key, results[key][i]) for key in results.keys()]
             )
 
         return full_results, avg_results
 
     def generate_full_results(self):
         """
         Generates a report by creating a list of the results for each metric.
         Each item in this list corresponds to a graph in labeled_graphs and
-        this list is ordered with respect to "graph_ids".
+        this list is ordered with respect to "ids".
 
         Parameters
         ----------
         None
 
         Results
         -------
-        graph_ids : list[str]
+        grids : list[str]
             Specifies the ordering of results for each value in "stats".
         stats : dict
             Dictionary where the keys are metrics and values are the result of
             computing that metric for each graph in labeled_graphs.
 
         """
-        graph_ids = list(self.labeled_graphs.keys())
-        graph_ids.sort()
+        ids = list(self.labeled_graphs.keys())
+        ids.sort()
         stats = {
-            "# splits": generate_result(graph_ids, self.split_cnts),
-            "# merges": generate_result(graph_ids, self.merge_cnts),
-            "% omit": generate_result(graph_ids, self.omit_percents),
-            "% merged": generate_result(graph_ids, self.merged_percents),
-            "edge accuracy": generate_result(graph_ids, self.edge_accuracy),
-            "erl": generate_result(graph_ids, self.erl),
-            "normalized erl": generate_result(graph_ids, self.normalized_erl),
+            "# splits": generate_result(ids, self.split_cnts),
+            "# merges": generate_result(ids, self.merge_cnts),
+            "% omit": generate_result(ids, self.omit_percents),
+            "% merged": generate_result(ids, self.merged_percents),
+            "edge accuracy": generate_result(ids, self.edge_accuracy),
+            "erl": generate_result(ids, self.erl),
+            "normalized erl": generate_result(ids, self.normalized_erl),
         }
-        return graph_ids, stats
+        return ids, stats
 
     def generate_avg_results(self):
         avg_stats = {
             "# splits": self.avg_result(self.split_cnts),
             "# merges": self.avg_result(self.merge_cnts) / 2,
             "% omit": self.avg_result(self.omit_percents),
             "% merged": self.avg_result(self.merged_percents),
@@ -750,72 +804,70 @@
             "normalized erl": self.avg_result(self.normalized_erl),
         }
         return avg_stats
 
     def avg_result(self, stats):
         result = []
         wgts = []
-        for graph_id, wgt in self.wgts.items():
-            if self.omit_percents[graph_id] < 1:
-                result.append(stats[graph_id])
+        for id, wgt in self.wgts.items():
+            if self.omit_percents[id] < 1:
+                result.append(stats[id])
                 wgts.append(wgt)
         return np.average(result, weights=wgts)
 
     def compute_edge_accuracy(self):
         """
-        Computes the edge accuracy of each labeled_target_graph.
+        Computes the edge accuracy of each self.labeled_graph.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
         self.edge_accuracy = dict()
-        for graph_id in self.graphs.keys():
-            omit_percent = self.omit_percents[graph_id]
-            merged_percent = self.merged_percents[graph_id]
-            self.edge_accuracy[graph_id] = 1 - omit_percent - merged_percent
+        for id in self.graphs.keys():
+            omit_percent = self.omit_percents[id]
+            merged_percent = self.merged_percents[id]
+            self.edge_accuracy[id] = 1 - omit_percent - merged_percent
 
     def compute_erl(self):
         """
-        Computes the expected run length (ERL) of each labeled_target_graph.
+        Computes the expected run length (ERL) of each labeled_graph.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
         self.erl = dict()
         self.normalized_erl = dict()
         self.wgts = dict()
         total_path_length = 0
-        for graph_id in self.graphs.keys():
-            labeled_target_graph = self.labeled_graphs[graph_id]
-            target_graph = self.graphs[graph_id]
-
-            path_length = gutils.compute_path_length(target_graph)
-            run_lengths = gutils.compute_run_lengths(labeled_target_graph)
+        for id in self.graphs.keys():
+            labeled_graph = self.labeled_graphs[id]
+            path_length = gutils.compute_path_length(self.graphs[id])
+            run_lengths = gutils.compute_run_lengths(labeled_graph)
             wgt = run_lengths / max(np.sum(run_lengths), 1)
 
-            self.erl[graph_id] = np.sum(wgt * run_lengths)
-            self.normalized_erl[graph_id] = self.erl[graph_id] / path_length
+            self.erl[id] = np.sum(wgt * run_lengths)
+            self.normalized_erl[id] = self.erl[id] / path_length
 
-            self.wgts[graph_id] = path_length
+            self.wgts[id] = path_length
             total_path_length += path_length
 
-        for graph_id in self.graphs.keys():
-            self.wgts[graph_id] = self.wgts[graph_id] / total_path_length
+        for id in self.graphs.keys():
+            self.wgts[id] = self.wgts[id] / total_path_length
 
     def list_metrics(self):
         """
         Lists metrics that are computed by this module.
 
         Parameters
         ----------
@@ -844,28 +896,27 @@
         xyz_2 = utils.to_world(xyz_2, self.anisotropy)
         color = "0.0 1.0 0.0" if mistake_type == "split" else "0.0 0.0 1.0"
         path = f"{self.output_dir}/{mistake_type}-{self.saved_site_cnt}.swc"
         save(path, xyz_1, xyz_2, color=color)
 
 
 # -- utils --
-def generate_result(graph_ids, stats):
+def generate_result(ids, stats):
     """
-    Reorders items in "stats" with respect to the order defined by
-    "graph_ids".
+    Reorders items in "stats" with respect to the order defined by "ids".
 
     Parameters
     ----------
-    graph_ids : list[str]
-        List of all "graph_ids" of graphs in "self.labeled_graphs".
+    ids : list[str]
+        List of all "ids" of graphs in "self.labeled_graphs".
     stats : dict
-        Dictionary where the keys are "graph_ids" and values are the result
+        Dictionary where the keys are "ids" and values are the result
         of computing some metrics.
 
     Returns
     -------
     list
         Reorded items in "stats" with respect to the order defined by
-        "graph_ids".
+        "ids".
 
     """
-    return [stats[graph_id] for graph_id in graph_ids]
+    return [stats[id] for id in ids]
```

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,15 +72,16 @@
         Node where possible split starts (i.e. zero-valued label).
 
     Returns
     -------
         dfs_edges : list[tuple].
             Updated "dfs_edges" with visited edges removed.
         labeled_graph : networkx.Graph
-            ...
+            Ground truth graph with nodes labeled with respect to
+            corresponding voxel in predicted segmentation.
 
     """
     # Search
     black_hole = False
     collision_labels = set()
     queue = [root]
     visited = set()
@@ -109,14 +110,42 @@
         label = collision_labels.pop()
         labeled_graph = gutils.upd_labels(labeled_graph, visited, label)
 
     return dfs_edges, labeled_graph
 
 
 def is_nonzero_misalignment(target_graph, labeled_graph, dfs_edges, nb, root):
+    """
+    Determines whether nonzero-valued labels correspond to a split or
+    misalignment between "target_graph" and the predicted segmentation
+    mask.
+
+    Parameters
+    ----------
+    target_graph : networkx.Graph
+        Graph built from a ground truth swc file.
+    labeled_graph : networkx.Graph
+        Labeled graph built from a ground truth swc file, where each node has
+        an attribute called 'label'.
+    dfs_edges : list[tuple]
+        List of edges to be processed for split detection.
+    nb : int
+        Neighbor of "root".
+    root : int
+        Node where possible split starts (i.e. zero-valued label).
+
+    Returns
+    -------
+        dfs_edges : list[tuple].
+            Updated "dfs_edges" with visited edges removed.
+        labeled_graph : networkx.Graph
+            Ground truth graph with nodes labeled with respect to
+            corresponding voxel in predicted segmentation.
+
+    """
     # Initialize
     origin_label = labeled_graph.nodes[nb]["label"]
     hit_label = labeled_graph.nodes[root]["label"]
 
     # Search
     queue = [(nb, root)]
     visited = set([nb])
```

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         coordinates read from cooresponding swc file.
 
     """
     valid_labels = dict()
     for path in swc_paths:
         contents = read_from_local(path)
         if len(contents) > min_size:
-            swc_id = int(utils.get_swc_id(path))
-            valid_labels[swc_id] = get_coords(contents, anisotropy)
+            id = int(utils.get_id(path))
+            valid_labels[id] = get_coords(contents, anisotropy)
     return valid_labels
 
 
 def parse_cloud_paths(cloud_dict, min_size, anisotropy):
     """
     Reads swc files from a GCS bucket and extracts the xyz coordinates.
 
@@ -359,15 +359,15 @@
 
     Returns
     -------
     networkx.Graph
         Graph built from an swc file.
 
     """
-    graph = nx.Graph(swc_id=utils.get_swc_id(path))
+    graph = nx.Graph(swc_id=utils.get_id(path))
     offset = [0, 0, 0]
     for line in read_from_local(path):
         if line.startswith("# OFFSET"):
             parts = line.split()
             offset = read_xyz(parts[2:5])
         if not line.startswith("#"):
             parts = line.split()
```

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,17 +228,23 @@
 def get_midpoint(xyz_1, xyz_2):
     """
     Computes the midpoint between "xyz_1" and "xyz_2".
 
     Parameters
     ----------
     xyz_1 : numpy.ndarray
-        n-dimensional coordinate.
+        xyz coordinate.
     xyz_2 : numpy.ndarray
-        n-dimensional coordinate.
+        xyz coordinate.
+
+    Returns
+    -------
+    numpy.ndarray
+        Midpoint between "xyz_1" and "xyz_2".
+
     """
     return np.array([np.mean([xyz_1[i], xyz_2[i]]) for i in range(3)])
 
 
 def to_world(xyz, anisotropy):
     """
     Converts "xyz" from image coordinates to real-world coordinates.
@@ -271,21 +277,38 @@
     while len(delete_keys) > 0:
         key = delete_keys.pop()
         del my_dict[key]
 
     return my_dict
 
 
-def resolve(multi_hits, dists, xyz_to_swc_node):
+def resolve(multi_hits, dists, xyz_to_id_node):
+    """
+    Resolves discrepancy when xyz coordinates project onto ground truth graphs
+    that contain nodes with same xyz coordinates.
+
+    Parameters
+    ----------
+    multi_hits : set
+        xyz coordinates that are common across multiple graphs.
+    dists : dict
+        Dictionary containing graph ids that predicted swc file has
+        intersected.
+    xyz_to_id_node : dict
+    
+
+    Return
+    ------
+    """
     for hat_xyz in multi_hits:
-        keys = list(xyz_to_swc_node[hat_xyz].keys())
-        swc_id = find_best(dists, keys)
-        if swc_id:
-            node = xyz_to_swc_node[hat_xyz][swc_id]
-            dists = append_dict_value(dists, swc_id, node)
+        keys = list(xyz_to_id_node[hat_xyz].keys())
+        id = find_best(dists, keys)
+        if id:
+            node = xyz_to_id_node[hat_xyz][id]
+            dists = append_dict_value(dists, id, node)
     return dists
 
 
 def append_dict_value(my_dict, key, value):
     """
     Appends "value" to the list stored at "key".
 
@@ -319,29 +342,29 @@
             vote_cnt = len(my_dict[key]) if key in my_dict.keys() else 0
             if vote_cnt > best_vote_cnt:
                 best_key = key
                 best_vote_cnt = vote_cnt
     return best_key
 
 
-def get_swc_id(path):
+def get_id(path):
     """
     Gets segment id of the swc file at "path".
 
     Parameters
     ----------
     path : str
         Path to an swc file
 
     Return
     ------
     Segment id of swc file.
 
     """
-    filename = path.split("/")[-1]
+    filename = os.path.basename(path)
     return filename.split(".")[0]
 
 
 def equiv_class_mappings(connections_path, labels):
     label_to_class = {0: 0}
     labels_graph = build_labels_graph(connections_path, labels)
     for i, component in enumerate(nx.connected_components(labels_graph)):
```

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.1
+Version: 4.1.2
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.2/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

