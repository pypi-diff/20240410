# Comparing `tmp/segmentation_skeleton_metrics-4.1.0.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.1.0.tar", last modified: Tue Apr  9 02:12:09 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.1.tar", last modified: Tue Apr  9 21:41:13 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.1.0.tar` & `segmentation_skeleton_metrics-4.1.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.753924 segmentation_skeleton_metrics-4.1.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.753924 segmentation_skeleton_metrics-4.1.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.753924 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.765924 segmentation_skeleton_metrics-4.1.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.777924 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.777924 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.777924 segmentation_skeleton_metrics-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.166676 segmentation_skeleton_metrics-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.130677 segmentation_skeleton_metrics-4.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 21:41:13.166676 segmentation_skeleton_metrics-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.138677 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.150677 segmentation_skeleton_metrics-4.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:41:13.166676 segmentation_skeleton_metrics-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.134677 segmentation_skeleton_metrics-4.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/merge_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28098 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 21:41:13.000000 segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:41:13.162676 segmentation_skeleton_metrics-4.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 21:41:03.000000 segmentation_skeleton_metrics-4.1.1/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.1/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.1/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/.gitignore` & `segmentation_skeleton_metrics-4.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/LICENSE` & `segmentation_skeleton_metrics-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/PKG-INFO` & `segmentation_skeleton_metrics-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.0
+Version: 4.1.1
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.0/README.md` & `segmentation_skeleton_metrics-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.1/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.1/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.1/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.1/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/pyproject.toml` & `segmentation_skeleton_metrics-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.1/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.1/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.1/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,24 +4,33 @@
 
 @author: Anna Grim
 @email: anna.grim@alleninstitute.org
 
 """
 
 import os
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import (
+    ProcessPoolExecutor,
+    ThreadPoolExecutor,
+    as_completed,
+)
 from time import time
 
 import networkx as nx
 import numpy as np
 import tensorstore as ts
 from scipy.spatial import KDTree
 
 from segmentation_skeleton_metrics import graph_utils as gutils
-from segmentation_skeleton_metrics import split_detection, swc_utils, utils
+from segmentation_skeleton_metrics import (
+    merge_detection,
+    split_detection,
+    swc_utils,
+    utils,
+)
 from segmentation_skeleton_metrics.swc_utils import save, to_graph
 
 CLOSE_DIST_THRESHOLD = 5
 INTERSECTION_THRESHOLD = 16
 MERGE_DIST_THRESHOLD = 30
 
 
@@ -111,16 +120,16 @@
         self.label_mask = pred_labels
         self.valid_labels = swc_utils.parse(
             pred_swc_paths, valid_size_threshold, anisotropy
         )
         self.init_equiv_labels(connections_path)
 
         # Build Graphs
-        self.target_graphs = self.init_graphs(target_swc_paths, anisotropy)
-        self.init_labeled_target_graphs()
+        self.graphs = self.init_graphs(target_swc_paths, anisotropy)
+        self.init_labeled_graphs()
 
         # Build kdtree
         self.init_xyz_to_id_node()
         self.init_kdtree()
 
     # -- Initialize and Label Graphs --
     def init_equiv_labels(self, path):
@@ -134,15 +143,15 @@
                 valid_labels[equiv_label] = values
             self.valid_labels = valid_labels
         else:
             self.equiv_labels_map = None
 
     def init_graphs(self, paths, anisotropy):
         """
-        Initializes "self.target_graphs" by iterating over "paths" which
+        Initializes "self.graphs" by iterating over "paths" which
         correspond to neurons in the ground truth.
 
         Parameters
         ----------
         paths : list[str]
             List of paths to swc files which correspond to neurons in the
             ground truth.
@@ -157,38 +166,38 @@
         """
         graphs = dict()
         for path in paths:
             swc_id = os.path.basename(path).replace(".swc", "")
             graphs[swc_id] = to_graph(path, anisotropy=anisotropy)
         return graphs
 
-    def init_labeled_target_graphs(self):
+    def init_labeled_graphs(self):
         """
-        Initializes "self.labeled_target_graphs" by copying each graph in
-        "self.target_graphs", then labels each node with the label in
+        Initializes "self.labeled_graphs" by copying each graph in
+        "self.graphs", then labels each node with the label in
         "self.label_mask" that coincides with it.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
-        print("Labelling Target Graphs...")
+        print("Labelling Graphs...")
         t0 = time()
-        self.labeled_target_graphs = dict()
-        self.id_to_label_nodes = dict()  # {target_id: {label: nodes}}
-        for cnt, (target_id, graph) in enumerate(self.target_graphs.items()):
-            utils.progress_bar(cnt + 1, len(self.target_graphs))
-            labeled_target_graph, id_to_label_nodes = self.label_graph(graph)
-            self.labeled_target_graphs[target_id] = labeled_target_graph
-            self.id_to_label_nodes[target_id] = id_to_label_nodes
+        self.labeled_graphs = dict()
+        self.id_to_label_nodes = dict()  # {graph_id: {label: nodes}}
+        for cnt, (graph_id, graph) in enumerate(self.graphs.items()):
+            utils.progress_bar(cnt + 1, len(self.graphs))
+            labeled_graph, id_to_label_nodes = self.label_graph(graph)
+            self.labeled_graphs[graph_id] = labeled_graph
+            self.id_to_label_nodes[graph_id] = id_to_label_nodes
 
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
 
     def label_graph(self, target_graph):
         """
         Iterates over nodes in "target_graph" and stores the label in the
@@ -272,15 +281,14 @@
         # Read image label
         if type(self.label_mask) == ts.TensorStore:
             return int(self.label_mask[coord].read().result())
         else:
             return self.label_mask[coord]
 
     def equivalent_label(self, label):
-        # Equivalent label
         if self.equiv_labels_map:
             if label in self.equiv_labels_map.keys():
                 return self.equiv_labels_map[label]
             else:
                 return 0
         else:
             return label
@@ -300,45 +308,45 @@
         label : int
             There are two possibilities: (1) original label if either "label"
             is contained in "self.valid_labels" or "self.valid_labels" is
             None, or (2) 0 if "label" is not contained in self.valid_labels.
 
         """
         if self.valid_labels:
-            if label not in self.valid_labels.keys():
-                return 0
-        return label
+            return 0 if label not in self.valid_labels.keys() else label
+        else:
+            return label
 
     def init_xyz_to_id_node(self):
         self.xyz_to_id_node = dict()
-        for target_id, graph in self.target_graphs.items():
+        for graph_id, graph in self.graphs.items():
             for i in graph.nodes:
                 xyz = tuple(graph.nodes[i]["xyz"])
                 if xyz in self.xyz_to_id_node.keys():
-                    self.xyz_to_id_node[xyz][target_id] = i
+                    self.xyz_to_id_node[xyz][graph_id] = i
                 else:
-                    self.xyz_to_id_node[xyz] = {target_id: i}
+                    self.xyz_to_id_node[xyz] = {graph_id: i}
 
     def get_pred_coords(self, label):
         if label in self.valid_labels.keys():
             return self.valid_labels[label]
         else:
             return []
 
     # -- Final Constructor Routines --
     def init_kdtree(self):
         xyz_list = []
-        for _, graph in self.target_graphs.items():
+        for _, graph in self.graphs.items():
             for i in graph.nodes:
                 xyz_list.append(graph.nodes[i]["xyz"])
-        self.target_graphs_kdtree = KDTree(xyz_list)
+        self.graphs_kdtree = KDTree(xyz_list)
 
     def get_projection(self, xyz):
-        d, idx = self.target_graphs_kdtree.query(xyz, k=1)
-        return tuple(self.target_graphs_kdtree.data[idx]), d
+        d, idx = self.graphs_kdtree.query(xyz, k=1)
+        return tuple(self.graphs_kdtree.data[idx]), d
 
     def init_black_holes(self, black_holes):
         if black_holes:
             black_holes_xyz = [bh_dict["xyz"] for bh_dict in black_holes]
             black_holes_id = [bh_dict["swc_id"] for bh_dict in black_holes]
             self.black_holes = KDTree(black_holes_xyz)
             self.black_hole_labels = set(black_holes_id)
@@ -382,204 +390,200 @@
 
         # Compute metrics
         full_results, avg_results = self.compile_results()
         return full_results, avg_results
 
     def get_all_labels(self):
         labels = set()
-        for target_id in self.target_graphs.keys():
-            labels = labels.union(self.get_labels(target_id))
+        for graph_id in self.graphs.keys():
+            labels = labels.union(self.get_labels(graph_id))
+        labels.discard(0)
         return labels
 
-    def get_labels(self, target_id):
+    def get_labels(self, graph_id):
         """
         Gets the predicted label ids that intersect with the target graph
-        corresponding to "target_id".
+        corresponding to "graph_id".
 
         Parameters
         ----------
-        target_id : str
+        graph_id : str
+
+        """
+        return set(self.id_to_label_nodes[graph_id].keys())
 
+    def zero_nodes(self, graph_id, label):
         """
-        return set(self.id_to_label_nodes[target_id].keys())
+        Zeros out nodes in "self.labeled_target_graph[graph_id" in the sense
+        the label of nodes with "label" is updated to zero.
+
+        Parameters
+        ----------
+        graph_id : str
+            ID of ground truth graph to be updated.
+        label : int
+            Label that identifies which nodes to have their label updated to
+            zero.
+
+        Returns
+        -------
+        None
 
-    def zero_nodes(self, target_id, label):
-        if label in self.id_to_label_nodes[target_id].keys():
-            for i in self.id_to_label_nodes[target_id][label]:
-                self.labeled_target_graphs[target_id].nodes[i]["label"] = 0
-            self.id_to_label_nodes[target_id][label] = set()
+        """
+        if label in self.id_to_label_nodes[graph_id].keys():
+            for i in self.id_to_label_nodes[graph_id][label]:
+                self.labeled_graphs[graph_id].nodes[i]["label"] = 0
+            self.id_to_label_nodes[graph_id][label] = set()
 
     def detect_splits(self):
         """
         Detects splits in the predicted segmentation, then deletes node and
-        edges in "self.labeled_target_graphs" that correspond to a split.
+        edges in "self.labeled_graphs" that correspond to a split.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
         t0 = time()
-        target_graphs = self.target_graphs.items()
-        for cnt, (target_id, target_graph) in enumerate(target_graphs):
+        for cnt, (graph_id, target_graph) in enumerate(self.graphs.items()):
             # Detection
-            utils.progress_bar(cnt + 1, len(self.target_graphs))
-            labeled_graph = self.labeled_target_graphs[target_id]
+            utils.progress_bar(cnt + 1, len(self.graphs))
+            labeled_graph = self.labeled_graphs[graph_id]
             labeled_graph = split_detection.run(target_graph, labeled_graph)
 
             # Update predicted graph
             labeled_graph = gutils.delete_nodes(labeled_graph, 0)
             labeled_graph = gutils.delete_nodes(labeled_graph, -1)
             id_to_label_nodes = gutils.store_labels(labeled_graph)
-            self.labeled_target_graphs[target_id] = labeled_graph
-            self.id_to_label_nodes[target_id] = id_to_label_nodes
+            self.labeled_graphs[graph_id] = labeled_graph
+            self.id_to_label_nodes[graph_id] = id_to_label_nodes
 
         # Report runtime
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
 
     def quantify_splits(self):
         """
         Counts the number of splits, number of omit edges, and percent of omit
-        edges for each graph in "self.labeled_target_graphs".
+        edges for each graph in "self.labeled_graphs".
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
         self.split_cnts = dict()
         self.omit_cnts = dict()
         self.omit_percents = dict()
-        for target_id in self.target_graphs.keys():
-            n_splits = gutils.count_splits(
-                self.labeled_target_graphs[target_id]
-            )
-            n_pred_edges = self.labeled_target_graphs[
-                target_id
-            ].number_of_edges()
-            n_target_edges = self.target_graphs[target_id].number_of_edges()
-
-            self.split_cnts[target_id] = n_splits
-            self.omit_cnts[target_id] = n_target_edges - n_pred_edges
-            self.omit_percents[target_id] = 1 - n_pred_edges / n_target_edges
+        for graph_id in self.graphs.keys():
+            n_splits = gutils.count_splits(self.labeled_graphs[graph_id])
+            n_pred_edges = self.labeled_graphs[graph_id].number_of_edges()
+            n_target_edges = self.graphs[graph_id].number_of_edges()
+
+            self.split_cnts[graph_id] = n_splits
+            self.omit_cnts[graph_id] = n_target_edges - n_pred_edges
+            self.omit_percents[graph_id] = 1 - n_pred_edges / n_target_edges
 
     def detect_merges(self):
         """
         Detects merges in the predicted segmentation, then deletes node and
-        edges in "self.labeled_target_graphs" that correspond to a merge.
+        edges in "self.labeled_graphs" that correspond to a merge.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
 
         """
         # Initilizations
         self.merge_cnts = self.init_counter()
         self.merged_cnts = self.init_counter()
         self.merged_percents = self.init_counter()
-        # self.rm_spurious_intersections()
+        self.rm_spurious_intersections()
 
-        # Run detection
+        # Check potential merge sites
         t0 = time()
-        detected_merges = set()
-        for cnt, target_id_1 in enumerate(self.labeled_target_graphs.keys()):
-            utils.progress_bar(cnt + 1, len(self.target_graphs))
-            for target_id_2 in self.labeled_target_graphs.keys():
-                # Check if identical
-                if target_id_1 == target_id_2:
-                    continue
-
-                # Compare labels contained in graph
-                labels_1 = self.get_labels(target_id_1)
-                labels_2 = self.get_labels(target_id_2)
-                intersection = labels_1.intersection(labels_2)
-                for label in intersection:
-                    # Process merge
-                    merge = (frozenset((target_id_1, target_id_2)), label)
-                    if merge not in detected_merges:
-                        detected_merges.add(merge)
-                        if self.save:
-                            site, d = self.localize_site(
-                                target_id_1, target_id_2, label
-                            )
-                            if d < MERGE_DIST_THRESHOLD:
-                                self.save_swc(site[0], site[1], "merge")
+        with ProcessPoolExecutor() as executor:
+            processes = []
+            for ids, label in self.detect_potential_merges():
+                id_1, id_2 = tuple(ids)
+                processes.append(
+                    executor.submit(
+                        merge_detection.localize,
+                        self.graphs[id_1],
+                        self.graphs[id_2],
+                        self.id_to_label_nodes[id_1][label],
+                        self.id_to_label_nodes[id_2][label],
+                        MERGE_DIST_THRESHOLD,
+                        (ids, label),
+                    )
+                )
+
+            # Compile results
+            cnt = 1
+            chunk_size = int(len(processes) * 0.02)
+            detected_merges = set()
+            for i, process in enumerate(as_completed(processes)):
+                # Check site
+                merge_id, site, d = process.result()
+                if d < MERGE_DIST_THRESHOLD:
+                    detected_merges.add(merge_id)
+                    if self.save:
+                        self.save_swc(site[0], site[1], "merge")
+
+                # Report process
+                if i > cnt * chunk_size:
+                    utils.progress_bar(i + 1, len(processes))
+                    cnt += 1
 
         # Update graph
-        for (target_ids, label) in detected_merges:
-            target_id_1, target_id_2 = tuple(target_ids)
-            self.process_merge(target_id_1, label)
-            self.process_merge(target_id_2, label)
-            self.merge_cnts[target_id_1] += 1
-            self.merge_cnts[target_id_2] += 1
+        for (id_1, id_2), label in detected_merges:
+            self.process_merge(id_1, label)
+            self.process_merge(id_2, label)
+            self.merge_cnts[id_1] += 1
+            self.merge_cnts[id_2] += 1
 
         # Report Runtime
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
 
     def rm_spurious_intersections(self):
-        for label in [label for label in self.get_all_labels() if label > 0]:
-            # Compute label intersect target_graphs
-            hit_target_ids = dict()
-            multi_hits = set()
-            for xyz in self.self.get_pred_coords(label):
-                hat_xyz, d = self.get_projection(xyz)
-                if d < CLOSE_DIST_THRESHOLD:
-                    hits = list(self.xyz_to_id_node[hat_xyz].keys())
-                    if len(hits) > 1:
-                        multi_hits.add(hat_xyz)
-                    else:
-                        hat_i = self.xyz_to_id_node[hat_xyz][hits[0]]
-                        hit_target_ids = utils.append_dict_value(
-                            hit_target_ids, hits[0], hat_i
-                        )
-            hit_target_ids = utils.resolve(
-                multi_hits, hit_target_ids, self.xyz_to_id_node
+        for label in self.get_all_labels():
+            # Compute intersections
+            hit_ids = merge_detection.label_intersections(
+                self.get_projection,
+                self.get_pred_coords(label),
+                self.xyz_to_id_node,
+                CLOSE_DIST_THRESHOLD,
             )
 
             # Remove spurious intersections
-            for target_id in self.target_graphs.keys():
-                if target_id in hit_target_ids.keys():
-                    n_hits = len(hit_target_ids[target_id])
-                    if n_hits < INTERSECTION_THRESHOLD:
-                        self.zero_nodes(target_id, label)
-                elif label in self.id_to_label_nodes[target_id]:
-                    self.zero_nodes(target_id, label)
-
-    def localize_site(self, target_id_1, target_id_2, label):
-        # Get merged nodes
-        merged_1 = self.id_to_label_nodes[target_id_1][label]
-        merged_2 = self.id_to_label_nodes[target_id_2][label]
-
-        # Find closest pair
-        min_dist = np.inf
-        xyz_pair = [None, None]
-        for i in merged_1:
-            for j in merged_2:
-                xyz_1 = self.target_graphs[target_id_1].nodes[i]["xyz"]
-                xyz_2 = self.target_graphs[target_id_2].nodes[j]["xyz"]
-                if utils.dist(xyz_1, xyz_2) < min_dist:
-                    min_dist = utils.dist(xyz_1, xyz_2)
-                    xyz_pair = [xyz_1, xyz_2]
-                    if min_dist < MERGE_DIST_THRESHOLD:
-                        return xyz_pair, min_dist
-        return xyz_pair, min_dist
+            for graph_id in self.graphs.keys():
+                if graph_id in hit_ids.keys():
+                    if len(hit_ids[graph_id]) < INTERSECTION_THRESHOLD:
+                        self.zero_nodes(graph_id, label)
+                elif label in self.id_to_label_nodes[graph_id]:
+                    self.zero_nodes(graph_id, label)
+
+    def detect_potential_merges(self):
+        return merge_detection.detect_potentials(
+            self.labeled_graphs, self.get_labels
+        )
 
     def near_bdd(self, xyz):
         """
         Determines whether "xyz" is near the boundary of the image.
 
         Parameters
         ----------
@@ -612,46 +616,46 @@
         Returns
         -------
         dict
             Dictionary used to count number of merge type mistakes.
 
         """
         counter = dict()
-        for label in self.labeled_target_graphs.keys():
+        for label in self.labeled_graphs.keys():
             counter[label] = 0
         return counter
 
     def init_tracker(self):
         tracker = dict()
-        for label in self.labeled_target_graphs.keys():
+        for label in self.labeled_graphs.keys():
             tracker[label] = set()
         return tracker
 
-    def process_merge(self, target_id, label):
+    def process_merge(self, graph_id, label):
         """
-        Once a merge has been detected that corresponds to "target_id", every
-        node in "self.labeled_target_graph[target_id]" with that "label" is
+        Once a merge has been detected that corresponds to "graph_id", every
+        node in "self.labeled_graph[graph_id]" with that "label" is
         deleted.
 
         Parameters
         ----------
-        target_id : str
-            Key associated with the labeled_target_graph to be searched.
+        graph_id : str
+            Key associated with the labeled_graph to be searched.
         label : int
             Label in prediction that is assocatied with a merge.
 
         Returns
         -------
         None
 
         """
-        graph = self.labeled_target_graphs[target_id].copy()
+        graph = self.labeled_graphs[graph_id].copy()
         graph, merged_cnt = gutils.delete_nodes(graph, label, return_cnt=True)
-        self.labeled_target_graphs[target_id] = graph
-        self.merged_cnts[target_id] += merged_cnt
+        self.labeled_graphs[graph_id] = graph
+        self.merged_cnts[graph_id] += merged_cnt
 
     def quantify_merges(self):
         """
         Computes the percentage of merged edges for each labeled_target_graph.
 
         Parameters
         ----------
@@ -659,85 +663,85 @@
 
         Returns
         -------
         None
 
         """
         self.merged_percents = dict()
-        for target_id in self.target_graphs.keys():
-            n_edges = self.target_graphs[target_id].number_of_edges()
-            percent = self.merged_cnts[target_id] / n_edges
-            self.merged_percents[target_id] = percent
+        for graph_id in self.graphs.keys():
+            n_edges = self.graphs[graph_id].number_of_edges()
+            percent = self.merged_cnts[graph_id] / n_edges
+            self.merged_percents[graph_id] = percent
 
     def compile_results(self):
         """
         Compiles a dictionary containing the metrics computed by this module.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         full_results : dict
-            Dictionary where the keys are target_ids and the values are the
+            Dictionary where the keys are graph_ids and the values are the
             result of computing each metric for the corresponding graphs.
         avg_result : dict
             Dictionary where the keys are names of metrics computed by this
-            module and values are the averaged result over all target_ids.
+            module and values are the averaged result over all graph_ids.
 
         """
         # Compute remaining metrics
         self.compute_edge_accuracy()
         self.compute_erl()
 
         # Summarize results
-        target_ids, results = self.generate_full_results()
+        graph_ids, results = self.generate_full_results()
         avg_results = self.generate_avg_results()
 
         # Reformat full results
         full_results = dict()
-        for i, target_id in enumerate(target_ids):
-            full_results[target_id] = dict(
+        for i, graph_id in enumerate(graph_ids):
+            full_results[graph_id] = dict(
                 [(key, results[key][i]) for key in results.keys()]
             )
 
         return full_results, avg_results
 
     def generate_full_results(self):
         """
         Generates a report by creating a list of the results for each metric.
-        Each item in this list corresponds to a graph in labeled_target_graphs
-        and this list is ordered with respect to "target_ids".
+        Each item in this list corresponds to a graph in labeled_graphs and
+        this list is ordered with respect to "graph_ids".
 
         Parameters
         ----------
         None
 
         Results
         -------
-        target_ids : list[str]
+        graph_ids : list[str]
             Specifies the ordering of results for each value in "stats".
         stats : dict
             Dictionary where the keys are metrics and values are the result of
-            computing that metric for each graph in labeled_target_graphs.
+            computing that metric for each graph in labeled_graphs.
 
         """
-        target_ids = list(self.labeled_target_graphs.keys())
-        target_ids.sort()
+        graph_ids = list(self.labeled_graphs.keys())
+        graph_ids.sort()
         stats = {
-            "# splits": generate_result(target_ids, self.split_cnts),
-            "# merges": generate_result(target_ids, self.merge_cnts),
-            "% omit": generate_result(target_ids, self.omit_percents),
-            "% merged": generate_result(target_ids, self.merged_percents),
-            "edge accuracy": generate_result(target_ids, self.edge_accuracy),
-            "erl": generate_result(target_ids, self.erl),
-            "normalized erl": generate_result(target_ids, self.normalized_erl),
+            "# splits": generate_result(graph_ids, self.split_cnts),
+            "# merges": generate_result(graph_ids, self.merge_cnts),
+            "% omit": generate_result(graph_ids, self.omit_percents),
+            "% merged": generate_result(graph_ids, self.merged_percents),
+            "edge accuracy": generate_result(graph_ids, self.edge_accuracy),
+            "erl": generate_result(graph_ids, self.erl),
+            "normalized erl": generate_result(graph_ids, self.normalized_erl),
         }
-        return target_ids, stats
+        return graph_ids, stats
 
     def generate_avg_results(self):
         avg_stats = {
             "# splits": self.avg_result(self.split_cnts),
             "# merges": self.avg_result(self.merge_cnts) / 2,
             "% omit": self.avg_result(self.omit_percents),
             "% merged": self.avg_result(self.merged_percents),
@@ -746,17 +750,17 @@
             "normalized erl": self.avg_result(self.normalized_erl),
         }
         return avg_stats
 
     def avg_result(self, stats):
         result = []
         wgts = []
-        for target_id, wgt in self.wgts.items():
-            if self.omit_percents[target_id] < 1:
-                result.append(stats[target_id])
+        for graph_id, wgt in self.wgts.items():
+            if self.omit_percents[graph_id] < 1:
+                result.append(stats[graph_id])
                 wgts.append(wgt)
         return np.average(result, weights=wgts)
 
     def compute_edge_accuracy(self):
         """
         Computes the edge accuracy of each labeled_target_graph.
 
@@ -766,18 +770,18 @@
 
         Returns
         -------
         None
 
         """
         self.edge_accuracy = dict()
-        for target_id in self.target_graphs.keys():
-            omit_percent = self.omit_percents[target_id]
-            merged_percent = self.merged_percents[target_id]
-            self.edge_accuracy[target_id] = 1 - omit_percent - merged_percent
+        for graph_id in self.graphs.keys():
+            omit_percent = self.omit_percents[graph_id]
+            merged_percent = self.merged_percents[graph_id]
+            self.edge_accuracy[graph_id] = 1 - omit_percent - merged_percent
 
     def compute_erl(self):
         """
         Computes the expected run length (ERL) of each labeled_target_graph.
 
         Parameters
         ----------
@@ -788,30 +792,30 @@
         None
 
         """
         self.erl = dict()
         self.normalized_erl = dict()
         self.wgts = dict()
         total_path_length = 0
-        for target_id in self.target_graphs.keys():
-            labeled_target_graph = self.labeled_target_graphs[target_id]
-            target_graph = self.target_graphs[target_id]
+        for graph_id in self.graphs.keys():
+            labeled_target_graph = self.labeled_graphs[graph_id]
+            target_graph = self.graphs[graph_id]
 
             path_length = gutils.compute_path_length(target_graph)
             run_lengths = gutils.compute_run_lengths(labeled_target_graph)
             wgt = run_lengths / max(np.sum(run_lengths), 1)
 
-            self.erl[target_id] = np.sum(wgt * run_lengths)
-            self.normalized_erl[target_id] = self.erl[target_id] / path_length
+            self.erl[graph_id] = np.sum(wgt * run_lengths)
+            self.normalized_erl[graph_id] = self.erl[graph_id] / path_length
 
-            self.wgts[target_id] = path_length
+            self.wgts[graph_id] = path_length
             total_path_length += path_length
 
-        for target_id in self.target_graphs.keys():
-            self.wgts[target_id] = self.wgts[target_id] / total_path_length
+        for graph_id in self.graphs.keys():
+            self.wgts[graph_id] = self.wgts[graph_id] / total_path_length
 
     def list_metrics(self):
         """
         Lists metrics that are computed by this module.
 
         Parameters
         ----------
@@ -840,28 +844,28 @@
         xyz_2 = utils.to_world(xyz_2, self.anisotropy)
         color = "0.0 1.0 0.0" if mistake_type == "split" else "0.0 0.0 1.0"
         path = f"{self.output_dir}/{mistake_type}-{self.saved_site_cnt}.swc"
         save(path, xyz_1, xyz_2, color=color)
 
 
 # -- utils --
-def generate_result(target_ids, stats):
+def generate_result(graph_ids, stats):
     """
     Reorders items in "stats" with respect to the order defined by
-    "target_ids".
+    "graph_ids".
 
     Parameters
     ----------
-    target_ids : list[str]
-        List of all |target_ids" of graphs in "self.labeled_target_graphs".
+    graph_ids : list[str]
+        List of all "graph_ids" of graphs in "self.labeled_graphs".
     stats : dict
-        Dictionary where the keys are "target_ids" and values are the result
+        Dictionary where the keys are "graph_ids" and values are the result
         of computing some metrics.
 
     Returns
     -------
     list
         Reorded items in "stats" with respect to the order defined by
-        "target_ids".
+        "graph_ids".
 
     """
-    return [stats[target_id] for target_id in target_ids]
+    return [stats[graph_id] for graph_id in graph_ids]
```

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.0
+Version: 4.1.1
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.1/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 resources/target_graphs/1.swc
 resources/target_graphs/2.swc
 resources/target_graphs/3.swc
 resources/target_graphs/4.swc
 resources/target_graphs/5.swc
 src/segmentation_skeleton_metrics/__init__.py
 src/segmentation_skeleton_metrics/graph_utils.py
+src/segmentation_skeleton_metrics/merge_detection.py
 src/segmentation_skeleton_metrics/skeleton_metric.py
 src/segmentation_skeleton_metrics/split_detection.py
 src/segmentation_skeleton_metrics/swc_utils.py
 src/segmentation_skeleton_metrics/utils.py
 src/segmentation_skeleton_metrics.egg-info/PKG-INFO
 src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
 src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
```

