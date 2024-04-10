# Comparing `tmp/pypromice-1.3.3.tar.gz` & `tmp/pypromice-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypromice-1.3.3.tar", last modified: Wed Jan  3 20:52:27 2024, max compression
+gzip compressed data, was "pypromice-1.3.4.tar", last modified: Wed Apr 10 12:50:44 2024, max compression
```

## Comparing `pypromice-1.3.3.tar` & `pypromice-1.3.4.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.906082 pypromice-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-01-03 20:52:20.000000 pypromice-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-03 20:52:20.000000 pypromice-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-01-03 20:52:27.906082 pypromice-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-01-03 20:52:20.000000 pypromice-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 20:52:27.906082 pypromice-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-01-03 20:52:20.000000 pypromice-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.890082 pypromice-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.890082 pypromice-1.3.3/src/pypromice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.890082 pypromice-1.3.3/src/pypromice/get/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/get/get.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/get/get_promice_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.894082 pypromice-1.3.3/src/pypromice/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20046 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/postprocess/csv2bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/postprocess/get_bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/postprocess/wmo_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.894082 pypromice-1.3.3/src/pypromice/process/
--rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/L0toL1.py
--rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/L1toL2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18238 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/L2toL3.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29844 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/get_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/join_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/value_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/process/variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.894082 pypromice-1.3.3/src/pypromice/qc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/github_data_issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.894082 pypromice-1.3.3/src/pypromice/qc/percentiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/percentiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/percentiles/compute_thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/percentiles/outlier_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/percentiles/thresholds.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/qc/persistence_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.906082 pypromice-1.3.3/src/pypromice/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_config1.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_config2.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_email
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_percentile.py
--rw-r--r--   0 runner    (1001) docker     (127)  1626942 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_raw1.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3337781 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_raw_DataTable2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   348047 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_raw_SlimTableMem1.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1993699 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_raw_transmitted1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/test/test_raw_transmitted2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.906082 pypromice-1.3.3/src/pypromice/tx/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/get_l0tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/get_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/get_watsontx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-01-03 20:52:20.000000 pypromice-1.3.3/src/pypromice/tx/tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:52:27.906082 pypromice-1.3.3/src/pypromice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-01-03 20:52:27.000000 pypromice-1.3.3/src/pypromice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-01-03 20:52:27.000000 pypromice-1.3.3/src/pypromice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:52:27.000000 pypromice-1.3.3/src/pypromice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-03 20:52:27.000000 pypromice-1.3.3/src/pypromice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-03 20:52:27.000000 pypromice-1.3.3/src/pypromice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-03 20:52:27.000000 pypromice-1.3.3/src/pypromice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.438857 pypromice-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-10 12:50:37.000000 pypromice-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 12:50:37.000000 pypromice-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 12:50:44.438857 pypromice-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-10 12:50:37.000000 pypromice-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:50:44.438857 pypromice-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-10 12:50:37.000000 pypromice-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.414857 pypromice-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.418857 pypromice-1.3.4/src/pypromice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.418857 pypromice-1.3.4/src/pypromice/get/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/get/get.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/get/get_promice_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/bufr_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/bufr_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/get_bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/positions_seed.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/real_time_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/station_configurations.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/process/
+-rw-r--r--   0 runner    (1001) docker     (127)    22818 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/L0toL1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/L1toL2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18238 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/L2toL3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29844 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/get_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/join_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/value_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/github_data_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/qc/percentiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/compute_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/outlier_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/thresholds.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/persistence_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.434857 pypromice-1.3.4/src/pypromice/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_config1.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_config2.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_email
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1626942 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3337781 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_DataTable2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   348047 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_SlimTableMem1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1993699 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_transmitted1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_transmitted2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.438857 pypromice-1.3.4/src/pypromice/tx/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/get_l0tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/get_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/get_watsontx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.438857 pypromice-1.3.4/src/pypromice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/top_level.txt
```

### Comparing `pypromice-1.3.3/LICENSE.txt` & `pypromice-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/PKG-INFO` & `pypromice-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.3.3
+Version: 1.3.4
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
@@ -23,14 +23,15 @@
 Requires-Dist: xarray>=2022.6.0
 Requires-Dist: toml
 Requires-Dist: scipy>=1.9.0
 Requires-Dist: scikit-learn>=1.1.0
 Requires-Dist: Bottleneck
 Requires-Dist: netcdf4
 Requires-Dist: pyDataverse
+Requires-Dist: eccodes
 
 # pypromice
 [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://badge.fury.io/py/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/version.svg)](https://anaconda.org/conda-forge/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/platforms.svg)](https://anaconda.org/conda-forge/pypromice) [![](<https://img.shields.io/badge/Dataverse DOI-10.22008/FK2/3TSBF0-orange>)](https://www.doi.org/10.22008/FK2/3TSBF0) [![DOI](https://joss.theoj.org/papers/10.21105/joss.05298/status.svg)](https://doi.org/10.21105/joss.05298) [![Documentation Status](https://readthedocs.org/projects/pypromice/badge/?version=latest)](https://pypromice.readthedocs.io/en/latest/?badge=latest)
  
 pypromice is designed for processing and handling [PROMICE](https://promice.org) automated weather station (AWS) data.
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information.
```

### Comparing `pypromice-1.3.3/README.md` & `pypromice-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/setup.py` & `pypromice-1.3.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypromice",
-    version="1.3.3",
+    version="1.3.4",
     author="GEUS Glaciology and Climate",
     description="PROMICE/GC-Net data processing toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GEUS-Glaciology-and-Climate/pypromice",
     project_urls={
         "Bug Tracker": "https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues",
@@ -26,21 +26,24 @@
         "Topic :: Scientific/Engineering",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     include_package_data = True,
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.8",
-    package_data={"pypromice.qc.percentiles": ["thresholds.csv"]},
-    install_requires=['numpy>=1.23.0', 'pandas>=1.5.0', 'xarray>=2022.6.0', 'toml', 'scipy>=1.9.0', 'scikit-learn>=1.1.0', 'Bottleneck', 'netcdf4', 'pyDataverse'],
+    package_data={
+        "pypromice.qc.percentiles": ["thresholds.csv"],
+        "pypromice.postprocess": ["station_configurations.toml", "positions_seed.csv"],
+    },
+    install_requires=['numpy>=1.23.0', 'pandas>=1.5.0', 'xarray>=2022.6.0', 'toml', 'scipy>=1.9.0', 'scikit-learn>=1.1.0', 'Bottleneck', 'netcdf4', 'pyDataverse', 'eccodes'],
     entry_points={
     'console_scripts': [
         'get_promice_data = pypromice.get.get_promice_data:get_promice_data',
         'get_l0tx = pypromice.tx.get_l0tx:get_l0tx',
         'get_l3 = pypromice.process.get_l3:get_l3',
         'join_l3 = pypromice.process.join_l3:join_l3',
         'get_watsontx = pypromice.tx.get_watsontx:get_watsontx',
-        'get_bufr = pypromice.postprocess.get_bufr:get_bufr',
+        'get_bufr = pypromice.postprocess.get_bufr:main',
         'get_msg = pypromice.tx.get_msg:get_msg'
     ],
 },
 )
```

### Comparing `pypromice-1.3.3/src/pypromice/get/get.py` & `pypromice-1.3.4/src/pypromice/get/get.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/get/get_promice_data.py` & `pypromice-1.3.4/src/pypromice/get/get_promice_data.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/postprocess/csv2bufr.py` & `pypromice-1.3.4/src/pypromice/postprocess/get_bufr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,508 +1,629 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
+#!/usr/bin/env python
+
 """
+Command-line script for running BUFR file generation
+
 Post-processing functions for AWS station data, such as converting PROMICE and GC-Net data files to WMO-compliant BUFR files
+
 """
-import pandas as pd
-import sys, traceback
-import os
+import argparse
+import glob
+import logging
+import pickle
+import sys
 from datetime import datetime, timedelta
-from eccodes import codes_set, codes_write, codes_release, \
-                    codes_bufr_new_from_samples, CodesInternalError, \
-                    codes_is_defined
-import math
-import numpy as np
-from sklearn.linear_model import LinearRegression
-
-from pypromice.postprocess.wmo_config import ibufr_settings, stid_to_skip, vars_to_skip, positions_update_timestamp_only
+from pathlib import Path
+from typing import List, Dict, Mapping, Optional, Collection, Sequence, Union, TextIO
 
-# from IPython import embed
+import attrs
+import numpy as np
+import pandas as pd
+import toml
 
-# To suppress pandas SettingWithCopyWarning
-pd.options.mode.chained_assignment = None # default='warn'
+from pypromice.postprocess.bufr_utilities import write_bufr_message, BUFRVariables
+from pypromice.postprocess.real_time_utilities import get_latest_data
 
-#------------------------------------------------------------------------------
+logger = logging.getLogger(__name__)
 
-def getBUFR(s1, outBUFR, stid, land_stids):
-    '''Construct and export .bufr messages to file from Series or DataFrame.
-    PRIMARY DRIVER FUNCTION
+DEFAULT_STATION_CONFIGURATION_PATH = Path(__file__).parent.joinpath(
+    "station_configurations.toml"
+)
+DEFAULT_POSITION_SEED_PATH = Path(__file__).parent.joinpath("positions_seed.csv")
+DEFAULT_LIN_REG_TIME_LIMIT = "91d"
+
+def parse_arguments_bufr() -> argparse.ArgumentParser:
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument(
+        "--store_positions",
+        "--positions",
+        action="store_true",
+        required=False,
+        default=False,
+        help="If included (True), make a positions dict and output AWS_latest_locations.csv file.",
+    )
+
+    parser.add_argument(
+        "--positions-filepath",
+        "-p",
+        type=Path,
+        required=False,
+        help="Path to write AWS_latest_locations.csv file.",
+    )
+
+    parser.add_argument(
+        "--time-limit",
+        default=DEFAULT_LIN_REG_TIME_LIMIT,
+        type=str,
+        required=False,
+        help="Previous time to limit dataframe before applying linear regression.",
+    )
+
+    parser.add_argument(
+        "--input_files",
+        "--l3-filepath",
+        "-i",
+        type=Path,
+        nargs="+",
+        required=True,
+        help="Path to L3 tx .csv files. Can be direct paths or glob patterns",
+    )
+
+    parser.add_argument(
+        "--bufr-out",
+        "-o",
+        type=Path,
+        required=True,
+        help="Path to the BUFR out directory.",
+    )
+
+    parser.add_argument(
+        "--timestamps-pickle-filepath",
+        type=Path,
+        required=False,
+        help="Path to the latest_timestamps.pickle file.",
+    )
+
+    parser.add_argument(
+        "--station_configuration_mapping",
+        default=DEFAULT_STATION_CONFIGURATION_PATH,
+        type=Path,
+        required=False,
+        help="Path to csv file with station meta data and BUFR export configuration",
+    )
+
+    parser.add_argument(
+        "--position_seed",
+        default=DEFAULT_POSITION_SEED_PATH,
+        type=Path,
+        required=False,
+        help="Path to csv file with seed values for output positions.",
+    )
+
+    parser.add_argument(
+        '--latest_timestamp',
+        default=datetime.utcnow(),
+        type=pd.Timestamp,
+        help="Timestamp used to determine latest data. Default utcnow."
+    )
+
+    parser.add_argument("--verbose", "-v", default=False, action="store_true")
+
+    return parser
+
+
+@attrs.define
+class StationConfiguration:
+    """
+    Helper class for storing station specific configurations with respect to
+
+    * Installation specific distance measurements such as height differences between instruments
+    * Reference strings such as stid, station_site and wmo_id
+    * BUFR export specific parameters
+
+    # TODO: The station related meta data should be fetched from a station specific configuration files in the future or
+    # from header data in data source.
+    """
+
+    stid: str
+    station_site: str = None
+    project: Optional[str] = None
+    station_type: Optional[str] = None
+    wmo_id: Optional[str] = None
+    barometer_from_gps: Optional[float] = None
+    anemometer_from_sonic_ranger: Optional[float] = None
+    temperature_from_sonic_ranger: Optional[float] = None
+    height_of_gps_from_station_ground: Optional[float] = None
+    sonic_ranger_from_gps: Optional[float] = None
+
+    # The station data will be exported to BUFR if True. Otherwise, it will only export latest position
+    export_bufr: bool = False
+    comment: Optional[str] = None
+
+    # skip specific variables for stations
+    # If a variable has known bad data, use this collection to skip the variable
+    # Note that if a station is not reporting both air temp and pressure it will be skipped,
+    # as currently implemented in csv2bufr.min_data_check().
+    # ['p_i'], # EXAMPLE
+    skipped_variables: List[str] = attrs.field(factory=list)
+
+    positions_update_timestamp_only: bool = False
+
+    def as_dict(self) -> Dict:
+        return attrs.asdict(self)
+
+
+def load_station_configuration_mapping(
+    fp: Union[str, Path, TextIO]
+) -> Mapping[str, StationConfiguration]:
+    """
+    Read station configurations from toml file
 
     Parameters
     ----------
-    s1 : pandas.Series
-        Pandas series of single most recent obset for a station
-    outBUFR : str
-        File path that .bufr file will be exported to
-    stid : str
-        The station ID to be processed. e.g. 'KPC_U'
-    land_stids : list
-        List of station IDs for land-based stations
+    fp :
+        Path to or open toml file
 
     Returns
     -------
-    remove_file : boolean
-        Status object to return to getBUFR indicating successful completion
-    '''
-    remove_file = False
-
-    # Open bufr file
-    fout = open(outBUFR, 'wb')
-
-    # Create new bufr message to write to
-    ibufr = codes_bufr_new_from_samples('BUFR4')
-    timestamp = datetime.strptime(s1['time'], '%Y-%m-%d %H:%M:%S')
-    config_key = 'mobile'
-    if stid in land_stids:
-        config_key = 'land'
-    try:
-        # we must pass all the following functions without error.
-        # If handled (or unhandled) errors occur, we re-raise and
-        # the exceptions below will set remove_file to True.
-        setTemplate(ibufr, timestamp, stid, config_key)
-        setStation(ibufr, stid, config_key)
-        setAWSvariables(ibufr, s1, timestamp, stid)
-
-        #Encode keys in data section
-        codes_set(ibufr, 'pack', 1)
-
-        #Write bufr message to bufr file
-        codes_write(ibufr, fout)
-
-    except CodesInternalError as ec:
-        print(traceback.format_exc())
-        # print(ec)
-        print(f'-----> CodesInternalError in getBUFR for {stid}!')
-        remove_file = True
-    except Exception as e:
-        # Catch anything else here...
-        print(traceback.format_exc())
-        # print(e)
-        print(f'-----> ERROR in getBUFR for {stid}')
-        remove_file = True
-
-    codes_release(ibufr)
-
-    fout.close()
-
-    if remove_file is True:
-        print(f'-----> Removing file for {stid}')
-        os.remove(fout.name)
-    return remove_file
+    Mapping from stid to StationConfiguration
+
+    """
+    return {
+        stid: StationConfiguration(**config_dict)
+        for stid, config_dict in toml.load(fp).items()
+    }
 
 
-def setTemplate(ibufr, timestamp, stid, config_key):
-    '''Set bufr message template.
+def write_station_configuration_mapping(
+    config_mapping: Mapping[str, StationConfiguration], fp: TextIO
+):
+    """
+    Write station configuration to toml file
 
     Parameters
     ----------
-    ibufr : bufr.msg
-        Bufr message object
-    timestamp : datetime.Datetime
-        Timestamp of observation
-    stid : str
-        The station ID to be processed. e.g. 'KPC_U'
-    config_key : str
-        Defines which config dict to use in wmo_config.ibufr_settings, 'mobile' or 'land'
-    '''
-    for k, v in ibufr_settings[config_key]['template'].items():
-        if codes_is_defined(ibufr, k) == 1:
-            codes_set(ibufr, k, v)
-        else:
-            print('-----> setTemplate Key not defined: {}'.format(k))
-            continue
-
-    codes_set(ibufr, 'typicalYear', timestamp.year)
-    codes_set(ibufr, 'typicalMonth', timestamp.month)
-    codes_set(ibufr, 'typicalDay', timestamp.day)
-    codes_set(ibufr, 'typicalHour', timestamp.hour)
-    codes_set(ibufr, 'typicalMinute', timestamp.minute)
-    # codes_set(ibufr, 'typicalSecond', timestamp.second)
+    config_mapping
+        Mapping from stid to StationConfiguration
+    fp
+        open writable TextIO
+    """
+    config_mapping = {
+        config.stid: config.as_dict() for config in config_mapping.values()
+    }
+    toml.dump(config_mapping, fp)
 
 
-def setStation(ibufr, stid, config_key):
-    '''Set station-specific info to bufr message.
+def process_station(
+    file_path: Path,
+    output_path: Path,
+    now_timestamp: datetime,
+    latest_timestamp: Optional[datetime],
+    time_limit: str,
+    stid: str,
+    station_configuration: StationConfiguration,
+) -> Optional[Dict]:
+    df = load_data(file_path, now_timestamp)
+
+    # Select current data
+    latest_data = get_latest_data(
+        df,
+        lin_reg_time_limit=time_limit,
+    )
+
+    if latest_data is None:
+        logger.info("No valid instantaneous timestamps!")
+        return None
+
+    latest_data = filter_skipped_variables(
+        latest_data, vars_to_skip=station_configuration.skipped_variables
+    )
+
+    # Check that we have minimum required valid data
+    sufficient_wx_data, sufficient_position_data = min_data_check(latest_data)
+
+    station_position = dict()
+    station_position["timestamp"] = latest_data.name
+    if sufficient_position_data:
+        station_position["lon"] = latest_data.get("gps_lon_fit")
+        station_position["lat"] = latest_data.get("gps_lat_fit")
+        station_position["alt"] = latest_data.get("gps_alt_fit")
+    else:
+        logger.warning("Insufficient position data")
+        # Don't use any position attributes from latest_data
+        station_position["lon"] = None
+        station_position["lat"] = None
+        station_position["alt"] = None
+        return station_position
+
+    if station_configuration.export_bufr:
+        if not sufficient_wx_data:
+            logger.warning(f"Failed min data wx {stid}")
+            return station_position
+
+        # Store current timest
+        if latest_data.name <= latest_timestamp:
+            logger.info(f"No new data {latest_data.name} <= {latest_timestamp}")
+            return station_position
+
+        # Construct and export BUFR file
+        bufr_variables = get_bufr_variables(
+            data=latest_data,
+            station_configuration=station_configuration,
+        )
+        with output_path.open("bw") as fp:
+            write_bufr_message(variables=bufr_variables, file=fp)
+
+    return station_position
+
+
+def load_data(file_path: Path, now_timestamp: datetime) -> pd.DataFrame:
+    """
+    Read AWS data from csv file using time as index and filter all rows after now_timestamp
 
     Parameters
     ----------
-    ibufr : bufr.msg
-        Bufr message object
-    stid : str
-        The station ID to be processed. e.g. 'KPC_U'
-    config_key : str
-        Defines which config dict to use in wmo_config.ibufr_settings, 'mobile' or 'land'
-    '''
-    station_indentifier_keys = ('shipOrMobileLandStationIdentifier','stationNumber')
-    for k, v in ibufr_settings[config_key]['station'].items():
-        if k in station_indentifier_keys:
-            # Deal with any string replacement of stid names before indexing
-            if ('v3' in stid) and (stid.replace('v3','') in stid_to_skip['use_v3']):
-                # We are reading the v3 station ID file, and the config says to use it!
-                # But we need to write to BUFR without v3 name
-                stid = stid.replace('v3','')
-            if stid == 'THU_U2':
-                stid = 'THU_U'
-            if stid in ('JAR_O','SWC_O'):
-                stid = stid.replace('_O','')
-            if stid == 'CEN2':
-                stid = 'CEN'
-            try:
-                codes_set(ibufr, k, v[stid])
-            except KeyError as e:
-                print(f'-----> ID not found for {stid}')
-                raise # throw error back to getBUFR where it is handled
-        else:
-            if codes_is_defined(ibufr, k) == 1:
-                codes_set(ibufr, k, v)
-            else:
-               print(f'-----> setStation Key for {stid} not defined: {k}')
-               continue
+    file_path
+    now_timestamp
 
+    Returns
+    -------
+    Dataframe with all columns from csv file and time as index
+    """
+    # Read csv file
+    df: pd.DataFrame = (
+        pd.read_csv(file_path, delimiter=",", parse_dates=["time"])
+        .set_index("time")
+        .sort_index()
+    )
+    df = df[:now_timestamp]
+    return df
 
-def setAWSvariables(ibufr, row, timestamp, stid):
-    '''Set AWS measurements to bufr message.
-    
-    Parameters
-    ----------
-    ibufr : bufr.msg
-        Bufr message object
-    row : pandas.DataFrame row, or pandas.Series
-        DataFrame row (or Series) with AWS variable data
-    timestamp : datetime.datetime
-        timestamp for this row
-    stid : str
-        The station ID to be processed. e.g. 'KPC_U'
-    '''
-    # Set timestamp fields
-    setBUFRvalue(ibufr, 'year', timestamp.year)
-    setBUFRvalue(ibufr, 'month', timestamp.month)
-    setBUFRvalue(ibufr, 'day', timestamp.day)
-    setBUFRvalue(ibufr, 'hour', timestamp.hour)
-    setBUFRvalue(ibufr, 'minute', timestamp.minute)
-
-    vars_dict = {
-        'relativeHumidity': 'rh_i', # DMI wants non-corrected rh
-        'airTemperature': 't_i',
-        'pressure': 'p_i',
-        'windDirection': 'wdir_i',
-        'windSpeed': 'wspd_i'
-    }
-    for bufr_key, source_var in vars_dict.items():
-        if (stid in vars_to_skip) and (source_var in vars_to_skip[stid]):
-            print('----> Skipping var: {} {}'.format(stid,source_var))
-        else:
-            setBUFRvalue(ibufr, bufr_key, row[source_var])
 
-    # Set position metadata
-    setBUFRvalue(ibufr, 'latitude', row['gps_lat_fit'])
-    setBUFRvalue(ibufr, 'longitude', row['gps_lon_fit'])
-    setBUFRvalue(ibufr, 'heightOfStationGroundAboveMeanSeaLevel', row['gps_alt_fit']) # also height and heightOfStation?
-
-    # The ## in the codes_set() indicate the position in the BUFR for the parameter.
-    # e.g. #10#timePeriod will assign to the 10th occurence of "timePeriod", which corresponds
-    # to the wind speed section. Note that both the "synopMobil" and "synopLand" templates
-    # appear to have the same positions for all parameters that are set here.
-    # View the output BUFR to see section keys with 'bufr_dump filename.bufr'.
-    if math.isnan(row['wspd_i']) is False:
-        #Set time significance (2=temporally averaged)
-        codes_set(ibufr, '#1#timeSignificance', 2)
-        #Set monitoring time period (-10=10 minutes)
-        codes_set(ibufr, '#10#timePeriod', -10)
-
-    #Set measurement heights
-    if math.isnan(row['z_boom_u_smooth']) is False:
-        codes_set(ibufr,
-                  '#1#heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform',
-                  row['z_boom_u_smooth']-0.1) # For air temp and RH
-        codes_set(ibufr,
-                  '#7#heightOfSensorAboveLocalGroundOrDeckOfMarinePlatform',
-                  row['z_boom_u_smooth']+0.4) # For wind speed
-        if math.isnan(row['gps_alt_fit']) is False:
-            codes_set(ibufr, 'heightOfBarometerAboveMeanSeaLevel',
-                      row['gps_alt_fit']+row['z_boom_u_smooth']) # For pressure
-
-
-def setBUFRvalue(ibufr, b_name, value):
-    '''Set variable in BUFR message
-    Called in setAWSvariables() to make sure we aren't passing NaNs
+def get_bufr(
+    bufr_out: Path,
+    input_files: Sequence[Path],
+    positions_filepath: Optional[Path],
+    timestamps_pickle_filepath: Optional[Path],
+    station_configuration_path: Optional[Path],
+    now_timestamp: Optional[datetime] = None,
+    positions_seed_path: Optional[Path] = None,
+    earliest_timestamp: datetime = None,
+    store_positions: bool = False,
+    time_limit: str = "91d",
+):
+    """
+    Main function for generating BUFR files and determine latest positions from a sequence of csv files
+
+    The file timestamps_pickle_filepath is used to maintain a local state in the execution environment to ensure the
+    same data is not processed multiple times.
+
 
     Parameters
     ----------
-    ibufr : bufr.msg                
-        Active BUFR message
-    b_name : str
-        BUFR message variable name
-    value : int/float
-        Value to be assigned to variable
-    '''
-    if math.isnan(value) is False:
-        try:
-            codes_set(ibufr, b_name, value)
-        except CodesInternalError as ec:
-            print(f'{ec}: {b_name}')
-            print('-----> CodesInternalError in setBUFRvalue!')
-            raise # throw error back to getBUFR where it is handled
+    bufr_out
+        Path to the BUFR out directory.
+    input_files
+        List of L3 csv file paths.
+    positions_filepath
+        Path to write latest positions. Used to retrieve a static set of positions to register stations with DMI/WMO
+    timestamps_pickle_filepath
+        Path to pickle file used for storing latest timestamp
+    station_configuration_path
+        Path to toml file with configuration entries for each station
+    now_timestamp
+        get_bufr will export the latest data before now_timestamp. Default datetime.utcnow()
+    positions_seed_path
+        Path to csv file with position data used as default values for the output position.
+    earliest_timestamp
+        The earliest allowed timestamp for data to be included in the output. Default now_timestamp - 2 days
+    store_positions
+        Flag determine if latest positions are exported.
+    time_limit
+        Previous time to limit dataframe before applying linear regression.
+
+    """
+    if now_timestamp is None:
+        now_timestamp = datetime.utcnow()
+
+    if earliest_timestamp is None:
+        earliest_timestamp = now_timestamp - timedelta(days=2)
+
+    # Prepare (latest) positions
+    positions = dict()
+    if positions_seed_path:
+        positions_seed = pd.read_csv(
+            positions_seed_path, index_col=0, delimiter=",", parse_dates=["timestamp"]
+        ).to_dict(orient="index")
+        logger.info(f"Seed positions for {positions_seed.keys()}")
+        positions.update(positions_seed)
+
+    # Prepare station configurations
+    if station_configuration_path is None:
+        station_configuration_mapping = dict()
+    else:
+        station_configuration_mapping = load_station_configuration_mapping(
+            station_configuration_path
+        )
+
+    # Prepare bufr output dir
+    bufr_out.mkdir(parents=True, exist_ok=True)
+
+    # Read existing timestamps pickle to dictionary
+    if timestamps_pickle_filepath and timestamps_pickle_filepath.exists():
+        with timestamps_pickle_filepath.open("rb") as handle:
+            latest_timestamps = pickle.load(handle)
     else:
-        print('----> {} {}'.format(b_name, value))
+        logger.info("latest_timestamps.pickle not found!")
+        latest_timestamps = {}
 
+    # Initiate a new dict for current timestamps
+    current_timestamps = {}
 
-def linear_fit(df, column, decimals, stid):
-    '''Apply a linear regression to the input column
+    # Setup diagnostic lists (logger.info at end)
+    skipped = []
+    no_recent_data = []
+    no_entry_latest_timestamps = []
+    failed_min_data_wx = []
+    failed_min_data_pos = []
+
+    # Iterate through csv files
+    for file_path in input_files:
+        stid = file_path.stem.rsplit("_", 1)[0]
+        logger.info("####### Processing {} #######".format(stid))
+
+        if stid not in station_configuration_mapping:
+            logger.info(f"Station id {stid} not in configuration mapping.")
+            station_configuration = StationConfiguration(stid=stid)
+            skipped.append(stid)
+        else:
+            station_configuration = station_configuration_mapping[stid]
 
-    Linear regression is following:
-    https://realpython.com/linear-regression-in-python/#simple-linear-regression-with-scikit-learn
+        output_path = bufr_out / f"{stid}.bufr"
+        logger.info(f"Generating {output_path} from {file_path}")
+        latest_timestamp = latest_timestamps.get(stid, earliest_timestamp)
+        latest_timestamp = max(earliest_timestamp, latest_timestamp)
 
-    Parameters
-    ----------
-    df : pandas.Dataframe
-        datetime-indexed df, limited to desired time length for linear fit
-    column : str
-        The target column for applying linear fit
-    decimals : int
-        How many decimals to round the output fit values
-    stid : str
-        The station ID to be processed. e.g. 'KPC_U'
-    extrapolate : boolean
-        If False (default), only apply linear fit to timestamps with valid data
-        If True, then extrapolate positions based on linear fit model
+        try:
+            station_position = process_station(
+                file_path=file_path,
+                output_path=output_path,
+                now_timestamp=now_timestamp,
+                latest_timestamp=latest_timestamp,
+                time_limit=time_limit,
+                stid=stid,
+                station_configuration=station_configuration,
+            )
+        except Exception:
+            logger.exception(f"Failed processing {stid}")
+            continue
+
+        if station_position is None:
+            logger.warning(f"No position information available for {stid}")
 
-    Returns
-    -------
-    df : pandas.Dataframe
-        The original input df, with added column for the linear regression values
-    pos_valid : boolean
-        If True (default), sufficient valid data found in recent (limited) data.
-        If False, we need to return this status to find_positions and use full station history instead.
-    '''
-    # print('=========== linear_fit ===========')
-    pos_valid = True
-    if column in df:
-        df_dropna = df[df[column].notna()] # limit to only non-nan for the target column
-        # if len(df_dropna[column].index.normalize().unique()) >= 10: # must have at least 10 unique days
-        if len(df_dropna[column]) >= 15: # must have at least 15 data points (could be hourly or daily)
-            # Get datetime x values into epoch sec integers
-            x_epoch = df_dropna.index.values.astype(np.int64) // 10 ** 9
-            x = x_epoch.reshape(-1,1)
-            y = df_dropna[column].values # can also reshape this, but not necessary
-            model = LinearRegression().fit(x, y)
-
-            # Adding prediction back to original df
-            x_all = df.index.values.astype(np.int64) // 10 ** 9
-            df['{}_fit'.format(column)] = model.predict(x_all.reshape(-1,1)).round(decimals=decimals)
-
-            # Plot data if desired
-            # if stid == 'LYN_T':
-            #     if (column == 'gps_lat') or (column == 'gps_lon') or (column == 'gps_alt'):
-            #         import matplotlib.pyplot as plt
-            #         plt.figure()
-            #         df_dropna[column].plot(marker='o',ls='None')
-            #         df['{}_fit'.format(column)].plot(marker='o', ls='None', color='red')
-            #         plt.title('{} {}'.format(stid, column))
-            #         plt.xlim(df.index.min(),df.index.max())
-            #         plt.show()
         else:
-            # Do not have 10 days of valid data, or all data is NaN.
-            print('----> Insufficient {} data for {}!'.format(column, stid))
-            pos_valid = False
-    else:
-        print('----> {} not found in dataframe!'.format(column))
-        pass
-    return df, pos_valid
+            if stid not in positions:
+                positions[stid] = dict()
 
+            if station_configuration.positions_update_timestamp_only:
+                positions[stid]["timestamp"] = station_position["timestamp"]
+            else:
+                positions[stid].update(station_position)
 
-def rolling_window(df, column, window, min_periods, decimals):
-    '''Apply a rolling window (smoothing) to the input column
+    # Write the most recent timestamps back to the pickle on disk
+    logger.info(f"writing latest_timestamps to {timestamps_pickle_filepath}")
+    if timestamps_pickle_filepath:
+        with timestamps_pickle_filepath.open("wb") as handle:
+            pickle.dump(current_timestamps, handle, protocol=pickle.HIGHEST_PROTOCOL)
+
+    if store_positions:
+        positions_df = pd.DataFrame.from_dict(
+            positions,
+            orient="index",
+            # columns=['timestamp','lat','lon','alt','lat_source','lon_source']
+            columns=["timestamp", "lat", "lon", "alt"],
+        )
+        positions_df.sort_index(inplace=True)
+        positions_df.to_csv(positions_filepath, index_label="stid")
+
+    logger.info("--------------------------------")
+    not_processed_wx_pos = set(failed_min_data_wx + failed_min_data_pos)
+    not_processed_count = (
+        len(skipped)
+        + len(no_recent_data)
+        + len(no_entry_latest_timestamps)
+        + len(not_processed_wx_pos)
+    )
+    logger.info(
+        "BUFR exported for {} of {} fpaths.".format(
+            (len(input_files) - not_processed_count), len(input_files)
+        )
+    )
+    logger.info("")
+    logger.info("skipped: {}".format(skipped))
+    logger.info("no_recent_data: {}".format(no_recent_data))
+    logger.info("no_entry_latest_timestamps: {}".format(no_entry_latest_timestamps))
+    logger.info("failed_min_data_wx: {}".format(failed_min_data_wx))
+    logger.info("failed_min_data_pos: {}".format(failed_min_data_pos))
+    logger.info("--------------------------------")
+
+
+def filter_skipped_variables(
+    row: pd.Series, vars_to_skip: Collection[str]
+) -> pd.Series:
+    """
+    Mutate input series by setting var_to_skip to np.nan
 
     Parameters
     ----------
-    df : pandas.Dataframe
-        datetime-indexed df
-    column : str
-        The target column for applying rolling window
-    window : str
-        Window size (e.g. '24H' or 30D')
-    min_periods : int
-        Minimum number of observations in window required to have a value;
-        otherwise, result is np.nan.
-    decimals : int
-        How many decimal places to round the output smoothed values
+    row
+    vars_to_skip
+        List of variable names to be skipped
 
     Returns
     -------
-    df : pandas.Dataframe
-        The original input df, with added column for the smoothed values
-    '''
-    df['{}_smooth'.format(column)] = df[column].rolling(
-        window,
-        min_periods=min_periods,
-        center=True, # set the window labels as the center of the window
-        closed='both' # no points in the window are excluded (first or last)
-        ).median().round(decimals=decimals) # could also round to whole meters (decimals=0)
-    return df
+    Input series
 
-def round_values(s):
-    '''Enforce precision
-    Note the sensor accuracies listed here:
-    https://essd.copernicus.org/articles/13/3819/2021/#section8
-    In addition to sensor accuracy, WMO requires pressure and heights
-    to be reported at 0.1 precision.
-    
-    Parameters
-    ----------
-    s : pandas series (could also be a dataframe)
-
-    Returns
-    -------
-    s : modified pandas series (could also be a dataframe)
-    '''
-    s['rh_i'] = s['rh_i'].round(decimals=0)
-    s['wspd_i'] = s['wspd_i'].round(decimals=1)
-    s['wdir_i'] = s['wdir_i'].round(decimals=0)
-    s['t_i'] = s['t_i'].round(decimals=1)
-    s['p_i'] = s['p_i'].round(decimals=1)
-
-    # gps_lat,gps_lon,gps_alt,z_boom_u are all rounded in linear_fit() or rolling_window()
-    return s
-
-
-def find_positions(df, stid, time_limit, current_timestamp=None, positions=None):
-    ''' Driver function to run linear_fit() and set valid lat, lon, and alt
-    to df_limited, which is then used to set position data in BUFR.
-    If 'positions' is not None (must pass --positions arg), we also write to
-    the positions dict which will be written to AWS_latest_locations.csv for
-    all stations (whether processed or skipped)
+    """
+    vars_to_skip = set(row.keys()) & set(vars_to_skip)
+    for var_key in vars_to_skip:
+        row[var_key] = np.nan
+        logger.info("----> Skipping var: {}".format(var_key))
+    return row
+
+
+def get_bufr_variables(
+    data: pd.Series,
+    station_configuration: StationConfiguration,
+) -> BUFRVariables:
+    """
+    Helper function for converting our  variables to the variables needed for bufr export.
 
     Parameters
     ----------
-    df : pandas dataframe
-        The full tx dataframe
-    stid : str
-        The station ID, such as NUK_L
-    time_limit : str
-        Previous time to limit dataframe before applying linear regression.
-        (e.g. '3M')
-    current_timestamp : datetime64 time
-        The timestamp for the most recent valid instantaneous data
-    positions : dict, or None
-        Dict storing current station positions. If present, we are writing
-        positions to file.
+    data
+        Series with processed l3 variables from get_latest_datas
+
+    station_configuration
 
     Returns
     -------
-    df_limited : pandas dataframe
-        Dataframe limited to time_limit, and including position data
-    positions : dict
-        Modified dict storing most-recent station positions.
-    '''
-    if stid in positions_update_timestamp_only:
-        # we don't have a position-associated timestamp, just use the most recent transmission.
-        # e.g. KAN_B (does not transmit position, and currently skipped because does not transmit
-        # instantaneous obs). If KAN_B ever submits inst data (but not position) we will need to use
-        # the config-seeded position coordinates to set positions here in df_limited.
-        positions[stid]['timestamp'] = df.index.max()
-        df_limited = df # just to return something
-    else:
-        print(f'finding positions for {stid}')
-        df_limited = df.last(time_limit).copy()
-        print(f'last transmission: {df_limited.index.max()}')
-
-        # Extrapolate recommended for altitude, optional for lat and lon.
-        df_limited, lat_valid = linear_fit(df_limited, 'gps_lat', 6, stid)
-        df_limited, lon_valid = linear_fit(df_limited, 'gps_lon', 6, stid)
-        df_limited, alt_valid = linear_fit(df_limited, 'gps_alt', 1, stid)
-
-        # If we have no valid lat, lon or alt data in the df_limited window, then interpolate
-        # using full tx dataset.
-        check_valid = {'gps_lat': lat_valid, 'gps_lon': lon_valid, 'gps_alt': alt_valid}
-        check_valid_again = {}
-        for k,v in check_valid.items():
-            if v is False:
-                print(f'----> Using full history for linear extrapolation: {k}')
-                print(f'first transmission: {df.index.min()}')
-                if k == 'gps_alt':
-                    df, valid = linear_fit(df, k, 1, stid)
-                else:
-                    df, valid = linear_fit(df, k, 6, stid)
-                check_valid_again[k] = valid
-                if check_valid_again[k] is True:
-                    df_limited[f'{k}_fit'] = df.last(time_limit)[f'{k}_fit']
-                else:
-                    print(f'----> No data exists for {k}. Stubbing out with NaN.')
-                    df_limited[f'{k}_fit'] = pd.Series(np.nan, index= df.last(time_limit).index)
-
-        # SET POSITIONS FOR CSV FILE
-        if positions is not None:
-            if current_timestamp is None:
-                # This is old data (> 2 days), not submitting to DMI, but writing to positions csv
-                # Find the most recent row that has valid lat, lon and alt
-                last_valid_timestamp = df_limited[['gps_lon_fit','gps_lat_fit','gps_alt_fit']].dropna().last_valid_index()
-                if last_valid_timestamp is None:
-                    # we are likely missing gps_alt_fit
-                    last_valid_timestamp = df_limited[['gps_lon_fit','gps_lat_fit']].dropna().last_valid_index()
-                    if last_valid_timestamp is None:
-                        # last ditch effort
-                        last_valid_timestamp = df_limited.index.max()
-                s = df_limited.loc[last_valid_timestamp]
-            else:
-                s = df_limited.loc[current_timestamp]
-            print(f'writing positions for {stid}')
-            pos_strings = ['lat','lon','alt']
-            for p in pos_strings:
-                if (f'gps_{p}_fit' in s) and (pd.isna(s[f'gps_{p}_fit']) is False):
-                    positions[stid][p] = s[f'gps_{p}_fit']
-            # Add timestamp
-            positions[stid]['timestamp'] = s['time']
+    BUFRVariables used by bufr_utilities
 
-    return df_limited, positions if positions else df_limited
+    """
+    heightOfStationGroundAboveMeanSeaLevel = np.nan
+    if isinstance(station_configuration.height_of_gps_from_station_ground, float):
+        heightOfStationGroundAboveMeanSeaLevel = (
+                data["gps_alt_fit"] - station_configuration.height_of_gps_from_station_ground
+        )
+
+    heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformTempRH = np.nan
+    if isinstance(station_configuration.temperature_from_sonic_ranger, float):
+        heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformTempRH = (
+                data["z_boom_u_smooth"]+ station_configuration.temperature_from_sonic_ranger
+        )
+
+    heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformWSPD = np.nan
+    if isinstance(station_configuration.anemometer_from_sonic_ranger, float):
+        heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformWSPD = (
+                data["z_boom_u_smooth"] + station_configuration.anemometer_from_sonic_ranger
+        )
+
+    heightOfBarometerAboveMeanSeaLevel = np.nan
+    if isinstance(station_configuration.barometer_from_gps, float):
+        heightOfBarometerAboveMeanSeaLevel = (
+                data["gps_alt_fit"] + station_configuration.barometer_from_gps
+        )
+
+
+    output_row = BUFRVariables(
+        wmo_id=station_configuration.wmo_id,
+        station_type=station_configuration.station_type,
+        timestamp=data.name,
+        # DMI wants non-corrected rh
+        relativeHumidity=data.rh_i,
+        # Convert air temp, C to Kelvin
+        airTemperature=data.t_i + 273.15,
+        # Convert pressure, correct the -1000 offset, then hPa to Pa
+        # note that instantaneous pressure has 0.1 hPa precision
+        pressure=(data.p_i + 1000.0) * 100.0,
+        windDirection=data.wdir_i,
+        windSpeed=data.wspd_i,
+        latitude=data.gps_lat_fit,
+        longitude=data.gps_lon_fit,
+        # TODO: This might need to be relative to snow height instead.
+        heightOfStationGroundAboveMeanSeaLevel=heightOfStationGroundAboveMeanSeaLevel,
+        heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformTempRH=heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformTempRH,
+        heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformWSPD=heightOfSensorAboveLocalGroundOrDeckOfMarinePlatformWSPD,
+        heightOfBarometerAboveMeanSeaLevel=heightOfBarometerAboveMeanSeaLevel,
+    )
+    return output_row
 
 
-def min_data_check(s, stid):
-    '''Check that we have minimum required fields to proceed with writing to BUFR
+def min_data_check(s):
+    """Check that we have minimum required fields to proceed with writing to BUFR
     For wx vars, we currently require both air temp and pressure to be non-NaN.
     If you know a specific var is reporting bad data, you can ignore just that var
     using the vars_to_skip dict in wmo_config.
 
     Parameters
     ----------
     s : pandas series
         The current obset we are working with (for BUFR submission)
-    stid : str
-        The station ID, such as NUK_L
 
     Returns
     -------
     min_data_wx_result : bool
         True (default), the test for min wx data passed. False, the test failed.
     min_data_pos_result : bool
         True (default), the test for min position data passed. False, the test failed.
-    '''
+    """
     min_data_wx_result = True
     min_data_pos_result = True
 
     # Can use pd.isna() or math.isnan() below...
 
     # Always require valid air temp and valid pressure (both must be non-nan)
     # if (pd.isna(s['t_i']) is False) and (pd.isna(s['p_i']) is False):
     #     pass
     # else:
     #     print('----> Failed min_data_check for air temp and pressure!')
     #     min_data_wx_result = False
 
     # If both air temp and pressure are nan, do not submit.
     # This will allow the case of having only one or the other.
-    if (pd.isna(s['t_i']) is True) and (pd.isna(s['p_i']) is True):
-        print('----> Failed min_data_check for air temp and pressure!')
+    if (pd.isna(s["t_i"]) is True) and (pd.isna(s["p_i"]) is True):
+        logger.warning("----> Failed min_data_check for air temp and pressure!")
         min_data_wx_result = False
 
     # Missing just elevation OK
     # if (pd.isna(s['gps_lat_fit']) is False) and (pd.isna(s['gps_lon_fit']) is False):
     #     pass
     # Require all three: lat, lon, elev
-    if ((pd.isna(s['gps_lat_fit']) is False) and
-        (pd.isna(s['gps_lon_fit']) is False) and
-        (pd.isna(s['gps_alt_fit']) is False)):
+    if (
+        (pd.isna(s["gps_lat_fit"]) is False)
+        and (pd.isna(s["gps_lon_fit"]) is False)
+        and (pd.isna(s["gps_alt_fit"]) is False)
+    ):
         pass
     else:
-        print('----> Failed min_data_check for position!')
+        logger.warning("----> Failed min_data_check for position!")
         min_data_pos_result = False
 
     return min_data_wx_result, min_data_pos_result
+
+def main():
+    args = parse_arguments_bufr().parse_args()
+
+    log_level = logging.INFO
+    if args.verbose:
+        log_level = logging.DEBUG
+    logging.basicConfig(
+        stream=sys.stdout,
+        format="%(asctime)s; %(levelname)s; %(name)s; %(message)s",
+        level=log_level,
+    )
+
+    # Interpret all input file paths as glob patterns if they don't exist
+    input_files: List[Path] = list()
+    for path in args.input_files:
+        if path.exists():
+            input_files.append(path)
+        else:
+            # The input path might be a glob pattern
+            input_files += map(Path, glob.glob(path.as_posix()))
+
+    get_bufr(
+        bufr_out=args.bufr_out,
+        input_files=input_files,
+        store_positions=args.store_positions,
+        positions_filepath=args.positions_filepath,
+        time_limit=args.time_limit,
+        timestamps_pickle_filepath=args.timestamps_pickle_filepath,
+        now_timestamp=args.latest_timestamp,
+        station_configuration_path=args.station_configuration_mapping,
+        positions_seed_path=args.position_seed,
+    )
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pypromice-1.3.3/src/pypromice/process/L0toL1.py` & `pypromice-1.3.4/src/pypromice/process/L0toL1.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,32 +168,34 @@
 
     if ds.attrs['format'] == 'raw':
         # 10-minute data, no shifting
         df_out = df
     elif ds.attrs['format'] == 'STM':
         # hourly-averaged, non-transmitted
         # shift everything except instantaneous, any logger type
-        df_a = df_a.shift(periods=-1, freq="H")
+        df_a = df_a.shift(periods=-1, freq="h")
         df_out = pd.concat([df_a, df_i], axis=1) # different columns, same datetime indices
+        df_out = df_out.sort_index()
     elif ds.attrs['format'] == 'TX':
         if ds.attrs['logger_type'] == 'CR1000X':
             # v3, data is hourly all year long
             # shift everything except instantaneous
             df_a = df_a.shift(periods=-1, freq="H")
             df_out = pd.concat([df_a, df_i], axis=1) # different columns, same datetime indices
+            df_out = df_out.sort_index()
         elif ds.attrs['logger_type'] == 'CR1000':
             # v2, data is hourly (6-hr for instantaneous) for DOY 100-300, otherwise daily at 00 UTC
             # shift non-instantaneous hourly for DOY 100-300, else do not shift daily
             df_a_hourly = df_a.loc[(df_a['doy'] >= 100) & (df_a['doy'] <= 300)]
             # df_a_hourly = df_a.loc[df_a['doy'].between(100, 300, inclusive='both')] # equivalent to above
             df_a_daily_1 = df_a.loc[(df_a['doy'] < 100)]
             df_a_daily_2 = df_a.loc[(df_a['doy'] > 300)]
 
             # shift the hourly ave data
-            df_a_hourly = df_a_hourly.shift(periods=-1, freq="H")
+            df_a_hourly = df_a_hourly.shift(periods=-1, freq="h")
 
             # stitch everything back together
             df_concat_u = pd.concat([df_a_daily_1, df_a_daily_2, df_a_hourly], axis=0) # same columns, different datetime indices
             # It's now possible for df_concat_u to have duplicate datetime indices
             df_concat_u = df_concat_u[~df_concat_u.index.duplicated(keep='first')] # drop duplicates, keep=first is arbitrary
 
             df_out = pd.concat([df_concat_u, df_i], axis=1) # different columns, same datetime indices
```

### Comparing `pypromice-1.3.3/src/pypromice/process/L1toL2.py` & `pypromice-1.3.4/src/pypromice/process/L1toL2.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/process/L2toL3.py` & `pypromice-1.3.4/src/pypromice/process/L2toL3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/process/aws.py` & `pypromice-1.3.4/src/pypromice/process/aws.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/process/get_l3.py` & `pypromice-1.3.4/src/pypromice/process/get_l3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/process/join_l3.py` & `pypromice-1.3.4/src/pypromice/process/join_l3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/process/metadata.csv` & `pypromice-1.3.4/src/pypromice/process/metadata.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/process/value_clipping.py` & `pypromice-1.3.4/src/pypromice/process/value_clipping.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,27 +29,18 @@
 
     variable_limits = var_configurations[cols].dropna(how="all")
     for var, row in variable_limits.iterrows():
 
         if var not in list(ds.variables):
             continue
 
-        if var in ["rh_u_cor", "rh_l_cor"]:
-            ds[var] = ds[var].where(ds[var] >= row.lo, other=0)
-            ds[var] = ds[var].where(ds[var] <= row.hi, other=100)
-
-            # Mask out invalid corrections based on uncorrected var
-            var_uncor = var.split("_cor")[0]
-            ds[var] = ds[var].where(~np.isnan(ds[var_uncor]), other=np.nan)
-
-        else:
-            if ~np.isnan(row.lo):
-                ds[var] = ds[var].where(ds[var] >= row.lo)
-            if ~np.isnan(row.hi):
-                ds[var] = ds[var].where(ds[var] <= row.hi)
+        if ~np.isnan(row.lo):
+            ds[var] = ds[var].where(ds[var] >= row.lo)
+        if ~np.isnan(row.hi):
+            ds[var] = ds[var].where(ds[var] <= row.hi)
 
         other_vars = row.OOL
         if isinstance(other_vars, str) and ~ds[var].isnull().all():
             for o in other_vars.split():
                 if o not in list(ds.variables):
                     continue
                 else:
```

### Comparing `pypromice-1.3.3/src/pypromice/process/variables.csv` & `pypromice-1.3.4/src/pypromice/process/variables.csv`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 field,standard_name,long_name,units,lo,hi,OOL,station_type,data_type,max_decimals,coverage_content_type,coordinates,instantaneous_hourly,comment
 time,time,Time,yyyy-mm-dd HH:MM:SS,,,,all,all,,physicalMeasurement,time lat lon alt,,
 rec,record,Record,-,,,,all,,0,referenceInformation,time lat lon alt,,L0 only
 p_u,air_pressure,Air pressure (upper boom),hPa,650,1100,z_pt z_pt_cor dshf_u dlhf_u qh_u,all,all,4,physicalMeasurement,time lat lon alt,False,
 p_l,air_pressure,Air pressure (lower boom),hPa,650,1100,dshf_l dlhf_l qh_l,two-boom,all,4,physicalMeasurement,time lat lon alt,False,
 t_u,air_temperature,Air temperature (upper boom),degrees_C,-80,40,rh_u_cor cc dsr_cor usr_cor z_boom z_stake dshf_u dlhf_u qh_u,all,all,4,physicalMeasurement,time lat lon alt,False,
 t_l,air_temperature,Air temperature (lower boom),degrees_C,-80,40,rh_l_cor z_boom_l dshf_l dlhf_l qh_l ,two-boom,all,4,physicalMeasurement,time lat lon alt,False,PT100 temperature at boom
-rh_u,relative_humidity,Relative humidity (upper boom),%,0,150,rh_u_cor,all,all,4,physicalMeasurement,time lat lon alt,False,
+rh_u,relative_humidity,Relative humidity (upper boom),%,0,100,rh_u_cor,all,all,4,physicalMeasurement,time lat lon alt,False,
 rh_u_cor,relative_humidity_corrected,Relative humidity (upper boom) - corrected,%,0,150,dshf_u dlhf_u qh_u,all,all,4,modelResult,time lat lon alt,False,
-qh_u,specific_humidity,Specific humidity (upper boom),%,0,100,,all,all,4,modelResult,time lat lon alt,False,Derived value (L2 or later)
-rh_l,relative_humidity,Relative humidity (lower boom),%,0,150,rh_l_cor,two-boom,all,4,physicalMeasurement,time lat lon alt,False,
+qh_u,specific_humidity,Specific humidity (upper boom),kg/kg,0,100,,all,all,4,modelResult,time lat lon alt,False,Derived value (L2 or later)
+rh_l,relative_humidity,Relative humidity (lower boom),%,0,100,rh_l_cor,two-boom,all,4,physicalMeasurement,time lat lon alt,False,
 rh_l_cor,relative_humidity_corrected,Relative humidity (lower boom) - corrected,%,0,150,dshf_l dlhf_l qh_l,two-boom,all,4,modelResult,time lat lon alt,False,
-qh_l,specific_humidity,Specific humidity (lower boom),%,0,100,,two-boom,all,4,modelResult,time lat lon alt,False,Derived value (L2 or later)
+qh_l,specific_humidity,Specific humidity (lower boom),kg/kg,0,100,,two-boom,all,4,modelResult,time lat lon alt,False,Derived value (L2 or later)
 wspd_u,wind_speed,Wind speed (upper boom),m s-1,0,100,"wdir_u wspd_x_u wspd_y_u dshf_u dlhf_u qh_u, precip_u",all,all,4,physicalMeasurement,time lat lon alt,False,
 wspd_l,wind_speed,Wind speed (lower boom),m s-1,0,100,"wdir_l wspd_x_l wspd_y_l dshf_l dlhf_l qh_l , precip_l",two-boom,all,4,physicalMeasurement,time lat lon alt,False,
 wdir_u,wind_from_direction,Wind from direction (upper boom),degrees,1,360,wspd_x_u wspd_y_u,all,all,4,physicalMeasurement,time lat lon alt,False,
 wdir_std_u,wind_from_direction_standard_deviation,Wind from direction (standard deviation),degrees,,,,one-boom,,4,qualityInformation,time lat lon alt,False,L0 only
 wdir_l,wind_from_direction,Wind from direction (lower boom),degrees,1,360,wspd_x_l wspd_y_l,two-boom,all,4,physicalMeasurement,time lat lon alt,False,
 wspd_x_u,wind_speed_from_x_direction,Wind speed from x direction (upper boom),m s-1,-100,100,wdir_u wspd_u,all,all,4,modelResult,time lat lon alt,False,L0 only
 wspd_y_u,wind_speed_from_y_direction,Wind speed from y direction (upper boom),m s-1,-100,100,wdir_u wspd_u,all,all,4,modelResult,time lat lon alt,False,L0 only
@@ -77,18 +77,16 @@
 batt_v_ini,,,-,0,30,,,all,2,physicalMeasurement,time lat lon alt,True,L0 only
 batt_v_ss,battery_voltage_at_sample_start,Battery voltage (sample start),V,0,30,,,all,2,physicalMeasurement,time lat lon alt,True,L0 only
 fan_dc_u,fan_current,Fan current (upper boom),mA,0,200,,all,all,2,physicalMeasurement,time lat lon alt,True,
 fan_dc_l,fan_current,Fan current (lower boom),mA,0,200,,two-boom,all,2,physicalMeasurement,time lat lon alt,True,
 freq_vw,frequency_of_precipitation_wire_vibration,Frequency of vibrating wire in precipitation gauge,Hz,0,10000,precip_u,,all,,physicalMeasurement,time lat lon alt,True,L0 only
 t_log,temperature_of_logger,Logger temperature,degrees_C,-80,40,,one-boom,all,4,physicalMeasurement,time lat lon alt,True,LoggerTemperature(C)
 t_rad,temperature_of_radiation_sensor,Radiation sensor temperature,degrees_C,-80,40,t_surf dlr ulr,all,all,4,physicalMeasurement,time lat lon alt,False,
-p_i,air_pressure,Air pressure (instantaneous) minus 1000,hPa,-350,100,,all,TX,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
-t_i,air_temperature,Air temperature (instantaneous),degrees_C,-80,40,,all,TX,4,physicalMeasurement,time lat lon alt,True,"PT100 temperature at boom, for meteorological observations"
-rh_i,relative_humidity,Relative humidity (instantaneous),%,0,150,rh_i_cor,all,TX,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
-rh_i_cor,relative_humidity_corrected,Relative humidity (instantaneous) – corrected,%,0,100,,all,TX,4,modelResult,time lat lon alt,True,For meteorological observations
-wspd_i,wind_speed,Wind speed (instantaneous),m s-1,0,100,wdir_i wspd_x_i wspd_y_i,all,TX,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
-wdir_i,wind_from_direction,Wind from direction (instantaneous),degrees,1,360,wspd_x_i wspd_y_i,all,TX,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
-wspd_x_i,wind_speed_from_x_direction,Wind speed from x direction (instantaneous),m s-1,-100,100,wdir_i wspd_i,all,TX,4,modelResult,time lat lon alt,True,For meteorological observations
-wspd_y_i,wind_speed_from_y_direction,Wind speed from y direction (instantaneous),m s-1,-100,100,wdir_i wspd_i,all,TX,4,modelResult,time lat lon alt,True,For meteorological observations
-msg_i,message,Message string (instantaneous),-,,,,all,TX,,qualityInformation,time lat lon alt,True,For meteorological observations
-msg_lat,message_latitude,latitude from modem (email text),degrees_north,50,83,,all,all,6,coordinate,time lat lon alt,True,
-msg_lon,message_longitude,longitude from modem (email text),degrees_east,-72,13,,all,all,6,coordinate,time lat lon alt,True,
+p_i,air_pressure,Air pressure (instantaneous) minus 1000,hPa,-350,100,,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
+t_i,air_temperature,Air temperature (instantaneous),degrees_C,-80,40,,all,all,4,physicalMeasurement,time lat lon alt,True,"PT100 temperature at boom, for meteorological observations"
+rh_i,relative_humidity,Relative humidity (instantaneous),%,0,150,rh_i_cor,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
+rh_i_cor,relative_humidity_corrected,Relative humidity (instantaneous) – corrected,%,0,100,,all,all,4,modelResult,time lat lon alt,True,For meteorological observations
+wspd_i,wind_speed,Wind speed (instantaneous),m s-1,0,100,wdir_i wspd_x_i wspd_y_i,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
+wdir_i,wind_from_direction,Wind from direction (instantaneous),degrees,1,360,wspd_x_i wspd_y_i,all,all,4,physicalMeasurement,time lat lon alt,True,For meteorological observations
+wspd_x_i,wind_speed_from_x_direction,Wind speed from x direction (instantaneous),m s-1,-100,100,wdir_i wspd_i,all,all,4,modelResult,time lat lon alt,True,For meteorological observations
+wspd_y_i,wind_speed_from_y_direction,Wind speed from y direction (instantaneous),m s-1,-100,100,wdir_i wspd_i,all,all,4,modelResult,time lat lon alt,True,For meteorological observations
+msg_i,message,Message string (instantaneous),-,,,,all,all,,qualityInformation,time lat lon alt,True,For meteorological observations
```

### Comparing `pypromice-1.3.3/src/pypromice/qc/github_data_issues.py` & `pypromice-1.3.4/src/pypromice/qc/github_data_issues.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,40 +13,34 @@
     'adjustData',
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def flagNAN(ds_in,
-            flag_url='https://raw.githubusercontent.com/GEUS-Glaciology-and-Climate/PROMICE-AWS-data-issues/master/flags/',
-            flag_dir='local/flags/'):
+            flag_dir='../PROMICE-AWS-data-issues/flags'):
     '''Read flagged data from .csv file. For each variable, and downstream
     dependents, flag as invalid (or other) if set in the flag .csv
 
     Parameters
     ----------
     ds_in : xr.Dataset
         Level 0 dataset
-    flag_url : str
-        URL to directory where .csv flag files can be found
     flag_dir : str
         File directory where .csv flag files can be found
 
     Returns
     -------
     ds : xr.Dataset
         Level 0 data with flagged data
     '''
     ds = ds_in.copy(deep=True)
     df = None
 
-    df = _getDF(flag_url + ds.attrs["station_id"] + ".csv",
-                os.path.join(flag_dir, ds.attrs["station_id"] + ".csv"),
-                # download = False,  # only for working on draft local flag'n'fix files
-                )
+    df = _getDF(os.path.join(flag_dir, ds.attrs["station_id"] + ".csv"))
 
     if isinstance(df, pd.DataFrame):
         df.t0 = pd.to_datetime(df.t0).dt.tz_localize(None)
         df.t1 = pd.to_datetime(df.t1).dt.tz_localize(None)
 
         if df.shape[0] > 0:
             for i in df.index:
@@ -67,47 +61,43 @@
                 if pd.isnull(t0):
                     t0 = ds['time'].values[0]
                 if pd.isnull(t1):
                     t1 = ds['time'].values[-1]
 
                 for v in varlist:
                     if v in list(ds.keys()):
-                        logger.info(f'---> flagging {v} between {t0} and {t1}')
+                        logger.info(f'---> flagging {t0} {t1} {v}')
                         ds[v] = ds[v].where((ds['time'] < t0) | (ds['time'] > t1))
                     else:
                         logger.info(f'---> could not flag {v} not in dataset')
 
     return ds
 
 
 def adjustTime(ds,
-               adj_url="https://raw.githubusercontent.com/GEUS-Glaciology-and-Climate/PROMICE-AWS-data-issues/master/adjustments/",
-               adj_dir='local/adjustments/',
+               adj_dir='../PROMICE-AWS-data-issues/adjustments/',
                var_list=[], skip_var=[]):
     '''Read adjustment data from .csv file. Only applies the "time_shift" adjustment
 
     Parameters
     ----------
     ds : xr.Dataset
         Level 0 dataset
-    adj_url : str
-        URL to directory where .csv adjustment files can be found
     adj_dir : str
         File directory where .csv adjustment files can be found
 
     Returns
     -------
     ds : xr.Dataset
         Level 0 data with flagged data
     '''
     ds_out = ds.copy(deep=True)
     adj_info=None
 
-    adj_info = _getDF(adj_url + ds.attrs["station_id"] + ".csv",
-                      os.path.join(adj_dir, ds.attrs["station_id"] + ".csv"),)
+    adj_info = _getDF(os.path.join(adj_dir, ds.attrs["station_id"] + ".csv"))
 
     if isinstance(adj_info, pd.DataFrame):
 
 
         if "time_shift" in adj_info.adjust_function.values:
             time_shifts = adj_info.loc[adj_info.adjust_function == "time_shift", :]
             # if t1 is left empty, then adjustment is applied until the end of the file
@@ -141,40 +131,34 @@
                 if t0 > pd.Timestamp.now():
                     ds_out = ds_out.sel(time=slice(pd.to_datetime(ds_out.time.values[0]),
                                                    t0))
     return ds_out
 
 
 def adjustData(ds,
-               adj_url="https://raw.githubusercontent.com/GEUS-Glaciology-and-Climate/PROMICE-AWS-data-issues/master/adjustments/",
-               adj_dir='local/adjustments/',
+               adj_dir='../PROMICE-AWS-data-issues/adjustments/',
                var_list=[], skip_var=[]):
     '''Read adjustment data from .csv file. For each variable, and downstream
     dependents, adjust data accordingly if set in the adjustment .csv
 
     Parameters
     ----------
     ds : xr.Dataset
         Level 0 dataset
-    adj_url : str
-        URL to directory where .csv adjustment files can be found
     adj_dir : str
         File directory where .csv adjustment files can be found
 
     Returns
     -------
     ds : xr.Dataset
         Level 0 data with flagged data
     '''
     ds_out = ds.copy(deep=True)
     adj_info=None
-    adj_info = _getDF(adj_url + ds.attrs["station_id"] + ".csv",
-                      os.path.join(adj_dir, ds.attrs["station_id"] + ".csv"),
-                      # download = False,  # only for working on draft local flag'n'fix files
-                      )
+    adj_info = _getDF(os.path.join(adj_dir, ds.attrs["station_id"] + ".csv"))
 
     if isinstance(adj_info, pd.DataFrame):
         # removing potential time shifts from the adjustment list
         adj_info = adj_info.loc[adj_info.adjust_function != "time_shift", :]
 
         # making sure that t0 and t1 columns are object dtype then replaceing nan with None
         adj_info[['t0','t1']] = adj_info[['t0','t1']].astype(object)
@@ -223,15 +207,15 @@
 
                 index_slice = dict(time=slice(t0, t1))
 
                 if len(ds_out[var].loc[index_slice].time.time) == 0:
                     logger.info("Time range does not intersect with dataset")
                     continue
 
-                logger.info(f'---> adjusting {var} between {t0} and {t1} ({func} {val})')
+                logger.info(f'---> {t0} {t1} {var} {func} {val}')
 				
                 if func == "add":
                     ds_out[var].loc[index_slice] = ds_out[var].loc[index_slice].values + val
                     # flagging adjusted values
                     # if var + "_adj_flag" not in ds_out.columns:
                     #     ds_out[var + "_adj_flag"] = 0
                     # msk = ds_out[var].loc[index_slice])].notnull()
@@ -301,44 +285,30 @@
 
                 if func == "rotate":
                     ds_out[var].loc[index_slice] = (ds_out[var].loc[index_slice].values + val) % 360
 
     return ds_out
 
 
-def _getDF(flag_url, flag_file, download=True):
+def _getDF(flag_file):
     '''Get dataframe from flag or adjust file. First attempt to retrieve from
     URL. If this fails then attempt to retrieve from local file
 
     Parameters
     ----------
-    flag_url : str
-        URL address to file
     flag_file : str
         Local path to file
-    download : bool
-        Flag to download file from URL
 
     Returns
     -------
     df : pd.DataFrame
         Flag or adjustment dataframe
     '''
 
-    # Download local copy as csv
-    if download==True:
-        os.makedirs(os.path.dirname(flag_file), exist_ok = True)
-
-        try:
-            urllib.request.urlretrieve(flag_url, flag_file)
-            logger.info(f"Downloaded a {flag_file.split('/')[-2][:-1],} file to {flag_file}")
-        except (HTTPError, URLError) as e:
-            logger.info(f"Unable to download {flag_file.split('/')[-2][:-1],} file, using local file: {flag_file}")
-    else:
-        logger.info(f"Using local {flag_file.split('/')[-2][:-1],} file: {flag_file}")
+    logger.info(f"Using file: {flag_file}")
 
     if os.path.isfile(flag_file):
         df = pd.read_csv(
                         flag_file,
                         comment="#",
                         skipinitialspace=True,
                         ).dropna(how='all', axis='rows')
```

### Comparing `pypromice-1.3.3/src/pypromice/qc/percentiles/compute_thresholds.py` & `pypromice-1.3.4/src/pypromice/qc/percentiles/compute_thresholds.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/qc/percentiles/outlier_detector.py` & `pypromice-1.3.4/src/pypromice/qc/percentiles/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/qc/percentiles/thresholds.csv` & `pypromice-1.3.4/src/pypromice/qc/percentiles/thresholds.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/qc/persistence.py` & `pypromice-1.3.4/src/pypromice/qc/persistence.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/qc/persistence_test.py` & `pypromice-1.3.4/src/pypromice/qc/persistence_test.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_config1.toml` & `pypromice-1.3.4/src/pypromice/test/test_config1.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_config2.toml` & `pypromice-1.3.4/src/pypromice/test/test_config2.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_email` & `pypromice-1.3.4/src/pypromice/test/test_email`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_percentile.py` & `pypromice-1.3.4/src/pypromice/test/test_percentile.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_raw1.txt` & `pypromice-1.3.4/src/pypromice/test/test_raw1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_raw_DataTable2.txt` & `pypromice-1.3.4/src/pypromice/test/test_raw_DataTable2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_raw_SlimTableMem1.txt` & `pypromice-1.3.4/src/pypromice/test/test_raw_SlimTableMem1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_raw_transmitted1.txt` & `pypromice-1.3.4/src/pypromice/test/test_raw_transmitted1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/test/test_raw_transmitted2.txt` & `pypromice-1.3.4/src/pypromice/test/test_raw_transmitted2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/tx/get_l0tx.py` & `pypromice-1.3.4/src/pypromice/tx/get_l0tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/tx/get_msg.py` & `pypromice-1.3.4/src/pypromice/tx/get_msg.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/tx/get_watsontx.py` & `pypromice-1.3.4/src/pypromice/tx/get_watsontx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/tx/payload_formats.csv` & `pypromice-1.3.4/src/pypromice/tx/payload_formats.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice/tx/tx.py` & `pypromice-1.3.4/src/pypromice/tx/tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.3/src/pypromice.egg-info/PKG-INFO` & `pypromice-1.3.4/src/pypromice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.3.3
+Version: 1.3.4
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
@@ -23,14 +23,15 @@
 Requires-Dist: xarray>=2022.6.0
 Requires-Dist: toml
 Requires-Dist: scipy>=1.9.0
 Requires-Dist: scikit-learn>=1.1.0
 Requires-Dist: Bottleneck
 Requires-Dist: netcdf4
 Requires-Dist: pyDataverse
+Requires-Dist: eccodes
 
 # pypromice
 [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://badge.fury.io/py/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/version.svg)](https://anaconda.org/conda-forge/pypromice) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pypromice/badges/platforms.svg)](https://anaconda.org/conda-forge/pypromice) [![](<https://img.shields.io/badge/Dataverse DOI-10.22008/FK2/3TSBF0-orange>)](https://www.doi.org/10.22008/FK2/3TSBF0) [![DOI](https://joss.theoj.org/papers/10.21105/joss.05298/status.svg)](https://doi.org/10.21105/joss.05298) [![Documentation Status](https://readthedocs.org/projects/pypromice/badge/?version=latest)](https://pypromice.readthedocs.io/en/latest/?badge=latest)
  
 pypromice is designed for processing and handling [PROMICE](https://promice.org) automated weather station (AWS) data.
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information.
```

### Comparing `pypromice-1.3.3/src/pypromice.egg-info/SOURCES.txt` & `pypromice-1.3.4/src/pypromice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 src/pypromice.egg-info/entry_points.txt
 src/pypromice.egg-info/requires.txt
 src/pypromice.egg-info/top_level.txt
 src/pypromice/get/__init__.py
 src/pypromice/get/get.py
 src/pypromice/get/get_promice_data.py
 src/pypromice/postprocess/__init__.py
-src/pypromice/postprocess/csv2bufr.py
+src/pypromice/postprocess/bufr_to_csv.py
+src/pypromice/postprocess/bufr_utilities.py
 src/pypromice/postprocess/get_bufr.py
-src/pypromice/postprocess/wmo_config.py
+src/pypromice/postprocess/positions_seed.csv
+src/pypromice/postprocess/real_time_utilities.py
+src/pypromice/postprocess/station_configurations.toml
 src/pypromice/process/L0toL1.py
 src/pypromice/process/L1toL2.py
 src/pypromice/process/L2toL3.py
 src/pypromice/process/__init__.py
 src/pypromice/process/aws.py
 src/pypromice/process/get_l3.py
 src/pypromice/process/join_l3.py
```

