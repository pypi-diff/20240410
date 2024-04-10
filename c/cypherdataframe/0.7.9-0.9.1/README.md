# Comparing `tmp/cypherdataframe-0.7.9.tar.gz` & `tmp/cypherdataframe-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.7.9.tar", last modified: Tue Sep  5 21:11:54 2023, max compression
+gzip compressed data, was "cypherdataframe-0.9.1.tar", last modified: Wed Apr 10 16:34:13 2024, max compression
```

## Comparing `cypherdataframe-0.7.9.tar` & `cypherdataframe-0.9.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.398779 cypherdataframe-0.7.9/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-09-05 21:11:54.398374 cypherdataframe-0.7.9/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.383880 cypherdataframe-0.7.9/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.7.9/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.7.9/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.7.9/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)    11070 2023-09-05 21:11:30.000000 cypherdataframe-0.7.9/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.386380 cypherdataframe-0.7.9/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1434 2023-09-01 17:45:35.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.387054 cypherdataframe-0.7.9/cypherdataframe/garner_domain/logistics/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:01:55.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/logistics/TransferBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/logistics/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.387523 cypherdataframe-0.7.9/cypherdataframe/garner_domain/measure/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:01:55.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/measure/MeasureBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/measure/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.388489 cypherdataframe-0.7.9/cypherdataframe/garner_domain/queries/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1322 2023-09-01 21:07:27.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/queries/AttachableTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1001 2023-07-11 22:52:04.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/queries/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.388951 cypherdataframe-0.7.9/cypherdataframe/garner_domain/reference/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      647 2023-07-11 23:02:18.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/reference/ReferenceBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/reference/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.390371 cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-07-11 23:02:18.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-07-11 23:02:18.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/AttainedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      692 2023-07-11 23:02:18.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      649 2023-07-11 23:02:18.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/ForecastedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.393020 cypherdataframe-0.7.9/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2641 2023-09-01 21:00:11.000000 cypherdataframe-0.7.9/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.7.9/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-07-11 22:49:50.000000 cypherdataframe-0.7.9/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.7.9/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2926 2023-09-01 20:58:26.000000 cypherdataframe-0.7.9/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2729 2023-09-01 21:00:38.000000 cypherdataframe-0.7.9/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.7.9/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.7.9/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.385511 cypherdataframe-0.7.9/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-09-05 21:11:54.000000 cypherdataframe-0.7.9/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2009 2023-09-05 21:11:54.000000 cypherdataframe-0.7.9/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-09-05 21:11:54.000000 cypherdataframe-0.7.9/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-09-05 21:11:54.000000 cypherdataframe-0.7.9/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-09-05 21:11:54.000000 cypherdataframe-0.7.9/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-09-05 21:11:54.398913 cypherdataframe-0.7.9/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-09-05 21:11:34.000000 cypherdataframe-0.7.9/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.394597 cypherdataframe-0.7.9/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.7.9/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.7.9/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.7.9/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.7.9/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.394896 cypherdataframe-0.7.9/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.7.9/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.396573 cypherdataframe-0.7.9/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.7.9/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.7.9/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.7.9/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.7.9/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.7.9/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-09-05 21:11:54.397939 cypherdataframe-0.7.9/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.7.9/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.7.9/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.7.9/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.7.9/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.7.9/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.7.9/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.7.9/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.310884 cypherdataframe-0.9.1/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2024-04-10 16:34:13.310650 cypherdataframe-0.9.1/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.298455 cypherdataframe-0.9.1/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)    11844 2024-03-11 19:52:52.000000 cypherdataframe-0.9.1/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.300612 cypherdataframe-0.9.1/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1434 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.301180 cypherdataframe-0.9.1/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.301658 cypherdataframe-0.9.1/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2543 2024-03-18 16:39:30.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.302455 cypherdataframe-0.9.1/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1486 2024-04-10 16:27:10.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/queries/AttachableTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1076 2024-02-13 20:56:34.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.303000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      652 2023-09-21 15:41:15.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.304329 cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      687 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      640 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      692 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      649 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.306120 cypherdataframe-0.9.1/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2756 2024-04-10 16:25:39.000000 cypherdataframe-0.9.1/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      860 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     3127 2024-02-13 20:57:05.000000 cypherdataframe-0.9.1/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2729 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-09-05 22:22:47.000000 cypherdataframe-0.9.1/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.299832 cypherdataframe-0.9.1/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2024-04-10 16:34:13.000000 cypherdataframe-0.9.1/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2009 2024-04-10 16:34:13.000000 cypherdataframe-0.9.1/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2024-04-10 16:34:13.000000 cypherdataframe-0.9.1/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2024-04-10 16:34:13.000000 cypherdataframe-0.9.1/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2024-04-10 16:34:13.000000 cypherdataframe-0.9.1/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2024-04-10 16:34:13.310989 cypherdataframe-0.9.1/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2024-04-10 16:33:54.000000 cypherdataframe-0.9.1/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.307898 cypherdataframe-0.9.1/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.9.1/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.9.1/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.9.1/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.9.1/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.308154 cypherdataframe-0.9.1/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.9.1/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.309383 cypherdataframe-0.9.1/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.9.1/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.9.1/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.9.1/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.9.1/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.9.1/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2024-04-10 16:34:13.310365 cypherdataframe-0.9.1/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.9.1/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.9.1/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.9.1/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.9.1/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.9.1/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.9.1/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.9.1/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/branch_maker.py` & `cypherdataframe-0.9.1/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/cypher.py` & `cypherdataframe-0.9.1/cypherdataframe/cypher.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,16 @@
             f"start_skip: {start_skip}, limit (chunk limit): {limit}"
         )
         this_query = Query(
             core_node=query.core_node,
             branches=query.branches,
             skip=skip,
             limit=step,
-            enforce_complete_chunks=query.enforce_complete_chunks
+            enforce_complete_chunks=query.enforce_complete_chunks,
+            disable_scan=query.disable_scan
         )
         start_time = time.time()
         df = query_to_dataframe(this_query, config)
 
         len_df = df.shape[0]
         print(f"rows returned {len_df}")
         print(f"--- {(time.time() - start_time)} seconds ---")
@@ -96,14 +97,22 @@
             'storage_time',
             'total_time'
         ]
     )
     df_meta.to_csv(meta_path, index=False)
 
 
+def __drop_gather_from_meta(
+        meta_path: str
+):
+    df_meta = pd.read_csv(meta_path)
+    df_meta = df_meta[df_meta['chunk_size'] > 0]
+    df_meta.to_csv(meta_path, index=False)
+
+
 def __add_to_meta(
     meta_path: str,
     increment: str,
     chunk_size: int,
     keys: int,
     rows: int,
     start_time,
@@ -153,65 +162,77 @@
         , gather_csv: bool = False
         , just_gather: bool = False
         , top_up: bool = False
         , deduplicate_gather: bool = False
         , first_chunk_set_size: int | None = None
         ) -> None:
     meta_path = f'{save_directory}/meta.csv'
+    if first_chunk_set_size is None and top_up:
+        first_chunk_set_size = 10
 
     if not os.path.isdir(meta_gather_dir):
         os.makedirs(meta_gather_dir)
 
     if not os.path.isdir(save_directory):
         os.makedirs(save_directory)
 
     if not os.path.isfile(meta_path):
         __make_meta(meta_path)
 
 
     process_start_time = time.time()
     df_meta = pd.read_csv(meta_path)
 
-
     if df_meta.shape[0] > 0:
         if ('gather' not in df_meta['increment'].values.tolist()) or top_up:
             df_meta_inc = df_meta[df_meta['chunk_size'] > 0]
             start_chunk = int(df_meta_inc['increment'].max()) + 1
             total_keys = df_meta_inc['keys'].sum()
+        elif just_gather:
+            pass
         else:
             print("Already Gathered")
             print()
             return None
     else:
         total_keys = 0
         start_chunk = 1
 
     exceptions = 0
     inc_chunk = 0
     runs_without_data = 0
-
+    this_chunk_size = chunk_size
     while not just_gather:
+        print("5")
         try:
             chunk_start_time = time.time()
             current_chunk = start_chunk + inc_chunk
 
             if current_chunk > max_total_chunks:
+                print("breaking")
                 break
             print()
             print(
                 f"Chunk: {current_chunk} "
                 f"Keys So Far: {total_keys} "
                 f"Time: {time.strftime('%H:%M:%S', time.localtime())}"
             )
 
+            if (first_chunk_set_size is not None) & (inc_chunk == 0):
+                this_chunk_size = first_chunk_set_size
+                this_step = first_chunk_set_size
+            else:
+                this_chunk_size = chunk_size
+                this_step = step
+
             df: pd.DataFrame | None = all_for_query_in_steps(
                 query
                 , config
-                , step=step
-                , limit=chunk_size
+                , step=this_step
+                , limit=this_chunk_size
                 , start_skip=total_keys
             )
             data_extracted_time = time.time()
             if df is not None:
                 df.to_csv(
                     f"{save_directory}/{table_name_root}_{current_chunk}.csv",
                     index=False
@@ -243,29 +264,29 @@
 
 
         __add_to_meta(
             meta_path,
             increment=current_chunk,
             keys=df_keys,
             rows=df_rows,
-            chunk_size=chunk_size,
+            chunk_size=this_chunk_size,
             start_time=datetime.fromtimestamp(chunk_start_time, tz=None),
             data_extracted_time=datetime.fromtimestamp(data_extracted_time, tz=None),
             data_stored_time=datetime.fromtimestamp(data_stored_time, tz=None),
             extraction_time=(data_extracted_time - chunk_start_time) / 60,
             storage_time=(data_stored_time - data_extracted_time) / 60,
             total_time=(data_stored_time - chunk_start_time) /60
         )
         total_keys += df_keys
         if df_rows < 1:
             runs_without_data += 1
         else:
             runs_without_data = 0
 
-        if df_keys < chunk_size and query.enforce_complete_chunks:
+        if df_keys < this_chunk_size and query.enforce_complete_chunks:
             print(f"Incomplete chunk with enforce_complete_chunks turned on")
             print("Chunk Done")
             break
 
         if runs_without_data == MAX_RUNS_WITHOUT_DATA:
             print(f"Consecutive runs_without_data: {runs_without_data} "
                   f"exceeded max: {MAX_RUNS_WITHOUT_DATA}")
@@ -281,14 +302,15 @@
         read_directory=save_directory,
         table_name_root=table_name_root,
         gather_csv=gather_csv,
         deduplicate_gather=deduplicate_gather
     )
     if (gather_success):
         df_meta = pd.read_csv(meta_path)
+        __drop_gather_from_meta(meta_path)
         __add_to_meta(
             meta_path,
             increment="gather",
             rows=0,
             keys=0,
             chunk_size=0,
             start_time=datetime.fromtimestamp(start_gather_time, tz=None),
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/logistics/TransferBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/logistics/TransferBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/measure/MeasureBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/measure/MeasureBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from datetime import datetime
 
 from cypherdataframe.model.Property import Property
 
 
 ID_PROP = Property(label='id', datatype=str, postfix="_id")
+QUANTITY_PROP = Property(label='quantity', datatype=str, postfix="_q")
 NUMBER_PROP = Property(label='number', datatype=str, postfix="_n")
+LOWER_MATID_PROP = Property(label='lowermaterialId', datatype=str, postfix="_mid")
 ID_PROP_COLLECT = Property(label='id', datatype=list[str], postfix="_id")
 ID_BRANCH_PROP = Property(label='id', datatype=str, postfix="_id")
 CODE_PROP = Property(label='code', datatype=str, postfix="_c")
 VALUE_PROP = Property(label='value', datatype=str, postfix="_v")
 OCCURSON_PROP = Property(label='occursOn', datatype=datetime, postfix="_o")
 OCCURSON_BRANCH_PROP = Property(label='occursOn', datatype=list[datetime], postfix="_o")
 CREATEDON_PROP = Property(label='createdOn', datatype=datetime, postfix="_cr")
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/queries/AttachableTableQuery.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/queries/AttachableTableQuery.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 @dataclass
 class AttachableTableQuery:
     attachable_label: str
     domain_label: str
     attachable_props: list[Property]
     post_label: str | None = None
     attachable_return_id: str = "a"
+    disable_scan: bool = False
+    relationship = None
+    away_from_core  = None
 
     def to_query(self, skip: int | None = None, limit: int | None = None):
         domain_branch = BranchMaker(
             props=[ID_PROP],
             label=self.domain_label,
             post_label=None,
-            relationship=None,
+            relationship=self.relationship,
             relationship_postfix=None,
-            required=False,
-            away_from_core=None,
+            required=True,
+            away_from_core=self.away_from_core,
             domain_label=None
         )
 
         table_current = LogisticsTableQuery(
             branchMakers=[domain_branch],
             label=self.attachable_label,
-            post_label=None,
+            post_label=self.post_label,
             return_id=self.attachable_return_id,
-            props=self.attachable_props
+            props=self.attachable_props,
+            disable_scan=self.disable_scan
         )
         return table_current.to_query(skip=skip, limit=limit)
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 @dataclass
 class LogisticsTableQuery:
     branchMakers: list[BranchMaker]
     label: str
     post_label: str | None = None
     return_id: str = "l"
     props: list[Property] = field(default_factory=lambda: [ID_PROP])
+    disable_scan: bool = False
     def to_query(self, skip: int | None = None, limit: int | None = None):
         return Query(
             LabelNode(
                 return_id=self.return_id,
                 label=self.label,
                 properties=self.props,
                 collect=False,
                 post_label_str=self.post_label
             ),
             branches=[b.to_branch() for b in self.branchMakers],
+            disable_scan=self.disable_scan,
             skip=skip,
             limit=limit
         )
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/reference/ReferenceBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/reference/ReferenceBranch.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 @dataclass
 class ReferenceBranch(BranchMaker):
     props: list[Property]
     post_label: str | None = None
     relationship: str = field(default_factory=lambda: REFERENCED_RELATIONSHIP)
     relationship_postfix: str | None = field(default_factory=lambda: REFERENCED_RETURN_POSTFIX)
     required: bool = False
-    archived: bool = False
+    away_from_core: bool = True
     domain_label: str | None = None
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/AttainedBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/AttainedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/garner_domain/status/ForecastedBranch.py` & `cypherdataframe-0.9.1/cypherdataframe/garner_domain/status/ForecastedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/model/Branch.py` & `cypherdataframe-0.9.1/cypherdataframe/model/Branch.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,23 @@
             , core_node_assignment: str
             ):
         if self.relationship == None:
             prop_by = {
                self.relationship_cypher_assignment(): (
                     f" type({self.relationship_cypher_assignment()})"
                     f" as {self.relationship_cypher_assignment()} "
-                ),
-                self.relationship_direction_cypher_assignment(): (
-                    f" (startNode({self.relationship_cypher_assignment()}) = {core_node_assignment})"
-                    f" as {self.relationship_direction_cypher_assignment()} "
                 )
             }
+            if self.away_from_core is None:
+                prop_by = prop_by | {
+                    self.relationship_direction_cypher_assignment(): (
+                        f" (startNode({self.relationship_cypher_assignment()}) = {core_node_assignment})"
+                        f" as {self.relationship_direction_cypher_assignment()} "
+                    )
+                }
         else:
             prop_by = {}
         return prop_by
 
     def relationship_direction_cypher_assignment(self) -> str:
         return self.relationship_cypher_assignment()+"d"
     def relationship_cypher_assignment(self) -> str:
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.9.1/cypherdataframe/model/LabelNode.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe/model/Query.py` & `cypherdataframe-0.9.1/cypherdataframe/model/Query.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 @dataclass(frozen=True)
 class Query:
     core_node: LabelNode
     branches: list[Branch]
     skip: int | None = field(default_factory=lambda: None)
     limit: int | None = field(default_factory=lambda: None)
     enforce_complete_chunks: bool = field(default_factory=lambda: True)
+    disable_scan:bool = False
 
     def all_properties_by_final_assigment(self) -> dict[str, Property]:
 
         branch_properties = {}
 
         for branch in self.branches:
             branch_properties.update(
@@ -34,18 +35,21 @@
             if (branch.relationship is None) and (not branch.optional):
                 print(
                     f"WARNING: Branch has a None relationship"
                     f" and is not optional."
                     f" Expect significantly degraded query time."
                     f" Branch: {branch}"
                 )
+        if self.core_node.post_label_str:
+            post_label = self.core_node.post_label_str
+        else:
+            post_label = ""
 
-        first_core_match = f'match({self.core_node.return_id}:{self.core_node.label}) '
-
-        if all([branch.away_from_core for branch in self.branches]):
+        first_core_match = f'match({self.core_node.return_id}:{self.core_node.label}{post_label}) '
+        if all([branch.away_from_core for branch in self.branches]) or self.disable_scan:
             scan_core_str = ""
         else:
             scan_core_str = f"USING SCAN {self.core_node.return_id}:{self.core_node.label}"
         accumulated_fragments = Accumulation(
             core_match_fragments=[first_core_match, scan_core_str],
             enforce_complete_chunks=self.enforce_complete_chunks
         )
```

### Comparing `cypherdataframe-0.7.9/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.9.1/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/cypherdataframe.egg-info/SOURCES.txt` & `cypherdataframe-0.9.1/cypherdataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/setup.py` & `cypherdataframe-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             'cypherdataframe.garner_domain.logistics',
             'cypherdataframe.garner_domain.measure',
             'cypherdataframe.garner_domain.queries',
             'cypherdataframe.garner_domain.reference',
             'cypherdataframe.garner_domain.status'
         ]
     ),
-    version='0.7.9',
+    version='0.9.1',
     description='Cypher Query to df Toolkit',
     author='Attila Vanderploeg',
     license='MIT',
     install_requires=['py2neo>=2021.2.3', 'dacite>=1.6.0'],
     setup_requires=[],
     tests_require=[],
     test_suite='tests',
```

### Comparing `cypherdataframe-0.7.9/tests/branch_maker_test.py` & `cypherdataframe-0.9.1/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.9.1/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.7.9/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.9.1/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

