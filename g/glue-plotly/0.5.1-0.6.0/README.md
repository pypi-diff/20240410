# Comparing `tmp/glue-plotly-0.5.1.tar.gz` & `tmp/glue-plotly-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-plotly-0.5.1.tar", last modified: Wed Oct  4 05:49:29 2023, max compression
+gzip compressed data, was "glue-plotly-0.6.0.tar", last modified: Wed Apr 10 21:04:37 2024, max compression
```

## Comparing `glue-plotly-0.5.1.tar` & `glue-plotly-0.6.0.tar`

### file list

```diff
@@ -1,112 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.129225 glue-plotly-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.101224 glue-plotly-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.105224 glue-plotly-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-04 05:49:29.129225 glue-plotly-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.109224 glue-plotly-0.5.1/glue_plotly/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.117225 glue-plotly-0.5.1/glue_plotly/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/scatter3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.117225 glue-plotly-0.5.1/glue_plotly/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/export_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.117225 glue-plotly-0.5.1/glue_plotly/html_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.121225 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.121225 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/save_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/save_hover.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/sort_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/sort_components.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/viewers/common/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/common/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/viewers/histogram/
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/histogram/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/histogram/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/viewers/scatter/
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/scatter/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/viewers/scatter/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/export_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/web/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/qt/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/qt/exporter.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/web/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/qt/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/qt/tests/test_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.125225 glue-plotly-0.5.1/glue_plotly/web/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/glue_plotly/web/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 05:49:29.113225 glue-plotly-0.5.1/glue_plotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-04 05:49:29.000000 glue-plotly-0.5.1/glue_plotly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-10-04 05:49:29.129225 glue-plotly-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-04 05:48:52.000000 glue-plotly-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.019477 glue-plotly-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.019477 glue-plotly-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.019477 glue-plotly-0.6.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/BqplotToolbarHighlighted.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/PlotlyViewerExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/QtChartStudioExport.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/QtToolbarExport.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.023477 glue-plotly-0.6.0/glue_plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.023477 glue-plotly-0.6.0/glue_plotly/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/scatter3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/export_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/save_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/save_hover.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/sort_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/sort_components.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/histogram/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/histogram/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/scatter/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/scatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/scatter/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/scatter/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/export_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/web/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/exporter.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/glue_plotly/web/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/glue_plotly/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/glue_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-10 21:04:37.000000 glue-plotly-0.6.0/glue_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/tox.ini
```

### Comparing `glue-plotly-0.5.1/.github/workflows/ci_workflows.yml` & `glue-plotly-0.6.0/.github/workflows/ci_workflows.yml`

 * *Files 25% similar despite different names*

```diff
@@ -32,24 +32,39 @@
           - libhdf5-dev
       envs: |
         # Standard tests
         - linux: py38-test
         - linux: py39-test
         - linux: py310-test
         - linux: py311-test
+        - linux: py311-glue113-test
+        - linux: py311-glue114-test
+        - linux: py311-glue115-test
+        - linux: py311-glue116-test
+        - linux: py311-glue117-test
 
         - macos: py38-test
         - macos: py39-test
         - macos: py310-test
         - macos: py311-test
+        - macos: py311-glue113-test
+        - macos: py311-glue114-test
+        - macos: py311-glue115-test
+        - macos: py311-glue116-test
+        - macos: py311-glue117-test
 
         - windows: py38-test
         - windows: py39-test
         - windows: py310-test
         - windows: py311-test
+        - windows: py311-glue113-test
+        - windows: py311-glue114-test
+        - windows: py311-glue115-test
+        - windows: py311-glue116-test
+        - windows: py311-glue117-test
 
   publish:
     needs: tests
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish_pure_python.yml@v1
     with:
       libraries: '^libxcb.*-dev libxkbcommon-x11-dev libgl1-mesa-glx xvfb'
       test_extras: 'test,qt,jupyter'
```

### Comparing `glue-plotly-0.5.1/.github/workflows/update-changelog.yaml` & `glue-plotly-0.6.0/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/CHANGES.md` & `glue-plotly-0.6.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Full changelog
 
+## v0.5.1 - 2023-10-04
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### Bug Fixes
+
+- Separate glue_qt and glue_jupyter import attempts by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/47
+
+**Full Changelog**: https://github.com/glue-viz/glue-plotly/compare/v0.5.0...v0.5.1
+
 ## v0.5.0 - 2023-09-16
 
 <!-- Release notes generated using configuration in .github/release.yml at main -->
 ### What's Changed
 
 #### New Features
```

### Comparing `glue-plotly-0.5.1/LICENSE` & `glue-plotly-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/__init__.py` & `glue-plotly-0.6.0/glue_plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/common.py` & `glue-plotly-0.6.0/glue_plotly/common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         linecolor=settings.FOREGROUND_COLOR,
         tickcolor=settings.FOREGROUND_COLOR,
         zeroline=False,
         mirror=True,
         ticks='outside',
         showline=True,
         showgrid=False,
+        fixedrange=True,
         showticklabels=True,
         tickfont=dict(
             family=DEFAULT_FONT,
             size=1.5 * ticklabel_size,
             color=settings.FOREGROUND_COLOR),
         range=range,
         type='log' if log else 'linear',
```

### Comparing `glue-plotly-0.5.1/glue_plotly/common/dendrogram.py` & `glue-plotly-0.6.0/glue_plotly/common/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/histogram.py` & `glue-plotly-0.6.0/glue_plotly/common/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/image.py` & `glue-plotly-0.6.0/glue_plotly/common/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,29 +151,37 @@
         size = 25 * (s - layer_state.size_vmin) / (
                         layer_state.size_vmax - layer_state.size_vmin)
         size[np.isnan(size)] = 0
         size[size < 0] = 0
         return size
 
 
-def get_stretch(stretch_name):
+def get_stretch_by_name(stretch_name):
     try:
         return stretches.members[stretch_name]
     except TypeError:
         return stretches[stretch_name]()
 
 
+def get_stretch(layer_state):
+    if hasattr(layer_state, 'stretch_object'):
+        return layer_state.stretch_object
+    else:
+        return get_stretch_by_name(layer_state.stretch)
+
+
 def colorscale_info(layer_state, interval, contrast_bias):
     if layer_state.v_min > layer_state.v_max:
         cmap = layer_state.cmap.reversed()
         bounds = [layer_state.v_max, layer_state.v_min]
     else:
         cmap = layer_state.cmap
         bounds = [layer_state.v_min, layer_state.v_max]
-    mapped_bounds = get_stretch(layer_state.stretch)(contrast_bias(interval(bounds)))
+    stretch = get_stretch(layer_state)
+    mapped_bounds = stretch(contrast_bias(interval(bounds)))
     unmapped_space = np.linspace(0, 1, 60)
     mapped_space = np.linspace(mapped_bounds[0], mapped_bounds[1], 60)
     color_space = [cmap(b)[:3] for b in mapped_space]
     color_values = [tuple(256 * v for v in p) for p in color_space]
     colorscale = [[0, 'rgb{0}'.format(color_values[0])]] + \
                  [[u, 'rgb{0}'.format(c)] for u, c in zip(unmapped_space, color_values)] + \
                  [[1, 'rgb{0}'.format(color_values[-1])]]
@@ -337,15 +345,16 @@
         array = array(bounds=None)
     if array is None:
         return []
 
     if np.isscalar(array):
         array = np.atleast_2d(array)
 
-    img = get_stretch(layer_state.stretch)(constrast_bias(interval(array)))
+    stretch = get_stretch(layer_state)
+    img = stretch(constrast_bias(interval(array)))
     img[np.isnan(img)] = 0
 
     z_bounds, colorscale = colorscale_info(layer_state, interval, constrast_bias)
     image_info = dict(z=img,
                       colorscale=colorscale,
                       hoverinfo='skip',
                       xaxis='x',
```

### Comparing `glue-plotly-0.5.1/glue_plotly/common/profile.py` & `glue-plotly-0.6.0/glue_plotly/common/profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/scatter2d.py` & `glue-plotly-0.6.0/glue_plotly/common/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/scatter3d.py` & `glue-plotly-0.6.0/glue_plotly/common/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/tests/test_dendrogram.py` & `glue-plotly-0.6.0/glue_plotly/common/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/tests/test_histogram.py` & `glue-plotly-0.6.0/glue_plotly/common/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/tests/test_profile.py` & `glue-plotly-0.6.0/glue_plotly/common/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/tests/test_scatter2d.py` & `glue-plotly-0.6.0/glue_plotly/common/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/common/tests/utils.py` & `glue-plotly-0.6.0/glue_plotly/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/export_dialog.py` & `glue-plotly-0.6.0/glue_plotly/export_dialog.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/base.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/base.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/histogram.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/image.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/profile.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/scatter2d.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_base.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class TestBqplotExporter:
 
     viewer_type = None
     tool_id = None
 
     def setup_method(self, method):
-        self.data = self.test_data()
+        self.data = self.make_data()
         self.app = jglue()
         self.app.session.data_collection.append(self.data)
         self.viewer = self.app.new_data_viewer(self.viewer_type)
         self.viewer.add_data(self.data)
         self.tool = self.viewer.toolbar.tools[self.tool_id]
 
     def teardown_method(self, method):
```

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_histogram.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class TestHistogram(TestBqplotExporter):
 
     viewer_type = BqplotHistogramView
     tool_id = 'save:bqplot_plotlyhist'
 
-    def test_data(self):
+    def make_data(self):
         return Data(x=[40, 41, 37, 63, 78, 35, 19, 100, 35, 86, 84, 99,
                        87, 56, 2, 71, 22, 36, 10, 1, 26, 70, 45, 20, 8],
                     label='d1')
 
     def test_default(self, tmpdir):
         output_path = self.export_figure(tmpdir, 'test_default.html')
         assert os.path.exists(output_path)
```

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_image.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
 
 class TestImage(TestBqplotExporter):
 
     viewer_type = BqplotImageView
     tool_id = 'save:bqplot_plotlyimage2d'
 
-    def test_data(self):
+    def make_data(self):
         return Data(label='d1', x=arange(24).reshape((2, 3, 4)), y=ones((2, 3, 4)))
 
     def test_default(self, tmpdir):
         output_path = self.export_figure(tmpdir, 'test_default.html')
         assert os.path.exists(output_path)
```

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_profile.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class TestProfile(TestBqplotExporter):
 
     viewer_type = BqplotProfileView
     tool_id = 'save:bqplot_plotlyprofile'
 
-    def test_data(self):
+    def make_data(self):
         return Data(x=[40, 41, 37, 63, 78, 35, 19, 100, 35, 86, 84, 99,
                        87, 56, 2, 71, 22, 36, 10, 1, 26, 70, 45, 20, 8],
                     label='d1')
 
     def test_default(self, tmpdir):
         output_path = self.export_figure(tmpdir, 'test_default.html')
         assert os.path.exists(output_path)
```

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 
 
 class TestScatter2D(TestBqplotExporter):
 
     viewer_type = BqplotScatterView
     tool_id = 'save:bqplot_plotly2d'
 
-    def test_data(self):
+    def make_data(self):
         return Data(x=[1, 2, 3], y=[4, 5, 6], z=[7, 8, 9], label='d1')
 
     def test_default(self, tmpdir):
         output_path = self.export_figure(tmpdir, 'test_default.html')
         assert os.path.exists(output_path)
```

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/dendrogram.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/histogram.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/image.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/profile.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/scatter2d.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/scatter3d.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/table.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/table.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_base.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_dendrogram.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_histogram.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_image.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_profile.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_scatter2d.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_scatter3d.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/html_exporters/qt/tests/test_table.py` & `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/logo.png` & `glue-plotly-0.6.0/glue_plotly/logo.png`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/logo.svg` & `glue-plotly-0.6.0/glue_plotly/logo.svg`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/save_hover.py` & `glue-plotly-0.6.0/glue_plotly/save_hover.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/save_hover.ui` & `glue-plotly-0.6.0/glue_plotly/save_hover.ui`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/sort_components.py` & `glue-plotly-0.6.0/glue_plotly/sort_components.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/sort_components.ui` & `glue-plotly-0.6.0/glue_plotly/sort_components.ui`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/utils.py` & `glue-plotly-0.6.0/glue_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/viewers/common/tools.py` & `glue-plotly-0.6.0/glue_plotly/viewers/common/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.viewer.set_selection_active(True)
         self.viewer.set_selection_callback(self.on_selection)
 
     def deactivate(self):
         self.viewer.set_selection_callback(None)
         self.viewer.set_selection_active(False)
         self.viewer.figure.on_edits_completed(self._clear_selection)
+        super().deactivate()
 
     def _clear_selection(self):
         self.viewer.figure.plotly_relayout({'selections': [], 'dragmode': False})
 
     def on_selection(self, trace, points, selector):
         self._on_selection(trace, points, selector)
         self.viewer.toolbar.active_tool = None
@@ -70,24 +71,80 @@
             viewer_state.x_min = xmin
             viewer_state.x_max = xmax
             viewer_state.y_min = ymin
             viewer_state.y_max = ymax
 
 
 @viewer_tool
+class PlotlyHZoomMode(PlotlySelectionMode):
+
+    icon = 'glue_zoom_to_rect'
+    tool_id = 'plotly:hzoom'
+    action_text = 'Horizontal zoom'
+    tool_tip = 'Horizontal zoom'
+
+    def __init__(self, viewer):
+        super().__init__(viewer, 'select')
+
+    def activate(self):
+        super().activate()
+        self.viewer.figure.update_layout(selectdirection="h")
+
+    def _on_selection(self, _trace, _points, selector):
+        xmin, xmax = selector.xrange
+        viewer_state = self.viewer.state
+        with self.viewer.figure.batch_update(), delay_callback(viewer_state, 'x_min', 'x_max'):
+            viewer_state.x_min = xmin
+            viewer_state.x_max = xmax
+
+
+@viewer_tool
+class PlotlyVZoomMode(PlotlySelectionMode):
+
+    icon = 'glue_zoom_to_rect'
+    tool_id = 'plotly:vzoom'
+    action_text = 'Vertical zoom'
+    tool_tip = 'Vertical zoom'
+
+    def __init__(self, viewer):
+        super().__init__(viewer, 'select')
+
+    def activate(self):
+        super().activate()
+        self.viewer.figure.update_layout(selectdirection="v")
+
+    def _on_selection(self, _trace, _points, selector):
+        ymin, ymax = selector.yrange
+        viewer_state = self.viewer.state
+        with self.viewer.figure.batch_update(), delay_callback(viewer_state, 'y_min', 'y_max'):
+            viewer_state.y_min = ymin
+            viewer_state.y_max = ymax
+
+
+@viewer_tool
 class PlotlyPanMode(PlotlyDragMode):
 
     icon = 'glue_move'
     tool_id = 'plotly:pan'
     action_text = 'Pan'
     tool_tip = 'Interactively pan'
 
     def __init__(self, viewer):
         super().__init__(viewer, 'pan')
 
+    def activate(self):
+        super().activate()
+        self.viewer.figure.layout['xaxis']['fixedrange'] = False
+        self.viewer.figure.layout['yaxis']['fixedrange'] = False
+
+    def deactivate(self):
+        self.viewer.figure.layout['xaxis']['fixedrange'] = True
+        self.viewer.figure.layout['yaxis']['fixedrange'] = True
+        super().deactivate()
+
 
 @viewer_tool
 class PlotlyHRangeSelectionMode(PlotlySelectionMode):
 
     icon = 'glue_xrange_select'
     tool_id = 'plotly:xrange'
     action_text = 'X range'
@@ -176,7 +233,22 @@
     tool_id = 'plotly:home'
     action_text = 'Home'
     tool_tip = 'Reset original zoom'
 
     def activate(self):
         with self.viewer.figure.batch_update():
             self.viewer.state.reset_limits()
+
+
+@viewer_tool
+class PlotlyHoverTool(CheckableTool):
+
+    icon = 'glue_point'
+    tool_id = 'plotly:hover'
+    action_text = 'Hover'
+    tool_tip = 'Show hover info'
+
+    def activate(self):
+        self.viewer.figure.update_layout(hovermode="closest")
+
+    def deactivate(self):
+        self.viewer.figure.update_layout(hovermode=False)
```

### Comparing `glue-plotly-0.5.1/glue_plotly/viewers/common/viewer.py` & `glue-plotly-0.6.0/glue_plotly/viewers/common/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 INTERACT_COLOR = "#cbcbcb"
 
 
 class PlotlyBaseView(IPyWidgetView):
 
     LAYOUT_SETTINGS = dict(
         include_dimensions=False,
+        hovermode=False, hoverdistance=1,
         dragmode=False, showlegend=False, grid=None,
         newselection=dict(line=dict(color=INTERACT_COLOR), mode='immediate'),
         modebar=dict(remove=['toimage', 'zoom', 'pan', 'lasso', 'zoomIn2d',
                              'zoomOut2d', 'select', 'autoscale', 'resetScale2d',
                              'resetViews'])
     )
 
@@ -80,15 +81,14 @@
         except ValueError:
             pass
 
     def _remove_traces(self, traces):
         self.figure.data = [t for t in self.figure.data if t not in traces]
 
     def _clear_traces(self):
-        print("In _clear_traces")
         self.figure.data = [self.selection_layer]
 
     @property
     def axis_x(self):
         return self.figure.layout.xaxis
 
     @property
```

### Comparing `glue-plotly-0.5.1/glue_plotly/viewers/histogram/layer_artist.py` & `glue-plotly-0.6.0/glue_plotly/viewers/histogram/layer_artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from glue.core.exceptions import IncompatibleAttribute
 from glue.viewers.common.layer_artist import LayerArtist
 from glue.viewers.histogram.state import HistogramLayerState
 from glue_plotly.common.common import fixed_color
 
 from glue_plotly.common.histogram import traces_for_layer
 
+__all__ = ["PlotlyHistogramLayerArtist"]
+
 SCALE_PROPERTIES = {'y_log', 'normalize', 'cumulative'}
 HISTOGRAM_PROPERTIES = SCALE_PROPERTIES | {'layer', 'x_att', 'hist_x_min',
                                            'hist_x_max', 'hist_n_bin', 'x_log'}
 VISUAL_PROPERTIES = {'alpha', 'color', 'zorder', 'visible'}
 DATA_PROPERTIES = {'layer', 'x_att', 'y_att'}
 
 
@@ -111,15 +113,15 @@
             with self.view.figure.batch_update():
                 for bar in old_bars:
                     self.view._remove_trace_index(bar)
             # self.view._remove_traces(old_bars)
 
         bars = traces_for_layer(self.view.state, self.state, add_data_label=True)
         for bar in bars:
-            bar.update(unselected=dict(marker=dict(opacity=self.state.alpha)))
+            bar.update(hoverinfo='all', unselected=dict(marker=dict(opacity=self.state.alpha)))
         self._bars_id = bars[0].meta if bars else None
         self.view.figure.add_traces(bars)
 
     def _update_zorder(self):
         traces = [self.view.selection_layer]
         for layer in self.view.layers:
             traces += list(layer.traces())
```

### Comparing `glue-plotly-0.5.1/glue_plotly/viewers/histogram/viewer.py` & `glue-plotly-0.6.0/glue_plotly/viewers/histogram/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from glue.core.subset import XRangeROI, roi_to_subset_state
 from glue.viewers.histogram.state import HistogramViewerState
 from glue_plotly.common import base_layout_config, base_rectilinear_axis
 from glue_plotly.viewers import PlotlyBaseView
 from glue_plotly.viewers.histogram.layer_artist import PlotlyHistogramLayerArtist
 
-
 from glue_jupyter.registries import viewer_registry
 from glue_jupyter.common.state_widgets.layer_histogram import HistogramLayerStateWidget
 from glue_jupyter.common.state_widgets.viewer_histogram import HistogramViewerStateWidget
 
 
+__all__ = ["PlotlyHistogramView"]
+
+
 @viewer_registry("plotly_histogram")
 class PlotlyHistogramView(PlotlyBaseView):
 
-    tools = ['plotly:home', 'plotly:zoom', 'plotly:pan', 'plotly:xrange']
+    tools = ['plotly:home', 'plotly:zoom', 'plotly:pan', 'plotly:xrange', 'plotly:hover']
 
     allow_duplicate_data = False
     allow_duplicate_subset = False
 
     _state_cls = HistogramViewerState
     _options_cls = HistogramViewerStateWidget
     _data_artist_cls = PlotlyHistogramLayerArtist
```

### Comparing `glue-plotly-0.5.1/glue_plotly/viewers/scatter/layer_artist.py` & `glue-plotly-0.6.0/glue_plotly/viewers/scatter/layer_artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from glue.utils import ensure_numerical
 from glue.viewers.common.layer_artist import LayerArtist
 from glue.viewers.scatter.state import ScatterLayerState
 
 from plotly.graph_objs import Scatter, Scatterpolar
 
 
+__all__ = ["PlotlyScatterLayerArtist"]
+
+
 CMAP_PROPERTIES = {"cmap_mode", "cmap_att", "cmap_vmin", "cmap_vmax", "cmap"}
 MARKER_PROPERTIES = {
     "size_mode",
     "size_att",
     "size_vmin",
     "size_vmax",
     "size_scaling",
@@ -125,15 +128,15 @@
         if isinstance(self.layer, BaseData):
             name = self.layer.label
         else:
             name = f"{self.layer.label} ({self.layer.data.label})"
 
         scatter_info = dict(mode=scatter_mode(self.state),
                             name=name,
-                            hoverinfo='skip',
+                            hoverinfo='all',
                             unselected=dict(marker=dict(opacity=self.state.alpha)),
                             meta=self._scatter_id)
         if self._viewer_state.using_rectilinear:
             scatter = Scatter(**scatter_info)
         else:
             theta_unit = 'degrees' if self.view.state.using_degrees else 'radians'
             scatter_info.update(thetaunit=theta_unit)
```

### Comparing `glue-plotly-0.5.1/glue_plotly/viewers/scatter/viewer.py` & `glue-plotly-0.6.0/glue_plotly/viewers/scatter/viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 from glue_jupyter.common.state_widgets.layer_scatter import ScatterLayerStateWidget
 from glue_jupyter.registries import viewer_registry
 
 from .layer_artist import PlotlyScatterLayerArtist
 from glue_plotly.viewers import PlotlyBaseView
 
 
+__all__ = ["PlotlyScatterView"]
+
+
 @viewer_registry("plotly_scatter")
 class PlotlyScatterView(PlotlyBaseView):
 
     tools = ['plotly:home', 'plotly:zoom', 'plotly:pan', 'plotly:xrange',
-             'plotly:yrange', 'plotly:rectangle', 'plotly:lasso']
+             'plotly:yrange', 'plotly:rectangle', 'plotly:lasso', 'plotly:hover']
 
     allow_duplicate_data = False
     allow_duplicate_subset = False
     large_data_size = 1e7
 
     _state_cls = ScatterViewerState
     _options_cls = ScatterViewerStateWidget
```

### Comparing `glue-plotly-0.5.1/glue_plotly/web/export_plotly.py` & `glue-plotly-0.6.0/glue_plotly/web/export_plotly.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/web/qt/__init__.py` & `glue-plotly-0.6.0/glue_plotly/web/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/web/qt/exporter.py` & `glue-plotly-0.6.0/glue_plotly/web/qt/exporter.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/web/qt/exporter.ui` & `glue-plotly-0.6.0/glue_plotly/web/qt/exporter.ui`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/web/qt/tests/test_exporter.py` & `glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly/web/qt/tests/test_plotly.py` & `glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_plotly.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.5.1/glue_plotly.egg-info/SOURCES.txt` & `glue-plotly-0.6.0/glue_plotly.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 codecov.yml
 setup.cfg
 setup.py
 tox.ini
 .github/release.yml
 .github/workflows/ci_workflows.yml
 .github/workflows/update-changelog.yaml
+doc/BqplotToolbarHighlighted.png
+doc/PlotlyViewerExample.ipynb
+doc/QtChartStudioExport.gif
+doc/QtToolbarExport.gif
 glue_plotly/__init__.py
 glue_plotly/conftest.py
 glue_plotly/export_dialog.py
 glue_plotly/logo.png
 glue_plotly/logo.svg
 glue_plotly/save_hover.py
 glue_plotly/save_hover.ui
@@ -72,16 +76,21 @@
 glue_plotly/html_exporters/qt/tests/test_scatter2d.py
 glue_plotly/html_exporters/qt/tests/test_scatter3d.py
 glue_plotly/html_exporters/qt/tests/test_table.py
 glue_plotly/viewers/__init__.py
 glue_plotly/viewers/common/__init__.py
 glue_plotly/viewers/common/tools.py
 glue_plotly/viewers/common/viewer.py
+glue_plotly/viewers/common/tests/__init__.py
+glue_plotly/viewers/common/tests/test_tools.py
+glue_plotly/viewers/common/tests/utils.py
+glue_plotly/viewers/histogram/__init__.py
 glue_plotly/viewers/histogram/layer_artist.py
 glue_plotly/viewers/histogram/viewer.py
+glue_plotly/viewers/scatter/__init__.py
 glue_plotly/viewers/scatter/layer_artist.py
 glue_plotly/viewers/scatter/viewer.py
 glue_plotly/web/__init__.py
 glue_plotly/web/export_plotly.py
 glue_plotly/web/qt/__init__.py
 glue_plotly/web/qt/exporter.py
 glue_plotly/web/qt/exporter.ui
```

### Comparing `glue-plotly-0.5.1/setup.cfg` & `glue-plotly-0.6.0/setup.cfg`

 * *Files identical despite different names*

