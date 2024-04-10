# Comparing `tmp/fmu-sumo-1.2.0.tar.gz` & `tmp/fmu-sumo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmu-sumo-1.2.0.tar", last modified: Wed Mar 27 16:06:14 2024, max compression
+gzip compressed data, was "fmu-sumo-1.2.1.tar", last modified: Wed Apr 10 09:04:44 2024, max compression
```

## Comparing `fmu-sumo-1.2.0.tar` & `fmu-sumo-1.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.836986 fmu-sumo-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/build_docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_manage_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_read_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_write_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.github/workflows/run_tests_access_no_access_login.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/_static/equinor-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/_static/equinor-logo2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/_static/equinor_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/_static/equinor_logo_only.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/_templates/layout.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2058 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/explorer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     9485 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/examples/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/examples/tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.836986 fmu-sumo-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/src/fmu/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.840986 fmu-sumo-1.2.0/src/fmu/sumo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.844986 fmu-sumo-1.2.0/src/fmu/sumo/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-27 16:06:14.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.844986 fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/realization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.844986 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_child_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_document_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/case_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/cube_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/dictionary_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/polygons_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/surface_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/table_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/table_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/src/fmu/sumo/explorer/timefilter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/src/fmu_sumo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-03-27 16:06:14.000000 fmu-sumo-1.2.0/src/fmu_sumo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-27 16:06:14.000000 fmu-sumo-1.2.0/src/fmu_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:06:14.000000 fmu-sumo-1.2.0/src/fmu_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-27 16:06:14.000000 fmu-sumo-1.2.0/src/fmu_sumo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-27 16:06:14.000000 fmu-sumo-1.2.0/src/fmu_sumo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.836986 fmu-sumo-1.2.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/tests/data/test_case_080/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/data/test_case_080/case2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:06:14.848986 fmu-sumo-1.2.0/tests/test_access/
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_access/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_access/tst_access_drogon_manage_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_access/tst_access_drogon_read_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_access/tst_access_drogon_write_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_access/tst_access_no_access_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-27 16:06:10.000000 fmu-sumo-1.2.0/tests/test_objects_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.244065 fmu-sumo-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.244065 fmu-sumo-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/build_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.github/workflows/run_tests_access_no_access_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.244065 fmu-sumo-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor-logo2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_static/equinor_logo_only.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/_templates/layout.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2058 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/explorer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/examples/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/examples/tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.240065 fmu-sumo-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/sumo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/sumo/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.248065 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/realization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.252065 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/src/fmu/sumo/explorer/timefilter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 09:04:44.000000 fmu-sumo-1.2.1/src/fmu_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.252065 fmu-sumo-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.240065 fmu-sumo-1.2.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.252065 fmu-sumo-1.2.1/tests/data/test_case_080/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/data/test_case_080/case2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:04:44.256065 fmu-sumo-1.2.1/tests/test_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_manage_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_read_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_write_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_access/tst_access_no_access_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 09:04:39.000000 fmu-sumo-1.2.1/tests/test_objects_table.py
```

### Comparing `fmu-sumo-1.2.0/.github/pull_request_template.md` & `fmu-sumo-1.2.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/build_docs.yaml` & `fmu-sumo-1.2.1/.github/workflows/build_docs.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/publish_release.yaml` & `fmu-sumo-1.2.1/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_manage_login.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_login.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_manage_sharedkey.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_read_login.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_login.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_read_sharedkey.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_write_login.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_login.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_drogon_write_sharedkey.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.github/workflows/run_tests_access_no_access_login.yaml` & `fmu-sumo-1.2.1/.github/workflows/run_tests_access_no_access_login.yaml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/.gitignore` & `fmu-sumo-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/CONTRIBUTING.md` & `fmu-sumo-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/LICENSE` & `fmu-sumo-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/PKG-INFO` & `fmu-sumo-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-sumo
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for interacting with Sumo in an FMU setting
 Author: Equinor
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fmu-sumo-1.2.0/SECURITY.md` & `fmu-sumo-1.2.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/docs/_static/equinor-logo.png` & `fmu-sumo-1.2.1/docs/_static/equinor-logo.png`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/docs/_static/equinor-logo2.jpg` & `fmu-sumo-1.2.1/docs/_static/equinor-logo2.jpg`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/docs/_static/equinor_logo.jpg` & `fmu-sumo-1.2.1/docs/_static/equinor_logo.jpg`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/docs/_static/equinor_logo_only.jpg` & `fmu-sumo-1.2.1/docs/_static/equinor_logo_only.jpg`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/docs/conf.py` & `fmu-sumo-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/docs/explorer.rst` & `fmu-sumo-1.2.1/docs/explorer.rst`

 * *Files 3% similar despite different names*

```diff
@@ -219,14 +219,20 @@
 
     sumo = Explorer() 
 
     case = sumo.get_case_by_uuid("1234567")
 
     surfaces = case.surfaces.filter(iteration="iter-0")
 
+    contents = surfaces.contents
+    
+    surfaces = surfaces.filter(
+        content=contents[0]
+        )
+
     names = surfaces.names 
 
     surfaces = surfaces.filter(
         name=names[0]
     )
 
     tagnames = surfaces.tagnames 
@@ -239,15 +245,16 @@
     vertical_domain = surfaces.filter(vertical_domain = "depth")
 
 
 The `SurfaceCollection.filter` method takes the following parameters:
 
 * uuid
 * name 
-* tagname
+* tagname 
+* content 
 * dataformat
 * iteration 
 * realization 
 * aggregation
 * stage 
 * time
 * stratigraphic
@@ -276,15 +283,16 @@
 
     # get names of aggregated surfaces 
     names = surfaces.names
 
 We can get list of filter values for the following properties:
 
 * names
-* tagnames
+* contents 
+* tagnames 
 * dataformats
 * iterations 
 * realizations
 * aggregations 
 * stages 
 * timestamps
 * intervals
@@ -300,14 +308,15 @@
 
     sumo = Explorer() 
 
     case = sumo.get_case_by_uuid("1234567")
 
     surface = case.surfaces[0]
 
+    print(surface.content)
     print(surface.uuid)
     print(surface.name)
     print(surface.tagname)
     print(surface.dataformat)
     print(surface.stratigraphic)
     print(surface.vertical_domain)
 
@@ -481,14 +490,15 @@
 
     sumo = Explorer() 
 
     case = sumo.get_case_by_uuid("1234567")
 
     surfaces = case.surfaces.filter(
         stage="realization",
+        content="depth",
         iteration="iter-0",
         name="Valysar Fm.",
         tagname="FACIES_Fraction_Channel"
         stratigraphic="false"
         vertical_domain="depth"
     )
```

### Comparing `fmu-sumo-1.2.0/docs/index.rst` & `fmu-sumo-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/examples/explorer.ipynb` & `fmu-sumo-1.2.1/examples/explorer.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997718383311603%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(8, '\\n'), (9, '# Get available contents\\n'), (10, "*

 * *            '\'print("Contents:", surfs.contents)\\n\'), (11, \'\\n\'), (12, \'# Filter on '*

 * *            'content\\n\'), (13, \'surfs = surfs.filter(content="depth")\\n\'), (39, \'# Select '*

 * *            'one surface instance\\n\'), (43, \'print("Uuid:", surf.uuid)\\n\'), (45, '*

 * *            '\'print("Content:", surf.content)\\n\'), (50, \'print("vertical domain:", '*

 * *            "surf.vertical_domain)\\n')], delete: [ […]*

```diff
@@ -108,14 +108,20 @@
                 "\n",
                 "# Get available iterations\n",
                 "print(\"Iterations:\", surfs.iterations)\n",
                 "\n",
                 "# Filter on iteration\n",
                 "surfs = surfs.filter(iteration=\"iter-0\")\n",
                 "\n",
+                "# Get available contents\n",
+                "print(\"Contents:\", surfs.contents)\n",
+                "\n",
+                "# Filter on content\n",
+                "surfs = surfs.filter(content=\"depth\")\n",
+                "\n",
                 "# Get available names\n",
                 "print(\"Names:\", surfs.names)\n",
                 "\n",
                 "# Filter on name\n",
                 "surfs = surfs.filter(name=\"Valysar Fm.\")\n",
                 "\n",
                 "# Filter on format\n",
@@ -132,26 +138,26 @@
                 "\n",
                 "for surf in surfs:\n",
                 "    print(\"\\n\")\n",
                 "    print(\"ID:\", surf.uuid)\n",
                 "    print(\"Format:\", surf.dataformat)\n",
                 "    print(\"Realization:\", surf.realization)\n",
                 "\n",
-                "# Select surface instance\n",
+                "# Select one surface instance\n",
                 "surf = surfs[0]\n",
                 "\n",
                 "print(\"\\nSelected surface:\")\n",
-                "print(\"ID:\", surf.uuid)\n",
+                "print(\"Uuid:\", surf.uuid)\n",
                 "print(\"Name:\", surf.name)\n",
+                "print(\"Content:\", surf.content)\n",
                 "print(\"Tagname:\", surf.tagname)\n",
                 "print(\"Format:\", surf.dataformat)\n",
                 "print(\"Iteration:\", surf.iteration)\n",
                 "print(\"Realization:\", surf.realization)\n",
-                "print(\"stratigraphic\", surf.stratigraphic)\n",
-                "print(\"vertical domain\", surf.vertical_domain)\n",
+                "print(\"vertical domain:\", surf.vertical_domain)\n",
                 "\n",
                 "# xtgeo.RegularSurface\n",
                 "reg_surf = surf.to_regular_surface()\n",
                 "reg_surf.quickplot()"
             ]
         },
         {
```

### Comparing `fmu-sumo-1.2.0/examples/tables.ipynb` & `fmu-sumo-1.2.1/examples/tables.ipynb`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/pyproject.toml` & `fmu-sumo-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/_utils.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/_utils.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/aggregation.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/aggregation.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/observation.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/observation.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/contexts/realization.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/contexts/realization.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/explorer.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/__init__.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_child.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
     @property
     def name(self) -> str:
         """Object name"""
         return self._get_property(["data", "name"])
 
     @property
+    def content(self) -> str:
+        """Content"""
+        return self._get_property(["data", "content"])
+
+    @property
     def tagname(self) -> str:
         """Object tagname"""
         return self._get_property(["data", "tagname"])
 
     @property
     def stratigraphic(self) -> str:
         """Object stratigraphic"""
```

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_child_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_child_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_document.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/_document_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/_document_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/case.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/case_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/case_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/cube.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/cube_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/cube_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/dictionary.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/dictionary_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/dictionary_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/polygons.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/polygons_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/polygons_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/surface.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/surface_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/surface_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/table.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/table_aggregated.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_aggregated.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/objects/table_collection.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/objects/table_collection.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/pit.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/pit.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu/sumo/explorer/timefilter.py` & `fmu-sumo-1.2.1/src/fmu/sumo/explorer/timefilter.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/src/fmu_sumo.egg-info/PKG-INFO` & `fmu-sumo-1.2.1/src/fmu_sumo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-sumo
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for interacting with Sumo in an FMU setting
 Author: Equinor
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fmu-sumo-1.2.0/src/fmu_sumo.egg-info/SOURCES.txt` & `fmu-sumo-1.2.1/src/fmu_sumo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/context.py` & `fmu-sumo-1.2.1/tests/context.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/data/test_case_080/case2.json` & `fmu-sumo-1.2.1/tests/data/test_case_080/case2.json`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/test_access/README.md` & `fmu-sumo-1.2.1/tests/test_access/README.md`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/test_access/tst_access_drogon_manage_login.py` & `fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_manage_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/test_access/tst_access_drogon_read_login.py` & `fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_read_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/test_access/tst_access_drogon_write_login.py` & `fmu-sumo-1.2.1/tests/test_access/tst_access_drogon_write_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/test_access/tst_access_no_access_login.py` & `fmu-sumo-1.2.1/tests/test_access/tst_access_no_access_login.py`

 * *Files identical despite different names*

### Comparing `fmu-sumo-1.2.0/tests/test_explorer.py` & `fmu-sumo-1.2.1/tests/test_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,21 @@
     real_surfs = real_surfs.filter(name="Valysar Fm.")
     assert len(real_surfs) == 56
 
     for surf in real_surfs:
         assert surf.iteration == "iter-0"
         assert surf.name == "Valysar Fm."
 
+    # filter on content
+    non_valid_content_surfs = real_surfs.filter(content="___not_valid")
+    assert len(non_valid_content_surfs) == 0
+
+    real_surfs = real_surfs.filter(content="depth")
+    assert len(real_surfs) == 56
+
     # filter on tagname
     non_valid_tagname_surfs = real_surfs.filter(tagname="___not_valid")
     assert len(non_valid_tagname_surfs) == 0
 
     real_surfs = real_surfs.filter(tagname="FACIES_Fraction_Channel")
     assert len(real_surfs) == 4
```

### Comparing `fmu-sumo-1.2.0/tests/test_objects_table.py` & `fmu-sumo-1.2.1/tests/test_objects_table.py`

 * *Files identical despite different names*

