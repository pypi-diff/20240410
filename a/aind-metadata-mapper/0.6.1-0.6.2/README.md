# Comparing `tmp/aind-metadata-mapper-0.6.1.tar.gz` & `tmp/aind-metadata-mapper-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-metadata-mapper-0.6.1.tar", last modified: Mon Apr  8 17:53:02 2024, max compression
+gzip compressed data, was "aind-metadata-mapper-0.6.2.tar", last modified: Wed Apr 10 20:05:35 2024, max compression
```

## Comparing `aind-metadata-mapper-0.6.1.tar` & `aind-metadata-mapper-0.6.2.tar`

### file list

```diff
@@ -1,81 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.314105 aind-metadata-mapper-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.314105 aind-metadata-mapper-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 17:52:51.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.318105 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 17:53:02.000000 aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.314105 aind-metadata-mapper-0.6.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.322106 aind-metadata-mapper-0.6.1/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:53:02.326105 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/resources/mesoscope/expected_session.json
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_bergamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-08 17:52:50.000000 aind-metadata-mapper-0.6.1/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.353698 aind-metadata-mapper-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/mismatched_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.353698 aind-metadata-mapper-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.361698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 20:05:35.000000 aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.357698 aind-metadata-mapper-0.6.2/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.365698 aind-metadata-mapper-0.6.2/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.369698 aind-metadata-mapper-0.6.2/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.369698 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/resources/neuropixels/sync_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_bergamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:35.373698 aind-metadata-mapper-0.6.2/tests/test_neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-10 20:05:25.000000 aind-metadata-mapper-0.6.2/tests/test_neuropixels/utils.py
```

### Comparing `aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind-metadata-mapper-0.6.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/.github/workflows/tag_and_publish.yml` & `aind-metadata-mapper-0.6.2/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/.github/workflows/test_and_lint.yml` & `aind-metadata-mapper-0.6.2/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/.gitignore` & `aind-metadata-mapper-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/LICENSE` & `aind-metadata-mapper-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/PKG-INFO` & `aind-metadata-mapper-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.1
+Version: 0.6.2
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,14 +17,15 @@
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: furo; extra == "dev"
+Requires-Dist: pyyaml>=6.0.0; extra == "dev"
 
 # aind-metadata-mapper
 
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
```

### Comparing `aind-metadata-mapper-0.6.1/README.md` & `aind-metadata-mapper-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/doc_template/Makefile` & `aind-metadata-mapper-0.6.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/doc_template/make.bat` & `aind-metadata-mapper-0.6.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/doc_template/source/_static/dark-logo.svg` & `aind-metadata-mapper-0.6.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/doc_template/source/_static/favicon.ico` & `aind-metadata-mapper-0.6.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/doc_template/source/_static/light-logo.svg` & `aind-metadata-mapper-0.6.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/doc_template/source/conf.py` & `aind-metadata-mapper-0.6.2/doc_template/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration file for the Sphinx documentation builder."""
+
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 from datetime import date
 
 # -- Path Setup --------------------------------------------------------------
```

### Comparing `aind-metadata-mapper-0.6.1/examples/bergamo_session.py` & `aind-metadata-mapper-0.6.2/examples/bergamo_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Example of how to use the bergamo session module"""
+
 from datetime import datetime
 from pathlib import Path
 
 from aind_metadata_mapper.bergamo.session import (
     BergamoEtl,
     JobSettings,
     RawImageInfo,
```

### Comparing `aind-metadata-mapper-0.6.1/pyproject.toml` & `aind-metadata-mapper-0.6.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 dev = [
     'black',
     'coverage',
     'flake8',
     'interrogate',
     'isort',
     'Sphinx',
-    'furo'
+    'furo',
+    "pyyaml>=6.0.0",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "aind_metadata_mapper.__version__"}
```

### Comparing `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/bergamo/session.py` & `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/core.py` & `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/ephys/session.py` & `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/ephys/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         ephys_session["data_streams"] = []
 
         for stage, data_stream in zip(
             stage_logs, experiment_data["data_streams"]
         ):
             session_stream = {}
             session_stream["stream_start_time"] = datetime.strptime(
-                stage[0][0], "%Y/%m/%d %H:%M:%S.%f"
+               stage[0][0], "%Y/%m/%d %H:%M:%S.%f"
             )
             session_stream["stream_end_time"] = datetime.strptime(
                 stage[-1][0], "%Y/%m/%d %H:%M:%S.%f"
             )
             session_stream["stream_modalities"] = [Modality.ECEPHYS]
             session_stream["stick_microscopes"] = stick_microscopes
             session_stream["camera_names"] = camera_names
```

### Comparing `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/fib/session.py` & `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/fib/session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper/mesoscope/session.py` & `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind-metadata-mapper-0.6.2/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.1
+Version: 0.6.2
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,14 +17,15 @@
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: furo; extra == "dev"
+Requires-Dist: pyyaml>=6.0.0; extra == "dev"
 
 # aind-metadata-mapper
 
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
```

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind-metadata-mapper-0.6.2/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_description0.txt` & `aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/bergamo/example_metadata.txt.gz` & `aind-metadata-mapper-0.6.2/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/bergamo/expected_session.json` & `aind-metadata-mapper-0.6.2/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/ephys/ephys_session.json` & `aind-metadata-mapper-0.6.2/tests/resources/ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_main.csv` & `aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/ephys/newscale_surface_finding.csv` & `aind-metadata-mapper-0.6.2/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_main.xml` & `aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/ephys/settings_surface_finding.xml` & `aind-metadata-mapper-0.6.2/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_rig.json` & `aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/fib/000000_ophys_session.json` & `aind-metadata-mapper-0.6.2/tests/resources/fib/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_extract.json` & `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/example_platform.json` & `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/resources/mesoscope/expected_session.json` & `aind-metadata-mapper-0.6.2/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/test_bergamo.py` & `aind-metadata-mapper-0.6.2/tests/test_bergamo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Tests parsing of session information from bergamo rig."""
-
 import gzip
 import json
 import os
 import unittest
 from datetime import datetime, timezone
 from pathlib import Path
 from unittest.mock import MagicMock, call, patch
```

### Comparing `aind-metadata-mapper-0.6.1/tests/test_ephys.py` & `aind-metadata-mapper-0.6.2/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `aind-metadata-mapper-0.6.1/tests/test_fib.py` & `aind-metadata-mapper-0.6.2/tests/test_fib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests parsing of session information from fib rig."""
 
+import zoneinfo
 import json
 import os
 import unittest
-import zoneinfo
 from datetime import datetime
 from pathlib import Path
 
 from aind_data_schema.core.session import Session
 
 from aind_metadata_mapper.fib.session import FIBEtl, JobSettings
 
@@ -119,8 +119,9 @@
         job = etl_job1.run_job()
         self.assertEqual(
             self.expected_session, Session(**json.loads(job.data))
         )
 
 
 if __name__ == "__main__":
+
     unittest.main()
```

### Comparing `aind-metadata-mapper-0.6.1/tests/test_legacy_core.py` & `aind-metadata-mapper-0.6.2/tests/test_legacy_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests legacy BaseEtl class methods. We can remove this once the other jobs
  are ported over."""
+
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 from unittest import TestCase
 from unittest import main as unittest_main
 from unittest.mock import MagicMock, patch
```

### Comparing `aind-metadata-mapper-0.6.1/tests/test_mesoscope.py` & `aind-metadata-mapper-0.6.2/tests/test_mesoscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,23 +172,23 @@
         # mock vasculature image
         mock_image = Image.new("RGB", (100, 100))
         mock_image.tag = {306: ("2024:02:12 11:02:22",)}
         mock_open.return_value = mock_image
 
         # mock scanimage metadata
         mock_meta = [{}]
-        mock_meta[0][
-            "SI.hRoiManager.linesPerFrame"
-        ] = self.example_scanimage_meta["lines_per_frame"]
-        mock_meta[0][
-            "SI.hRoiManager.pixelsPerLine"
-        ] = self.example_scanimage_meta["pixels_per_line"]
-        mock_meta[0][
-            "SI.hRoiManager.scanZoomFactor"
-        ] = self.example_scanimage_meta["fov_scale_factor"]
+        mock_meta[0]["SI.hRoiManager.linesPerFrame"] = (
+            self.example_scanimage_meta["lines_per_frame"]
+        )
+        mock_meta[0]["SI.hRoiManager.pixelsPerLine"] = (
+            self.example_scanimage_meta["pixels_per_line"]
+        )
+        mock_meta[0]["SI.hRoiManager.scanZoomFactor"] = (
+            self.example_scanimage_meta["fov_scale_factor"]
+        )
         mock_scanimage.return_value = mock_meta
 
         extract = etl._extract()
         transformed_session = etl._transform(extract)
         for stream in transformed_session.data_streams:
             stream.stream_start_time = stream.stream_start_time.replace(
                 tzinfo=zoneinfo.ZoneInfo("UTC")
```

