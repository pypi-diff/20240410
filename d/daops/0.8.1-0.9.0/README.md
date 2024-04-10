# Comparing `tmp/daops-0.8.1.tar.gz` & `tmp/daops-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daops-0.8.1.tar", last modified: Thu May 12 15:44:02 2022, max compression
+gzip compressed data, was "daops-0.9.0.tar", last modified: Fri Nov 17 13:54:49 2023, max compression
```

## Comparing `daops-0.8.1.tar` & `daops-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.300532 daops-0.8.1/
--rw-r--r--   0 pingu      (501) staff       (20)      271 2022-04-12 15:23:46.000000 daops-0.8.1/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     1516 2021-08-11 09:41:41.000000 daops-0.8.1/LICENSE
--rw-r--r--   0 pingu      (501) staff       (20)      171 2021-08-11 09:41:41.000000 daops-0.8.1/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     3412 2022-05-12 15:44:02.300754 daops-0.8.1/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     2035 2021-08-11 09:41:41.000000 daops-0.8.1/README.rst
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.272786 daops-0.8.1/daops/
--rw-r--r--   0 pingu      (501) staff       (20)      562 2022-05-12 15:43:38.000000 daops-0.8.1/daops/__init__.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.278988 daops-0.8.1/daops/catalog/
--rw-r--r--   0 pingu      (501) staff       (20)      402 2021-08-11 09:41:41.000000 daops-0.8.1/daops/catalog/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     1591 2022-01-19 12:12:53.000000 daops-0.8.1/daops/catalog/base.py
--rw-r--r--   0 pingu      (501) staff       (20)     1780 2022-01-19 12:12:53.000000 daops-0.8.1/daops/catalog/intake.py
--rw-r--r--   0 pingu      (501) staff       (20)      944 2022-04-12 15:23:46.000000 daops-0.8.1/daops/catalog/util.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.282275 daops-0.8.1/daops/data_utils/
--rw-r--r--   0 pingu      (501) staff       (20)      110 2021-08-11 09:41:41.000000 daops-0.8.1/daops/data_utils/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/daops/data_utils/array_utils.py
--rw-r--r--   0 pingu      (501) staff       (20)     1775 2022-01-19 12:12:53.000000 daops-0.8.1/daops/data_utils/attr_utils.py
--rw-r--r--   0 pingu      (501) staff       (20)      403 2022-01-19 12:12:53.000000 daops-0.8.1/daops/data_utils/common_utils.py
--rw-r--r--   0 pingu      (501) staff       (20)     2439 2022-01-19 12:12:53.000000 daops-0.8.1/daops/data_utils/coord_utils.py
--rw-r--r--   0 pingu      (501) staff       (20)      468 2022-01-19 12:12:53.000000 daops-0.8.1/daops/data_utils/var_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.283002 daops-0.8.1/daops/etc/
--rw-r--r--   0 pingu      (501) staff       (20)      122 2022-05-06 14:42:24.000000 daops-0.8.1/daops/etc/roocs.ini
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.284346 daops-0.8.1/daops/fix_utils/
--rw-r--r--   0 pingu      (501) staff       (20)     4498 2022-01-19 12:12:53.000000 daops-0.8.1/daops/fix_utils/decadal_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.287459 daops-0.8.1/daops/ops/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/daops/ops/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     4209 2022-03-15 18:33:51.000000 daops-0.8.1/daops/ops/average.py
--rw-r--r--   0 pingu      (501) staff       (20)     2943 2021-08-11 09:41:41.000000 daops-0.8.1/daops/ops/base.py
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/daops/ops/regrid.py
--rw-r--r--   0 pingu      (501) staff       (20)     2733 2022-01-19 12:12:53.000000 daops-0.8.1/daops/ops/subset.py
--rw-r--r--   0 pingu      (501) staff       (20)      820 2022-04-12 15:23:46.000000 daops-0.8.1/daops/processor.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.291729 daops-0.8.1/daops/utils/
--rw-r--r--   0 pingu      (501) staff       (20)       35 2021-08-11 09:41:41.000000 daops-0.8.1/daops/utils/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     1240 2022-03-15 18:33:51.000000 daops-0.8.1/daops/utils/base_lookup.py
--rw-r--r--   0 pingu      (501) staff       (20)      420 2022-04-12 15:23:46.000000 daops-0.8.1/daops/utils/common.py
--rw-r--r--   0 pingu      (501) staff       (20)     5614 2022-04-12 15:23:46.000000 daops-0.8.1/daops/utils/consolidate.py
--rw-r--r--   0 pingu      (501) staff       (20)     3161 2022-04-12 15:23:46.000000 daops-0.8.1/daops/utils/core.py
--rw-r--r--   0 pingu      (501) staff       (20)     1819 2021-08-11 09:41:41.000000 daops-0.8.1/daops/utils/fixer.py
--rw-r--r--   0 pingu      (501) staff       (20)     1570 2022-04-12 15:23:46.000000 daops-0.8.1/daops/utils/normalise.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.276099 daops-0.8.1/daops.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     3412 2022-05-12 15:44:01.000000 daops-0.8.1/daops.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1220 2022-05-12 15:44:02.000000 daops-0.8.1/daops.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2022-05-12 15:44:01.000000 daops-0.8.1/daops.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)      238 2022-05-12 15:44:01.000000 daops-0.8.1/daops.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)       12 2022-05-12 15:44:02.000000 daops-0.8.1/daops.egg-info/top_level.txt
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.292491 daops-0.8.1/etc/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/etc/daops_eg.cfg
--rw-r--r--   0 pingu      (501) staff       (20)      238 2022-05-12 12:23:52.000000 daops-0.8.1/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      198 2022-04-12 15:23:46.000000 daops-0.8.1/requirements_dev.txt
--rw-r--r--   0 pingu      (501) staff       (20)      939 2022-05-12 15:44:02.301840 daops-0.8.1/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     3012 2022-05-12 15:43:38.000000 daops-0.8.1/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.297135 daops-0.8.1/tests/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/tests/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     3160 2022-04-12 15:23:46.000000 daops-0.8.1/tests/_common.py
--rw-r--r--   0 pingu      (501) staff       (20)     1108 2021-08-11 09:41:41.000000 daops-0.8.1/tests/conftest.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.298684 daops-0.8.1/tests/test_catalog/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/tests/test_catalog/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     3137 2021-08-11 09:41:41.000000 daops-0.8.1/tests/test_catalog/test_intake.py
--rw-r--r--   0 pingu      (501) staff       (20)      524 2022-01-19 12:12:53.000000 daops-0.8.1/tests/test_catalog/test_util.py
--rw-r--r--   0 pingu      (501) staff       (20)     5537 2021-08-11 09:41:41.000000 daops-0.8.1/tests/test_daops.py
--rw-r--r--   0 pingu      (501) staff       (20)    27358 2022-01-19 12:12:53.000000 daops-0.8.1/tests/test_fixes_applied.py
--rw-r--r--   0 pingu      (501) staff       (20)     2314 2022-04-12 15:23:46.000000 daops-0.8.1/tests/test_func_chainer.py
--rw-r--r--   0 pingu      (501) staff       (20)     1879 2022-04-12 15:23:46.000000 daops-0.8.1/tests/test_logging.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2022-05-12 15:44:02.299937 daops-0.8.1/tests/test_xarray/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2021-08-11 09:41:41.000000 daops-0.8.1/tests/test_xarray/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     7183 2022-04-12 15:23:46.000000 daops-0.8.1/tests/test_xarray/test_xarray_aggregation.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.764862 daops-0.9.0/
+-rw-r--r--   0 pingu      (501) staff       (20)      271 2023-11-15 14:06:34.000000 daops-0.9.0/AUTHORS.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     1516 2023-11-08 16:10:30.000000 daops-0.9.0/LICENSE
+-rw-r--r--   0 pingu      (501) staff       (20)      171 2023-11-08 16:10:30.000000 daops-0.9.0/MANIFEST.in
+-rw-r--r--   0 pingu      (501) staff       (20)     4079 2023-11-17 13:54:49.764385 daops-0.9.0/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     2035 2023-11-08 16:10:30.000000 daops-0.9.0/README.rst
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.695252 daops-0.9.0/daops/
+-rw-r--r--   0 pingu      (501) staff       (20)      562 2023-11-17 13:52:43.000000 daops-0.9.0/daops/__init__.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.704682 daops-0.9.0/daops/catalog/
+-rw-r--r--   0 pingu      (501) staff       (20)      402 2023-11-08 16:10:30.000000 daops-0.9.0/daops/catalog/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1591 2023-11-15 14:06:34.000000 daops-0.9.0/daops/catalog/base.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1780 2023-11-15 14:06:34.000000 daops-0.9.0/daops/catalog/intake.py
+-rw-r--r--   0 pingu      (501) staff       (20)      944 2023-11-15 14:06:34.000000 daops-0.9.0/daops/catalog/util.py
+-rw-r--r--   0 pingu      (501) staff       (20)     3447 2023-11-17 13:52:43.000000 daops-0.9.0/daops/cli.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.716005 daops-0.9.0/daops/data_utils/
+-rw-r--r--   0 pingu      (501) staff       (20)      110 2023-11-08 16:10:30.000000 daops-0.9.0/daops/data_utils/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-08 16:10:30.000000 daops-0.9.0/daops/data_utils/array_utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1775 2023-11-15 14:06:34.000000 daops-0.9.0/daops/data_utils/attr_utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)      403 2023-11-15 14:06:34.000000 daops-0.9.0/daops/data_utils/common_utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2439 2023-11-15 14:06:34.000000 daops-0.9.0/daops/data_utils/coord_utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)      468 2023-11-15 14:06:34.000000 daops-0.9.0/daops/data_utils/var_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.720384 daops-0.9.0/daops/etc/
+-rw-r--r--   0 pingu      (501) staff       (20)      122 2023-11-08 16:10:30.000000 daops-0.9.0/daops/etc/roocs.ini
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.723661 daops-0.9.0/daops/fix_utils/
+-rw-r--r--   0 pingu      (501) staff       (20)     4497 2023-11-15 14:06:34.000000 daops-0.9.0/daops/fix_utils/decadal_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.731807 daops-0.9.0/daops/ops/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-08 16:10:30.000000 daops-0.9.0/daops/ops/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     4209 2023-11-15 14:33:55.000000 daops-0.9.0/daops/ops/average.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2943 2023-11-08 16:10:30.000000 daops-0.9.0/daops/ops/base.py
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-17 12:51:13.000000 daops-0.9.0/daops/ops/regrid.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2733 2023-11-15 14:06:34.000000 daops-0.9.0/daops/ops/subset.py
+-rw-r--r--   0 pingu      (501) staff       (20)      820 2023-11-15 14:06:34.000000 daops-0.9.0/daops/processor.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.741695 daops-0.9.0/daops/utils/
+-rw-r--r--   0 pingu      (501) staff       (20)       35 2023-11-08 16:10:30.000000 daops-0.9.0/daops/utils/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1240 2023-11-15 14:06:34.000000 daops-0.9.0/daops/utils/base_lookup.py
+-rw-r--r--   0 pingu      (501) staff       (20)      420 2023-11-15 14:06:34.000000 daops-0.9.0/daops/utils/common.py
+-rw-r--r--   0 pingu      (501) staff       (20)     5611 2023-11-15 14:06:34.000000 daops-0.9.0/daops/utils/consolidate.py
+-rw-r--r--   0 pingu      (501) staff       (20)     3161 2023-11-15 14:06:34.000000 daops-0.9.0/daops/utils/core.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1818 2023-11-15 14:06:34.000000 daops-0.9.0/daops/utils/fixer.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1569 2023-11-15 14:06:34.000000 daops-0.9.0/daops/utils/normalise.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.700315 daops-0.9.0/daops.egg-info/
+-rw-r--r--   0 pingu      (501) staff       (20)     4079 2023-11-17 13:54:49.000000 daops-0.9.0/daops.egg-info/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     1283 2023-11-17 13:54:49.000000 daops-0.9.0/daops.egg-info/SOURCES.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2023-11-17 13:54:49.000000 daops-0.9.0/daops.egg-info/dependency_links.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       41 2023-11-17 13:54:49.000000 daops-0.9.0/daops.egg-info/entry_points.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      239 2023-11-17 13:54:49.000000 daops-0.9.0/daops.egg-info/requires.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       12 2023-11-17 13:54:49.000000 daops-0.9.0/daops.egg-info/top_level.txt
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.742729 daops-0.9.0/etc/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-08 16:10:30.000000 daops-0.9.0/etc/daops_eg.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)      167 2023-11-17 13:52:43.000000 daops-0.9.0/requirements.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      203 2023-11-17 13:52:43.000000 daops-0.9.0/requirements_dev.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      939 2023-11-17 13:54:49.766766 daops-0.9.0/setup.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     3114 2023-11-17 13:52:43.000000 daops-0.9.0/setup.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.755074 daops-0.9.0/tests/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-08 16:10:30.000000 daops-0.9.0/tests/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     3160 2023-11-15 14:07:57.000000 daops-0.9.0/tests/_common.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1108 2023-11-15 14:34:34.000000 daops-0.9.0/tests/conftest.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.759025 daops-0.9.0/tests/test_catalog/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-08 16:10:30.000000 daops-0.9.0/tests/test_catalog/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     3137 2023-11-08 16:10:30.000000 daops-0.9.0/tests/test_catalog/test_intake.py
+-rw-r--r--   0 pingu      (501) staff       (20)      524 2023-11-15 14:06:34.000000 daops-0.9.0/tests/test_catalog/test_util.py
+-rw-r--r--   0 pingu      (501) staff       (20)    21002 2023-11-17 13:52:43.000000 daops-0.9.0/tests/test_cli.py
+-rw-r--r--   0 pingu      (501) staff       (20)     5542 2023-11-15 14:06:34.000000 daops-0.9.0/tests/test_daops.py
+-rw-r--r--   0 pingu      (501) staff       (20)    27358 2023-11-15 14:06:34.000000 daops-0.9.0/tests/test_fixes_applied.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2314 2023-11-15 14:06:34.000000 daops-0.9.0/tests/test_func_chainer.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1877 2023-11-15 14:06:34.000000 daops-0.9.0/tests/test_logging.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-17 13:54:49.760716 daops-0.9.0/tests/test_xarray/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-08 16:10:30.000000 daops-0.9.0/tests/test_xarray/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     7183 2023-11-15 14:06:34.000000 daops-0.9.0/tests/test_xarray/test_xarray_aggregation.py
```

### Comparing `daops-0.8.1/LICENSE` & `daops-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/README.rst` & `daops-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/__init__.py` & `daops-0.9.0/daops/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Top-level package for daops.
 daops - Dataset-Aware Operations"""
 
 __author__ = """Elle Smith"""
 __contact__ = "eleanor.smith@stfc.ac.uk"
 __copyright__ = "Copyright 2018 United Kingdom Research and Innovation"
 __license__ = "BSD"
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 from loguru import logger
 
 from roocs_utils.config import get_config
 
 import daops
```

### Comparing `daops-0.8.1/daops/catalog/base.py` & `daops-0.9.0/daops/catalog/base.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/catalog/intake.py` & `daops-0.9.0/daops/catalog/intake.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/catalog/util.py` & `daops-0.9.0/daops/catalog/util.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/data_utils/attr_utils.py` & `daops-0.9.0/daops/data_utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/data_utils/coord_utils.py` & `daops-0.9.0/daops/data_utils/coord_utils.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/fix_utils/decadal_utils.py` & `daops-0.9.0/daops/fix_utils/decadal_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 def get_time_calendar(ds_id, ds):
     times = ds.time.values
     cal = times[0].calendar
     return cal
 
 
 def get_lead_times(ds_id, ds):
-
     start_date = datetime.fromisoformat(get_start_date(ds_id, ds))
 
     cal = get_time_calendar(ds_id, ds)
     reftime = cftime.datetime(
         start_date.year,
         start_date.month,
         start_date.day,
```

### Comparing `daops-0.8.1/daops/ops/average.py` & `daops-0.9.0/daops/ops/average.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/ops/base.py` & `daops-0.9.0/daops/ops/base.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/ops/subset.py` & `daops-0.9.0/daops/ops/subset.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/processor.py` & `daops-0.9.0/daops/processor.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/utils/base_lookup.py` & `daops-0.9.0/daops/utils/base_lookup.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/utils/consolidate.py` & `daops-0.9.0/daops/utils/consolidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,27 +82,25 @@
         return file_paths
 
     logger.info(f"Testing {len(file_paths)} files in time range: ...")
     files_in_time_range = []
 
     # Handle times differently depending on the type of time parameter
     if time_param.type == "interval":
-
         tp_start, tp_end = time_param.get_bounds()
         req_start_year = get_year(tp_start, default=-99999999)
         req_end_year = get_year(tp_end, default=999999999)
 
         # Work through the list of file paths checking if each matches
         for fpath in file_paths:
             years = get_years_from_file(fpath)
             if min(years) <= req_end_year and max(years) >= req_start_year:
                 files_in_time_range.append(fpath)
 
     elif time_param.type == "series":
-
         # Get requested years and match to files whose years intersect
         req_years = {to_year(tm) for tm in time_param.asdict().get("time_values", [])}
 
         for fpath in file_paths:
             years = get_years_from_file(fpath)
             if req_years.intersection(years):
                 files_in_time_range.append(fpath)
@@ -131,15 +129,14 @@
         catalog = get_catalog(project)
 
     filtered_refs = collections.OrderedDict()
 
     time_param = kwargs.get("time")
 
     for dset in collection:
-
         if not catalog:
             file_paths = dset_to_filepaths(dset, force=True)
 
             if time_param:
                 file_paths = get_files_matching_time_range(time_param, file_paths)
 
             # If no files are matched then raise an exception
```

### Comparing `daops-0.8.1/daops/utils/core.py` & `daops-0.9.0/daops/utils/core.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/daops/utils/fixer.py` & `daops-0.9.0/daops/utils/fixer.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         Lookup.__init__(self, dset)
         self._lookup_fix()
 
     def _gather_fixes(self, content):
         """Gathers pre and post processing fixes together"""
         if content["_source"]["fixes"]:
             for fix in content["_source"]["fixes"]:
-
                 ref_implementation = fix["reference_implementation"]
                 func = locate(ref_implementation)
 
                 if fix["process_type"] == "post_processor":
                     self.post_processors.append([func, fix["operands"]])
                 else:
                     self.pre_processors.append(func)
```

### Comparing `daops-0.8.1/daops/utils/normalise.py` & `daops-0.9.0/daops/utils/normalise.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     :return: An ordered dictionary of ds ids and their fixed xarray Dataset.
     """
 
     logger.info(f"Working on datasets: {collection}")
     norm_collection = collections.OrderedDict()
 
     for dset, file_paths in collection.items():
-
         ds = open_dataset(dset, file_paths, apply_fixes)
         norm_collection[dset] = ds
 
     return norm_collection
 
 
 class ResultSet(object):
```

### Comparing `daops-0.8.1/daops.egg-info/SOURCES.txt` & `daops-0.9.0/daops.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 MANIFEST.in
 README.rst
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 daops/__init__.py
+daops/cli.py
 daops/processor.py
 daops.egg-info/PKG-INFO
 daops.egg-info/SOURCES.txt
 daops.egg-info/dependency_links.txt
+daops.egg-info/entry_points.txt
 daops.egg-info/requires.txt
 daops.egg-info/top_level.txt
 daops/catalog/__init__.py
 daops/catalog/base.py
 daops/catalog/intake.py
 daops/catalog/util.py
 daops/data_utils/__init__.py
@@ -37,14 +39,15 @@
 daops/utils/core.py
 daops/utils/fixer.py
 daops/utils/normalise.py
 etc/daops_eg.cfg
 tests/__init__.py
 tests/_common.py
 tests/conftest.py
+tests/test_cli.py
 tests/test_daops.py
 tests/test_fixes_applied.py
 tests/test_func_chainer.py
 tests/test_logging.py
 tests/test_catalog/__init__.py
 tests/test_catalog/test_intake.py
 tests/test_catalog/test_util.py
```

### Comparing `daops-0.8.1/setup.cfg` & `daops-0.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.1
+current_version = 0.9.0
 commit = True
 tag = True
 
 [bumpversion:file:daops/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `daops-0.8.1/setup.py` & `daops-0.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """The setup script."""
 
 __author__ = """Elle Smith"""
 __contact__ = "eleanor.smith@stfc.ac.uk"
 __copyright__ = "Copyright 2018 United Kingdom Research and Innovation"
 __license__ = "BSD"
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 import os
 from setuptools import setup, find_packages
 
 # One strategy for storing the overall version is to put it in the top-level
 # package's __init__ but Nb. __init__.py files are not needed to declare
 # packages in Python 3
@@ -73,14 +73,19 @@
     license=__license__,
     # This qualifier can be used to selectively exclude Python versions -
     # in this case early Python 2 and 3 releases
     python_requires=">=3.7.0",
     install_requires=[
         requirements,
     ],
+    entry_points={
+        "console_scripts": [
+            "daops=daops.cli:main",
+        ],
+    },
     long_description=_long_description,
     long_description_content_type="text/x-rst",
     include_package_data=True,
     package_data={"daops": ["etc/roocs.ini"]},
     keywords="daops",
     name="daops",
     packages=find_packages(),
```

### Comparing `daops-0.8.1/tests/_common.py` & `daops-0.9.0/tests/_common.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/tests/conftest.py` & `daops-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/tests/test_catalog/test_intake.py` & `daops-0.9.0/tests/test_catalog/test_intake.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/tests/test_catalog/test_util.py` & `daops-0.9.0/tests/test_catalog/test_util.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/tests/test_daops.py` & `daops-0.9.0/tests/test_daops.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,16 @@
     Check response when all required is False for none characterised."""
     pass
 
 
 # consolidate fixes data inputs so they can be passed to xarray
 def test_consolidate_data_ref_fpath():
     """Tests daops utils._consolidate_data_ref with file path e.g.
-    /badc/cmip5/data/cmip5/output1/MOHC/HadGEM2-ES/historical/mon/atmos/Amon/r1i1p1/latest/tas/*.nc"""
+    /badc/cmip5/data/cmip5/output1/MOHC/HadGEM2-ES/historical/mon/atmos/Amon/r1i1p1/latest/tas/*.nc
+    """
     pass
 
 
 def test_consolidate_data_ref_drs():
     """Tests daops utils._consolidate_data_ref with DRS e.g.
     cmip5.output1.MOHC.HadGEM2-ES.historical.mon.land.Lmon.r1i1p1.latest.rh"""
     pass
```

### Comparing `daops-0.8.1/tests/test_fixes_applied.py` & `daops-0.9.0/tests/test_fixes_applied.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/tests/test_func_chainer.py` & `daops-0.9.0/tests/test_func_chainer.py`

 * *Files identical despite different names*

### Comparing `daops-0.8.1/tests/test_logging.py` & `daops-0.9.0/tests/test_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             _logging_examples()  # noqa
 
             assert ("daops.utils.common", 10, "1") not in caplog.record_tuples
             assert ("daops.utils.common", 40, "4") in caplog.record_tuples
 
     def test_disabled_enabled_logging(self, capsys):
         with ContextLogger() as _logger:
-
             _logger.disable("daops")
 
             # DAOPS disabled
             _logger.add(sys.stderr, level="WARNING")
             _logger.add(sys.stdout, level="INFO")
 
             _logging_examples()  # noqa
@@ -43,15 +42,14 @@
             captured = capsys.readouterr()
             assert "INFO" not in captured.err
             assert "WARNING" in captured.err
             assert "INFO" in captured.out
 
     def test_logging_enabler(self, capsys):
         with ContextLogger():
-
             _logging_examples()  # noqa
 
             captured = capsys.readouterr()
             assert "WARNING" not in captured.err
             assert "INFO" not in captured.out
 
             enable_logging()
```

### Comparing `daops-0.8.1/tests/test_xarray/test_xarray_aggregation.py` & `daops-0.9.0/tests/test_xarray/test_xarray_aggregation.py`

 * *Files identical despite different names*

