# Comparing `tmp/GenomicRanges-0.4.8.tar.gz` & `tmp/GenomicRanges-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenomicRanges-0.4.8.tar", last modified: Fri Jan  5 06:46:09 2024, max compression
+gzip compressed data, was "GenomicRanges-0.4.9.tar", last modified: Mon Jan 22 00:20:57 2024, max compression
```

## Comparing `GenomicRanges-0.4.8.tar` & `GenomicRanges-0.4.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.043032 GenomicRanges-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.027032 GenomicRanges-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.031032 GenomicRanges-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-01-05 06:46:09.043032 GenomicRanges-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.031032 GenomicRanges-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.035032 GenomicRanges-0.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-05 06:46:09.043032 GenomicRanges-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.027032 GenomicRanges-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.043032 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-01-05 06:46:08.000000 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-05 06:46:09.000000 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 06:46:08.000000 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 06:45:17.000000 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-05 06:46:08.000000 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-05 06:46:08.000000 GenomicRanges-0.4.8/src/GenomicRanges.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.035032 GenomicRanges-0.4.8/src/genomicranges/
--rw-r--r--   0 runner    (1001) docker     (127)    91903 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/GenomicRanges.py
--rw-r--r--   0 runner    (1001) docker     (127)    26386 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/GenomicRangesList.py
--rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/SeqInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.035032 GenomicRanges-0.4.8/src/genomicranges/io/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/io/gtf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/io/ucsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/src/genomicranges/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:46:09.039032 GenomicRanges-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_SeqInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_binnedAvg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_inter_range_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_methods_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_methods_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_methods_flank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_methods_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_methods_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_methods_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_seqInfo_trim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_set_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_gr_tiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_grl_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_grl_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tests/test_ucsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-01-05 06:45:10.000000 GenomicRanges-0.4.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.793883 GenomicRanges-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.777883 GenomicRanges-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.781883 GenomicRanges-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-01-22 00:20:57.793883 GenomicRanges-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.785883 GenomicRanges-0.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.785883 GenomicRanges-0.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-22 00:20:57.793883 GenomicRanges-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.781883 GenomicRanges-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.793883 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-01-22 00:20:57.000000 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-22 00:20:57.000000 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 00:20:57.000000 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 00:20:00.000000 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-22 00:20:57.000000 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-22 00:20:57.000000 GenomicRanges-0.4.9/src/GenomicRanges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.785883 GenomicRanges-0.4.9/src/genomicranges/
+-rw-r--r--   0 runner    (1001) docker     (127)    91903 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/GenomicRanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26386 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/GenomicRangesList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21454 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/SeqInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.789883 GenomicRanges-0.4.9/src/genomicranges/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/io/gtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/io/ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/src/genomicranges/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 00:20:57.793883 GenomicRanges-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_SeqInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_binnedAvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_inter_range_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_methods_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_methods_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_methods_flank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_methods_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_methods_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_methods_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_seqInfo_trim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_set_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_gr_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_grl_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_grl_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tests/test_ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-01-22 00:19:43.000000 GenomicRanges-0.4.9/tox.ini
```

### Comparing `GenomicRanges-0.4.8/.coveragerc` & `GenomicRanges-0.4.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/.github/workflows/pypi-publish.yml` & `GenomicRanges-0.4.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/.github/workflows/pypi-test.yml` & `GenomicRanges-0.4.9/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/.gitignore` & `GenomicRanges-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/.pre-commit-config.yaml` & `GenomicRanges-0.4.9/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   rev: 23.12.1
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: v0.1.9
+  rev: v0.1.13
   hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
 
 ## If like to embrace black styles even in the docs:
 # - repo: https://github.com/asottile/blacken-docs
 #   rev: v1.13.0
```

### Comparing `GenomicRanges-0.4.8/CHANGELOG.md` & `GenomicRanges-0.4.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # Changelog
 
-## Version 0.4.0 to 0.4.5
+## Version 0.4.9
+
+Bring `SeqInfo` upto speed with the rest of the class implementations. Added subset and pretty print functionality.
+
+## Version 0.4.0 to 0.4.8
 
 This is a complete rewrite of both these classes following the functional paradigm from our [developer notes](https://github.com/BiocPy/developer_guide#use-functional-discipline).
 
 `GenomicRanges` is now closer to Bioconductor's GenomicRanges class both in the design and implementation.
 
 The package does not rely on pandas anymore. While we try to provide backwards compatibility to construct a GenomicRanges object from a pandas dataframe using the `from_pandas` method, please note that the default constructor to genomic ranges does not accept a pandas data frame anymore!
 
 Most range based methods have been reimplemented and the heavy lifting is done in the [IRanges package](https://github.com/BiocPy/IRanges) for interval operations. The package indirectly depends on [NCLS](https://github.com/pyranges/ncls) interval tree data structure to perform search and overlap operations.
 
 Tests, documentation and readme has been updated to reflect these changes.
 
 ## Version 0.3.0
+
 This release migrates the package to a more palatable Google's Python style guide. A major modification to the package is with casing, all `camelCase` methods, functions and parameters are now `snake_case`.
 
 In addition, docstrings and documentation has been updated to use sphinx's features of linking objects to their types. Sphinx now also documents private and special dunder methods (e.g. `__getitem__`, `__copy__` etc). Intersphinx has been updated to link to references from dependent packages.
 
 Configuration for flake8, ruff and black has been added to pyproject.toml and setup.cfg to be less annoying.
 
 Finally, pyscaffold has been updated to use "myst-parser" as the markdown compiler instead of recommonmark. As part of the pyscaffold setup, one may use pre-commits to run some of the routine tasks of linting and formatting before every commit. While this is sometimes annoying and can be ignored with `--no-verify`, it brings some consistency to the code base.
 
 ## Version 0.2
+
 - Now uses BiocFrame as the underlying class
 - Implement interval based operations
 - update documentation, readme
 - comprehensive tests
 
 ## Version 0.1
```

### Comparing `GenomicRanges-0.4.8/CONTRIBUTING.md` & `GenomicRanges-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/LICENSE.txt` & `GenomicRanges-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/PKG-INFO` & `GenomicRanges-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenomicRanges
-Version: 0.4.8
+Version: 0.4.9
 Summary: Container class to represent and operate over genomic regions and annotations.
 Home-page: https://github.com/BiocPy/GenomicRanges
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/GenomicRanges
 Platform: any
```

### Comparing `GenomicRanges-0.4.8/README.md` & `GenomicRanges-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/docs/Makefile` & `GenomicRanges-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/docs/changelog.md` & `GenomicRanges-0.4.9/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # Changelog
 
-## Version 0.4.0 to 0.4.5
+## Version 0.4.9
+
+Bring `SeqInfo` upto speed with the rest of the class implementations. Added subset and pretty print functionality.
+
+## Version 0.4.0 to 0.4.8
 
 This is a complete rewrite of both these classes following the functional paradigm from our [developer notes](https://github.com/BiocPy/developer_guide#use-functional-discipline).
 
 `GenomicRanges` is now closer to Bioconductor's GenomicRanges class both in the design and implementation.
 
 The package does not rely on pandas anymore. While we try to provide backwards compatibility to construct a GenomicRanges object from a pandas dataframe using the `from_pandas` method, please note that the default constructor to genomic ranges does not accept a pandas data frame anymore!
 
 Most range based methods have been reimplemented and the heavy lifting is done in the [IRanges package](https://github.com/BiocPy/IRanges) for interval operations. The package indirectly depends on [NCLS](https://github.com/pyranges/ncls) interval tree data structure to perform search and overlap operations.
 
 Tests, documentation and readme has been updated to reflect these changes.
 
 ## Version 0.3.0
+
 This release migrates the package to a more palatable Google's Python style guide. A major modification to the package is with casing, all `camelCase` methods, functions and parameters are now `snake_case`.
 
 In addition, docstrings and documentation has been updated to use sphinx's features of linking objects to their types. Sphinx now also documents private and special dunder methods (e.g. `__getitem__`, `__copy__` etc). Intersphinx has been updated to link to references from dependent packages.
 
 Configuration for flake8, ruff and black has been added to pyproject.toml and setup.cfg to be less annoying.
 
 Finally, pyscaffold has been updated to use "myst-parser" as the markdown compiler instead of recommonmark. As part of the pyscaffold setup, one may use pre-commits to run some of the routine tasks of linting and formatting before every commit. While this is sometimes annoying and can be ignored with `--no-verify`, it brings some consistency to the code base.
 
 ## Version 0.2
+
 - Now uses BiocFrame as the underlying class
 - Implement interval based operations
 - update documentation, readme
 - comprehensive tests
 
 ## Version 0.1
```

### Comparing `GenomicRanges-0.4.8/docs/conf.py` & `GenomicRanges-0.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/docs/index.md` & `GenomicRanges-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/docs/readme.md` & `GenomicRanges-0.4.9/docs/readme.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/docs/tutorial.md` & `GenomicRanges-0.4.9/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/pyproject.toml` & `GenomicRanges-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/setup.cfg` & `GenomicRanges-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/setup.py` & `GenomicRanges-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/GenomicRanges.egg-info/PKG-INFO` & `GenomicRanges-0.4.9/src/GenomicRanges.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenomicRanges
-Version: 0.4.8
+Version: 0.4.9
 Summary: Container class to represent and operate over genomic regions and annotations.
 Home-page: https://github.com/BiocPy/GenomicRanges
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/GenomicRanges
 Platform: any
```

### Comparing `GenomicRanges-0.4.8/src/GenomicRanges.egg-info/SOURCES.txt` & `GenomicRanges-0.4.9/src/GenomicRanges.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/genomicranges/GenomicRanges.py` & `GenomicRanges-0.4.9/src/genomicranges/GenomicRanges.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/genomicranges/GenomicRangesList.py` & `GenomicRanges-0.4.9/src/genomicranges/GenomicRangesList.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/genomicranges/__init__.py` & `GenomicRanges-0.4.9/src/genomicranges/__init__.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/genomicranges/io/gtf.py` & `GenomicRanges-0.4.9/src/genomicranges/io/gtf.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/genomicranges/io/ucsc.py` & `GenomicRanges-0.4.9/src/genomicranges/io/ucsc.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/src/genomicranges/utils.py` & `GenomicRanges-0.4.9/src/genomicranges/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,22 @@
         return np.array(strand, dtype=np.int8)
 
     raise TypeError(
         "'strand' must be either a numpy vector, a list of integers or strings representing strand."
     )
 
 
+def _sanitize_vec(x: Sequence):
+    if isinstance(x, np.ma.MaskedArray):
+        x.filled(fill_value=None)
+        return x.tolist()
+
+    return list(x)
+
+
 def _sanitize_strand_search_ops(query_strand, subject_strand):
     query_strand = REV_STRAND_MAP[query_strand]
     subject_strand = REV_STRAND_MAP[subject_strand]
 
     out = None
 
     if query_strand == "+":
```

### Comparing `GenomicRanges-0.4.8/tests/test_SeqInfo.py` & `GenomicRanges-0.4.9/tests/test_SeqInfo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from genomicranges.SeqInfo import SeqInfo, merge_SeqInfo
 from random import random
 import pytest
+import numpy as np
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def test_create_SeqInfo():
@@ -46,14 +47,77 @@
     )
 
     with pytest.raises(ValueError) as ex:
         si.set_seqnames([None, "chrB", "chrC"])
     assert str(ex.value).find("list of strings") >= 0
 
 
+def test_create_seqInfo_numpy():
+    si = SeqInfo(
+        ["chrA", "chrB", "chrC"],
+        np.array([10, None, 2200]),
+        np.array([None, True, False]),
+        ["hg19", "hg38", None],
+    )
+
+    with pytest.raises(ValueError) as ex:
+        si.set_seqnames([None, "chrB", "chrC"])
+    assert str(ex.value).find("list of strings") >= 0
+
+
+def test_create_seqInfo_numpy_masked():
+    si = SeqInfo(
+        ["chrA", "chrB", "chrC"],
+        np.ma.MaskedArray([10, None, 2200], mask=[0, 1, 0]),
+        np.array([None, True, False]),
+        ["hg19", "hg38", None],
+    )
+
+    assert isinstance(si, SeqInfo)
+
+
+def test_create_empty():
+    si = SeqInfo.empty()
+
+    with pytest.raises(ValueError) as ex:
+        si.set_seqnames([None, "chrB", "chrC"])
+
+
+def test_subset_seqinfo_modifiers():
+    circ = [random() < 0.5 for _ in range(3)]
+    seq = SeqInfo(
+        seqnames=["chr1", "chr2", "chr3"],
+        seqlengths=range(100, 103),
+        is_circular=circ,
+        genome="hg19",
+    )
+
+    seq.seqnames = ["rch1", "rch2", "rch3"]
+    assert seq.seqnames == ["rch1", "rch2", "rch3"]
+
+    new_seq = seq.set_genome("hg38")
+    assert new_seq.genome == ["hg38"] * 3
+
+
+def test_subset_seqinfo():
+    circ = [random() < 0.5 for _ in range(3)]
+    seq = SeqInfo(
+        seqnames=["chr1", "chr2", "chr3"],
+        seqlengths=range(100, 103),
+        is_circular=circ,
+        genome="hg19",
+    )
+
+    subset = seq[["chr2", "chr3"]]
+
+    assert isinstance(subset, SeqInfo)
+    assert subset.seqnames == ["chr2", "chr3"]
+    assert subset.seqlengths == [101, 102]
+
+
 def test_merge_SeqInfo():
     seq = SeqInfo(
         seqnames=["chr1", "chr2", "chr3"],
         seqlengths=range(100, 103),
         is_circular=[False, True, False],
         genome="hg19",
     )
```

### Comparing `GenomicRanges-0.4.8/tests/test_gr_binnedAvg.py` & `GenomicRanges-0.4.9/tests/test_gr_binnedAvg.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_comparisons.py` & `GenomicRanges-0.4.9/tests/test_gr_comparisons.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_initialize.py` & `GenomicRanges-0.4.9/tests/test_gr_initialize.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_inter_range_methods.py` & `GenomicRanges-0.4.9/tests/test_gr_inter_range_methods.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_methods_basic.py` & `GenomicRanges-0.4.9/tests/test_gr_methods_basic.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_methods_coverage.py` & `GenomicRanges-0.4.9/tests/test_gr_methods_coverage.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_methods_flank.py` & `GenomicRanges-0.4.9/tests/test_gr_methods_flank.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_methods_other.py` & `GenomicRanges-0.4.9/tests/test_gr_methods_other.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_methods_resize.py` & `GenomicRanges-0.4.9/tests/test_gr_methods_resize.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_methods_search.py` & `GenomicRanges-0.4.9/tests/test_gr_methods_search.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_misc.py` & `GenomicRanges-0.4.9/tests/test_gr_misc.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_overlaps.py` & `GenomicRanges-0.4.9/tests/test_gr_overlaps.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_seqInfo_trim.py` & `GenomicRanges-0.4.9/tests/test_gr_seqInfo_trim.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_set_ops.py` & `GenomicRanges-0.4.9/tests/test_gr_set_ops.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_gr_tiling.py` & `GenomicRanges-0.4.9/tests/test_gr_tiling.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_grl_initialize.py` & `GenomicRanges-0.4.9/tests/test_grl_initialize.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tests/test_grl_methods.py` & `GenomicRanges-0.4.9/tests/test_grl_methods.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.4.8/tox.ini` & `GenomicRanges-0.4.9/tox.ini`

 * *Files identical despite different names*

