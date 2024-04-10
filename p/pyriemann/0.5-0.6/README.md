# Comparing `tmp/pyriemann-0.5.tar.gz` & `tmp/pyriemann-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriemann-0.5.tar", last modified: Tue Jun 20 08:33:53 2023, max compression
+gzip compressed data, was "pyriemann-0.6.tar", last modified: Wed Apr 10 11:45:56 2024, max compression
```

## Comparing `pyriemann-0.5.tar` & `pyriemann-0.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.908144 pyriemann-0.5/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     1527 2023-05-09 10:50:37.000000 pyriemann-0.5/LICENSE
--rw-r--r--   0 plcrodrigues   (501) staff       (20)       18 2022-07-12 09:17:11.000000 pyriemann-0.5/MANIFEST.in
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7514 2023-06-20 08:33:53.908227 pyriemann-0.5/PKG-INFO
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     6930 2023-06-16 09:10:00.000000 pyriemann-0.5/README.md
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.896208 pyriemann-0.5/pyriemann/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      521 2023-06-19 12:13:12.000000 pyriemann-0.5/pyriemann/__init__.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)       20 2023-06-20 08:28:01.000000 pyriemann-0.5/pyriemann/_version.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     6273 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/channelselection.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    36629 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/classification.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    27622 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/clustering.py
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.898133 pyriemann-0.5/pyriemann/datasets/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      456 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/datasets/__init__.py
--rwxr-xr-x   0 plcrodrigues   (501) staff       (20)    20032 2023-06-20 08:10:03.000000 pyriemann-0.5/pyriemann/datasets/sampling.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    17672 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/datasets/simulated.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    13538 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/embedding.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    28565 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/estimation.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7442 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/preprocessing.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     8495 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/regression.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    28957 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/spatialfilters.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    15272 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/stats.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    12756 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/tangentspace.py
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.899166 pyriemann-0.5/pyriemann/transfer/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      438 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/transfer/__init__.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    31390 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/transfer/_estimators.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7662 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/transfer/_rotate.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     5025 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/transfer/_tools.py
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.902724 pyriemann-0.5/pyriemann/utils/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      745 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/utils/__init__.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    10256 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/utils/ajd.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     6189 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/base.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    26662 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/covariance.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    16702 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/utils/distance.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     2888 2022-07-12 09:17:11.000000 pyriemann-0.5/pyriemann/utils/docs.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     3808 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/geodesic.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7687 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/kernel.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    25249 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/utils/mean.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     5543 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/utils/median.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    10771 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/tangentspace.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     5117 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/test.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     2008 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/utils.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7624 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/viz.py
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.897386 pyriemann-0.5/pyriemann.egg-info/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7514 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/PKG-INFO
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     1783 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/SOURCES.txt
--rw-r--r--   0 plcrodrigues   (501) staff       (20)        1 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/dependency_links.txt
--rw-r--r--   0 plcrodrigues   (501) staff       (20)        1 2022-07-12 09:17:30.000000 pyriemann-0.5/pyriemann.egg-info/not-zip-safe
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      145 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/requires.txt
--rw-r--r--   0 plcrodrigues   (501) staff       (20)       10 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/top_level.txt
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      182 2023-06-20 08:33:53.908509 pyriemann-0.5/setup.cfg
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     1719 2023-06-16 09:10:00.000000 pyriemann-0.5/setup.py
-drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.908008 pyriemann-0.5/tests/
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     1026 2022-07-12 09:17:11.000000 pyriemann-0.5/tests/test_channelselection.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    12791 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_classification.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    11515 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_clustering.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     6018 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_embedding.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    11686 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_estimation.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     3883 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_preprocessing.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     7493 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_regression.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     3426 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_sampling.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     6457 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_simulated.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    11694 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_spatialfilters.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     2578 2022-07-12 09:17:11.000000 pyriemann-0.5/tests/test_stats.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     5039 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_tangentspace.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    11477 2023-06-20 08:10:03.000000 pyriemann-0.5/tests/test_transfer.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     2630 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_utils_ajd.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     4412 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_base.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    16131 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_utils_covariance.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     9482 2023-06-19 13:13:37.000000 pyriemann-0.5/tests/test_utils_distance.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     3637 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_geodesic.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     3508 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_kernel.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)    10391 2023-06-19 13:13:37.000000 pyriemann-0.5/tests/test_utils_mean.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     2765 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_median.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     4868 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_tangent_space.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     3420 2023-06-19 13:13:37.000000 pyriemann-0.5/tests/test_utils_test.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)      908 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_utils_utils.py
--rw-r--r--   0 plcrodrigues   (501) staff       (20)     1451 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.640777 pyriemann-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 11:45:52.000000 pyriemann-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 11:45:52.000000 pyriemann-0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-10 11:45:56.640777 pyriemann-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-10 11:45:52.000000 pyriemann-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.628777 pyriemann-0.6/pyriemann/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/channelselection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37125 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28581 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.632777 pyriemann-0.6/pyriemann/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/datasets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20032 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/datasets/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/datasets/simulated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30546 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/spatialfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/tangentspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.632777 pyriemann-0.6/pyriemann/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/transfer/_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/transfer/_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/transfer/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.636777 pyriemann-0.6/pyriemann/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/ajd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29153 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25531 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/tangentspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-04-10 11:45:52.000000 pyriemann-0.6/pyriemann/utils/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.640777 pyriemann-0.6/pyriemann.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-10 11:45:56.000000 pyriemann-0.6/pyriemann.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-10 11:45:56.000000 pyriemann-0.6/pyriemann.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:45:56.000000 pyriemann-0.6/pyriemann.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:45:56.000000 pyriemann-0.6/pyriemann.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 11:45:56.000000 pyriemann-0.6/pyriemann.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 11:45:56.000000 pyriemann-0.6/pyriemann.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-10 11:45:56.640777 pyriemann-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-10 11:45:52.000000 pyriemann-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:45:56.640777 pyriemann-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_channelselection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_simulated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_spatialfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_tangentspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13763 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_ajd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_tangent_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 11:45:52.000000 pyriemann-0.6/tests/test_utils_viz.py
```

### Comparing `pyriemann-0.5/LICENSE` & `pyriemann-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/PKG-INFO` & `pyriemann-0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,78 @@
 Metadata-Version: 2.1
 Name: pyriemann
-Version: 0.5
+Version: 0.6
 Summary: Biosignals classification with Riemannian geometry
 Home-page: https://pyriemann.readthedocs.io
 Author: Alexandre Barachant
 Author-email: alexandre.barachant@gmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://pyriemann.readthedocs.io
 Project-URL: Source, https://github.com/pyRiemann/pyRiemann
 Project-URL: Tracker, https://github.com/pyRiemann/pyRiemann/issues/
 Platform: any
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy!=1.24.0
+Requires-Dist: scipy
+Requires-Dist: scikit-learn>=0.24
+Requires-Dist: joblib
+Requires-Dist: matplotlib
 Provides-Extra: docs
+Requires-Dist: sphinx<=7.0.1,>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-gallery; extra == "docs"
+Requires-Dist: sphinx-bootstrap_theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: mne; extra == "docs"
+Requires-Dist: seaborn; extra == "docs"
+Requires-Dist: pandas; extra == "docs"
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: seaborn; extra == "tests"
+Requires-Dist: flake8; extra == "tests"
 
 # pyRiemann
 
-[![Code PythonVersion](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
+[![Code PythonVersion](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
 [![PyPI version](https://badge.fury.io/py/pyriemann.svg)](https://badge.fury.io/py/pyriemann)
 [![Build Status](https://github.com/pyRiemann/pyRiemann/workflows/testing/badge.svg?branch=master&event=push)](https://github.com/pyRiemann/pyRiemann/actions)
 [![codecov](https://codecov.io/gh/pyRiemann/pyRiemann/branch/master/graph/badge.svg)](https://codecov.io/gh/pyRiemann/pyRiemann)
 [![Documentation Status](https://readthedocs.org/projects/pyriemann/badge/?version=latest)](http://pyriemann.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.593816.svg)](https://doi.org/10.5281/zenodo.593816)
 [![Downloads](https://pepy.tech/badge/pot)](https://pepy.tech/project/pyriemann)
 
 pyRiemann is a Python machine learning package based on [scikit-learn](http://scikit-learn.org/stable/modules/classes.html) API.
-It provides a high-level interface for processing and classification of multivariate time series
-through the Riemannian geometry of symmetric positive definite (SPD) matrices.
-
-pyRiemann aims at being a generic package for multivariate time series classification
-but has been designed around multichannel biosignals (like EEG, MEG or EMG) manipulation applied to brain-computer interface (BCI),
-transforming multichannel time series into covariance matrices, and classifying them using the Riemannian geometry of SPD matrices [[1]](#1).
+It provides a high-level interface for processing and classification of real (*resp*. complex)-valued multivariate data
+through the Riemannian geometry of symmetric (*resp*. Hermitian) 
+[positive definite](https://en.wikipedia.org/wiki/Definite_matrix) (SPD) (*resp*. HPD) matrices.
+
+pyRiemann aims at being a generic package for multivariate data analysis
+but has been designed around [biosignals](https://en.wikipedia.org/wiki/Biosignal) (like EEG, MEG or EMG)
+manipulation applied to [brain-computer interface](https://en.wikipedia.org/wiki/Brain%E2%80%93computer_interface) (BCI),
+estimating [covariance matrices](https://en.wikipedia.org/wiki/Covariance_matrix) from multichannel time series,
+and classifying them using the Riemannian geometry of SPD matrices [[1]](#1).
 
 For BCI applications, studied paradigms are motor imagery [[2]](#2) [[3]](#3), event-related potentials (ERP) [[4]](#4) and steady-state visually evoked potentials (SSVEP) [[5]](#5).
 Using extended labels, API allows transfer learning between sessions or subjects [[6]](#6).
 
-This code is BSD-licenced (3 clause).
+This code is BSD-licensed (3 clause).
 
 ## Documentation
 
 The documentation is available on http://pyriemann.readthedocs.io/en/latest/
 
-## Install
+# Installation
 
 #### Using PyPI
 
 ```
 pip install pyriemann
 ```
-or using pip+git for the latest version of the code :
+or using pip+git for the latest version of the code:
 
 ```
 pip install git+https://github.com/pyRiemann/pyRiemann
 ```
 
 #### Using conda
 
@@ -75,15 +93,15 @@
 
 or in editable mode to be able to modify the sources:
 
 ```shell
 pip install -e .
 ```
 
-## How to use it
+# How to use
 
 Most of the functions mimic the scikit-learn API, and therefore can be directly used with sklearn.
 For example, for cross-validation classification of EEG signal using the MDM algorithm described in [[2]](#2), it is easy as:
 
 ```python
 import pyriemann
 from sklearn.model_selection import cross_val_score
@@ -128,15 +146,15 @@
 # cross validation
 accuracy = cross_val_score(clf, X, y)
 
 print(accuracy.mean())
 
 ```
 
-**Check out the example folder for more examples !**
+**Check out the example folder for more examples.**
 
 # Contribution Guidelines
 
 The package aims at adopting the [scikit-learn](http://scikit-learn.org/stable/developers/contributing.html#contributing-code)
 and [MNE-Python](https://mne.tools/stable/install/contributing.html) conventions as much as possible.
 See their contribution guidelines before contributing to the repository.
 
@@ -163,21 +181,21 @@
                   Gabriel Wagner vom Berg and
                   Ghiles Reguig and
                   Arthur Lebeurrier and
                   Erik Bjäreholt and
                   Maria Sayu Yamamoto and
                   Pierre Clisson and
                   Marie-Constance Corsi},
-  title        = {pyRiemann/pyRiemann: v0.3},
-  month        = jul,
-  year         = 2022,
+  title        = {pyRiemann/pyRiemann: v0.5},
+  month        = june,
+  year         = 2023,
   publisher    = {Zenodo},
-  version      = {v0.3},
-  doi          = {10.5281/zenodo.7547583},
-  url          = {https://doi.org/10.5281/zenodo.7547583}
+  version      = {v0.5},
+  doi          = {10.5281/zenodo.8059038},
+  url          = {https://doi.org/10.5281/zenodo.8059038}
 }
 ```
 
 # References
 
 <a id="1">[1]</a>
 M. Congedo, A. Barachant and R. Bhatia, "Riemannian geometry for EEG-based brain-computer interfaces; a primer and a review".
```

### Comparing `pyriemann-0.5/README.md` & `pyriemann-0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # pyRiemann
 
-[![Code PythonVersion](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
+[![Code PythonVersion](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
 [![PyPI version](https://badge.fury.io/py/pyriemann.svg)](https://badge.fury.io/py/pyriemann)
 [![Build Status](https://github.com/pyRiemann/pyRiemann/workflows/testing/badge.svg?branch=master&event=push)](https://github.com/pyRiemann/pyRiemann/actions)
 [![codecov](https://codecov.io/gh/pyRiemann/pyRiemann/branch/master/graph/badge.svg)](https://codecov.io/gh/pyRiemann/pyRiemann)
 [![Documentation Status](https://readthedocs.org/projects/pyriemann/badge/?version=latest)](http://pyriemann.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.593816.svg)](https://doi.org/10.5281/zenodo.593816)
 [![Downloads](https://pepy.tech/badge/pot)](https://pepy.tech/project/pyriemann)
 
 pyRiemann is a Python machine learning package based on [scikit-learn](http://scikit-learn.org/stable/modules/classes.html) API.
-It provides a high-level interface for processing and classification of multivariate time series
-through the Riemannian geometry of symmetric positive definite (SPD) matrices.
-
-pyRiemann aims at being a generic package for multivariate time series classification
-but has been designed around multichannel biosignals (like EEG, MEG or EMG) manipulation applied to brain-computer interface (BCI),
-transforming multichannel time series into covariance matrices, and classifying them using the Riemannian geometry of SPD matrices [[1]](#1).
+It provides a high-level interface for processing and classification of real (*resp*. complex)-valued multivariate data
+through the Riemannian geometry of symmetric (*resp*. Hermitian) 
+[positive definite](https://en.wikipedia.org/wiki/Definite_matrix) (SPD) (*resp*. HPD) matrices.
+
+pyRiemann aims at being a generic package for multivariate data analysis
+but has been designed around [biosignals](https://en.wikipedia.org/wiki/Biosignal) (like EEG, MEG or EMG)
+manipulation applied to [brain-computer interface](https://en.wikipedia.org/wiki/Brain%E2%80%93computer_interface) (BCI),
+estimating [covariance matrices](https://en.wikipedia.org/wiki/Covariance_matrix) from multichannel time series,
+and classifying them using the Riemannian geometry of SPD matrices [[1]](#1).
 
 For BCI applications, studied paradigms are motor imagery [[2]](#2) [[3]](#3), event-related potentials (ERP) [[4]](#4) and steady-state visually evoked potentials (SSVEP) [[5]](#5).
 Using extended labels, API allows transfer learning between sessions or subjects [[6]](#6).
 
-This code is BSD-licenced (3 clause).
+This code is BSD-licensed (3 clause).
 
 ## Documentation
 
 The documentation is available on http://pyriemann.readthedocs.io/en/latest/
 
-## Install
+# Installation
 
 #### Using PyPI
 
 ```
 pip install pyriemann
 ```
-or using pip+git for the latest version of the code :
+or using pip+git for the latest version of the code:
 
 ```
 pip install git+https://github.com/pyRiemann/pyRiemann
 ```
 
 #### Using conda
 
@@ -57,15 +60,15 @@
 
 or in editable mode to be able to modify the sources:
 
 ```shell
 pip install -e .
 ```
 
-## How to use it
+# How to use
 
 Most of the functions mimic the scikit-learn API, and therefore can be directly used with sklearn.
 For example, for cross-validation classification of EEG signal using the MDM algorithm described in [[2]](#2), it is easy as:
 
 ```python
 import pyriemann
 from sklearn.model_selection import cross_val_score
@@ -110,15 +113,15 @@
 # cross validation
 accuracy = cross_val_score(clf, X, y)
 
 print(accuracy.mean())
 
 ```
 
-**Check out the example folder for more examples !**
+**Check out the example folder for more examples.**
 
 # Contribution Guidelines
 
 The package aims at adopting the [scikit-learn](http://scikit-learn.org/stable/developers/contributing.html#contributing-code)
 and [MNE-Python](https://mne.tools/stable/install/contributing.html) conventions as much as possible.
 See their contribution guidelines before contributing to the repository.
 
@@ -145,21 +148,21 @@
                   Gabriel Wagner vom Berg and
                   Ghiles Reguig and
                   Arthur Lebeurrier and
                   Erik Bjäreholt and
                   Maria Sayu Yamamoto and
                   Pierre Clisson and
                   Marie-Constance Corsi},
-  title        = {pyRiemann/pyRiemann: v0.3},
-  month        = jul,
-  year         = 2022,
+  title        = {pyRiemann/pyRiemann: v0.5},
+  month        = june,
+  year         = 2023,
   publisher    = {Zenodo},
-  version      = {v0.3},
-  doi          = {10.5281/zenodo.7547583},
-  url          = {https://doi.org/10.5281/zenodo.7547583}
+  version      = {v0.5},
+  doi          = {10.5281/zenodo.8059038},
+  url          = {https://doi.org/10.5281/zenodo.8059038}
 }
 ```
 
 # References
 
 <a id="1">[1]</a>
 M. Congedo, A. Barachant and R. Bhatia, "Riemannian geometry for EEG-based brain-computer interfaces; a primer and a review".
```

### Comparing `pyriemann-0.5/pyriemann/__init__.py` & `pyriemann-0.6/pyriemann/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/channelselection.py` & `pyriemann-0.6/pyriemann/channelselection.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,20 @@
     This algorithm is described in [1]_.
 
     Parameters
     ----------
     nelec : int, default=16
         The number of electrode to keep in the final subset.
     metric : string | dict, default='riemann'
-        The type of metric used for centroid and distance estimation.
-        see `mean_covariance` for the list of supported metric.
-        the metric could be a dict with two keys, `mean` and `distance` in
-        order to pass different metric for the centroid estimation and the
-        distance estimation. Typical usecase is to pass 'logeuclid' metric for
-        the mean in order to boost the computional speed and 'riemann' for the
-        distance in order to keep the good sensitivity for the selection.
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     n_jobs : int, default=1
         The number of jobs to use for the computation. This works by computing
         each of the class centroid in parallel.
         If -1 all CPUs are used. If 1 is given, no parallel computing code is
         used at all, which is useful for debugging. For n_jobs below -1,
         (n_cpus + 1 + n_jobs) are used. Thus for n_jobs = -2, all CPUs but one
         are used.
@@ -53,15 +52,15 @@
     .. [1] `Channel selection procedure using riemannian distance for BCI
         applications
         <https://hal.archives-ouvertes.fr/hal-00602707>`_
         A. Barachant and S. Bonnet. The 5th International IEEE EMBS Conference
         on Neural Engineering, Apr 2011, Cancun, Mexico.
     """
 
-    def __init__(self, nelec=16, metric='riemann', n_jobs=1):
+    def __init__(self, nelec=16, metric="riemann", n_jobs=1):
         """Init."""
         self.nelec = nelec
         self.metric = metric
         self.n_jobs = n_jobs
 
     def fit(self, X, y=None, sample_weight=None):
         """Find the optimal subset of electrodes.
```

### Comparing `pyriemann-0.5/pyriemann/classification.py` & `pyriemann-0.6/pyriemann/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 """Module for classification function."""
 import functools
 
 import numpy as np
-from scipy import stats
 from sklearn.base import BaseEstimator, ClassifierMixin, TransformerMixin
 from sklearn.svm import SVC as sklearnSVC
 from sklearn.utils.extmath import softmax
 from sklearn.linear_model import LogisticRegression
 from sklearn.pipeline import make_pipeline
 from joblib import Parallel, delayed
+import warnings
 
 from .utils.kernel import kernel
 from .utils.mean import mean_covariance, mean_power
 from .utils.distance import distance
+from .utils.utils import check_metric
 from .tangentspace import FGDA, TangentSpace
 
 
-def _check_metric(metric):
-    if isinstance(metric, str):
-        metric_mean = metric
-        metric_dist = metric
-
-    elif isinstance(metric, dict):
-        # check keys
-        for key in ['mean', 'distance']:
-            if key not in metric.keys():
-                raise KeyError('metric must contain "mean" and "distance"')
+def _mode_1d(X):
+    vals, counts = np.unique(X, return_counts=True)
+    mode = vals[counts.argmax()]
+    return mode
 
-        metric_mean = metric['mean']
-        metric_dist = metric['distance']
 
-    else:
-        raise TypeError('metric must be dict or str')
-
-    return metric_mean, metric_dist
+def _mode_2d(X, axis=1):
+    mode = np.apply_along_axis(_mode_1d, axis, X)
+    return mode
 
 
 class MDM(BaseEstimator, ClassifierMixin, TransformerMixin):
-    """Classification by Minimum Distance to Mean.
+    r"""Classification by Minimum Distance to Mean.
+
+    For each of the given classes :math:`k = 1, \ldots, K`, a centroid
+    :math:`\mathbf{M}^k` is estimated according to the chosen metric.
 
-    Classification by nearest centroid. For each of the given classes, a
-    centroid is estimated according to the chosen metric. Then, for each new
-    point, the class is affected according to the nearest centroid.
+    Then, for each new matrix :math:`\mathbf{X}`, the class is affected
+    according to the nearest centroid [1]_:
+
+    .. math::
+        \hat{k} = \arg \min_{k} d (\mathbf{X}, \mathbf{M}^k)
 
     Parameters
     ----------
-    metric : string | dict, default='riemann'
-        The type of metric used for centroid and distance estimation.
-        see `mean_covariance` for the list of supported metric.
-        the metric could be a dict with two keys, `mean` and `distance` in
-        order to pass different metrics for the centroid estimation and the
-        distance estimation. Typical usecase is to pass 'logeuclid' metric for
-        the mean in order to boost the computional speed and 'riemann' for the
-        distance in order to keep the good sensitivity for the classification.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
+        Typical usecase is to pass "logeuclid" metric for the "mean" in order
+        to boost the computional speed, and "riemann" for the "distance" in
+        order to keep the good sensitivity for the classification.
     n_jobs : int, default=1
         The number of jobs to use for the computation. This works by computing
         each of the class centroid in parallel.
         If -1 all CPUs are used. If 1 is given, no parallel computing code is
         used at all, which is useful for debugging. For n_jobs below -1,
         (n_cpus + 1 + n_jobs) are used. Thus for n_jobs = -2, all CPUs but one
         are used.
 
     Attributes
     ----------
     classes_ : ndarray, shape (n_classes,)
         Labels for each class.
-    covmeans_ : list of ``n_classes`` ndarrays of shape (n_channels, \
-            n_channels)
+    covmeans_ : ndarray, shape (n_classes, n_channels, n_channels)
         Centroids for each class.
 
     See Also
     --------
     Kmeans
     FgMDM
     KNearestNeighbor
@@ -85,15 +83,15 @@
     .. [2] `Riemannian geometry applied to BCI classification
         <https://hal.archives-ouvertes.fr/hal-00602700/>`_
         A. Barachant, S. Bonnet, M. Congedo and C. Jutten. 9th International
         Conference Latent Variable Analysis and Signal Separation
         (LVA/ICA 2010), LNCS vol. 6365, 2010, p. 629-636.
     """
 
-    def __init__(self, metric='riemann', n_jobs=1):
+    def __init__(self, metric="riemann", n_jobs=1):
         """Init."""
         self.metric = metric
         self.n_jobs = n_jobs
 
     def fit(self, X, y, sample_weight=None):
         """Fit (estimates) the centroids.
 
@@ -107,15 +105,15 @@
             Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         self : MDM instance
             The MDM instance.
         """
-        self.metric_mean, self.metric_dist = _check_metric(self.metric)
+        self.metric_mean, self.metric_dist = check_metric(self.metric)
         self.classes_ = np.unique(y)
 
         if sample_weight is None:
             sample_weight = np.ones(X.shape[0])
 
         if self.n_jobs == 1:
             self.covmeans_ = [
@@ -124,14 +122,16 @@
                 for ll in self.classes_]
         else:
             self.covmeans_ = Parallel(n_jobs=self.n_jobs)(
                 delayed(mean_covariance)(X[y == ll], metric=self.metric_mean,
                                          sample_weight=sample_weight[y == ll])
                 for ll in self.classes_)
 
+        self.covmeans_ = np.stack(self.covmeans_, axis=0)
+
         return self
 
     def _predict_distances(self, X):
         """Helper to predict the distance. Equivalent to transform."""
         n_centroids = len(self.covmeans_)
 
         if self.n_jobs == 1:
@@ -204,22 +204,22 @@
     The geodesic filtering is achieved in tangent space with a Linear
     Discriminant Analysis, then data are projected back to the manifold and
     classifier with a regular MDM.
     This is basically a pipeline of FGDA and MDM.
 
     Parameters
     ----------
-    metric : string | dict, default='riemann'
-        The type of metric used for reference matrix estimation (see
-        `mean_covariance` for the list of supported metric), for distance
-        estimation, and for tangent space map (see `tangent_space` for the list
-        of supported metric).
-        The metric could be a dict with three keys, `mean`, `dist` and `map` in
-        order to pass different metrics for the reference matrix estimation,
-        the distance estimation, and the tangent space mapping.
+    metric : string | dict, default="riemann"
+        Metric used for reference matrix estimation (for the list of supported
+        metrics, see :func:`pyriemann.utils.mean.mean_covariance`),
+        for distance estimation (see :func:`pyriemann.utils.distance.distance`)
+        and for tangent space map
+        (see :func:`pyriemann.utils.tangent_space.tangent_space`).
+        The metric can be a dict with three keys, "mean", "dist" and "map" in
+        order to pass different metrics.
     tsupdate : bool, default=False
         Activate tangent space update for covariante shift correction between
         training and test, as described in [2]_. This is not compatible with
         online implementation. Performance are better when the number of
         matrices for prediction is higher.
     n_jobs : int, default=1
         The number of jobs to use for the computation. This works by computing
@@ -250,15 +250,15 @@
     .. [2] `Classification of covariance matrices using a Riemannian-based
         kernel for BCI applications
         <https://hal.archives-ouvertes.fr/hal-00820475/>`_
         A. Barachant, S. Bonnet, M. Congedo and C. Jutten. Neurocomputing,
         Elsevier, 2013, 112, pp.172-178.
     """
 
-    def __init__(self, metric='riemann', tsupdate=False, n_jobs=1):
+    def __init__(self, metric="riemann", tsupdate=False, n_jobs=1):
         """Init."""
         self.metric = metric
         self.n_jobs = n_jobs
         self.tsupdate = tsupdate
 
     def fit(self, X, y, sample_weight=None):
         """Fit FgMDM.
@@ -340,21 +340,22 @@
 
     Project data in the tangent space and apply a classifier on the projected
     data. This is a simple helper to pipeline the tangent space projection and
     a classifier. Default classifier is LogisticRegression
 
     Parameters
     ----------
-    metric : string | dict, default='riemann'
-        The type of metric used for reference matrix estimation (see
-        `mean_covariance` for the list of supported metric) and for tangent
-        space map (see `tangent_space` for the list of supported metric).
-        The metric could be a dict with two keys, `mean` and `map` in
-        order to pass different metrics for the reference matrix estimation
-        and the tangent space mapping.
+    metric : string | dict, default="riemann"
+        The type of metric used
+        for reference matrix estimation (for the list of supported metrics
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for tangent space map
+        (see :func:`pyriemann.utils.tangent_space.tangent_space`).
+        The metric can be a dict with two keys, "mean" and "map"
+        in order to pass different metrics.
     tsupdate : bool, default=False
         Activate tangent space update for covariate shift correction between
         training and test, as described in [2]. This is not compatible with
         online implementation. Performance are better when the number of
         matrices for prediction is higher.
     clf : sklearn classifier, default=LogisticRegression()
         The classifier to apply in the tangent space.
@@ -369,15 +370,15 @@
     TangentSpace
 
     Notes
     -----
     .. versionadded:: 0.2.4
     """
 
-    def __init__(self, metric='riemann', tsupdate=False,
+    def __init__(self, metric="riemann", tsupdate=False,
                  clf=LogisticRegression()):
         """Init."""
         self.metric = metric
         self.tsupdate = tsupdate
         self.clf = clf
 
     def fit(self, X, y, sample_weight=None):
@@ -449,17 +450,21 @@
     estimated. The class is affected according to the majority class of the
     k-nearest neighbors.
 
     Parameters
     ----------
     n_neighbors : int, default=5
         Number of neighbors.
-    metric : string | dict, default='riemann'
-        The type of metric used for distance estimation.
-        see `distance` for the list of supported metric.
+    metric : string | dict, default="riemann"
+        Metric used for means estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     n_jobs : int, default=1
         The number of jobs to use for the computation. This works by computing
         each of the distance to the training set in parallel.
         If -1 all CPUs are used. If 1 is given, no parallel computing code is
         used at all, which is useful for debugging. For n_jobs below -1,
         (n_cpus + 1 + n_jobs) are used. Thus for n_jobs = -2, all CPUs but one
         are used.
@@ -476,15 +481,15 @@
     See Also
     --------
     Kmeans
     MDM
 
     """
 
-    def __init__(self, n_neighbors=5, metric='riemann', n_jobs=1):
+    def __init__(self, n_neighbors=5, metric="riemann", n_jobs=1):
         """Init."""
         self.n_neighbors = n_neighbors
         MDM.__init__(self, metric=metric, n_jobs=n_jobs)
 
     def fit(self, X, y, sample_weight=None):
         """Fit (store the training data).
 
@@ -498,38 +503,44 @@
             Not used, here for compatibility with sklearn API.
 
         Returns
         -------
         self : NearestNeighbor instance
             The NearestNeighbor instance.
         """
-        self.metric_mean, self.metric_dist = _check_metric(self.metric)
+        self.metric_mean, self.metric_dist = check_metric(self.metric)
         self.covmeans_ = X
         self.classmeans_ = y
         self.classes_ = np.unique(y)
 
         return self
 
-    def predict(self, covtest):
+    def predict(self, X=None, covtest=None):
         """Get the predictions.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
 
         Returns
         -------
         pred : ndarray of int, shape (n_matrices,)
             Predictions for each matrix according to the closest centroid.
         """
-        dist = self._predict_distances(covtest)
+        if covtest is not None:
+            warnings.warn("Input covtest has been renamed into X and will be "
+                          "removed in 0.8.0.", category=DeprecationWarning)
+            assert (X is None)
+            X = covtest
+
+        dist = self._predict_distances(X)
         neighbors_classes = self.classmeans_[np.argsort(dist)]
-        out, _ = stats.mode(neighbors_classes[:, 0:self.n_neighbors], axis=1)
-        return out.ravel()
+        pred = _mode_2d(neighbors_classes[:, 0:self.n_neighbors], axis=1)
+        return pred
 
     def predict_proba(self, X):
         """Predict proba using softmax.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
@@ -562,24 +573,24 @@
     """Classification by support-vector machine.
 
     Support-vector machine (SVM) classification with precomputed Riemannian
     kernel matrix according to different metrics as described in [1]_.
 
     Parameters
     ----------
-    metric : {'riemann', 'euclid', 'logeuclid'}, default='riemann'
+    metric : {"euclid", "logeuclid", "riemann"}, default="riemann"
         Metric for kernel matrix computation.
     Cref : None | callable | ndarray, shape (n_channels, n_channels)
         Reference point for kernel matrix computation.
         If None, the mean of the training data according to the metric is used.
         If callable, the function is called on the training data to calculate
         Cref.
-    kernel_fct : None | 'precomputed' | callable
-        If 'precomputed', the kernel matrix for datasets X and Y is estimated
-        according to `pyriemann.utils.kernel(X, Y, Cref, metric)`.
+    kernel_fct : None | "precomputed" | callable
+        If None or "precomputed", the kernel matrix for datasets X and Y is
+        estimated according to `pyriemann.utils.kernel(X, Y, Cref, metric)`.
         If callable, the callable is passed as the kernel parameter to
         `sklearn.svm.SVC()` [2]_. The callable has to be of the form
         `kernel(X, Y, Cref, metric)`.
     C : float, default=1.0
         Regularization parameter. The strength of the regularization is
         inversely proportional to C. Must be strictly positive. The penalty
         is a squared l2 penalty.
@@ -638,15 +649,15 @@
         Elsevier, 2013, 112, pp.172-178.
     .. [2]
         https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html
     """
 
     def __init__(self,
                  *,
-                 metric='riemann',
+                 metric="riemann",
                  kernel_fct=None,
                  Cref=None,
                  C=1.0,
                  shrinking=True,
                  probability=False,
                  tol=1e-3,
                  cache_size=200,
@@ -657,15 +668,15 @@
                  break_ties=False,
                  random_state=None):
         """Init."""
         self.Cref = Cref
         self.metric = metric
         self.Cref_ = None
         self.kernel_fct = kernel_fct
-        super().__init__(kernel='precomputed',
+        super().__init__(kernel="precomputed",
                          C=C,
                          shrinking=shrinking,
                          probability=probability,
                          tol=tol,
                          cache_size=cache_size,
                          class_weight=class_weight,
                          verbose=verbose,
@@ -703,30 +714,32 @@
         if self.Cref is None:
             self.Cref_ = mean_covariance(X, metric=self.metric)
         elif callable(self.Cref):
             self.Cref_ = self.Cref(X)
         elif isinstance(self.Cref, np.ndarray):
             self.Cref_ = self.Cref
         else:
-            raise TypeError(f'Cref must be np.ndarray, callable or None, is'
-                            f' {self.Cref}.')
+            raise TypeError(f"Cref must be np.ndarray, callable or None, is "
+                            f"{self.Cref}.")
 
     def _set_kernel(self):
         if callable(self.kernel_fct):
             self.kernel = functools.partial(self.kernel_fct,
                                             Cref=self.Cref_,
                                             metric=self.metric)
-
-        elif self.kernel_fct is None:
+        elif self.kernel_fct is None or (isinstance(self.kernel_fct, str) and
+                                         self.kernel_fct == "precomputed"):
             self.kernel = functools.partial(kernel,
                                             Cref=self.Cref_,
                                             metric=self.metric)
         else:
-            raise TypeError(f"kernel must be 'precomputed' or callable, is "
-                            f"{self.kernel}.")
+            raise TypeError(
+                "kernel_fct must be None, 'precomputed' or callable, is "
+                f"{self.kernel}."
+            )
 
 
 class MeanField(BaseEstimator, ClassifierMixin, TransformerMixin):
     """Classification by Minimum Distance to Mean Field.
 
     Classification by Minimum Distance to Mean Field [1]_, defining several
     power means for each class.
@@ -738,17 +751,18 @@
     method_label : {'sum_means', 'inf_means'}, default='sum_means'
         Method to combine labels:
 
         * sum_means: it assigns the covariance to the class whom the sum of
           distances to means of the field is the lowest;
         * inf_means: it assigns the covariance to the class of the closest mean
           of the field.
-    metric : string | dict, default='riemann'
-        The type of metric used for distance estimation during prediction.
-        See `distance` for the list of supported metric.
+    metric : string, default="riemann"
+        Metric used for distance estimation during prediction.
+        For the list of supported metrics,
+        see :func:`pyriemann.utils.distance.distance`.
 
     Attributes
     ----------
     classes_ : ndarray, shape (n_classes,)
         Labels for each class.
     covmeans_ : dict of ``n_powers`` lists of ``n_classes`` ndarrays of shape \
             (n_channels, n_channels)
@@ -767,15 +781,15 @@
     .. [1] `The Riemannian Minimum Distance to Means Field Classifier
         <https://hal.archives-ouvertes.fr/hal-02315131>`_
         M Congedo, PLC Rodrigues, C Jutten. BCI 2019 - 8th International
         Brain-Computer Interface Conference, Sep 2019, Graz, Austria.
     """
 
     def __init__(self, power_list=[-1, 0, 1], method_label='sum_means',
-                 metric='riemann', n_jobs=1):
+                 metric="riemann", n_jobs=1):
         """Init."""
         self.power_list = power_list
         self.method_label = method_label
         self.metric = metric
         self.n_jobs = n_jobs
 
     def fit(self, X, y, sample_weight=None):
@@ -903,46 +917,47 @@
         -------
         prob : ndarray, shape (n_matrices, n_classes)
             Probabilities for each class.
         """
         return softmax(-self._predict_distances(X) ** 2)
 
 
-def class_distinctiveness(X, y, exponent=1, metric='riemann',
+def class_distinctiveness(X, y, exponent=1, metric="riemann",
                           return_num_denom=False):
     r"""Measure class distinctiveness between classes of SPD matrices.
 
-    For two class problem, the class distinctiveness between class A
-    and B on the manifold of SPD matrices is quantified as [1]_:
+    For two class problem, the class distinctiveness between class :math:`K_1`
+    and :math:`K_2` on the manifold of SPD matrices is quantified as [1]_:
 
     .. math::
-        \mathrm{classDis}(A, B, p) = \frac{d \left(\bar{X}^{A},
-        \bar{X}^{B}\right)^p}
-        {\frac{1}{2} \left( \sigma_{X^{A}}^p + \sigma_{X^{B}}^p \right)}
-
-    where :math:`\bar{X}^{K}` is the center of class K, ie the mean of matrices
-    from class K (see :func:`pyriemann.utils.mean.mean_covariance`) and
-    :math:`\sigma_{X^{K}}` is the class dispersion, ie the mean of distances
-    between matrices from class K and their center of class
-    :math:`\bar{X}^{K}`:
+        \mathrm{classDis}(K_1, K_2, p) =
+        \frac{d \left( \mathbf{M}_{K_1}, \mathbf{M}_{K_2} \right)^p}
+        {\frac{1}{2} \left( \sigma_{K_1}^p + \sigma_{K_2}^p \right)}
+
+    where :math:`\mathbf{M}_K` is the center of class :math:`K`, ie the mean of
+    matrices from class :math:`K`; and
+    :math:`\sigma_K` is the class dispersion, ie the mean of distances between
+    matrices from class :math:`K` and their center of class
+    :math:`\mathbf{M}_K`:
 
     .. math::
-        \sigma_{X^{K}}^p = \frac{1}{m} \sum_{i=1}^m d
-        \left(X_i, \bar{X}^{K}\right)^p
+        \sigma_K^p = \frac{1}{m} \sum_{i=1}^m d
+        \left(X_i, \mathbf{M}_K \right)^p
+
+    and :math:`p` is the exponentiation of the distance.
 
     For more than two classes, it is quantified as:
 
     .. math::
-        \mathrm{classDis}\left(\left\{K_{j}\right\}, p\right) =
-        \frac{\sum_{j=1}^{c} d\left(\bar{X}^{K_{j}}, \tilde{X}\right)^p}
-        {\sum_{j=1}^{c} \sigma_{X^{K_{j}}}^p}
-
-    where :math:`\tilde{X}` is the mean of centers of class of all :math:`c`
-    classes and :math:`p` is the exponentiation of the distance measure
-    named exponent at the input of this function.
+        \mathrm{classDis} \left( \left\{K_{j} \right\}_{j=1}^c, p \right) =
+        \frac{\sum_{j=1}^c d\left(\mathbf{M}_{K_{j}},\bar{\mathbf{M}}\right)^p}
+        {\sum_{j=1}^c \sigma_{K_{j}}^p}
+
+    where :math:`\bar{\mathbf{M}}` is the mean of centers of class of all
+    :math:`c` classes.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_channels)
         Set of SPD matrices.
     y : ndarray, shape (n_matrices,)
         Labels for each matrix.
@@ -950,23 +965,24 @@
         Parameter for exponentiation of distances, corresponding to p in the
         above equations:
 
         - exponent = 1 gives the formula originally defined in [1]_;
         - exponent = 2 gives the Fisher criterion generalized on the manifold,
           ie the ratio of the variance between the classes to the variance
           within the classes.
-    metric : string | dict, default='riemann'
-        The type of metric used for centroid and distance estimation.
-        See `mean_covariance` for the list of supported metric.
-        The metric could be a dict with two keys, `mean` and `distance` in
-        order to pass different metrics for the centroid estimation and the
-        distance estimation. The original equation of class distinctiveness
-        in [1]_ uses 'riemann' for both the centroid estimation and the
-        distance estimation but you can customize other metrics with your
-        interests.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
+        The original equation of class distinctiveness in [1]_ uses "riemann"
+        for both the centroid estimation and the distance estimation but you
+        can provide other metrics depending on your interests.
     return_num_denom : bool, default=False
         Whether to return numerator and denominator of class_dis.
 
     Returns
     -------
     class_dis : float
         Class distinctiveness value.
@@ -986,18 +1002,18 @@
     .. [1] `Defining and quantifying users’ mental imagery-based
        BCI skills: a first step
        <https://hal.archives-ouvertes.fr/hal-01846434/>`_
        F. Lotte, and C. Jeunet. Journal of neural engineering,
        15(4), 046030, 2018.
     """
 
-    metric_mean, metric_dist = _check_metric(metric)
+    metric_mean, metric_dist = check_metric(metric)
     classes = np.unique(y)
     if len(classes) <= 1:
-        raise ValueError('X must contain at least two classes')
+        raise ValueError("X must contain at least two classes")
 
     means = np.array([
         mean_covariance(X[y == ll], metric=metric_mean) for ll in classes
     ])
 
     if len(classes) == 2:
         num = distance(means[0], means[1], metric=metric_dist) ** exponent
```

### Comparing `pyriemann-0.5/pyriemann/clustering.py` & `pyriemann-0.6/pyriemann/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 """Clustering functions."""
 import numpy as np
+from joblib import Parallel, delayed
 from scipy.stats import norm, chi2
+import sklearn
 from sklearn.base import (BaseEstimator, ClassifierMixin, TransformerMixin,
                           ClusterMixin, clone)
+from sklearn.cluster import KMeans as _KMeans
+
+from .classification import MDM
+from .utils.mean import mean_covariance
+from .utils.geodesic import geodesic
+from .utils.utils import check_metric
+
 
-try:
-    from sklearn.cluster._kmeans import _init_centroids
-except ImportError:
-    # Workaround for scikit-learn v0.24.0rc1+
-    # See issue: https://github.com/alexandrebarachant/pyRiemann/issues/92
-    from sklearn.cluster import KMeans as _KMeans
-
-    def _init_centroids(X, n_clusters, init, random_state, x_squared_norms):
-        if random_state is not None:
-            random_state = np.random.RandomState(random_state)
+def _init_centroids(X, n_clusters, init, random_state, x_squared_norms):
+    if random_state is not None:
+        random_state = np.random.RandomState(random_state)
+    if sklearn.__version__ < '1.3.0':
         return _KMeans(n_clusters=n_clusters, init=init)._init_centroids(
             X,
             x_squared_norms,
             init,
             random_state,
         )
+    else:
+        n_samples = X.shape[0]
+        return _KMeans(n_clusters=n_clusters, init=init)._init_centroids(
+            X,
+            x_squared_norms,
+            init,
+            random_state,
+            sample_weight=np.ones(n_samples) / n_samples,
+        )
 
 
-from joblib import Parallel, delayed
-
-from .classification import MDM, _check_metric
-from .utils.mean import mean_covariance
-from .utils.geodesic import geodesic
-
 #######################################################################
 
 
 def _fit_single(X, y=None, n_clusters=2, init='random', random_state=None,
                 metric='riemann', max_iter=100, tol=1e-4, n_jobs=1):
     """helper to fit a single run of centroid."""
     # init random state if provided
     mdm = MDM(metric=metric, n_jobs=n_jobs)
-    mdm.metric_mean, mdm.metric_dist = _check_metric(metric)
-    squared_nomrs = [np.linalg.norm(x, ord='fro')**2 for x in X]
+    mdm.metric_mean, mdm.metric_dist = check_metric(metric)
+    squared_norms = [np.linalg.norm(x, ord='fro')**2 for x in X]
     mdm.covmeans_ = _init_centroids(X, n_clusters, init,
                                     random_state=random_state,
-                                    x_squared_norms=squared_nomrs)
+                                    x_squared_norms=squared_norms)
     if y is not None:
         mdm.classes_ = np.unique(y)
     else:
         mdm.classes_ = np.arange(n_clusters)
 
     labels = mdm.predict(X)
     k = 0
@@ -71,16 +77,21 @@
 
     Parameters
     ----------
     n_cluster : int, default=2
         Number of clusters.
     max_iter : int, default=100
         The maximum number of iteration to reach convergence.
-    metric : string, default='riemann'
-        The type of metric used for centroid and distance estimation.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     random_state : integer or np.RandomState, optional
         The generator used to initialize the centers. If an integer is
         given, it fixes the seed. Defaults to the global numpy random
         number generator.
     init : 'random' or ndarray, shape (n_clusters, n_channels, n_channels), \
             default='random'
         Method for initialization of centers.
@@ -118,15 +129,15 @@
 
     See Also
     --------
     Kmeans
     MDM
     """
 
-    def __init__(self, n_clusters=2, max_iter=100, metric='riemann',
+    def __init__(self, n_clusters=2, max_iter=100, metric="riemann",
                  random_state=None, init='random', n_init=10, n_jobs=1,
                  tol=1e-4):
         """Init."""
         self.metric = metric
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.seed = random_state
@@ -264,30 +275,35 @@
             self.km.fit(X[y == c])
             self.covmeans_.extend(self.km.centroids())
         return self
 
     def transform(self, X):
         """Transform."""
         mdm = MDM(metric=self.metric, n_jobs=self.km.n_jobs)
-        mdm.metric_mean, mdm.metric_dist = _check_metric(self.metric)
+        mdm.metric_mean, mdm.metric_dist = check_metric(self.metric)
         mdm.covmeans_ = self.covmeans_
         return mdm._predict_distances(X)
 
 
 class Potato(BaseEstimator, TransformerMixin, ClassifierMixin):
     """Artefact detection with the Riemannian Potato.
 
     The Riemannian Potato [1]_ is a clustering method used to detect artifact
     in EEG signals. The algorithm iteratively estimates the centroid of clean
     signal by rejecting every trial that is too far from it.
 
     Parameters
     ----------
-    metric : string, default='riemann'
-        The type of metric used for centroid and distance estimation.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     threshold : float, default=3
         Threshold on z-score of distance to reject artifacts. It is the number
         of standard deviations from the mean of distances to the centroid.
     n_iter_max : int, default=100
         The maximum number of iteration to reach convergence.
     pos_label : int, default=1
         The positive label corresponding to clean data.
@@ -352,15 +368,15 @@
         self : Potato instance
             The Potato instance.
         """
         if self.pos_label == self.neg_label:
             raise ValueError("Positive and negative labels must be different")
 
         self._mdm = MDM(metric=self.metric)
-        self._mdm.metric_mean, self._mdm.metric_dist = _check_metric(
+        self._mdm.metric_mean, self._mdm.metric_dist = check_metric(
             self.metric
         )
 
         y_old = self._check_labels(X, y)
 
         for _ in range(self.n_iter_max):
             ix = (y_old == 1)
@@ -549,16 +565,21 @@
         Number of potatoes in the field.
     p_threshold : float, default=0.01
         Threshold on probability to being clean, in (0, 1), combining
         probabilities of potatoes using Fisher's method.
     z_threshold : float, default=3
         Threshold on z-score of distance to reject artifacts. It is the number
         of standard deviations from the mean of distances to the centroid.
-    metric : string, default='riemann'
-        The type of metric used for centroid and distance estimation.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     n_iter_max : int, default=10
         The maximum number of iteration to reach convergence.
     pos_label: int, default=1
         The positive label corresponding to clean data.
     neg_label: int, default=0
         The negative label corresponding to artifact data.
 
@@ -577,15 +598,15 @@
         <https://hal.archives-ouvertes.fr/hal-02015909>`_
         Q. Barthélemy, L. Mayaud, D. Ojeda, and M. Congedo. IEEE Transactions
         on Neural Systems and Rehabilitation Engineering, IEEE Institute of
         Electrical and Electronics Engineers, 2019, 27 (2), pp.244-255
     """
 
     def __init__(self, n_potatoes=1, p_threshold=0.01, z_threshold=3,
-                 metric='riemann', n_iter_max=10, pos_label=1, neg_label=0):
+                 metric="riemann", n_iter_max=10, pos_label=1, neg_label=0):
         """Init."""
         self.n_potatoes = int(n_potatoes)
         self.p_threshold = p_threshold
         self.metric = metric
         self.z_threshold = z_threshold
         self.n_iter_max = n_iter_max
         self.pos_label = pos_label
```

### Comparing `pyriemann-0.5/pyriemann/datasets/sampling.py` & `pyriemann-0.6/pyriemann/datasets/sampling.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/datasets/simulated.py` & `pyriemann-0.6/pyriemann/datasets/simulated.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,64 +2,14 @@
 from sklearn.utils.validation import check_random_state
 
 from ..utils.mean import mean_riemann
 from ..utils.distance import distance_riemann
 from ..utils.base import invsqrtm, powm, sqrtm, expm
 from .sampling import generate_random_spd_matrix, sample_gaussian_spd
 from ..transfer import encode_domains
-from ..utils import deprecated
-
-
-@deprecated(
-    "make_covariances is deprecated and will be removed in 0.6.0; "
-    "please use make_matrices."
-)
-def make_covariances(n_matrices, n_channels, rs=None, return_params=False,
-                     evals_mean=2.0, evals_std=0.1):
-    """Generate a set of covariances matrices, with the same eigenvectors.
-
-    Parameters
-    ----------
-    n_matrices : int
-        Number of matrices to generate.
-    n_channels : int
-        Number of channels in covariance matrices.
-    rs : RandomState instance, default=None
-        Random state for reproducible output across multiple function calls.
-    return_params : bool, default=False
-        If True, then return parameters.
-    evals_mean : float, default=2.0
-        Mean of eigen values.
-    evals_std : float, default=0.1
-        Standard deviation of eigen values.
-
-    Returns
-    -------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Covariances matrices.
-    evals : ndarray, shape (n_matrices, n_channels)
-        Eigen values used for each covariance matrix.
-        Only returned if ``return_params=True``.
-    evecs : ndarray, shape (n_channels, n_channels)
-        Eigen vectors used for all covariance matrices.
-        Only returned if ``return_params=True``.
-    """
-    rs = check_random_state(rs)
-
-    evals = np.abs(evals_mean + evals_std * rs.randn(n_matrices, n_channels))
-    evecs, _ = np.linalg.qr(rs.randn(n_channels, n_channels))
-
-    covmats = np.empty((n_matrices, n_channels, n_channels))
-    for i in range(n_matrices):
-        covmats[i] = evecs @ np.diag(evals[i]) @ evecs.T
-
-    if return_params:
-        return covmats, evals, evecs
-    else:
-        return covmats
 
 
 def make_matrices(n_matrices, n_dim, kind, rs=None, return_params=False,
                   evals_low=0.5, evals_high=2.0, eigvecs_same=False):
     """Generate a set of matrices, with specific properties.
 
     Parameters
```

### Comparing `pyriemann-0.5/pyriemann/embedding.py` & `pyriemann-0.6/pyriemann/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,32 @@
     are the SPD matrices and the weights of the links are determined by the
     Riemannian distance between each pair of them.
 
     Parameters
     ----------
     n_components : integer, default=2
         The dimension of the projected subspace.
-    metric : string | dict, default='riemann'
-        The type of metric to be used for defining pairwise distance between
-        SPD matrices.
+    metric : string, default="riemann"
+        Metric used for defining pairwise distance between SPD matrices.
+        For the list of supported metrics,
+        see :func:`pyriemann.utils.distance.pairwise_distance`.
     eps : None | float, default=None
         The scaling of the Gaussian kernel. If none is given it will use the
         square of the median of pairwise distances between points.
 
     References
     ----------
     .. [1] `Laplacian Eigenmaps for dimensionality
         reduction and data representation
         <https://ieeexplore.ieee.org/document/6789755>`_
         M. Belkin and P. Niyogi, in Neural Computation, vol. 15, no. 6,
         p. 1373-1396 , 2003
     """
 
-    def __init__(self, n_components=2, metric='riemann', eps=None):
+    def __init__(self, n_components=2, metric="riemann", eps=None):
         """Init."""
         self.metric = metric
         self.n_components = n_components
         self.eps = eps
 
     def _get_affinity_matrix(self, X, eps):
 
@@ -132,15 +133,15 @@
 
     Parameters
     ----------
     n_components : int, default=2
         Dimensionality of projected space.
     n_neighbors : int, default=5
         Number of neighbors for reconstruction of each point.
-    metric : {'riemann', 'logeuclid', 'euclid'}, default: 'riemann'
+    metric : {"euclid", "logeuclid", "riemann"}, default: "riemann"
         Metric used for KNN and Kernel estimation.
     reg : float, default=1e-3
         Regularization parameter.
 
     Attributes
     ----------
     embedding_ : ndarray, shape (n_matrices, n_components)
@@ -164,15 +165,15 @@
     .. [2] `Clustering and dimensionality reduction
         on Riemannian manifolds
         <https://ieeexplore.ieee.org/document/4587422>`_
         A. Goh and R. Vidal, in 2008 IEEE Conference on Computer Vision and
         Pattern Recognition
     """
 
-    def __init__(self, n_components=2, n_neighbors=5, metric='riemann',
+    def __init__(self, n_components=2, n_neighbors=5, metric="riemann",
                  reg=1e-3):
         self.n_components = n_components
         self.n_neighbors = n_neighbors
         self.metric = metric
         self.reg = reg
 
     def fit(self, X, y=None):
@@ -261,29 +262,29 @@
         X_new : ndarray, shape (n_matrices, n_components)
             Coordinates of embedded matrices.
         """
         self.fit(X)
         return self.embedding_
 
 
-def barycenter_weights(X, Y, indices, metric='riemann', reg=1e-3):
+def barycenter_weights(X, Y, indices, metric="riemann", reg=1e-3):
     """Compute Riemannian barycenter weights of X from Y along the first axis.
 
     Estimates the weights to assign to each point in Y[indices] to recover
     the point X[i] by geodesic interpolation. The barycenter weights sum to 1.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_channels)
         Set of SPD matrices.
     Y : ndarray, shape (n_matrices, n_channels, n_channels)
         Set of SPD matrices.
     indices : ndarray, shape (n_matrices, n_neighbors)
         Indices of the points in Y used to compute the barycenter
-    metric : {'riemann', 'logeuclid', 'euclid'}, default='riemann'
+    metric : {"euclid", "logeuclid", "riemann"}, default="riemann"
         Kernel metric.
     reg : float, default=1e-3
         Amount of regularization to add for the problem to be
         well-posed in the case of n_neighbors > n_channels.
 
     Returns
     -------
@@ -316,15 +317,15 @@
     return B
 
 
 def locally_linear_embedding(X,
                              *,
                              n_components=2,
                              n_neighbors=5,
-                             metric='riemann',
+                             metric="riemann",
                              reg=1e-3):
     """Perform a Locally Linear Embedding (LLE) of SPD matrices.
 
     As proposed in [1]_, Locally Linear Embedding (LLE) is a non-linear,
     neighborhood-preserving dimensionality reduction algorithm which consists
     of three main steps. For each point xi,
 
@@ -338,15 +339,15 @@
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_channels)
         Set of SPD matrices.
     n_components : int, default=2
         Dimensionality of projected space.
     n_neighbors : int, default=5
         Number of neighbors for reconstruction of each point.
-    metric : {'riemann', 'logeuclid', 'euclid'}, default: 'riemann'
+    metric : {"euclid", "logeuclid", "riemann"}, default: "riemann"
         Metric used for KNN and Kernel estimation.
     reg : float, default=1e-3
         Regularization parameter.
 
     Returns
     -------
     embd : ndarray, shape (n_matrices, n_components)
@@ -380,15 +381,15 @@
     )
     # M = (W - I).T * (W - I) = W.T * W - W.T - W + I
     # calculated in the two following lines
     M = (W.T * W - W.T - W).toarray()
     M.flat[:: M.shape[0] + 1] += 1
 
     eigen_values, eigen_vectors = eigh(
-        M, eigvals=(1, n_components), overwrite_a=True
+        M, subset_by_index=(1, n_components), overwrite_a=True
     )
     index = np.argsort(np.abs(eigen_values))
     embd, error = eigen_vectors[:, index], np.sum(eigen_values)
 
     return embd, error
```

### Comparing `pyriemann-0.5/pyriemann/estimation.py` & `pyriemann-0.6/pyriemann/estimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Estimation of SPD matrices."""
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.covariance import shrunk_covariance
 from sklearn.metrics.pairwise import pairwise_kernels
 
 from .spatialfilters import Xdawn
-from .utils.covariance import (covariances, covariances_EP, cospectrum,
+from .utils.covariance import (covariances, covariances_EP, cross_spectrum,
                                coherence, block_covariances)
+from .utils import deprecated
 
 
 def _nextpow2(i):
     """Find next power of 2."""
     n = 1
     while n < i:
         n *= 2
     return n
 
 
 class Covariances(BaseEstimator, TransformerMixin):
-    """Estimation of covariance matrix.
+    """Estimation of covariance matrices.
 
     Perform a simple covariance matrix estimation for each given input.
 
     Parameters
     ----------
     estimator : string, default='scm'
         Covariance matrix estimator, see
@@ -30,16 +31,14 @@
     **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     See Also
     --------
     ERPCovariances
     XdawnCovariances
-    CospCovariances
-    HankelCovariances
     """
 
     def __init__(self, estimator='scm', **kwds):
         """Init."""
         self.estimator = estimator
         self.kwds = kwds
 
@@ -76,17 +75,18 @@
             Covariance matrices.
         """
         covmats = covariances(X, estimator=self.estimator, **self.kwds)
         return covmats
 
 
 class ERPCovariances(BaseEstimator, TransformerMixin):
-    r"""Estimate special form covariance matrix for ERP.
+    r"""Estimate special form covariance matrices for ERP.
 
-    Estimation of special form covariance matrix dedicated to ERP processing.
+    Estimation of special form covariance matrix dedicated to event-related
+    potentials (ERP) processing.
     For each class, a prototyped response is obtained by average across trials:
 
     .. math::
         \mathbf{P} = \frac{1}{m} \sum_{i=1}^{m} \mathbf{X}_i
 
     and a super trial is built using the concatenation of :math:`\mathbf{P}`
     and the trial :math:`\mathbf{X}_i`:
@@ -121,16 +121,14 @@
         equal to `n_classes x n_channels` if `svd` is None,
         and to `n_classes x min(svd, n_channels)` otherwise.
 
     See Also
     --------
     Covariances
     XdawnCovariances
-    CospCovariances
-    HankelCovariances
 
     References
     ----------
     .. [1] `A Plug and Play P300 BCI Using Information Geometry
         <https://arxiv.org/abs/1409.0107>`_
         A. Barachant, M. Congedo. Research report, 2014.
     .. [2] `A New generation of Brain-Computer Interface Based on Riemannian
@@ -213,15 +211,15 @@
             estimator=self.estimator,
             **self.kwds
         )
         return covmats
 
 
 class XdawnCovariances(BaseEstimator, TransformerMixin):
-    """Estimate special form covariance matrix for ERP combined with Xdawn.
+    """Estimate special form covariance matrices for ERP combined with Xdawn.
 
     Estimation of special form covariance matrix dedicated to ERP processing
     combined with `Xdawn` spatial filtering.
     This is similar to :class:`pyriemann.estimation.ERPCovariances` but data
     are spatially filtered with :class:`pyriemann.spatialfilters.Xdawn`.
     A complete description of the method is available in [1]_.
 
@@ -343,15 +341,15 @@
             estimator=self.estimator,
             **self.kwds
         )
         return covmats
 
 
 class BlockCovariances(BaseEstimator, TransformerMixin):
-    """Estimation of block covariance matrix.
+    """Estimation of block covariance matrices.
 
     Perform a block covariance estimation for each given matrix. The
     resulting matrices are block diagonal matrices.
 
     The blocks on the diagonal are calculated as individual covariance
     matrices for a subset of channels using the given the estimator.
     Varying block sized possible by passing a list to allow incorporation
@@ -430,22 +428,21 @@
 
         return block_covariances(X, blocks, self.estimator, **self.kwds)
 
 
 ###############################################################################
 
 
-class CospCovariances(BaseEstimator, TransformerMixin):
-    """Estimation of cospectral covariance matrix.
+class CrossSpectra(BaseEstimator, TransformerMixin):
+    """Estimation of cross-spectral matrices.
 
-    Co-spectral matrices are the real part of complex cross-spectral matrices
-    (see :func:`pyriemann.utils.covariance.cross_spectrum`), estimated as the
-    spectrum covariance in the frequency domain. This method returns a 4-d
-    array with a cospectral covariance matrix for each input and in each
-    frequency bin of the FFT.
+    Complex cross-spectral matrices are HPD matrices estimated as the spectrum
+    covariance in the frequency domain [1]_. It returns a 4-d array with a
+    cross-spectral matrix for each input and in each frequency bin of the
+    Fourier transform.
 
     Parameters
     ----------
     window : int, default=128
         The length of the FFT window used for spectral estimation.
     overlap : float, default=0.75
         The percentage of overlap between window.
@@ -455,22 +452,29 @@
         The maximal frequency to be returned.
     fs : float | None, default=None
         The sampling frequency of the signal.
 
     Attributes
     ----------
     freqs_ : ndarray, shape (n_freqs,)
-        If transformed, the frequencies associated to cospectra.
+        If transformed, the frequencies associated to cross-spectra.
         None if ``fs`` is None.
 
+    Notes
+    -----
+    .. versionadded:: 0.6
+
     See Also
     --------
-    Covariances
-    HankelCovariances
+    CoSpectra
     Coherences
+
+    References
+    ----------
+    .. [1] https://en.wikipedia.org/wiki/Cross-spectrum
     """
 
     def __init__(self, window=128, overlap=0.75, fmin=None, fmax=None,
                  fs=None):
         """Init."""
         self.window = _nextpow2(window)
         self.overlap = overlap
@@ -488,46 +492,104 @@
         X : ndarray, shape (n_matrices, n_channels, n_times)
             Multi-channel time-series.
         y : None
             Not used, here for compatibility with sklearn API.
 
         Returns
         -------
-        self : CospCovariances instance
-            The CospCovariances instance.
+        self : CrossSpectra instance
+            The CrossSpectra instance.
         """
         return self
 
     def transform(self, X):
-        """Estimate the cospectral covariance matrices.
+        """Estimate cross-spectral matrices.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_times)
             Multi-channel time-series.
 
         Returns
         -------
-        covmats : ndarray, shape (n_matrices, n_channels, n_channels, n_freqs)
-            Covariance matrices for each input and for each frequency bin.
+        X_new : ndarray, shape (n_matrices, n_channels, n_channels, n_freqs)
+            Cross-spectral matrices for each input and for each frequency bin.
         """
-        out = []
+        X_new = []
 
         for i in range(len(X)):
-            S, freqs = cospectrum(
+            S, freqs = cross_spectrum(
                 X[i],
                 window=self.window,
                 overlap=self.overlap,
                 fmin=self.fmin,
                 fmax=self.fmax,
                 fs=self.fs)
-            out.append(S)
+            X_new.append(S)
         self.freqs_ = freqs
 
-        return np.array(out)
+        return np.array(X_new)
+
+
+class CoSpectra(CrossSpectra):
+    """Estimation of co-spectral matrices.
+
+    Co-spectral matrices are SPD matrices estimated as the real part of the
+    :class:`pyriemann.estimation.CrossSpectra`. It returns a 4-d array with a
+    co-spectral matrix for each input and in each frequency bin of the
+    Fourier transform.
+
+    Parameters
+    ----------
+    window : int, default=128
+        The length of the FFT window used for spectral estimation.
+    overlap : float, default=0.75
+        The percentage of overlap between window.
+    fmin : float | None, default=None
+        The minimal frequency to be returned.
+    fmax : float | None, default=None
+        The maximal frequency to be returned.
+    fs : float | None, default=None
+        The sampling frequency of the signal.
+
+    Attributes
+    ----------
+    freqs_ : ndarray, shape (n_freqs,)
+        If transformed, the frequencies associated to cospectra.
+        None if ``fs`` is None.
+
+    See Also
+    --------
+    CrossSpectra
+    Coherences
+    """
+
+    def transform(self, X):
+        """Estimate co-spectral matrices.
+
+        Parameters
+        ----------
+        X : ndarray, shape (n_matrices, n_channels, n_times)
+            Multi-channel time-series.
+
+        Returns
+        -------
+        X_new : ndarray, shape (n_matrices, n_channels, n_channels, n_freqs)
+            Co-spectral matrices for each input and for each frequency bin.
+        """
+        X_new = super().transform(X)
+        return X_new.real
+
+
+@deprecated(
+    "CospCovariances is deprecated and will be removed in 0.8.0; "
+    "please use CoSpectra."
+)
+class CospCovariances(CoSpectra):
+    pass
 
 
 class Coherences(CospCovariances):
     """Estimation of squared coherence matrices.
 
     Squared coherence matrices estimation [1]_. This method will return a 4-d
     array with a squared coherence matrix estimation for each input and in
@@ -570,17 +632,16 @@
 
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
     --------
-    Covariances
-    HankelCovariances
-    CospCovariances
+    CrossSpectra
+    TimeDelayCovariances
 
     References
     ----------
     .. [1] `Instantaneous and lagged measurements of linear
         and nonlinear dependence between groups of multivariate time series:
         frequency decomposition
         <https://arxiv.org/ftp/arxiv/papers/0711/0711.1455.pdf>`_
@@ -634,42 +695,47 @@
                 coh=self.coh)
             out.append(S)
         self.freqs_ = freqs
 
         return np.array(out)
 
 
-class HankelCovariances(BaseEstimator, TransformerMixin):
-    """Estimation of covariance matrix with time delayed Hankel matrices.
+class TimeDelayCovariances(BaseEstimator, TransformerMixin):
+    """Estimation of covariance matrices with time delay matrices.
 
-    Hankel covariance matrices [1]_ are useful to catch spectral dynamics of
-    the signal, similarly to the CSSP method [2]_. It is done by concatenating
+    Time delay covariance matrices are useful to catch spectral dynamics of
+    the signal, similarly to the CSSP method [1]_. It is done by concatenating
     time delayed version of the signal before covariance estimation.
 
     Parameters
     ----------
     delays : int | list of int, default=4
         The delays to apply for the Hankel matrices. If `int`, it use a range
         of delays up to the given value. A list of int can be given.
     estimator : string, default='scm'
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
     **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
+    Attributes
+    ----------
+    Xtd_ : ndarray, shape (n_matrices, n_channels x n_delays, n_times)
+        Time delay multi-channel time-series, where `n_delays` is equal to:
+        `delays` when it is a int, and `1 + len(delays)` when it is a list.
+
     See Also
     --------
     Covariances
     ERPCovariances
     CospCovariances
 
     References
     ----------
-    .. [1] https://en.wikipedia.org/wiki/Hankel_matrix
-    .. [2] `Spatio-spectral filters for improving the classification of single
+    .. [1] `Spatio-spectral filters for improving the classification of single
         trial EEG
         <http://doc.ml.tu-berlin.de/bbci/publications/LemBlaCurMue05.pdf>`_
         S. Lemm, B. Blankertz, B. Curio, K-R. Muller. IEEE Transactions on
         Biomedical Engineering 52(9), 1541-1548, 2005.
     """
 
     def __init__(self, delays=4, estimator='scm', **kwds):
@@ -688,58 +754,64 @@
         X : ndarray, shape (n_matrices, n_channels, n_times)
             Multi-channel time-series.
         y : None
             Not used, here for compatibility with sklearn API.
 
         Returns
         -------
-        self : HankelCovariances instance
-            The HankelCovariances instance.
+        self : TimeDelayCovariances instance
+            The TimeDelayCovariances instance.
         """
         return self
 
     def transform(self, X):
-        """Estimate the Hankel covariance matrices.
+        """Estimate the time delay covariance matrices.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_times)
             Multi-channel time-series.
 
         Returns
         -------
-        covmats : ndarray, shape (n_matrices, n_delays x n_channels, \
-                n_delays x n_channels)
-            Hankel covariance matrices, where n_delays is equal to `delays`
-            when it is a int, and to `1 + len(delays)` when it is a list.
+        covmats : ndarray, shape (n_matrices, n_channels x n_delays, \
+                n_channels x n_delays)
+            Time delay covariance matrices, where `n_delays` is equal to:
+            `delays` when it is a int, and `1 + len(delays)` when it is a list.
         """
 
         if isinstance(self.delays, int):
             delays = range(1, self.delays)
         elif isinstance(self.delays, list):
             delays = self.delays
         else:
             raise ValueError('delays must be an integer or a list')
 
-        X2 = []
-        for x in X:
-            tmp = x
-            for d in delays:
-                tmp = np.r_[tmp, np.roll(x, d, axis=-1)]
-            X2.append(tmp)
-        X2 = np.array(X2)
-        covmats = covariances(X2, estimator=self.estimator, **self.kwds)
+        Xtd = [X]
+        for d in delays:
+            Xtd.append(np.roll(X, d, axis=-1))
+        self.Xtd_ = np.concatenate(Xtd, axis=-2)
+
+        covmats = covariances(self.Xtd_, estimator=self.estimator, **self.kwds)
         return covmats
 
 
+@deprecated(
+    "HankelCovariances is deprecated and will be removed in 0.8.0; "
+    "please use TimeDelayCovariances."
+)
+class HankelCovariances(TimeDelayCovariances):
+    pass
+
+
 ###############################################################################
 
 
 class Kernels(BaseEstimator, TransformerMixin):
-    r"""Estimation of kernel matrix between channels of time series.
+    r"""Estimation of kernel matrices between channels of time series.
 
     Perform a kernel matrix estimation for each given time series, evaluating a
     kernel function between each pair of channels (rather than between pairs of
     time samples) and allowing to extract nonlinear channel relationship [1]_.
 
     For an input time series :math:`X \in \mathbb{R}^{c \times t}`, composed of
     :math:`c` channels and :math:`t` time samples, kernel function
```

### Comparing `pyriemann-0.5/pyriemann/preprocessing.py` & `pyriemann-0.6/pyriemann/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,19 @@
     """Whitening, and optional unsupervised dimension reduction.
 
     Implementation of the whitening, and an optional unsupervised dimension
     reduction, with SPD matrices as inputs.
 
     Parameters
     ----------
-    metric : str, default='euclid'
-        The metric for the estimation of mean matrix used for whitening and
+    metric : str, default="euclid"
+        Metric for the estimation of mean matrix used for whitening and
         dimension reduction.
+        For the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`.
     dim_red : None | dict, default=None
         If ``None`` :
             no dimension reduction during whitening.
         If ``{'n_components': val}`` :
             dimension reduction defining the number of components;
             ``val`` must be an integer superior to 1.
         If ``{'expl_var': val}`` :
@@ -54,15 +56,15 @@
 
     Notes
     -----
     .. versionadded:: 0.2.7
 
     """
 
-    def __init__(self, metric='euclid', dim_red=None, verbose=False):
+    def __init__(self, metric="euclid", dim_red=None, verbose=False):
         """Init."""
         self.metric = metric
         self.dim_red = dim_red
         self.verbose = verbose
 
     def fit(self, X, y=None, sample_weight=None):
         """Train whitening spatial filters.
```

### Comparing `pyriemann-0.5/pyriemann/regression.py` & `pyriemann-0.6/pyriemann/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Module for regression functions."""
 import functools
 
 import numpy as np
-
 from sklearn.metrics import r2_score
 from sklearn.svm import SVR as sklearnSVR
 from sklearn.utils.extmath import softmax
 
 from .utils.kernel import kernel
-from .classification import MDM, _check_metric
+from .classification import MDM
 from .utils.mean import mean_covariance
+from .utils.utils import check_metric
 
 
 class SVR(sklearnSVR):
     """Regression by support-vector machine.
 
     Support-vector machine (SVM) regression with precomputed Riemannian kernel
     matrix according to different metrics, extending the idea described in [1]_
     to regression.
 
     Parameters
     ----------
-    metric : {'riemann', 'euclid', 'logeuclid'}, default='riemann'
+    metric : {"euclid", "logeuclid", "riemann"}, default="riemann"
         Metric for kernel matrix computation.
     Cref : None | ndarray, shape (n_channels, n_channels)
         Reference point for kernel matrix computation. If None, the mean of
         the training data according to the metric is used.
     kernel_fct : 'precomputed' | callable
         If 'precomputed', the kernel matrix for datasets X and Y is estimated
         according to `pyriemann.utils.kernel(X, Y, Cref, metric)`.
@@ -167,32 +167,36 @@
 
     DISCLAIMER: This is an unpublished algorithm.
 
     Parameters
     ----------
     n_neighbors : int, default=5
         Number of neighbors.
-    metric : string | dict, default='riemann'
-        The type of metric used for distance estimation.
-        See `distance` for the list of supported metric.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
 
     Attributes
     ----------
     values_ : ndarray, shape (n_matrices,)
         Training target values.
     covmeans_ : ndarray, shape (n_matrices, n_channels, n_channels)
         Training set of SPD matrices.
 
     Notes
     -----
     .. versionadded:: 0.3
 
     """
 
-    def __init__(self, n_neighbors=5, metric='riemann'):
+    def __init__(self, n_neighbors=5, metric="riemann"):
         """Init."""
         self.n_neighbors = n_neighbors
         self._estimator_type = "regressor"
         super().__init__(metric=metric)
 
     def fit(self, X, y, sample_weight=None):
         """Fit (store the training data).
@@ -207,15 +211,15 @@
             Not used, here for compatibility with sklearn API.
 
         Returns
         -------
         self : KNearestNeighborRegressor instance
             The KNearestNeighborRegressor instance.
         """
-        self.metric_mean, self.metric_dist = _check_metric(self.metric)
+        self.metric_mean, self.metric_dist = check_metric(self.metric)
         self.values_ = y
         self.covmeans_ = X
 
         return self
 
     def predict(self, X):
         """Get the predictions.
```

### Comparing `pyriemann-0.5/pyriemann/spatialfilters.py` & `pyriemann-0.6/pyriemann/spatialfilters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Spatial filtering function."""
 import warnings
 
 import numpy as np
 from scipy.linalg import eigh, inv
 from sklearn.base import BaseEstimator, TransformerMixin
 
-from .utils.covariance import _check_est, normalize, get_nondiag_weight
+from .utils.covariance import normalize, get_nondiag_weight, cov_est_functions
 from .utils.mean import mean_covariance
+from .utils.utils import check_function
 from .utils.ajd import ajd_pham
 from . import estimation as est
 from .preprocessing import Whitening
 
 
 class Xdawn(BaseEstimator, TransformerMixin):
     """Xdawn algorithm.
@@ -75,15 +76,15 @@
         self.nfilter = nfilter
         self.classes = classes
         self.estimator = estimator
         self.baseline_cov = baseline_cov
 
     @property
     def estimator_fn(self):
-        return _check_est(self.estimator)
+        return check_function(self.estimator, cov_est_functions)
 
     def fit(self, X, y):
         """Train Xdawn spatial filters.
 
         Parameters
         ----------
         X : ndarray, shape (n_trials, n_channels, n_times)
@@ -155,20 +156,20 @@
 class BilinearFilter(BaseEstimator, TransformerMixin):
     r"""Bilinear spatial filter.
 
     Bilinear spatial filter for SPD matrices allows to define a custom spatial
     filter for bilinear projection of the data:
 
     .. math::
-        \mathbf{Cf}_i = \mathbf{V} \mathbf{C}_i \mathbf{V}^T
+        \mathbf{Xf}_i = \mathbf{V} \mathbf{X}_i \mathbf{V}^T
 
     If log parameter is set to true, will return the log of the diagonal:
 
     .. math::
-        \mathbf{cf}_i = \log [ \mathrm{diag} (\mathbf{Cf}_i) ]
+        \mathbf{xf}_i = \log ( \mathrm{diag} (\mathbf{Xf}_i) )
 
     Parameters
     ----------
     filters : ndarray, shape (n_filters, n_channels)
         The filters for bilinear transform.
     log : bool, default=False
         If true, return the log variance, otherwise return the spatially
@@ -253,16 +254,18 @@
     diagonalization. In this case, the spatial filter selection is achieved
     according to [4]_.
 
     Parameters
     ----------
     nfilter : int, default=4
         The number of components to decompose M/EEG signals.
-    metric : str, default='euclid'
-        The metric for the estimation of mean covariance matrices.
+    metric : str, default="euclid"
+        Metric used for the estimation of mean covariance matrices.
+        For the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`.
     log : bool, default=True
         If true, return the log variance, otherwise return the spatially
         filtered covariance matrices.
 
     Attributes
     ----------
     filters_ : ndarray, shape (min(n_channels, n_filters), n_channels)
@@ -291,15 +294,15 @@
     .. [4] `Multiclass common spatial patterns and information theoretic
         feature extraction
         <https://ieeexplore.ieee.org/document/4473042>`_
         IEEE Transactions on Biomedical Engineering, Volume 55, Issue 8,
         August 2008. pp. 1991 - 2000
     """
 
-    def __init__(self, nfilter=4, metric='euclid', log=True):
+    def __init__(self, nfilter=4, metric="euclid", log=True):
         """Init."""
         self.nfilter = nfilter
         self.metric = metric
         self.log = log
 
     def fit(self, X, y):
         """Train CSP spatial filters.
@@ -398,16 +401,18 @@
     applications include extraction of motor patterns using EMG power or audio
     paterns using sound envelope.
 
     Parameters
     ----------
     nfilter : int, default=4
         The number of components to decompose M/EEG signals.
-    metric : str, default='euclid'
-        The metric for the estimation of mean covariance matrices.
+    metric : str, default="euclid"
+        Metric used for the estimation of mean covariance matrices.
+        For the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`.
     log : bool, default=True
         If true, return the log variance, otherwise return the spatially
         filtered covariance matrices.
 
     Attributes
     ----------
     filters_ : ndarray, shape (min(n_channels, n_filters), n_channels)
```

### Comparing `pyriemann-0.5/pyriemann/stats.py` & `pyriemann-0.6/pyriemann/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import sys
 import math
 import numpy as np
+from sklearn.model_selection import cross_val_score
 
-from .utils.utils import check_version
 from .utils.distance import distance, pairwise_distance
 from .utils.mean import mean_covariance
-from .classification import MDM, _check_metric
-
-if check_version('sklearn', '0.18'):
-    from sklearn.model_selection import cross_val_score
-else:
-    from sklearn.cross_validation import cross_val_score
+from .utils.utils import check_metric
+from .classification import MDM
 
 
 def multiset_perm_number(y):
     """return the number of unique permutation in a multiset."""
     pr = 1
     for i in np.unique(y):
         pr *= math.factorial(np.sum(y == i))
@@ -259,22 +255,21 @@
         are estimated for each permutation.
 
     Parameters
     ----------
     n_perms : int, default=100
         The number of permutation. The minimum should be 20 for a resolution of
         0.05 p-value.
-    metric : string | dict, default='riemann'
-        The type of metric used for centroid and distance estimation.
-        see `distance` anb `mean_covariance` for the list of supported metric.
-        the metric could be a dict with two keys, `mean` and `distance` in
-        order to pass different metric for the centroid estimation and the
-        distance estimation. Typical usecase is to pass 'logeuclid' metric for
-        the mean in order to boost the computional speed and 'riemann' for the
-        distance in order to keep the good sensitivity for the classification.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     mode : string, default='pairwise'
         Type of statistic to use. could be 'pairwise', 'ttest' of 'ftest'
     n_jobs : integer, default=1
         The number of CPUs to use to do the computation. -1 means
         'all CPUs'.
     random_state : int, default=42
         random state for the permutation test.
@@ -300,15 +295,15 @@
     .. [1] `A new method for non-parametric multivariate analysis of variance
         <https://doi.org/10.1111/j.1442-9993.2001.01070.pp.x>`_
         M. Anderson. Austral ecology, Volume 26, Issue 1, February 2001.
     """
 
     def __init__(self,
                  n_perms=100,
-                 metric='riemann',
+                 metric="riemann",
                  mode='pairwise',
                  n_jobs=1,
                  random_state=42,
                  estimator=None):
         """Init."""
         self.n_perms = n_perms
         if mode not in ['pairwise', 'ttest', 'ftest']:
@@ -349,17 +344,15 @@
             return X
 
         return self.__init_transform(X)
 
     def __init_transform(self, X):
         """Init tr"""
         self.mdm = MDM(metric=self.metric, n_jobs=self.n_jobs)
-        self.mdm.metric_mean, self.mdm.metric_dist = _check_metric(
-            self.metric
-        )
+        self.mdm.metric_mean, self.mdm.metric_dist = check_metric(self.metric)
         if self.mode == 'ftest':
             self.global_mean = mean_covariance(X, metric=self.mdm.metric_mean)
         elif self.mode == 'pairwise':
             X = pairwise_distance(X, metric=self.mdm.metric_dist, squared=True)
         return X
 
     def _score_ftest(self, X, y):
```

### Comparing `pyriemann-0.5/pyriemann/tangentspace.py` & `pyriemann-0.6/pyriemann/tangentspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """Tangent space functions."""
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA
 
-from .utils.utils import check_version
 from .utils.mean import mean_covariance
 from .utils.tangentspace import tangent_space, untangent_space
-
-if check_version('sklearn', '0.17'):
-    from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA
-else:
-    from sklearn.lda import LDA
+from .utils.utils import check_metric
 
 
 class TangentSpace(BaseEstimator, TransformerMixin):
 
     """Tangent space project TransformerMixin.
 
     Tangent space projection map a set of SPD matrices to their
@@ -38,20 +34,21 @@
 
     After projection, it is possible to go back in the manifold using the
     inverse transform.
 
     Parameters
     ----------
     metric : string | dict, default='riemann'
-        The type of metric used for reference matrix estimation (see
-        `mean_covariance` for the list of supported metric) and for tangent
-        space map (see `tangent_space` for the list of supported metric).
-        The metric could be a dict with two keys, `mean` and `map` in
-        order to pass different metrics for the reference matrix estimation
-        and the tangent space mapping.
+        The type of metric used
+        for reference matrix estimation (for the list of supported metrics
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for tangent space map
+        (see :func:`pyriemann.utils.tangent_space.tangent_space`).
+        The metric can be a dict with two keys, "mean" and "map"
+        in order to pass different metrics.
     tsupdate : bool, default=False
         Activate tangent space update for covariante shift correction between
         training and test, as described in [2]_. This is not compatible with
         online implementation. Performance are better when the number of
         matrices for prediction is higher.
 
     Attributes
@@ -96,43 +93,25 @@
             Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         self : TangentSpace instance
             The TangentSpace instance.
         """
-        self.metric_mean, self.metric_map = self._check_metric(self.metric)
+        self.metric_mean, self.metric_map = check_metric(
+            self.metric, ["mean", "map"]
+        )
 
         self.reference_ = mean_covariance(
             X,
             metric=self.metric_mean,
             sample_weight=sample_weight
         )
         return self
 
-    def _check_metric(self, metric):
-
-        if isinstance(metric, str):
-            metric_mean = metric
-            metric_map = metric
-
-        elif isinstance(metric, dict):
-            # check keys
-            for key in ['mean', 'map']:
-                if key not in metric.keys():
-                    raise KeyError('metric must contain "mean" and "map"')
-
-            metric_mean = metric['mean']
-            metric_map = metric['map']
-
-        else:
-            raise TypeError('metric must be dict or str')
-
-        return metric_mean, metric_map
-
     def _check_data_dim(self, X):
         """Check data shape and return the size of SPD matrix."""
         shape_X = X.shape
         if len(X.shape) == 2:
             n_channels = (np.sqrt(1 + 8 * shape_X[1]) - 1) / 2
             if n_channels != int(n_channels):
                 raise ValueError("Shape of Tangent space vector does not"
@@ -165,15 +144,17 @@
             Set of SPD matrices.
 
         Returns
         -------
         ts : ndarray, shape (n_matrices, n_ts)
             Tangent space projections of SPD matrices.
         """
-        self.metric_mean, self.metric_map = self._check_metric(self.metric)
+        self.metric_mean, self.metric_map = check_metric(
+            self.metric, ["mean", "map"]
+        )
         self._check_reference_points(X)
 
         if self.tsupdate:
             Cr = mean_covariance(X, metric=self.metric_mean)
         else:
             Cr = self.reference_
         return tangent_space(X, Cr, metric=self.metric_map)
@@ -191,15 +172,17 @@
             Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         ts : ndarray, shape (n_matrices, n_ts)
             Tangent space projections of SPD matrices.
         """
-        self.metric_mean, self.metric_map = self._check_metric(self.metric)
+        self.metric_mean, self.metric_map = check_metric(
+            self.metric, ["mean", "map"]
+        )
 
         self.reference_ = mean_covariance(
             X,
             metric=self.metric_mean,
             sample_weight=sample_weight
         )
         return tangent_space(X, self.reference_, metric=self.metric_map)
@@ -217,36 +200,39 @@
             Not used, here for compatibility with sklearn API.
 
         Returns
         -------
         cov : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices corresponding to each of tangent vector.
         """
-        self.metric_mean, self.metric_map = self._check_metric(self.metric)
+        self.metric_mean, self.metric_map = check_metric(
+            self.metric, ["mean", "map"]
+        )
         self._check_reference_points(X)
         return untangent_space(X, self.reference_, metric=self.metric_map)
 
 
 class FGDA(BaseEstimator, TransformerMixin):
 
     """Fisher Geodesic Discriminant analysis.
 
     Project data in Tangent space, apply a FLDA to reduce dimention, and
     project filtered data back in the manifold.
     For a complete description of the algorithm, see [1]_.
 
     Parameters
     ----------
-    metric : string | dict, default='riemann'
-        The type of metric used for reference matrix estimation (see
-        `mean_covariance` for the list of supported metric) and for tangent
-        space map (see `tangent_space` for the list of supported metric).
-        The metric could be a dict with two keys, `mean` and `map` in
-        order to pass different metrics for the reference matrix estimation
-        and the tangent space mapping.
+    metric : string | dict, default="riemann"
+        The type of metric used
+        for reference matrix estimation (for the list of supported metrics
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for tangent space map
+        (see :func:`pyriemann.utils.tangent_space.tangent_space`).
+        The metric can be a dict with two keys, "mean" and "map"
+        in order to pass different metrics.
     tsupdate : bool, default=False
         Activate tangent space update for covariante shift correction between
         training and test, as described in [2]_. This is not compatible with
         online implementation. Performance are better when the number of
         matrices for prediction is higher.
 
     See Also
@@ -264,15 +250,15 @@
     .. [2] `Classification of covariance matrices using a Riemannian-based
         kernel for BCI applications
         <https://hal.archives-ouvertes.fr/hal-00820475/>`_
         A. Barachant, S. Bonnet, M. Congedo and C. Jutten. Neurocomputing,
         Elsevier, 2013, 112, pp.172-178.
     """
 
-    def __init__(self, metric='riemann', tsupdate=False):
+    def __init__(self, metric="riemann", tsupdate=False):
         """Init."""
         self.metric = metric
         self.tsupdate = tsupdate
 
     def _fit_lda(self, X, y, sample_weight=None):
         """Helper to fit LDA."""
         self.classes_ = np.unique(y)
```

### Comparing `pyriemann-0.5/pyriemann/transfer/_estimators.py` & `pyriemann-0.6/pyriemann/transfer/_estimators.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from sklearn.pipeline import Pipeline
 from sklearn.metrics import accuracy_score, r2_score
 
 from ..utils.mean import mean_covariance, mean_riemann
 from ..utils.distance import distance
 from ..utils.base import invsqrtm, powm, sqrtm
 from ..utils.geodesic import geodesic
+from ..utils.utils import check_weights, check_metric
 from ._rotate import _get_rotation_matrix
-from ..classification import MDM, _check_metric
+from ..classification import MDM
 from ..preprocessing import Whitening
 from ._tools import decode_domains
 
 
 class TLDummy(BaseEstimator, TransformerMixin):
     """No transformation on data for transfer learning.
 
@@ -99,66 +100,72 @@
        training dataset (target and source) and .transform() on the test
        partition of the target dataset.
 
     Parameters
     ----------
     target_domain : str
         Domain to consider as target.
-    metric : str, default='riemann'
-        The metric for mean, can be: 'ale', 'alm', 'euclid', 'harmonic',
-        'identity', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
-        'wasserstein', or a callable function. Note, however, that only when
-        using the 'riemann' metric that we are ensured to re-center the data
-        points precisely to the Identity.
+    metric : str, default="riemann"
+        Metric used for mean estimation. For the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`.
+        Note, however, that only when using the "riemann" metric that we are
+        ensured to re-center the data points precisely to the Identity.
 
     Attributes
     ----------
     recenter_ : dict
-        Dictionary with key=domain_name and value=domain_mean
+        Dictionary with key=domain_name and value=domain_mean.
 
     References
     ----------
     .. [1] `Transfer Learning: A Riemannian Geometry Framework With
         Applications to Brain–Computer Interfaces
         <https://hal.archives-ouvertes.fr/hal-01923278/>`_
         P Zanini et al, IEEE Transactions on Biomedical Engineering, vol. 65,
         no. 5, pp. 1107-1116, August, 2017
 
     Notes
     -----
     .. versionadded:: 0.4
     """
 
-    def __init__(self, target_domain, metric='riemann'):
+    def __init__(self, target_domain, metric="riemann"):
         """Init"""
         self.target_domain = target_domain
         self.metric = metric
 
-    def fit(self, X, y_enc):
+    def fit(self, X, y_enc, sample_weight=None):
         """Fit TLCenter.
 
         Calculate the mean of all matrices in each domain.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
         y_enc : ndarray, shape (n_matrices,)
             Extended labels for each matrix.
+        sample_weight : None | ndarray, shape (n_matrices,), default=None
+            Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         self : TLCenter instance
             The TLCenter instance.
         """
         _, _, domains = decode_domains(X, y_enc)
+        n_matrices, _, _ = X.shape
+        sample_weight = check_weights(sample_weight, n_matrices)
+
         self.recenter_ = {}
         for d in np.unique(domains):
             idx = domains == d
-            self.recenter_[d] = Whitening(metric=self.metric).fit(X[idx])
+            self.recenter_[d] = Whitening(metric=self.metric).fit(
+                X[idx], sample_weight=sample_weight[idx]
+            )
         return self
 
     def transform(self, X, y_enc=None):
         """Re-center the data points in the target domain to Identity.
 
         Parameters
         ----------
@@ -171,15 +178,15 @@
         -------
         X : ndarray, shape (n_matrices, n_classes)
             Set of SPD matrices with mean in the Identity.
         """
         # Used during inference, apply recenter from specified target domain.
         return self.recenter_[self.target_domain].transform(X)
 
-    def fit_transform(self, X, y_enc):
+    def fit_transform(self, X, y_enc, sample_weight=None):
         """Fit TLCenter and then transform data points.
 
         Calculate the mean of all matrices in each domain and then recenter
         them to Identity.
 
         .. note::
            This method is designed for using at training time. The output for
@@ -188,23 +195,26 @@
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
         y_enc : ndarray, shape (n_matrices,)
             Extended labels for each matrix.
+        sample_weight : None | ndarray, shape (n_matrices,), default=None
+            Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         X : ndarray, shape (n_matrices, n_classes)
             Set of SPD matrices with mean in the Identity.
         """
         # Used during fit, in pipeline
-        self.fit(X, y_enc)
+        self.fit(X, y_enc, sample_weight)
         _, _, domains = decode_domains(X, y_enc)
+
         X_rct = np.zeros_like(X)
         for d in np.unique(domains):
             idx = domains == d
             X_rct[idx] = self.recenter_[d].transform(X[idx])
         return X_rct
 
 
@@ -224,18 +234,18 @@
     ----------
     target_domain : str
         Domain to consider as target.
     dispersion : float, default=1.0
         Target value for the dispersion of the data points.
     centered_data : bool, default=False
         Whether the data has been re-centered to the Identity beforehand.
-    metric : str, default='riemann'
-        The metric for calculating the dispersion can be: 'ale', 'alm',
-        'euclid', 'harmonic', 'identity', 'kullback_sym', 'logdet',
-        'logeuclid', 'riemann', 'wasserstein', or a callable function.
+    metric : str, default="riemann"
+        Metric used for calculating the dispersion.
+        For the list of supported metrics,
+        see :func:`pyriemann.utils.distance.distance`.
 
     Attributes
     ----------
     dispersions_ : dict
         Dictionary with key=domain_name and value=domain_dispersion.
 
     References
@@ -248,55 +258,61 @@
 
     Notes
     -----
     .. versionadded:: 0.4
     """
 
     def __init__(self, target_domain, final_dispersion=1.0,
-                 centered_data=False, metric='riemann'):
+                 centered_data=False, metric="riemann"):
         """Init"""
         self.target_domain = target_domain
         self.final_dispersion = final_dispersion
         self.centered_data = centered_data
         self.metric = metric
 
-    def fit(self, X, y_enc):
+    def fit(self, X, y_enc, sample_weight=None):
         """Fit TLStretch.
 
         Calculate the dispersion around the mean for each domain.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
         y_enc : ndarray, shape (n_matrices,)
             Extended labels for each matrix.
+        sample_weight : None | ndarray, shape (n_matrices,), default=None
+            Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         self : TLStretch instance
             The TLStretch instance.
         """
-
         _, _, domains = decode_domains(X, y_enc)
-        n_dim = X[0].shape[1]
-        self._means = {}
-        self.dispersions_ = {}
+        n_matrices, n_channels, _ = X.shape
+        sample_weight = check_weights(sample_weight, n_matrices)
+
+        self._means, self.dispersions_ = {}, {}
         for d in np.unique(domains):
+            idx = domains == d
+            sample_weight_d = check_weights(sample_weight[idx], np.sum(idx))
             if self.centered_data:
-                self._means[d] = np.eye(n_dim)
+                self._means[d] = np.eye(n_channels)
             else:
-                self._means[d] = mean_riemann(X[domains == d])
-            disp_domain = distance(
-                X[domains == d],
+                self._means[d] = mean_riemann(
+                    X[idx], sample_weight=sample_weight_d
+                )
+            dist = distance(
+                X[idx],
                 self._means[d],
                 metric=self.metric,
                 squared=True,
-            ).sum()
-            self.dispersions_[d] = disp_domain
+            )
+            self.dispersions_[d] = np.sum(sample_weight_d * np.squeeze(dist))
 
         return self
 
     def _center(self, X, mean):
         Mean_isqrt = invsqrtm(mean)
         return Mean_isqrt @ X @ Mean_isqrt
 
@@ -338,15 +354,15 @@
 
         if not self.centered_data:
             # re-center back to previous mean
             X_str = self._uncenter(X_str, self._means[self.target_domain])
 
         return X_str
 
-    def fit_transform(self, X, y_enc):
+    def fit_transform(self, X, y_enc, sample_weight=None):
         """Fit TLStretch and then transform data points.
 
         Calculate the dispersion around the mean for each domain and then
         stretch the data points to the desired final dispersion.
 
         .. note::
            This method is designed for using at training time. The output for
@@ -355,24 +371,27 @@
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
         y_enc : ndarray, shape (n_matrices,)
             Extended labels for each matrix.
+        sample_weight : None | ndarray, shape (n_matrices,), default=None
+            Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         X : ndarray, shape (n_matrices, n_classes)
             Set of SPD matrices with desired final dispersion.
         """
 
         # used during fit, in pipeline
-        self.fit(X, y_enc)
+        self.fit(X, y_enc, sample_weight)
         _, _, domains = decode_domains(X, y_enc)
+
         X_str = np.zeros_like(X)
         for d in np.unique(domains):
             idx = domains == d
 
             if not self.centered_data:
                 # re-center matrices to Identity
                 X[idx] = self._center(X[idx], self._means[d])
@@ -410,17 +429,16 @@
     Parameters
     ----------
     target_domain : str
         Domain to consider as target.
     weights : None | array, shape (n_classes,), default=None
         Weights to assign for each class. If None, then give the same weight
         for each class.
-    metric : {'euclid', 'riemann'}, default='euclid'
-        Metric for the distance to minimize between class means. Options are
-        either the Euclidean ('euclid') or Riemannian ('riemann') distance.
+    metric : {"euclid", "riemann"}, default="euclid"
+        Metric for the distance to minimize between class means.
     n_jobs : int, default=1
         The number of jobs to use for the computation. This works by computing
         the rotation matrix for each source domain in parallel. If -1 all CPUs
         are used.
 
     Attributes
     ----------
@@ -446,58 +464,68 @@
     def __init__(self, target_domain, weights=None, metric='euclid', n_jobs=1):
         """Init"""
         self.target_domain = target_domain
         self.weights = weights
         self.metric = metric
         self.n_jobs = n_jobs
 
-    def fit(self, X, y_enc):
+    def fit(self, X, y_enc, sample_weight=None):
         """Fit TLRotate.
 
         Calculate the rotations matrices to transform each source domain into
         the target domain.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
         y_enc : ndarray, shape (n_matrices,)
             Extended labels for each matrix.
+        sample_weight : None | ndarray, shape (n_matrices,), default=None
+            Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         self : TLRotate instance
             The TLRotate instance.
         """
 
         _, _, domains = decode_domains(X, y_enc)
+        n_matrices, _, _ = X.shape
+        sample_weight = check_weights(sample_weight, n_matrices)
 
         idx = domains == self.target_domain
         X_target, y_target = X[idx], y_enc[idx]
         M_target = np.stack([
-            mean_riemann(X_target[y_target == label])
+            mean_riemann(X_target[y_target == label],
+                         sample_weight=sample_weight[idx][y_target == label])
             for label in np.unique(y_target)
         ])
 
-        source_names = np.unique(domains)
-        source_names = source_names[source_names != self.target_domain]
+        source_domains = np.unique(domains)
+        source_domains = source_domains[source_domains != self.target_domain]
         rotations = Parallel(n_jobs=self.n_jobs)(
             delayed(_get_rotation_matrix)(
                 np.stack([
-                    mean_riemann(X[domains == d][y_enc[domains == d] == label])
-                    for label in np.unique(y_enc[domains == d])
+                    mean_riemann(
+                        X[domains == d][y_enc[domains == d] == label],
+                        sample_weight=sample_weight[domains == d][
+                            y_enc[domains == d] == label
+                        ]
+                    ) for label in np.unique(y_enc[domains == d])
                 ]),
                 M_target,
                 self.weights,
                 metric=self.metric,
-            ) for d in source_names
+            ) for d in source_domains
         )
+
         self.rotations_ = {}
-        for di, roti in zip(source_names, rotations):
-            self.rotations_[di] = roti
+        for d, rot in zip(source_domains, rotations):
+            self.rotations_[d] = rot
 
         return self
 
     def transform(self, X, y_enc=None):
         """Rotate the data points in the target domain.
 
         The rotations are done from source to target, so in this step the data
@@ -515,15 +543,15 @@
         X : ndarray, shape (n_matrices, n_classes)
             Same set of SPD matrices as in the input.
         """
 
         # used during inference on target domain
         return X
 
-    def fit_transform(self, X, y_enc):
+    def fit_transform(self, X, y_enc, sample_weight=None):
         """Fit TLRotate and then transform data points.
 
         Calculate the rotation matrix for matching each source domain to the
         target domain.
 
         .. note::
            This method is designed for using at training time. The output for
@@ -532,24 +560,27 @@
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
         y_enc : ndarray, shape (n_matrices,)
             Extended labels for each matrix.
+        sample_weight : None | ndarray, shape (n_matrices,), default=None
+            Weights for each matrix. If None, it uses equal weights.
 
         Returns
         -------
         X : ndarray, shape (n_matrices, n_classes)
             Set of SPD matrices after rotation step.
         """
 
         # used during fit in pipeline, rotate each source domain
-        self.fit(X, y_enc)
+        self.fit(X, y_enc, sample_weight)
         _, _, domains = decode_domains(X, y_enc)
+
         X_rot = np.zeros_like(X)
         for d in np.unique(domains):
             idx = domains == d
             if d != self.target_domain:
                 X_rot[idx] = self.rotations_[d] @ X[idx] @ self.rotations_[d].T
             else:
                 X_rot[idx] = X[idx]
@@ -597,16 +628,15 @@
             Extended labels for each matrix.
 
         Returns
         -------
         self : TLEstimator instance
             The TLEstimator instance.
         """
-        if not is_regressor(self.estimator) \
-                and not is_classifier(self.estimator):
+        if not (is_regressor(self.estimator) or is_classifier(self.estimator)):
             raise TypeError(
                 'Estimator has to be either a classifier or a regressor.')
 
         X_dec, y_dec, domains = decode_domains(X, y_enc)
 
         if is_regressor(self.estimator):
             y_dec = y_dec.astype(float)
@@ -801,36 +831,34 @@
         source and target domains.
         At 0, there is no transfer, only matrices acquired from the source
         domain are used.
         At 1, this is a calibration-free system as no matrices are required
         from the source domain.
     target_domain : string
         Name of the target domain in extended labels.
-    metric : string | dict, default='riemann'
-        The type of metric used for centroid and distance estimation.
-        see `mean_covariance` for the list of supported metric.
-        the metric could be a dict with two keys, `mean` and `distance` in
-        order to pass different metric for the centroid estimation and the
-        distance estimation. Typical usecase is to pass 'logeuclid' metric for
-        the mean in order to boost the computional speed and 'riemann' for the
-        distance in order to keep the good sensitivity for the classification.
+    metric : string | dict, default="riemann"
+        Metric used for mean estimation (for the list of supported metrics,
+        see :func:`pyriemann.utils.mean.mean_covariance`) and
+        for distance estimation
+        (see :func:`pyriemann.utils.distance.distance`).
+        The metric can be a dict with two keys, "mean" and "distance"
+        in order to pass different metrics.
     n_jobs : int, default=1
         The number of jobs to use for the computation. This works by computing
         each of the class centroid in parallel.
         If -1 all CPUs are used. If 1 is given, no parallel computing code is
         used at all, which is useful for debugging. For n_jobs below -1,
         (n_cpus + 1 + n_jobs) are used. Thus for n_jobs = -2, all CPUs but one
         are used.
 
     Attributes
     ----------
     classes_ : ndarray, shape (n_classes,)
         Labels for each class.
-    covmeans_ : list of ``n_classes`` ndarrays of shape (n_channels, \
-            n_channels)
+    covmeans_ : ndarray, shape (n_classes, n_channels, n_channels)
         Centroids for each class.
 
     See Also
     --------
     MDM
 
     References
@@ -852,15 +880,15 @@
     .. versionadded:: 0.4
     """
 
     def __init__(
             self,
             domain_tradeoff,
             target_domain,
-            metric='riemann',
+            metric="riemann",
             n_jobs=1):
         """Init."""
         self.domain_tradeoff = domain_tradeoff
         self.target_domain = target_domain
         self.metric = metric
         self.n_jobs = n_jobs
 
@@ -879,43 +907,37 @@
             If None, it uses equal weights.
 
         Returns
         -------
         self : MDWM instance
             The MDWM instance.
         """
-        self.metric_mean, self.metric_dist = _check_metric(self.metric)
+        self.metric_mean, self.metric_dist = check_metric(self.metric)
 
         if not 0 <= self.domain_tradeoff <= 1:
             raise ValueError(
-                'Value domain_tradeoff must be included in [0, 1] (Got %d)'
+                "Value domain_tradeoff must be included in [0, 1] (Got %d)"
                 % self.domain_tradeoff)
 
         X_dec, y_dec, domains = decode_domains(X, y_enc)
         X_src = X_dec[domains != self.target_domain]
         y_src = y_dec[domains != self.target_domain]
         X_tgt = X_dec[domains == self.target_domain]
         y_tgt = y_dec[domains == self.target_domain]
 
         self.classes_ = np.unique(y_src)
 
-        if self.domain_tradeoff != 0:
-            if set(y_tgt) != set(y_src):
-                raise ValueError(
-                    f"classes in source domain must match classes in target \
-                    domain. Classes in source are {self.classes_} while \
-                    classes in target are {np.unique(y_tgt)}")
-
-        if sample_weight is not None:
-            if (sample_weight.shape != (X_src.shape[0], 1)) and \
-                                (sample_weight.shape != (X_src.shape[0],)):
-                raise ValueError("Parameter sample_weight should either be \
-                    None or an ndarray shape (n_matrices, 1)")
-        else:
-            sample_weight = np.ones(X_src.shape[0])
+        if self.domain_tradeoff != 0 and set(y_tgt) != set(y_src):
+            raise ValueError(
+                "Classes in source domain must match classes in target domain."
+                f"Classes in source are {self.classes_} while classes in "
+                f"target are {np.unique(y_tgt)}"
+            )
+
+        sample_weight = check_weights(sample_weight, X_src.shape[0])
 
         self.source_means_ = np.stack(
             Parallel(n_jobs=self.n_jobs)(
                 delayed(mean_covariance)(
                     X_src[y_src == ll],
                     metric=self.metric_mean,
                     sample_weight=sample_weight[y_src == ll],
```

### Comparing `pyriemann-0.5/pyriemann/transfer/_rotate.py` & `pyriemann-0.6/pyriemann/transfer/_rotate.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/transfer/_tools.py` & `pyriemann-0.6/pyriemann/transfer/_tools.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/utils/__init__.py` & `pyriemann-0.6/pyriemann/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/utils/ajd.py` & `pyriemann-0.6/pyriemann/utils/ajd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 """Aproximate joint diagonalization algorithms."""
 
 import numpy as np
-from .utils import check_weights
+import warnings
+
+from .utils import check_weights, check_function
 
 
 def _check_init_diag(init, n):
     if init.shape != (n, n):
         raise ValueError(
-            'Initial diagonalizer shape must be %d x % d (Got %s).'
+            "Initial diagonalizer shape must be %d x % d (Got %s)."
             % (n, n, init.shape,))
     return init
 
 
-def rjd(X, *, init=None, eps=1e-8, n_iter_max=1000):
-    """Approximate joint diagonalization based on Jacobi angles.
+def rjd(X, *, init=None, eps=1e-8, n_iter_max=100):
+    """Approximate joint diagonalization based on JADE.
 
-    This is a direct implementation of the AJD algorithm by Cardoso and
-    Souloumiac [1]_ used in JADE. The code is a translation of the Matlab code
-    provided in the author website.
+    This is an implementation of the orthogonal AJD algorithm [1]_: joint
+    approximate diagonalization of eigen-matrices (JADE), based on Jacobi
+    angles.
+    The code is a translation of the Matlab code provided on the author's
+    website.
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices, n_channels, n_channels)
+    X : ndarray, shape (n_matrices, n, n)
         Set of symmetric matrices to diagonalize.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
+    init : None | ndarray, shape (n, n), default=None
         Initialization for the diagonalizer.
     eps : float, default=1e-8
         Tolerance for stopping criterion.
-    n_iter_max : int, default=1000
+    n_iter_max : int, default=100
         The maximum number of iterations to reach convergence.
 
     Returns
     -------
-    V : ndarray, shape (n_channels, n_channels)
+    V : ndarray, shape (n, n)
         The diagonalizer, an orthogonal matrix.
-    D : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of quasi diagonal matrices.
+    D : ndarray, shape (n_matrices, n, n)
+        Set of quasi diagonal matrices, D = V^T X V.
 
     Notes
     -----
     .. versionadded:: 0.2.4
 
     See Also
     --------
-    ajd_pham
-    uwedge
+    ajd
 
     References
     ----------
     .. [1] `Jacobi angles for simultaneous diagonalization
         <https://epubs.siam.org/doi/abs/10.1137/S0895479893259546>`_
         J.-F. Cardoso and A. Souloumiac, SIAM Journal on Matrix Analysis and
-        Applications, Volume 17, Issue 1, Jan. 1996.
+        Applications, 17(1), pp. 161–164, 1996.
     """
-
+    n_matrices, _, _ = X.shape
     # reshape input matrix
     A = np.concatenate(X, 0).T
+    n, n_matrices_x_n = A.shape
 
     # init variables
-    m, nm = A.shape  # n_channels, n_matrices_x_channels
     if init is None:
-        V = np.eye(m)
+        V = np.eye(n)
     else:
-        V = _check_init_diag(init, m)
+        V = _check_init_diag(init, n)
     encore = True
     k = 0
 
     while encore:
         encore = False
         k += 1
         if k > n_iter_max:
             break
-        for p in range(m - 1):
-            for q in range(p + 1, m):
+        for p in range(n - 1):
+            for q in range(p + 1, n):
 
-                Ip = np.arange(p, nm, m)
-                Iq = np.arange(q, nm, m)
+                Ip = np.arange(p, n_matrices_x_n, n)
+                Iq = np.arange(q, n_matrices_x_n, n)
 
                 # computation of Givens angle
                 g = np.array([A[p, Ip] - A[q, Iq], A[p, Iq] + A[q, Ip]])
-                gg = np.dot(g, g.T)
+                gg = g @ g.T
                 ton = gg[0, 0] - gg[1, 1]
                 toff = gg[0, 1] + gg[1, 0]
                 theta = 0.5 * np.arctan2(
                     toff, ton + np.sqrt(ton * ton + toff * toff))
                 c = np.cos(theta)
                 s = np.sin(theta)
                 encore = encore | (np.abs(s) > eps)
@@ -96,85 +99,85 @@
                     A[p, :] = c * A[p, :] + s * A[q, :]
                     A[q, :] = c * A[q, :] - s * tmp
 
                     tmp = V[:, p].copy()
                     V[:, p] = c * V[:, p] + s * V[:, q]
                     V[:, q] = c * V[:, q] - s * tmp
 
-    D = np.reshape(A, (m, int(nm / m), m)).transpose(1, 0, 2)
+    D = np.reshape(A, (n, n_matrices, n)).transpose(1, 0, 2)
     return V, D
 
 
-def ajd_pham(X, *, init=None, eps=1e-6, n_iter_max=15, sample_weight=None):
+def ajd_pham(X, *, init=None, eps=1e-6, n_iter_max=20, sample_weight=None):
     """Approximate joint diagonalization based on Pham's algorithm.
 
-    This is a direct implementation of the Pham's AJD algorithm [1]_.
+    This is a direct implementation of the AJD algorithm [1]_, optimizing a
+    log-likelihood criterion based on the Kullback-Leibler divergence.
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices, n_channels, n_channels)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD matrices to diagonalize.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
+    init : None | ndarray, shape (n, n), default=None
         Initialization for the diagonalizer.
     eps : float, default=1e-6
         Tolerance for stoping criterion.
-    n_iter_max : int, default=15
+    n_iter_max : int, default=20
         The maximum number of iterations to reach convergence.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix, strictly positive.
         If None, it uses equal weights.
 
     Returns
     -------
-    V : ndarray, shape (n_channels, n_channels)
+    V : ndarray, shape (n, n)
         The diagonalizer, an invertible matrix.
-    D : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of quasi diagonal matrices.
+    D : ndarray, shape (n_matrices, n, n)
+        Set of quasi diagonal matrices, D = V X V^T.
 
     Notes
     -----
     .. versionadded:: 0.2.4
 
     See Also
     --------
-    rjd
-    uwedge
+    ajd
 
     References
     ----------
     .. [1] `Joint approximate diagonalization of positive definite
         Hermitian matrices
         <https://epubs.siam.org/doi/10.1137/S089547980035689X>`_
-        D.-T. Pham. SIAM Journal on Matrix Analysis and Applications, Volume 22
-        Issue 4, 2000
+        D.-T. Pham. SIAM Journal on Matrix Analysis and Applications, 22(4),
+        pp. 1136-1152, 2000.
     """
     n_matrices, _, _ = X.shape
     normalized_weight = check_weights(
         sample_weight,
         n_matrices,
         check_positivity=True,
     )  # sum = 1
 
-    # Reshape input matrix
+    # reshape input matrix
     A = np.concatenate(X, axis=0).T
+    n, n_matrices_x_n = A.shape
 
-    # Init variables
-    n_channels, n_matrices_x_channels = A.shape
+    # init variables
     if init is None:
-        V = np.eye(n_channels)
+        V = np.eye(n)
     else:
-        V = _check_init_diag(init, n_channels)
-    epsilon = n_channels * (n_channels - 1) * eps
+        V = _check_init_diag(init, n)
+    epsilon = n * (n - 1) * eps
 
-    for it in range(n_iter_max):
+    for _ in range(n_iter_max):
         decr = 0
-        for ii in range(1, n_channels):
+        for ii in range(1, n):
             for jj in range(ii):
-                Ii = np.arange(ii, n_matrices_x_channels, n_channels)
-                Ij = np.arange(jj, n_matrices_x_channels, n_channels)
+                Ii = np.arange(ii, n_matrices_x_n, n)
+                Ij = np.arange(jj, n_matrices_x_n, n)
 
                 c1 = A[ii, Ii]
                 c2 = A[jj, Ij]
 
                 g12 = np.average(A[ii, Ij] / c1, weights=normalized_weight)
                 g21 = np.average(A[ii, Ij] / c2, weights=normalized_weight)
 
@@ -187,128 +190,196 @@
                 tmp2 = (tmp * g12 - g21) / max(omega - 1, 1e-9)
 
                 h12 = tmp1 + tmp2
                 h21 = np.conj((tmp1 - tmp2) / tmp)
 
                 decr += n_matrices * (g12 * np.conj(h12) + g21 * h21) / 2.0
 
-                tmp = 1 + 1.j * 0.5 * np.imag(h12 * h21)
+                tmp = 1 + 0.5j * np.imag(h12 * h21)
                 tmp = np.real(tmp + np.sqrt(tmp ** 2 - h12 * h21))
                 tau = np.array([[1, -h12 / tmp], [-h21 / tmp, 1]])
 
-                A[[ii, jj], :] = np.dot(tau, A[[ii, jj], :])
+                A[[ii, jj], :] = tau @ A[[ii, jj], :]
                 tmp = np.c_[A[:, Ii], A[:, Ij]]
-                tmp = np.reshape(tmp, (n_channels * n_matrices, 2), order='F')
-                tmp = np.dot(tmp, tau.T)
+                tmp = np.reshape(tmp, (n * n_matrices, 2), order='F')
+                tmp = tmp @ tau.T
 
-                tmp = np.reshape(tmp, (n_channels, n_matrices * 2), order='F')
+                tmp = np.reshape(tmp, (n, n_matrices * 2), order='F')
                 A[:, Ii] = tmp[:, :n_matrices]
                 A[:, Ij] = tmp[:, n_matrices:]
-                V[[ii, jj], :] = np.dot(tau, V[[ii, jj], :])
+                V[[ii, jj], :] = tau @ V[[ii, jj], :]
         if decr < epsilon:
             break
-    D = np.reshape(A, (n_channels, -1, n_channels)).transpose(1, 0, 2)
+    else:
+        warnings.warn("Convergence not reached")
+
+    D = np.reshape(A, (n, -1, n)).transpose(1, 0, 2)
     return V, D
 
 
 def uwedge(X, *, init=None, eps=1e-7, n_iter_max=100):
     """Approximate joint diagonalization based on UWEDGE.
 
-    Implementation of the AJD algorithm by Tichavsky and Yeredor [1]_ [2]_:
-    uniformly weighted exhaustive diagonalization using Gauss iterations
-    (U-WEDGE). This is a translation from the matlab code provided by the
-    authors.
+    This is an implementation of the AJD algorithm [1]_ [2]_: uniformly
+    weighted exhaustive diagonalization using Gauss iterations (U-WEDGE).
+    It is a translation from the Matlab code provided by the authors.
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices, n_channels, n_channels)
+    X : ndarray, shape (n_matrices, n, n)
         Set of symmetric matrices to diagonalize.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
+    init : None | ndarray, shape (n, n), default=None
         Initialization for the diagonalizer.
     eps : float, default=1e-7
         Tolerance for stoping criterion.
     n_iter_max : int, default=100
         The maximum number of iterations to reach convergence.
 
     Returns
     -------
-    V : ndarray, shape (n_channels, n_channels)
+    V : ndarray, shape (n, n)
         The diagonalizer.
-    D : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of quasi diagonal matrices.
+    D : ndarray, shape (n_matrices, n, n)
+        Set of quasi diagonal matrices, D = V X V^T.
 
     Notes
     -----
     .. versionadded:: 0.2.4
 
     See Also
     --------
-    ajd_pham
-    rjd
+    ajd
 
     References
     ----------
     .. [1] `A Fast Approximate Joint Diagonalization Algorithm Using a
         Criterion with a Block Diagonal Weight Matrix
         <https://ieeexplore.ieee.org/abstract/document/4518361>`_
         P. Tichavsky, A. Yeredor and J. Nielsen. 2008 IEEE International
-        Conference on Acoustics, Speech and Signal ProcessingICASSP.
+        Conference on Acoustics, Speech and Signal Processing ICASSP.
     .. [2] `Fast Approximate Joint Diagonalization Incorporating Weight
         Matrices
         <https://ieeexplore.ieee.org/document/4671095>`_
-        P. Tichavsky and A. Yeredor. IEEE Transactions on Signal Processing,
-        Volume 57, Issue 3, March 2009.
+        P. Tichavsky and A. Yeredor. IEEE Trans Signal Process, 57(3), pp.
+        878 - 891, 2009.
     """
-    n_matrices, d, _ = X.shape
+    n_matrices, _, _ = X.shape
     # reshape input matrix
     M = np.concatenate(X, 0).T
+    n, n_matrices_x_n = M.shape
 
     # init variables
-    d, Md = M.shape  # n_channels, n_matrices_x_channels
     iteration = 0
     improve = 10
-
     if init is None:
-        E, H = np.linalg.eig(M[:, 0:d])
-        W_est = H.T / np.sqrt(np.abs(E))[:, np.newaxis]
+        E, H = np.linalg.eig(M[:, 0:n])
+        V = H.T / np.sqrt(np.abs(E))[:, np.newaxis]
     else:
-        W_est = _check_init_diag(init, d)
+        V = _check_init_diag(init, n)
 
     Ms = np.array(M)
-    Rs = np.zeros((d, n_matrices))
+    Rs = np.zeros((n, n_matrices))
 
     for k in range(n_matrices):
-        ini = k*d
-        Il = np.arange(ini, ini + d)
-        M[:, Il] = 0.5*(M[:, Il] + M[:, Il].T)
-        Ms[:, Il] = np.dot(np.dot(W_est, M[:, Il]), W_est.T)
+        ini = k * n
+        Il = np.arange(ini, ini + n)
+        M[:, Il] = 0.5 * (M[:, Il] + M[:, Il].T)
+        Ms[:, Il] = V @ M[:, Il] @ V.T
         Rs[:, k] = np.diag(Ms[:, Il])
 
-    crit = np.sum(Ms**2) - np.sum(Rs**2)
+    crit = np.sum(Ms ** 2) - np.sum(Rs ** 2)
     while (improve > eps) & (iteration < n_iter_max):
         B = Rs @ Rs.T
-        C1 = np.zeros((d, d))
-        for i in range(d):
-            C1[:, i] = np.sum(Ms[:, i:Md:d]*Rs, axis=1)
+        C1 = np.zeros((n, n))
+        for i in range(n):
+            C1[:, i] = np.sum(Ms[:, i:n_matrices_x_n:n] * Rs, axis=1)
 
         D0 = B * B.T - np.outer(np.diag(B), np.diag(B))
-        A0 = (C1 * B - np.diag(np.diag(B)) @ C1.T) / (D0 + np.eye(d))
-        A0 += np.eye(d)
-        W_est = np.linalg.solve(A0, W_est)
+        A0 = (C1 * B - np.diag(B)[:, np.newaxis] * C1.T) / (D0 + np.eye(n))
+        A0.flat[:: n + 1] += 1
+        V = np.linalg.solve(A0, V)
 
-        Raux = np.dot(np.dot(W_est, M[:, 0:d]), W_est.T)
+        Raux = V @ M[:, 0:n] @ V.T
         aux = 1. / np.sqrt(np.abs(np.diag(Raux)))
-        W_est = np.diag(aux) @ W_est
+        V = aux[:, np.newaxis] * V
 
         for k in range(n_matrices):
-            ini = k*d
-            Il = np.arange(ini, ini + d)
-            Ms[:, Il] = np.dot(np.dot(W_est, M[:, Il]), W_est.T)
+            ini = k * n
+            Il = np.arange(ini, ini + n)
+            Ms[:, Il] = V @ M[:, Il] @ V.T
             Rs[:, k] = np.diag(Ms[:, Il])
 
-        crit_new = np.sum(Ms**2) - np.sum(Rs**2)
+        crit_new = np.sum(Ms ** 2) - np.sum(Rs ** 2)
         improve = np.abs(crit_new - crit)
         crit = crit_new
         iteration += 1
 
-    D = np.reshape(Ms, (d, n_matrices, d)).transpose(1, 0, 2)
-    return W_est, D
+    D = np.reshape(Ms, (n, n_matrices, n)).transpose(1, 0, 2)
+    return V, D
+
+
+###############################################################################
+
+
+ajd_functions = {
+    "ajd_pham": ajd_pham,
+    "rjd": rjd,
+    "uwedge": uwedge,
+}
+
+
+def ajd(X, method="ajd_pham", init=None, eps=1e-6, n_iter_max=100, **kwargs):
+    """Aproximate joint diagonalization (AJD) according to a method.
+
+    Compute the AJD of a set of matrices according to a method [1]_, estimating
+    the joint diagonalizer matrix, diagonalizing the set as much as possible.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices, n, n)
+        Set of symmetric matrices to diagonalize.
+    method : string | callable, default="ajd_pham"
+        Method for AJD, can be: "ajd_pham", "rjd", "uwedge", or a callable
+        function.
+    init : None | ndarray, shape (n, n), default=None
+        Initialization for the diagonalizer.
+    eps : float, default=1e-6
+        Tolerance for stopping criterion.
+    n_iter_max : int, default=100
+        The maximum number of iterations to reach convergence.
+    kwargs : dict
+        The keyword arguments passed to the sub function.
+
+    Returns
+    -------
+    V : ndarray, shape (n, n)
+        The diagonalizer.
+    D : ndarray, shape (n_matrices, n, n)
+        Set of quasi diagonal matrices.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+
+    See Also
+    --------
+    ajd_pham
+    rjd
+    uwedge
+
+    References
+    ----------
+    .. [1] `Joint Matrices Decompositions and Blind Source Separation: A survey
+        of methods, identification, and applications
+        <http://library.utia.cas.cz/separaty/2014/SI/tichavsky-0427607.pdf>`_
+        G. Chabriel, M. Kleinsteuber, E. Moreau, H. Shen; P. Tichavsky and A.
+        Yeredor. IEEE Signal Process Mag, 31(3), pp. 34-43, 2014.
+    """
+    ajd_function = check_function(method, ajd_functions)
+    V, D = ajd_function(
+        X,
+        init=init,
+        eps=eps,
+        n_iter_max=n_iter_max,
+        **kwargs,
+    )
+    return V, D
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyriemann-0.5/pyriemann/utils/base.py` & `pyriemann-0.6/pyriemann/utils/base.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/utils/covariance.py` & `pyriemann-0.6/pyriemann/utils/covariance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,85 @@
 import warnings
+from functools import wraps
 
 import numpy as np
 from scipy.linalg import block_diag
 from scipy.stats import chi2
-from sklearn.covariance import oas, ledoit_wolf, fast_mcd, empirical_covariance
+from sklearn.covariance import oas, ledoit_wolf, fast_mcd
 
 from .distance import distance_mahalanobis
-from .test import is_square
+from .test import is_square, is_real_type
+from .utils import check_function
 
 
+def _complex_estimator(func):
+    """Decorator to extend a real-valued covariance estimator to complex data.
+
+    Applied to a real-valued covariance estimator, this decorator allows to
+    estimate complex covariance matrices from complex-valued multi-channel
+    time-series. See Eq.(4) in [1]_.
+
+    Parameters
+    ----------
+    func : callable
+        Real-valued covariance estimator.
+
+    Returns
+    -------
+    output : callable
+        Complex-valued covariance estimator.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+
+    References
+    ----------
+    .. [1] `Enhanced Covariance Matrix Estimators in Adaptive Beamforming
+        <https://doi.org/10.1109/ICASSP.2007.366399>`_
+        R. Abrahamsson, Y. Selen and P. Stoica. 2007 IEEE International
+        Conference on Acoustics, Speech and Signal Processing, Volume 2, 2007.
+    """
+    @wraps(func)
+    def wrapper(X, **kwds):
+        iscomplex = np.iscomplexobj(X)
+        if iscomplex:
+            n_channels, n_times = X.shape
+            X = np.concatenate((X.real, X.imag), axis=0)
+        cov = func(X, **kwds)
+        if iscomplex:
+            cov = cov[:n_channels, :n_channels] \
+                + cov[n_channels:, n_channels:] \
+                + 1j * (cov[n_channels:, :n_channels]
+                        - cov[:n_channels, n_channels:])
+        return cov
+    return wrapper
+
+
+@_complex_estimator
 def _lwf(X, **kwds):
     """Wrapper for sklearn ledoit wolf covariance estimator"""
     C, _ = ledoit_wolf(X.T, **kwds)
     return C
 
 
+@_complex_estimator
 def _mcd(X, **kwds):
     """Wrapper for sklearn mcd covariance estimator"""
     _, C, _, _ = fast_mcd(X.T, **kwds)
     return C
 
 
+@_complex_estimator
 def _oas(X, **kwds):
     """Wrapper for sklearn oas covariance estimator"""
     C, _ = oas(X.T, **kwds)
     return C
 
 
-def _scm(X, **kwds):
-    """Wrapper for sklearn sample covariance estimator"""
-    return empirical_covariance(X.T, **kwds)
-
-
 def _hub(X, **kwds):
     """Wrapper for Huber's M-estimator"""
     return covariance_mest(X, 'hub', **kwds)
 
 
 def _stu(X, **kwds):
     """Wrapper for Student-t's M-estimator"""
@@ -64,20 +108,20 @@
     Mahalanobis distance depending on the M-estimator type: Huber, Student-t or
     Tyler.
 
     Parameters
     ----------
     X : ndarray, shape (n_channels, n_times)
         Multi-channel time-series, real or complex-valued.
-    m_estimator : {'hub', 'stu', 'tyl'}
+    m_estimator : {"hub", "stu", "tyl"}
         Type of M-estimator:
 
-        - 'hub' for Huber's M-estimator [2]_;
-        - 'stu' for Student-t's M-estimator [3]_;
-        - 'tyl' for Tyler's M-estimator [4]_.
+        - "hub" for Huber's M-estimator [2]_;
+        - "stu" for Student-t's M-estimator [3]_;
+        - "tyl" for Tyler's M-estimator [4]_.
     init : None | ndarray, shape (n_channels, n_channels), default=None
         A matrix used to initialize the algorithm.
         If None, the sample covariance matrix is used.
     tol : float, default=10e-3
         The tolerance to stop the fixed point estimation.
     n_iter_max : int, default=50
         The maximum number of iterations.
@@ -156,15 +200,15 @@
     if init is None:
         cov = X @ X.conj().T / n_times
     else:
         cov = init
 
     for _ in range(n_iter_max):
 
-        dist2 = distance_mahalanobis(X, cov) ** 2
+        dist2 = distance_mahalanobis(X, cov, squared=True)
         Xw = np.sqrt(weight_func(dist2)) * X
         cov_new = Xw @ Xw.conj().T / n_times
 
         norm_delta = np.linalg.norm(cov_new - cov, ord='fro')
         norm_cov = np.linalg.norm(cov, ord='fro')
         cov = cov_new
         if (norm_delta / norm_cov) <= tol:
@@ -176,14 +220,15 @@
         cov = normalize(cov, norm)
         if norm == "trace":
             cov *= n_channels
 
     return cov
 
 
+@_complex_estimator
 def covariance_sch(X):
     r"""Schaefer-Strimmer shrunk covariance estimator.
 
     Shrinkage covariance estimator [1]_:
 
     .. math::
         C = (1 - \gamma) C_\text{scm} + \gamma T
@@ -194,15 +239,15 @@
         T[i,j] = \{ C_\text{scm}[i,i] \ \text{if} i = j, 0 \text{otherwise} \}
 
     Note that the optimal :math:`\gamma` is estimated by the authors' method.
 
     Parameters
     ----------
     X : ndarray, shape (n_channels, n_times)
-        Multi-channel time-series.
+        Multi-channel time-series, real-valued.
 
     Returns
     -------
     cov : ndarray, shape (n_channels, n_channels)
         Schaefer-Strimmer shrunk covariance matrix.
 
     Notes
@@ -215,15 +260,15 @@
         implications for functional genomics
         <http://doi.org/10.2202/1544-6115.1175>`_
         J. Schafer, and K. Strimmer. Statistical Applications in Genetics and
         Molecular Biology, Volume 4, Issue 1, 2005.
     """
     _, n_times = X.shape
     X_c = X - X.mean(axis=1, keepdims=True)
-    C_scm = 1. / n_times * X_c @ X_c.T
+    C_scm = X_c @ X_c.T / n_times
 
     # Compute optimal gamma, the weigthing between SCM and shrinkage estimator
     R = (n_times / ((n_times - 1.) * np.outer(X.std(axis=1), X.std(axis=1))))
     R *= C_scm
     var_R = (X_c ** 2) @ (X_c ** 2).T - 2 * C_scm * (X_c @ X_c.T)
     var_R += n_times * C_scm ** 2
     Xvar = np.outer(X.var(axis=1), X.var(axis=1))
@@ -233,76 +278,102 @@
     gamma = max(0, min(1, var_R.sum() / (R ** 2).sum()))
 
     sigma = (1. - gamma) * (n_times / (n_times - 1.)) * C_scm
     shrinkage = gamma * (n_times / (n_times - 1.)) * np.diag(np.diag(C_scm))
     return sigma + shrinkage
 
 
-def _check_est(est):
-    """Check if a given estimator is valid."""
+def covariance_scm(X, *, assume_centered=False):
+    """Sample covariance estimator.
 
-    # Check estimator exist and return the correct function
-    estimators = {
-        'corr': np.corrcoef,
-        'cov': np.cov,
-        'hub': _hub,
-        'lwf': _lwf,
-        'mcd': _mcd,
-        'oas': _oas,
-        'scm': _scm,
-        'sch': covariance_sch,
-        'stu': _stu,
-        'tyl': _tyl,
-    }
-
-    if callable(est):
-        # All good (cross your fingers)
-        pass
-    elif est in estimators.keys():
-        # Map the corresponding estimator
-        est = estimators[est]
+    Sample covariance estimator, re-implementing `empirical_covariance` of
+    scikit-learn [1]_, but supporting real and complex-valued data.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_channels, n_times)
+        Multi-channel time-series, real or complex-valued.
+    assume_centered : bool, default=False
+        If `True`, data will not be centered before computation.
+        Useful when working with data whose mean is almost, but not exactly
+        zero.
+        If `False`, data will be centered before computation.
+
+    Returns
+    -------
+    cov : ndarray, shape (n_channels, n_channels)
+        Sample covariance matrix.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+
+    References
+    ----------
+    .. [1] https://scikit-learn.org/stable/modules/generated/sklearn.covariance.empirical_covariance.html
+    """  # noqa
+    _, n_times = X.shape
+
+    if assume_centered:
+        cov = X @ X.conj().T / n_times
     else:
-        # raise an error
-        raise ValueError(
-            """%s is not an valid estimator ! Valid estimators are : %s or a
-             callable function""" % (est, (' , ').join(estimators.keys())))
-    return est
+        cov = np.cov(X, bias=1)
+
+    return cov
 
 
-def covariances(X, estimator='cov', **kwds):
-    """Estimation of covariance matrix.
+###############################################################################
+
+
+cov_est_functions = {
+    "corr": np.corrcoef,
+    "cov": np.cov,
+    "hub": _hub,
+    "lwf": _lwf,
+    "mcd": _mcd,
+    "oas": _oas,
+    "sch": covariance_sch,
+    "scm": covariance_scm,
+    "stu": _stu,
+    "tyl": _tyl,
+}
+
+
+def covariances(X, estimator="cov", **kwds):
+    """Estimation of covariance matrices.
+
+    Estimates covariance matrices from multi-channel time-series according to
+    a covariance estimator. It supports real and complex-valued data.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_times)
-        Multi-channel time-series.
-    estimator : {'corr', 'cov', 'hub', 'lwf', 'mcd', 'oas', 'sch', 'scm', \
-            'stu', 'tyl'}, default='scm'
+        Multi-channel time-series, real or complex-valued.
+    estimator : string | callable, default="cov"
         Covariance matrix estimator [est]_:
 
-        * 'corr' for correlation coefficient matrix [corr]_ supporting complex
-          inputs,
-        * 'cov' for numpy based covariance matrix [cov]_ supporting complex
-          inputs,
-        * 'hub' for Huber's M-estimator based covariance matrix [mest]_
-          supporting complex inputs,
-        * 'lwf' for Ledoit-Wolf shrunk covariance matrix [lwf]_,
-        * 'mcd' for minimum covariance determinant matrix [mcd]_,
-        * 'oas' for oracle approximating shrunk covariance matrix [oas]_,
-        * 'sch' for Schaefer-Strimmer shrunk covariance matrix [sch]_,
-        * 'scm' for sample covariance matrix [scm]_,
-        * 'stu' for Student-t's M-estimator based covariance matrix [mest]_
-          supporting complex inputs,
-        * 'tyl' for Tyler's M-estimator based covariance matrix [mest]_
-          supporting complex inputs,
+        * "corr" for correlation coefficient matrix [corr]_,
+        * "cov" for NumPy based covariance matrix [cov]_,
+        * "hub" for Huber's M-estimator based covariance matrix [mest]_,
+        * "lwf" for Ledoit-Wolf shrunk covariance matrix [lwf]_,
+        * "mcd" for minimum covariance determinant matrix [mcd]_,
+        * "oas" for oracle approximating shrunk covariance matrix [oas]_,
+        * "sch" for Schaefer-Strimmer shrunk covariance matrix [sch]_,
+        * "scm" for sample covariance matrix [scm]_,
+        * "stu" for Student-t's M-estimator based covariance matrix [mest]_,
+        * "tyl" for Tyler's M-estimator based covariance matrix [mest]_,
         * or a callable function.
 
-        For regularization, consider 'lwf' or 'oas'.
-        For robustness, consider 'hub', 'mcd', 'stu' or 'tyl'.
-    **kwds : optional keyword parameters
+        For regularization, consider "lwf" or "oas".
+
+        For robustness, consider "hub", "mcd", "stu" or "tyl".
+
+        For "lwf", "mcd", "oas" and "sch" estimators,
+        complex covariance matrices are estimated according to [comp]_.
+    **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     Returns
     -------
     covmats : ndarray, shape (n_matrices, n_channels, n_channels)
         Covariance matrices.
 
@@ -310,68 +381,72 @@
     ----------
     .. [est] https://scikit-learn.org/stable/modules/covariance.html
     .. [corr] https://numpy.org/doc/stable/reference/generated/numpy.corrcoef.html
     .. [cov] https://numpy.org/doc/stable/reference/generated/numpy.cov.html
     .. [lwf] https://scikit-learn.org/stable/modules/generated/sklearn.covariance.ledoit_wolf.html
     .. [mcd] https://scikit-learn.org/stable/modules/generated/sklearn.covariance.MinCovDet.html
     .. [mest] :func:`pyriemann.utils.covariance.covariance_mest`
-    .. [oas] https://scikit-learn.org/stable/modules/generated/sklearn.covariance.OAS.html
+    .. [oas] https://scikit-learn.org/stable/modules/generated/oas-function.html
     .. [sch] :func:`pyriemann.utils.covariance.covariance_sch`
-    .. [scm] https://scikit-learn.org/stable/modules/generated/sklearn.covariance.empirical_covariance.html
+    .. [scm] :func:`pyriemann.utils.covariance.covariance_scm`
+    .. [comp] `Enhanced Covariance Matrix Estimators in Adaptive Beamforming
+        <https://doi.org/10.1109/ICASSP.2007.366399>`_
+        R. Abrahamsson, Y. Selen and P. Stoica. 2007 IEEE International
+        Conference on Acoustics, Speech and Signal Processing, Volume 2, 2007.
     """  # noqa
-    est = _check_est(estimator)
+    est = check_function(estimator, cov_est_functions)
     n_matrices, n_channels, n_times = X.shape
     covmats = np.empty((n_matrices, n_channels, n_channels), dtype=X.dtype)
     for i in range(n_matrices):
         covmats[i] = est(X[i], **kwds)
     return covmats
 
 
-def covariances_EP(X, P, estimator='cov', **kwds):
+def covariances_EP(X, P, estimator="cov", **kwds):
     """Special form covariance matrix, concatenating a prototype P.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_times)
         Multi-channel time-series.
     P : ndarray, shape (n_channels_proto, n_times)
         Multi-channel prototype.
-    estimator : string, default='scm'
+    estimator : string, default="cov"
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
     **kwds : optional keyword parameters
         Any further parameters are passed directly to the covariance estimator.
 
     Returns
     -------
     covmats : ndarray, shape (n_matrices, n_channels + n_channels_proto, \
             n_channels + n_channels_proto)
         Covariance matrices.
     """
-    est = _check_est(estimator)
+    est = check_function(estimator, cov_est_functions)
     n_matrices, n_channels, n_times = X.shape
     n_channels_proto, n_times_p = P.shape
     if n_times_p != n_times:
         raise ValueError(
             f"X and P do not have the same n_times: {n_times} and {n_times_p}")
     covmats = np.empty((n_matrices, n_channels + n_channels_proto,
-                        n_channels + n_channels_proto))
+                        n_channels + n_channels_proto), dtype=X.dtype)
     for i in range(n_matrices):
         covmats[i] = est(np.concatenate((P, X[i]), axis=0), **kwds)
     return covmats
 
 
-def covariances_X(X, estimator='scm', alpha=0.2, **kwds):
+def covariances_X(X, estimator="cov", alpha=0.2, **kwds):
     """Special form covariance matrix, embedding input X.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_times)
         Multi-channel time-series.
-    estimator : string, default='scm'
+    estimator : string, default="cov"
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
     alpha : float, default=0.2
         Regularization parameter (strictly positive).
     **kwds : optional keyword parameters
         Any further parameters are passed directly to the covariance estimator.
 
@@ -389,15 +464,15 @@
         M. Congedo and A. Barachant, MaxEnt - 34th International Workshop on
         Bayesian Inference and Maximun Entropy Methods in Science and
         Engineering (MaxEnt'14), Sep 2014, Amboise, France. pp.495
     """
     if alpha <= 0:
         raise ValueError(
             f"Parameter alpha must be strictly positive (Got {alpha})")
-    est = _check_est(estimator)
+    est = check_function(estimator, cov_est_functions)
     n_matrices, n_channels, n_times = X.shape
 
     Hchannels = np.eye(n_channels) \
         - np.outer(np.ones(n_channels), np.ones(n_channels)) / n_channels
     Htimes = np.eye(n_times) \
         - np.outer(np.ones(n_times), np.ones(n_times)) / n_times
     X = Hchannels @ X @ Htimes  # Eq(8), double centering
@@ -409,40 +484,40 @@
             np.concatenate((X[i], alpha * np.eye(n_channels)), axis=1),  # top
             np.concatenate((alpha * np.eye(n_times), X[i].T), axis=1)  # bottom
         ), axis=0)  # Eq(9)
         covmats[i] = est(Y, **kwds)
     return covmats / (2 * alpha)  # Eq(10)
 
 
-def block_covariances(X, blocks, estimator='cov', **kwds):
+def block_covariances(X, blocks, estimator="cov", **kwds):
     """Compute block diagonal covariance.
 
     Calculates block diagonal matrices where each block is a covariance
     matrix of a subset of channels.
     Block sizes are passed as a list of integers and can vary. The sum
     of block sizes must equal the number of channels in X.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_times)
         Multi-channel time-series.
     blocks: list of int
         List of block sizes.
-    estimator : string, default='scm'
+    estimator : string, default="cov"
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
     **kwds : optional keyword parameters
         Any further parameters are passed directly to the covariance estimator.
 
     Returns
     -------
-    C : ndarray, shape (n_matrices, n_channels, n_channels)
+    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
         Block diagonal covariance matrices.
     """
-    est = _check_est(estimator)
+    est = check_function(estimator, cov_est_functions)
     n_matrices, n_channels, n_times = X.shape
 
     if np.sum(blocks) != n_channels:
         raise ValueError("Sum of individual block sizes "
                          "must match number of channels of X.")
 
     covmats = np.empty((n_matrices, n_channels, n_channels))
@@ -455,17 +530,17 @@
 
     return covmats
 
 
 ###############################################################################
 
 
-def eegtocov(sig, window=128, overlapp=0.5, padding=True, estimator='cov'):
+def eegtocov(sig, window=128, overlapp=0.5, padding=True, estimator="cov"):
     """Convert EEG signal to covariance using sliding window."""
-    est = _check_est(estimator)
+    est = check_function(estimator, cov_est_functions)
     X = []
     if padding:
         padd = np.zeros((int(window / 2), sig.shape[1]))
         sig = np.concatenate((padd, sig, padd), axis=0)
 
     n_times, n_channels = sig.shape
     jump = int(window * overlapp)
@@ -482,15 +557,15 @@
 
 def cross_spectrum(X, window=128, overlap=0.75, fmin=None, fmax=None, fs=None):
     """Compute the complex cross-spectral matrices of a real signal X.
 
     Parameters
     ----------
     X : ndarray, shape (n_channels, n_times)
-        Multi-channel time-series.
+        Multi-channel time-series, real-valued.
     window : int, default=128
         The length of the FFT window used for spectral estimation.
     overlap : float, default=0.75
         The percentage of overlap between window.
     fmin : float | None, default=None
         The minimal frequency to be returned.
     fmax : float | None, default=None
@@ -505,14 +580,16 @@
     freqs : ndarray, shape (n_freqs,)
         The frequencies associated to cross-spectra.
 
     References
     ----------
     .. [1] https://en.wikipedia.org/wiki/Cross-spectrum
     """
+    if not is_real_type(X):
+        raise ValueError("Input must be real-valued.")
     window = int(window)
     if window < 1:
         raise ValueError("Value window must be a positive integer")
     if not 0 < overlap < 1:
         raise ValueError(
             f"Value overlap must be included in (0, 1) (Got {overlap})")
 
@@ -567,15 +644,15 @@
 
 def cospectrum(X, window=128, overlap=0.75, fmin=None, fmax=None, fs=None):
     """Compute co-spectral matrices, the real part of cross-spectra.
 
     Parameters
     ----------
     X : ndarray, shape (n_channels, n_times)
-        Multi-channel time-series.
+        Multi-channel time-series, real-valued.
     window : int, default=128
         The length of the FFT window used for spectral estimation.
     overlap : float, default=0.75
         The percentage of overlap between window.
     fmin : float | None, default=None
         The minimal frequency to be returned.
     fmax : float | None, default=None
@@ -604,15 +681,15 @@
 def coherence(X, window=128, overlap=0.75, fmin=None, fmax=None, fs=None,
               coh='ordinary'):
     """Compute squared coherence.
 
     Parameters
     ----------
     X : ndarray, shape (n_channels, n_times)
-        Multi-channel time-series.
+        Multi-channel time-series, real-valued.
     window : int, default=128
         The length of the FFT window used for spectral estimation.
     overlap : float, default=0.75
         The percentage of overlap between window.
     fmin : float | None, default=None
         The minimal frequency to be returned.
     fmax : float | None, default=None
```

### Comparing `pyriemann-0.5/pyriemann/utils/distance.py` & `pyriemann-0.6/pyriemann/utils/distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Distances between SPD/HPD matrices."""
 
 import numpy as np
 from scipy.linalg import eigvalsh, solve
+from sklearn.metrics import euclidean_distances
 
 from .base import logm, sqrtm, invsqrtm
+from .utils import check_function
 
 
 def _check_inputs(A, B):
     if not isinstance(A, np.ndarray) or not isinstance(B, np.ndarray):
         raise ValueError("Inputs must be ndarrays")
     if not A.shape == B.shape:
         raise ValueError("Inputs must have equal dimensions")
@@ -135,15 +137,15 @@
         S. Kullback S, R. Leibler.
         The Annals of Mathematical Statistics, 1951, 22 (1), pp. 79-86
     """
     _check_inputs(A, B)
     n = A.shape[-1]
     tr = np.trace(_recursive(solve, B, A, assume_a='pos'), axis1=-2, axis2=-1)
     logdet = np.linalg.slogdet(B)[1] - np.linalg.slogdet(A)[1]
-    d = 0.5 * (tr - n + logdet)
+    d = 0.5 * (tr - n + logdet).real
     return d ** 2 if squared else d
 
 
 def distance_kullback_right(A, B, squared=False):
     """Wrapper for right Kullback-Leibler divergence."""
     return distance_kullback(B, A, squared=squared)
 
@@ -360,63 +362,47 @@
         the tensor product of semifinite w*-algebras
         <https://www.ams.org/journals/tran/1969-135-00/S0002-9947-1969-0236719-2/S0002-9947-1969-0236719-2.pdf>`_
         D. Bures. Trans Am Math Soc, 1969, 135, pp. 199-212
     """  # noqa
     _check_inputs(A, B)
     B12 = sqrtm(B)
     d2 = np.trace(A + B - 2 * sqrtm(B12 @ A @ B12), axis1=-2, axis2=-1)
-    d2 = np.maximum(0, d2)
+    d2 = np.maximum(0, d2.real)
     return d2 if squared else np.sqrt(d2)
 
 
-###############################################################################
-
-
 distance_functions = {
-    'euclid': distance_euclid,
-    'harmonic': distance_harmonic,
-    'kullback': distance_kullback,
-    'kullback_right': distance_kullback_right,
-    'kullback_sym': distance_kullback_sym,
-    'logdet': distance_logdet,
-    'logeuclid': distance_logeuclid,
-    'riemann': distance_riemann,
-    'wasserstein': distance_wasserstein,
+    "euclid": distance_euclid,
+    "harmonic": distance_harmonic,
+    "kullback": distance_kullback,
+    "kullback_right": distance_kullback_right,
+    "kullback_sym": distance_kullback_sym,
+    "logdet": distance_logdet,
+    "logeuclid": distance_logeuclid,
+    "riemann": distance_riemann,
+    "wasserstein": distance_wasserstein,
 }
 
 
-def _check_distance_function(metric):
-    """Check distance function."""
-    if isinstance(metric, str):
-        if metric not in distance_functions.keys():
-            raise ValueError(f"Unknown distance metric '{metric}'")
-        else:
-            metric = distance_functions[metric]
-    elif not hasattr(metric, '__call__'):
-        raise ValueError("Distance metric must be a function or a string "
-                         f"(Got {type(metric)}.")
-    return metric
-
-
-def distance(A, B, metric='riemann', squared=False):
+def distance(A, B, metric="riemann", squared=False):
     """Distance between matrices according to a metric.
 
     Compute the distance between two matrices A and B according to a metric
     [1]_, or between a set of matrices A and another matrix B.
 
     Parameters
     ----------
     A : ndarray, shape (n, n) or shape (n_matrices, n, n)
         First matrix, or set of matrices.
     B : ndarray, shape (n, n)
         Second matrix.
-    metric : string, default='riemann'
-        The metric for distance, can be: 'euclid', 'harmonic', 'kullback',
-        'kullback_right', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
-        'wasserstein', or a callable function.
+    metric : string | callable, default="riemann"
+        Metric for distance, can be: "euclid", "harmonic", "kullback",
+        "kullback_right", "kullback_sym", "logdet", "logeuclid", "riemann",
+        "wasserstein", or a callable function.
     squared : bool, default False
         Return squared distance.
 
         .. versionadded:: 0.5
 
     Returns
     -------
@@ -427,60 +413,227 @@
     ----------
     .. [1] `Review of Riemannian distances and divergences, applied to
         SSVEP-based BCI
         <https://hal.archives-ouvertes.fr/LISV/hal-03015762v1>`_
         S. Chevallier, E. K. Kalunga, Q. Barthélemy, E. Monacelli.
         Neuroinformatics, Springer, 2021, 19 (1), pp.93-106
     """
-    distance_function = _check_distance_function(metric)
+    distance_function = check_function(metric, distance_functions)
 
     shape_A, shape_B = A.shape, B.shape
     if shape_A == shape_B:
         d = distance_function(A, B, squared=squared)
     elif len(shape_A) == 3 and len(shape_B) == 2:
         d = np.empty((shape_A[0], 1))
         for i in range(shape_A[0]):
             d[i] = distance_function(A[i], B, squared=squared)
     else:
         raise ValueError("Inputs have incompatible dimensions.")
 
     return d
 
 
-def pairwise_distance(X, Y=None, metric='riemann', squared=False):
+###############################################################################
+
+
+def _pairwise_distance_euclid(X, Y=None, squared=False):
+    """Pairwise Euclidean distance matrix.
+
+    Compute the matrix of Euclidean distances between pairs of elements of X
+    and Y.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices_X, n, n)
+        First set of matrices.
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
+        Second set of matrices. If None, Y is set to X.
+    squared : bool, default False
+        Return squared distances.
+
+    Returns
+    -------
+    dist : ndarray, shape (n_matrices_X, n_matrices_X) or (n_matrices_X, \
+            n_matrices_Y)
+        Euclidean distances between pairs of elements of X if Y is None, or
+        between elements of X and Y.
+
+    See Also
+    --------
+    pairwise_distance
+    distance_euclid
+    """
+    if Y is None:
+        dist = euclidean_distances(X.reshape(len(X), -1), squared=squared)
+    else:
+        dist = euclidean_distances(X.reshape(len(X), -1),
+                                   Y.reshape(len(Y), -1),
+                                   squared=squared)
+    return dist
+
+
+def _pairwise_distance_harmonic(X, Y=None, squared=False):
+    """Pairwise harmonic distance matrix.
+
+    Compute the matrix of harmonic distances between pairs of elements of X and
+    Y.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices_X, n, n)
+        First set of matrices.
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
+        Second set of matrices. If None, Y is set to X.
+    squared : bool, default False
+        Return squared distances.
+
+    Returns
+    -------
+    dist : ndarray, shape (n_matrices_X, n_matrices_X) or (n_matrices_X, \
+            n_matrices_Y)
+        Harmonic distances between pairs of elements of X if Y is None, or
+        between elements of X and Y.
+
+    See Also
+    --------
+    pairwise_distance
+    distance_harmonic
+    """
+    invX = np.linalg.inv(X)
+    if Y is None:
+        invY = None
+    else:
+        invY = np.linalg.inv(Y)
+
+    return _pairwise_distance_euclid(invX, invY, squared=squared)
+
+
+def _pairwise_distance_logeuclid(X, Y=None, squared=False):
+    """Pairwise Log-Euclidean distance matrix.
+
+    Compute the matrix of Log-Euclidean distances between pairs of elements of
+    X and Y.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices_X, n, n)
+        First set of matrices.
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
+        Second set of matrices. If None, Y is set to X.
+    squared : bool, default False
+        Return squared distances.
+
+    Returns
+    -------
+    dist : ndarray, shape (n_matrices_X, n_matrices_X) or (n_matrices_X, \
+            n_matrices_Y)
+        Log-Euclidean distances between pairs of elements of X if Y is None, or
+        between elements of X and Y.
+
+    See Also
+    --------
+    pairwise_distance
+    distance_logeuclid
+    """
+    logX = logm(X)
+    if Y is None:
+        logY = None
+    else:
+        logY = logm(Y)
+
+    return _pairwise_distance_euclid(logX, logY, squared=squared)
+
+
+def _pairwise_distance_riemann(X, Y=None, squared=False):
+    """Pairwise Riemannian distance matrix.
+
+    Compute the matrix of Riemannian distances between pairs of elements of X
+    and Y.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices_X, n, n)
+        First set of matrices.
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
+        Second set of matrices. If None, Y is set to X.
+    squared : bool, default False
+        Return squared distances.
+
+    Returns
+    -------
+    dist : ndarray, shape (n_matrices_X, n_matrices_X) or (n_matrices_X, \
+            n_matrices_Y)
+        Riemannian distances between pairs of elements of X if Y is None, or
+        between elements of X and Y.
+
+    See Also
+    --------
+    pairwise_distance
+    distance_riemann
+    """
+    XisY = False
+    if Y is None:
+        XisY = True
+        Y = X
+
+    n_matrices_X, n_matrices_Y = len(X), len(Y)
+    Xinv12 = invsqrtm(X)
+    dist = np.zeros((n_matrices_X, n_matrices_Y))
+
+    # row by row so it fits in memory
+    for i, x_ in enumerate(Xinv12):
+        evals_ = np.linalg.eigvalsh(x_ @ Y[i * XisY:] @ x_)
+        d2 = np.sum(np.log(evals_) ** 2, -1)
+        dist[i, i * XisY:] = d2
+
+    if XisY:
+        dist += dist.T
+
+    return dist if squared else np.sqrt(dist)
+
+
+def pairwise_distance(X, Y=None, metric="riemann", squared=False):
     """Pairwise distance matrix.
 
     Compute the matrix of distances between pairs of elements of X and Y.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices_X, n, n)
         First set of matrices.
     Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
         Second set of matrices. If None, Y is set to X.
     metric : string, default='riemann'
-        The metric for distance, can be: 'euclid', 'harmonic', 'kullback',
-        'kullback_right', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
-        'wasserstein', or a callable function.
+        Metric for pairwise distance. For the list of supported metrics,
+        see :func:`pyriemann.utils.distance.distance`.
     squared : bool, default False
-        Return squared distance.
+        Return squared distances.
 
         .. versionadded:: 0.5
 
     Returns
     -------
     dist : ndarray, shape (n_matrices_X, n_matrices_X) or (n_matrices_X, \
             n_matrices_Y)
         Distances between pairs of elements of X if Y is None, or between
         elements of X and Y.
 
     See Also
     --------
     distance
     """
+    if metric == "euclid":
+        return _pairwise_distance_euclid(X, Y=Y, squared=squared)
+    elif metric == "harmonic":
+        return _pairwise_distance_harmonic(X, Y=Y, squared=squared)
+    elif metric == "logeuclid":
+        return _pairwise_distance_logeuclid(X, Y=Y, squared=squared)
+    elif metric == "riemann":
+        return _pairwise_distance_riemann(X, Y=Y, squared=squared)
+
     n_matrices_X, _, _ = X.shape
 
     # compute full pairwise matrix for non-symmetric metrics
     if Y is None and metric in ["kullback", "kullback_right"]:
         Y = X
 
     if Y is None:
```

### Comparing `pyriemann-0.5/pyriemann/utils/docs.py` & `pyriemann-0.6/pyriemann/utils/docs.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/utils/geodesic.py` & `pyriemann-0.6/pyriemann/utils/geodesic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Geodesics for SPD/HPD matrices."""
 
 from .base import sqrtm, invsqrtm, powm, logm, expm
+from .utils import check_function
 
 
 def geodesic_euclid(A, B, alpha=0.5):
     r"""Euclidean geodesic between matrices.
 
     The matrix at position :math:`\alpha` on the Euclidean geodesic
     between two matrices :math:`\mathbf{A}` and :math:`\mathbf{B}` is:
@@ -18,15 +19,15 @@
     Parameters
     ----------
     A : ndarray, shape (..., n, m)
         First matrices.
     B : ndarray, shape (..., n, m)
         Second matrices.
     alpha : float, default=0.5
-        The position on the geodesic.
+        Position on the geodesic.
 
     Returns
     -------
     C : ndarray, shape (..., n, m)
         Matrices on the Euclidean geodesic.
     """
     return (1 - alpha) * A + alpha * B
@@ -48,15 +49,15 @@
     Parameters
     ----------
     A : ndarray, shape (..., n, n)
         First SPD/HPD matrices.
     B : ndarray, shape (..., n, n)
         Second SPD/HPD matrices.
     alpha : float, default=0.5
-        The position on the geodesic.
+        Position on the geodesic.
 
     Returns
     -------
     C : ndarray, shape (..., n, n)
         SPD/HPD matrices on the Log-Euclidean geodesic.
     """
     return expm((1 - alpha) * logm(A) + alpha * logm(B))
@@ -79,15 +80,15 @@
     Parameters
     ----------
     A : ndarray, shape (..., n, n)
         First SPD/HPD matrices.
     B : ndarray, shape (..., n, n)
         Second SPD/HPD matrices.
     alpha : float, default=0.5
-        The position on the geodesic.
+        Position on the geodesic.
 
     Returns
     -------
     C : ndarray, shape (..., n, n)
         SPD/HPD matrices on the affine-invariant Riemannian geodesic.
     """
     sA, isA = sqrtm(A), invsqrtm(A)
@@ -96,36 +97,40 @@
     E = sA @ D @ sA
     return E
 
 
 ###############################################################################
 
 
-def geodesic(A, B, alpha, metric='riemann'):
+geodesic_functions = {
+    "euclid": geodesic_euclid,
+    "logeuclid": geodesic_logeuclid,
+    "riemann": geodesic_riemann,
+}
+
+
+def geodesic(A, B, alpha, metric="riemann"):
     """Geodesic between matrices according to a metric.
 
     Return the matrix at the position alpha on the geodesic between matrices
     A and B according to a metric.
 
     Parameters
     ----------
     A : ndarray, shape (..., n, n)
         First matrices.
     B : ndarray, shape (..., n, n)
         Second matrices.
     alpha : float
-        The position on the geodesic.
-    metric : string, default='riemann'
-        The metric used for geodesic, can be: 'euclid', 'logeuclid', 'riemann'.
+        Position on the geodesic.
+    metric : string | callable, default="riemann"
+        Metric used for geodesic, can be: "euclid", "logeuclid", "riemann",
+        or a callable function.
 
     Returns
     -------
     C : ndarray, shape (..., n, n)
         Matrices on the geodesic.
     """
-    geodesic_functions = {
-        'euclid': geodesic_euclid,
-        'logeuclid': geodesic_logeuclid,
-        'riemann': geodesic_riemann,
-    }
-    C = geodesic_functions[metric](A, B, alpha)
+    geodesic_function = check_function(metric, geodesic_functions)
+    C = geodesic_function(A, B, alpha)
     return C
```

### Comparing `pyriemann-0.5/pyriemann/utils/kernel.py` & `pyriemann-0.6/pyriemann/utils/kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Kernels for SPD matrices."""
 
 import numpy as np
 
 from .base import invsqrtm, logm
 from .mean import mean_riemann
+from .utils import check_function
 
 
 def kernel_euclid(X, Y=None, *, reg=1e-10, **kwargs):
     r"""Euclidean kernel between two sets of matrices.
 
     Calculates the Euclidean kernel matrix :math:`\mathbf{K}` of inner products
     of two sets :math:`\mathbf{X}` and :math:`\mathbf{Y}` of matrices in
@@ -189,31 +190,39 @@
     # regularization due to numerical errors
     if np.array_equal(X_, Y_):
         K.flat[:: n_matrices_X + 1] += reg
 
     return K
 
 
-def kernel(X, Y=None, *, Cref=None, metric='riemann', reg=1e-10):
+kernel_functions = {
+    "euclid": kernel_euclid,
+    "logeuclid": kernel_logeuclid,
+    "riemann": kernel_riemann,
+}
+
+
+def kernel(X, Y=None, *, Cref=None, metric="riemann", reg=1e-10):
     """Kernel matrix between matrices according to a specified metric.
 
     Calculates the kernel matrix K of inner products of two sets X and Y of
     matrices on the tangent space at Cref according to a specified metric.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices_X, n, n)
         First set of matrices.
     Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
         Second set of matrices. If None, Y is set to X.
     Cref : None | ndarray, shape (n, n), default=None
         Reference point for the tangent space and inner product
-        calculation. Only used if metric='riemann'.
-    metric : {'euclid', 'logeuclid', 'riemann'}, default='riemann'
-        The type of metric used for tangent space and mean estimation.
+        calculation. Only used if metric="riemann".
+    metric : string | callable, default="riemann"
+        Metric used for tangent space and mean estimation, can be:
+        "euclid", "logeuclid", "riemann", or a callable function.
     reg : float, default=1e-10
         Regularization parameter to mitigate numerical errors in kernel
         matrix estimation, to provide a positive-definite kernel matrix.
 
     Returns
     -------
     K : ndarray, shape (n_matrices_X, n_matrices_Y)
@@ -225,12 +234,10 @@
 
     See Also
     --------
     kernel_euclid
     kernel_logeuclid
     kernel_riemann
     """
-    try:
-        return globals()[f'kernel_{metric}'](X, Y, Cref=Cref, reg=reg)
-    except KeyError:
-        raise ValueError("Kernel metric must be 'euclid', 'logeuclid', or "
-                         "'riemann'.")
+    kernel_function = check_function(metric, kernel_functions)
+    K = kernel_function(X, Y, Cref=Cref, reg=reg)
+    return K
```

### Comparing `pyriemann-0.5/pyriemann/utils/mean.py` & `pyriemann-0.6/pyriemann/utils/mean.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,45 @@
 import numpy as np
 import warnings
 
 from .ajd import ajd_pham
 from .base import sqrtm, invsqrtm, logm, expm, powm
 from .distance import distance_riemann
 from .geodesic import geodesic_riemann
-from .utils import check_weights
+from .utils import check_weights, check_function
 
 
-def mean_ale(covmats, tol=10e-7, maxiter=50, sample_weight=None):
+def _deprecate_covmats(covmats, X):
+    if covmats is not None:
+        print("DeprecationWarning: input covmats has been renamed into X and "
+              "will be removed in 0.8.0.")
+        X = covmats
+    return X
+
+
+def mean_ale(X=None, tol=10e-7, maxiter=50, sample_weight=None, covmats=None):
     """AJD-based log-Euclidean (ALE) mean of SPD matrices.
 
     Return the mean of a set of SPD matrices using the approximate joint
     diagonalization (AJD) based log-Euclidean (ALE) mean [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD matrices.
     tol : float, default=10e-7
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         ALE mean.
 
     Notes
     -----
     .. versionadded:: 0.2.4
 
     See Also
@@ -44,69 +52,66 @@
     References
     ----------
     .. [1] `Approximate Joint Diagonalization and Geometric Mean of Symmetric
         Positive Definite Matrices
         <https://arxiv.org/abs/1505.07343>`_
         M. Congedo, B. Afsari, A. Barachant, M. Moakher. PLOS ONE, 2015
     """
-    n_matrices, n, _ = covmats.shape
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, n, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
 
     # init with AJD
-    B = ajd_pham(covmats)[0]
+    B = ajd_pham(X)[0]
 
     eye_n = np.eye(n)
     crit = np.inf
     for _ in range(maxiter):
-        J = np.einsum(
-            'a,abc->bc',
-            sample_weight,
-            logm(B @ covmats @ B.conj().T)
-        )
+        J = np.einsum('a,abc->bc', sample_weight, logm(B @ X @ B.conj().T))
         delta = np.real(np.diag(expm(J)))
         B = (np.abs(delta) ** -.5)[:, np.newaxis] * B
 
         crit = distance_riemann(eye_n, np.diag(delta))
         if crit <= tol:
             break
     else:
         warnings.warn("Convergence not reached")
 
-    J = np.einsum('a,abc->bc', sample_weight, logm(B @ covmats @ B.conj().T))
+    J = np.einsum('a,abc->bc', sample_weight, logm(B @ X @ B.conj().T))
     A = np.linalg.inv(B)
-    C = A @ expm(J) @ A.conj().T
-    return C
+    M = A @ expm(J) @ A.conj().T
+    return M
 
 
-def mean_alm(covmats, tol=1e-14, maxiter=100, sample_weight=None):
+def mean_alm(X=None, tol=1e-14, maxiter=100, sample_weight=None, covmats=None):
     r"""Ando-Li-Mathias (ALM) mean of SPD/HPD matrices.
 
     Return the geometric mean recursively [1]_, generalizing from:
 
     .. math::
-        \mathbf{C} = X_1^{\frac{1}{2}} (X_1^{-\frac{1}{2}}X_2^{\frac{1}{2}}
+        \mathbf{M} = X_1^{\frac{1}{2}} (X_1^{-\frac{1}{2}}X_2^{\frac{1}{2}}
                      X_1^{-\frac{1}{2}})^{\frac{1}{2}} X_1^{\frac{1}{2}}
 
     and requiring a high number of iterations.
     Extremely slow, due to the recursive formulation.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     tol : float, default=10e-14
         The tolerance to stop the gradient descent.
     maxiter : int, default=100
         The maximum number of iterations.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         ALM mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
@@ -116,275 +121,284 @@
     References
     ----------
     .. [1] `Geometric Means
         <https://www.sciencedirect.com/science/article/pii/S0024379503008693>`_
         T. Ando, C.-K. Li, and R. Mathias. Linear Algebra and its Applications.
         Volume 385, July 2004, Pages 305-334.
     """
-    n_matrices, _, _ = covmats.shape
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, _, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
 
     if n_matrices == 2:
         alpha = sample_weight[1] / sample_weight[0] / 2
-        C = geodesic_riemann(covmats[0], covmats[1], alpha=alpha)
-        return C
+        M = geodesic_riemann(X[0], X[1], alpha=alpha)
+        return M
 
-    C = covmats
-    C_iter = np.zeros_like(C)
+    M = X
+    M_iter = np.zeros_like(M)
     for _ in range(maxiter):
         for h in range(n_matrices):
             s = np.mod(np.arange(h, h + n_matrices - 1) + 1, n_matrices)
-            C_iter[h] = mean_alm(C[s], sample_weight=sample_weight[s])
+            M_iter[h] = mean_alm(M[s], sample_weight=sample_weight[s])
 
-        norm_iter = np.linalg.norm(C_iter[0] - C[0], 2)
-        norm_c = np.linalg.norm(C[0], 2)
+        norm_iter = np.linalg.norm(M_iter[0] - M[0], 2)
+        norm_c = np.linalg.norm(M[0], 2)
         if (norm_iter / norm_c) < tol:
             break
-        C = deepcopy(C_iter)
+        M = deepcopy(M_iter)
     else:
         warnings.warn("Convergence not reached")
 
-    return C_iter.mean(axis=0)
+    return M_iter.mean(axis=0)
 
 
-def mean_euclid(covmats, sample_weight=None):
+def mean_euclid(X=None, sample_weight=None, covmats=None):
     r"""Mean of matrices according to the Euclidean metric.
 
     .. math::
-        \mathbf{C} = \sum_i w_i \ \mathbf{X}_i
+        \mathbf{M} = \sum_i w_i \ \mathbf{X}_i
 
     This mean is also called arithmetic.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, m)
+    X : ndarray, shape (n_matrices, n, m)
         Set of matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, m)
+    M : ndarray, shape (n, m)
         Euclidean mean.
 
     See Also
     --------
     mean_covariance
     """
-    return np.average(covmats, axis=0, weights=sample_weight)
+    X = _deprecate_covmats(covmats, X)
+    return np.average(X, axis=0, weights=sample_weight)
 
 
-def mean_harmonic(covmats, sample_weight=None):
+def mean_harmonic(X=None, sample_weight=None, covmats=None):
     r"""Harmonic mean of invertible matrices.
 
     .. math::
-        \mathbf{C} = \left( \sum_i wi \ {\mathbf{X}_i}^{-1} \right)^{-1}
+        \mathbf{M} = \left( \sum_i w_i \ {\mathbf{X}_i}^{-1} \right)^{-1}
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of invertible matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Harmonic mean.
 
     See Also
     --------
     mean_covariance
     """
-    T = mean_euclid(np.linalg.inv(covmats), sample_weight=sample_weight)
-    C = np.linalg.inv(T)
-    return C
+    X = _deprecate_covmats(covmats, X)
+    T = mean_euclid(np.linalg.inv(X), sample_weight=sample_weight)
+    M = np.linalg.inv(T)
+    return M
 
 
-def mean_identity(covmats, sample_weight=None):
+def mean_identity(X=None, sample_weight=None, covmats=None):
     r"""Identity matrix corresponding to the matrices dimension.
 
     .. math::
-        \mathbf{C} = \mathbf{I}_n
+        \mathbf{M} = \mathbf{I}_n
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of square matrices.
     sample_weight : None
         Not used, here for compatibility with other means.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Identity matrix.
 
     See Also
     --------
     mean_covariance
     """
-    C = np.eye(covmats.shape[-1])
-    return C
+    X = _deprecate_covmats(covmats, X)
+    M = np.eye(X.shape[-1])
+    return M
 
 
-def mean_kullback_sym(covmats, sample_weight=None):
+def mean_kullback_sym(X=None, sample_weight=None, covmats=None):
     """Mean of SPD/HPD matrices according to Kullback-Leibler divergence.
 
     Symmetrized Kullback-Leibler mean is the geometric mean between the
     Euclidean and the harmonic means [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Symmetrized Kullback-Leibler mean.
 
     See Also
     --------
     mean_covariance
 
     References
     ----------
     .. [1] `Symmetric positive-definite matrices: From geometry to applications
         and visualization
         <https://link.springer.com/chapter/10.1007/3-540-31272-2_17>`_
         M. Moakher and P. Batchelor. Visualization and Processing of Tensor
         Fields, pp. 285-298, 2006
     """
-    C_euclid = mean_euclid(covmats, sample_weight=sample_weight)
-    C_harmonic = mean_harmonic(covmats, sample_weight=sample_weight)
-    C = geodesic_riemann(C_euclid, C_harmonic, 0.5)
-    return C
+    X = _deprecate_covmats(covmats, X)
+    M_euclid = mean_euclid(X, sample_weight=sample_weight)
+    M_harmonic = mean_harmonic(X, sample_weight=sample_weight)
+    M = geodesic_riemann(M_euclid, M_harmonic, 0.5)
+    return M
 
 
-def mean_logdet(covmats, tol=10e-5, maxiter=50, init=None, sample_weight=None):
+def mean_logdet(X=None, tol=10e-5, maxiter=50, init=None, sample_weight=None,
+                covmats=None):
     r"""Mean of SPD/HPD matrices according to the log-det metric.
 
     Log-det mean is obtained by an iterative procedure where the update is:
 
     .. math::
-        \mathbf{C} = \left( \sum_i w_i \ \left( 0.5 \mathbf{C}
+        \mathbf{M} = \left( \sum_i w_i \ \left( 0.5 \mathbf{M}
                      + 0.5 \mathbf{X}_i \right)^{-1} \right)^{-1}
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     tol : float, default=10e-5
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
     init : None | ndarray, shape (n, n), default=None
         A SPD/HPD matrix used to initialize the gradient descent.
         If None, the weighted Euclidean mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Log-det mean.
 
     See Also
     --------
     mean_covariance
     """
-    n_matrices, _, _ = covmats.shape
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, _, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     if init is None:
-        C = mean_euclid(covmats, sample_weight=sample_weight)
+        M = mean_euclid(X, sample_weight=sample_weight)
     else:
-        C = init
+        M = init
 
     crit = np.finfo(np.float64).max
     for _ in range(maxiter):
-        icovmats = np.linalg.inv(0.5 * covmats + 0.5 * C)
-        J = np.einsum('a,abc->bc', sample_weight, icovmats)
-        Cnew = np.linalg.inv(J)
+        invX = np.linalg.inv(0.5 * X + 0.5 * M)
+        J = np.einsum('a,abc->bc', sample_weight, invX)
+        Mnew = np.linalg.inv(J)
 
-        crit = np.linalg.norm(Cnew - C, ord='fro')
-        C = Cnew
+        crit = np.linalg.norm(Mnew - M, ord='fro')
+        M = Mnew
         if crit <= tol:
             break
     else:
         warnings.warn("Convergence not reached")
 
-    return C
+    return M
 
 
-def mean_logeuclid(covmats, sample_weight=None):
+def mean_logeuclid(X=None, sample_weight=None, covmats=None):
     r"""Mean of SPD/HPD matrices according to the log-Euclidean metric.
 
     Log-Euclidean mean is [1]_:
 
     .. math::
-        \mathbf{C} = \exp{ \left( \sum_i w_i \ \log{\mathbf{X}_i} \right) }
+        \mathbf{M} = \exp{ \left( \sum_i w_i \ \log{\mathbf{X}_i} \right) }
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Log-Euclidean mean.
 
     See Also
     --------
     mean_covariance
 
     References
     ----------
     .. [1] `Geometric means in a novel vector space structure on symmetric
         positive-definite matrices
         <https://epubs.siam.org/doi/abs/10.1137/050637996?journalCode=sjmael>`_
         V. Arsigny, P. Fillard, X. Pennec, and N. Ayache. SIAM Journal on
         Matrix Analysis and Applications. Volume 29, Issue 1 (2007).
     """
-    C = expm(mean_euclid(logm(covmats), sample_weight=sample_weight))
-    return C
+    X = _deprecate_covmats(covmats, X)
+    M = expm(mean_euclid(logm(X), sample_weight=sample_weight))
+    return M
 
 
-def mean_power(covmats, p, *, sample_weight=None, zeta=10e-10, maxiter=100):
+def mean_power(X=None, p=None, *, sample_weight=None, zeta=10e-10, maxiter=100,
+               covmats=None):
     r"""Power mean of SPD/HPD matrices.
 
     Power mean of order p is the solution of [1]_ [2]_:
 
     .. math::
-        \mathbf{C} = \sum_i w_i \ \mathbf{C} \sharp_p \mathbf{X}_i
+        \mathbf{M} = \sum_i w_i \ \mathbf{M} \sharp_p \mathbf{X}_i
 
     where :math:`\mathbf{A} \sharp_p \mathbf{B}` is the geodesic between
     matrices :math:`\mathbf{A}` and :math:`\mathbf{B}`.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     p : float
         Exponent, in [-1,+1]. For p=0, it returns
         :func:`pyriemann.utils.mean.mean_riemann`.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
     zeta : float, default=10e-10
         Stopping criterion.
     maxiter : int, default=100
         The maximum number of iterations.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Power mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
@@ -399,87 +413,90 @@
         Issue 4, 15 February 2012, Pages 1498-1514.
     .. [2] `Fixed Point Algorithms for Estimating Power Means of Positive
         Definite Matrices
         <https://hal.archives-ouvertes.fr/hal-01500514>`_
         M. Congedo, A. Barachant, and R. Bhatia. IEEE Transactions on Signal
         Processing, Volume 65, Issue 9, pp.2211-2220, May 2017
     """
+    X = _deprecate_covmats(covmats, X)
+    if p is None:
+        raise ValueError("Input p can not be None")
     if not isinstance(p, (int, float)):
         raise ValueError("Power mean only defined for a scalar exponent")
     if p < -1 or 1 < p:
         raise ValueError("Exponent must be in [-1,+1]")
 
     if p == 1:
-        return mean_euclid(covmats, sample_weight=sample_weight)
+        return mean_euclid(X, sample_weight=sample_weight)
     elif p == 0:
-        return mean_riemann(covmats, sample_weight=sample_weight)
+        return mean_riemann(X, sample_weight=sample_weight)
     elif p == -1:
-        return mean_harmonic(covmats, sample_weight=sample_weight)
+        return mean_harmonic(X, sample_weight=sample_weight)
 
-    n_matrices, n, _ = covmats.shape
+    n_matrices, n, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     phi = 0.375 / np.abs(p)
 
-    G = np.einsum('a,abc->bc', sample_weight, powm(covmats, p))
+    G = np.einsum('a,abc->bc', sample_weight, powm(X, p))
     if p > 0:
-        X = invsqrtm(G)
+        K = invsqrtm(G)
     else:
-        X = sqrtm(G)
+        K = sqrtm(G)
 
     eye_n, sqrt_n = np.eye(n), np.sqrt(n)
     crit = 10 * zeta
     for _ in range(maxiter):
         H = np.einsum(
             'a,abc->bc',
             sample_weight,
-            powm(X @ powm(covmats, np.sign(p)) @ X.conj().T, np.abs(p))
+            powm(K @ powm(X, np.sign(p)) @ K.conj().T, np.abs(p))
         )
-        X = powm(H, -phi) @ X
+        K = powm(H, -phi) @ K
 
         crit = np.linalg.norm(H - eye_n) / sqrt_n
         if crit <= zeta:
             break
     else:
         warnings.warn("Convergence not reached")
 
-    C = X.conj().T @ X
+    M = K.conj().T @ K
     if p > 0:
-        C = np.linalg.inv(C)
+        M = np.linalg.inv(M)
 
-    return C
+    return M
 
 
-def mean_riemann(covmats, tol=10e-9, maxiter=50, init=None,
-                 sample_weight=None):
+def mean_riemann(X=None, tol=10e-9, maxiter=50, init=None, sample_weight=None,
+                 covmats=None):
     r"""Mean of SPD/HPD matrices according to the Riemannian metric.
 
     The affine-invariant Riemannian mean minimizes the sum of squared
     affine-invariant Riemannian distances :math:`d_R` to all SPD/HPD matrices
     [1]_ [2]_:
 
     .. math::
-         \arg \min_{\mathbf{C}} \sum_i w_i \ d_R (\mathbf{C}, \mathbf{X}_i)^2
+         \arg \min_{\mathbf{M}} \sum_i w_i \ d_R (\mathbf{M}, \mathbf{X}_i)^2
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     tol : float, default=10e-9
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
     init : None | ndarray, shape (n, n), default=None
         A SPD/HPD matrix used to initialize the gradient descent.
         If None, the weighted Euclidean mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Affine-invariant Riemannian mean.
 
     See Also
     --------
     mean_covariance
 
     References
@@ -490,224 +507,215 @@
         P.T. Fletcher, C. Lu, S. M. Pizer, S. Joshi.
         IEEE Trans Med Imaging, 2004, 23(8), pp. 995-1005
     .. [2] `A differential geometric approach to the geometric mean of
         symmetric positive-definite matrices
         <https://epubs.siam.org/doi/10.1137/S0895479803436937>`_
         M. Moakher. SIAM J Matrix Anal Appl, 2005, 26 (3), pp. 735-747
     """
-    n_matrices, _, _ = covmats.shape
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, _, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     if init is None:
-        C = mean_euclid(covmats, sample_weight=sample_weight)
+        M = mean_euclid(X, sample_weight=sample_weight)
     else:
-        C = init
+        M = init
 
     nu = 1.0
     tau = np.finfo(np.float64).max
     crit = np.finfo(np.float64).max
     for _ in range(maxiter):
-        C12, Cm12 = sqrtm(C), invsqrtm(C)
-        J = np.einsum('a,abc->bc', sample_weight, logm(Cm12 @ covmats @ Cm12))
-        C = C12 @ expm(nu * J) @ C12
+        M12, Mm12 = sqrtm(M), invsqrtm(M)
+        J = np.einsum('a,abc->bc', sample_weight, logm(Mm12 @ X @ Mm12))
+        M = M12 @ expm(nu * J) @ M12
 
         crit = np.linalg.norm(J, ord='fro')
         h = nu * crit
         if h < tau:
             nu = 0.95 * nu
             tau = h
         else:
             nu = 0.5 * nu
         if crit <= tol or nu <= tol:
             break
     else:
         warnings.warn("Convergence not reached")
 
-    return C
+    return M
 
 
-def mean_wasserstein(covmats, tol=10e-4, maxiter=50, init=None,
-                     sample_weight=None):
+def mean_wasserstein(X=None, tol=10e-4, maxiter=50, init=None,
+                     sample_weight=None, covmats=None):
     r"""Mean of SPD/HPD matrices according to the Wasserstein metric.
 
     Wasserstein mean is obtained by an iterative procedure where the update is
     [1]_:
 
     .. math::
         \mathbf{K} = \left( \sum_i w_i \ \left( \mathbf{K} \mathbf{X}_i
                      \mathbf{K} \right)^{1/2} \right)^{1/2}
 
-    with :math:`\mathbf{K} = \mathbf{C}^{1/2}`.
+    with :math:`\mathbf{K} = \mathbf{M}^{1/2}`.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     tol : float, default=10e-4
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
     init : None | ndarray, shape (n, n), default=None
         A SPD/HPD matrix used to initialize the gradient descent.
         If None the Euclidean mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Wasserstein mean.
 
     See Also
     --------
     mean_covariance
 
     References
     ----------
     .. [1] `Geometric Radar Processing based on Frechet distance: Information
         geometry versus Optimal Transport Theory
         <https://ieeexplore.ieee.org/document/6042179>`_
         F. Barbaresco. 12th International Radar Symposium (IRS), October 2011
     """
-    n_matrices, _, _ = covmats.shape
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, _, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     if init is None:
-        C = mean_euclid(covmats, sample_weight=sample_weight)
+        M = mean_euclid(X, sample_weight=sample_weight)
     else:
-        C = init
-    K = sqrtm(C)
+        M = init
+    K = sqrtm(M)
 
     crit = np.finfo(np.float64).max
     for _ in range(maxiter):
-        J = np.einsum('a,abc->bc', sample_weight, sqrtm(K @ covmats @ K))
+        J = np.einsum('a,abc->bc', sample_weight, sqrtm(K @ X @ K))
         Knew = sqrtm(J)
 
         crit = np.linalg.norm(Knew - K, ord='fro')
         K = Knew
         if crit <= tol:
             break
     else:
         warnings.warn("Convergence not reached")
 
-    C = K @ K
-    return C
+    M = K @ K
+    return M
 
 
 ###############################################################################
 
 
 mean_functions = {
-    'ale': mean_ale,
-    'alm': mean_alm,
-    'euclid': mean_euclid,
-    'harmonic': mean_harmonic,
-    'identity': mean_identity,
-    'kullback_sym': mean_kullback_sym,
-    'logdet': mean_logdet,
-    'logeuclid': mean_logeuclid,
-    'riemann': mean_riemann,
-    'wasserstein': mean_wasserstein,
+    "ale": mean_ale,
+    "alm": mean_alm,
+    "euclid": mean_euclid,
+    "harmonic": mean_harmonic,
+    "identity": mean_identity,
+    "kullback_sym": mean_kullback_sym,
+    "logdet": mean_logdet,
+    "logeuclid": mean_logeuclid,
+    "riemann": mean_riemann,
+    "wasserstein": mean_wasserstein,
 }
 
 
-def _check_mean_function(metric):
-    """Check mean function."""
-    if isinstance(metric, str):
-        if metric not in mean_functions.keys():
-            raise ValueError(f"Unknown mean metric '{metric}'")
-        else:
-            metric = mean_functions[metric]
-    elif not hasattr(metric, '__call__'):
-        raise ValueError("Mean metric must be a function or a string "
-                         f"(Got {type(metric)}.")
-    return metric
-
-
-def mean_covariance(covmats, metric='riemann', sample_weight=None, **kwargs):
+def mean_covariance(X=None, metric="riemann", sample_weight=None, covmats=None,
+                    **kwargs):
     """Mean of matrices according to a metric.
 
     Compute the mean of a set of matrices according to a metric [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of matrices.
-    metric : string, default='riemann'
-        The metric for mean, can be: 'ale', 'alm', 'euclid', 'harmonic',
-        'identity', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
-        'wasserstein', or a callable function.
+    metric : string | callable, default="riemann"
+        Metric for mean estimation, can be: "ale", "alm", "euclid", "harmonic",
+        "identity", "kullback_sym", "logdet", "logeuclid", "riemann",
+        "wasserstein", or a callable function.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
     **kwargs : dict
         The keyword arguments passed to the sub function.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Mean of matrices.
 
     References
     ----------
     .. [1] `Review of Riemannian distances and divergences, applied to
         SSVEP-based BCI
         <https://hal.archives-ouvertes.fr/LISV/hal-03015762v1>`_
         S. Chevallier, E. K. Kalunga, Q. Barthélemy, E. Monacelli.
         Neuroinformatics, Springer, 2021, 19 (1), pp.93-106
     """
-    mean_function = _check_mean_function(metric)
-    C = mean_function(
-        covmats,
+    X = _deprecate_covmats(covmats, X)
+    mean_function = check_function(metric, mean_functions)
+    M = mean_function(
+        X,
         sample_weight=sample_weight,
         **kwargs,
     )
-    return C
+    return M
 
 
 ###############################################################################
 
 
-def _get_mask_from_nan(covmat):
-    nan_col = np.all(np.isnan(covmat), axis=0)
-    nan_row = np.all(np.isnan(covmat), axis=1)
+def _get_mask_from_nan(X):
+    nan_col = np.all(np.isnan(X), axis=0)
+    nan_row = np.all(np.isnan(X), axis=1)
     if not np.array_equal(nan_col, nan_row):
         raise ValueError("NaN values are not symmetric.")
     nan_inds = np.where(nan_col)
-    subcovmat_ = np.delete(covmat, nan_inds, axis=0)
-    subcovmat = np.delete(subcovmat_, nan_inds, axis=1)
-    if np.any(np.isnan(subcovmat)):
+    subX_ = np.delete(X, nan_inds, axis=0)
+    subX = np.delete(subX_, nan_inds, axis=1)
+    if np.any(np.isnan(subX)):
         raise ValueError("NaN values must fill rows and columns.")
-    mask = np.delete(np.eye(covmat.shape[0]), nan_inds, axis=1)
+    mask = np.delete(np.eye(X.shape[0]), nan_inds, axis=1)
     return mask
 
 
-def _get_masks_from_nan(covmats):
+def _get_masks_from_nan(X):
     masks = []
-    for i in range(len(covmats)):
-        masks.append(_get_mask_from_nan(covmats[i]))
+    for i in range(len(X)):
+        masks.append(_get_mask_from_nan(X[i]))
     return masks
 
 
-def _apply_masks(covmats, masks):
-    maskedcovmats = []
-    for i in range(len(covmats)):
-        maskedcovmats.append(masks[i].T @ covmats[i] @ masks[i])
-    return maskedcovmats
+def _apply_masks(X, masks):
+    maskedX = []
+    for i in range(len(X)):
+        maskedX.append(masks[i].T @ X[i] @ masks[i])
+    return maskedX
 
 
-def maskedmean_riemann(covmats, masks, tol=10e-9, maxiter=100, init=None,
-                       sample_weight=None):
+def maskedmean_riemann(X=None, masks=None, tol=10e-9, maxiter=100, init=None,
+                       sample_weight=None, covmats=None):
     """Masked Riemannian mean of SPD/HPD matrices.
 
     Given masks defined as semi-orthogonal matrices, the masked Riemannian mean
     of SPD/HPD matrices is obtained with a gradient descent minimizing the sum
     of affine-invariant Riemannian distances between masked SPD/HPD matrices
     and the masked mean [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices.
     masks : list of n_matrices ndarray of shape (n, n_i), \
             with different n_i, such that n_i <= n
         Masks, defined as semi-orthogonal matrices. See [1]_.
     tol : float, default=10e-9
         The tolerance to stop the gradient descent.
     maxiter : int, default=100
@@ -716,15 +724,15 @@
         A SPD/HPD matrix used to initialize the gradient descent.
         If None, the Identity is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Masked Riemannian mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
@@ -736,74 +744,77 @@
     ----------
     .. [1] `Geodesically-convex optimization for averaging partially observed
         covariance matrices
         <https://hal.archives-ouvertes.fr/hal-02984423>`_
         F. Yger, S. Chevallier, Q. Barthélemy, and S. Sra. Asian Conference on
         Machine Learning (ACML), Nov 2020, Bangkok, Thailand. pp.417 - 432.
     """
-    n_matrices, n, _ = covmats.shape
+    if masks is None:
+        raise ValueError("Input masks can not be None")
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, n, _ = X.shape
     sample_weight = check_weights(sample_weight, n_matrices)
-    maskedcovmats = _apply_masks(covmats, masks)
+    maskedX = _apply_masks(X, masks)
     if init is None:
-        C = np.eye(n)
+        M = np.eye(n)
     else:
-        C = init
+        M = init
 
     nu = 1.0
     tau = np.finfo(np.float64).max
     crit = np.finfo(np.float64).max
     for _ in range(maxiter):
-        maskedC = _apply_masks(np.tile(C, (n_matrices, 1, 1)), masks)
-        J = np.zeros((n, n), dtype=covmats.dtype)
+        maskedM = _apply_masks(np.tile(M, (n_matrices, 1, 1)), masks)
+        J = np.zeros((n, n), dtype=X.dtype)
         for i in range(n_matrices):
-            C12, Cm12 = sqrtm(maskedC[i]), invsqrtm(maskedC[i])
-            tmp = C12 @ logm(Cm12 @ maskedcovmats[i] @ Cm12) @ C12
+            M12, Mm12 = sqrtm(maskedM[i]), invsqrtm(maskedM[i])
+            tmp = M12 @ logm(Mm12 @ maskedX[i] @ Mm12) @ M12
             J += sample_weight[i] * masks[i] @ tmp @ masks[i].T
-        C12, Cm12 = sqrtm(C), invsqrtm(C)
-        C = C12 @ expm(Cm12 @ (nu * J) @ Cm12) @ C12
+        M12, Mm12 = sqrtm(M), invsqrtm(M)
+        M = M12 @ expm(Mm12 @ (nu * J) @ Mm12) @ M12
 
         crit = np.linalg.norm(J, ord='fro')
         h = nu * crit
         if h < tau:
             nu = 0.95 * nu
             tau = h
         else:
             nu = 0.5 * nu
         if crit <= tol or nu <= tol:
             break
     else:
         warnings.warn("Convergence not reached")
 
-    return C
+    return M
 
 
-def nanmean_riemann(covmats, tol=10e-9, maxiter=100, init=None,
-                    sample_weight=None):
+def nanmean_riemann(X=None, tol=10e-9, maxiter=100, init=None,
+                    sample_weight=None, covmats=None):
     """Riemannian NaN-mean of SPD/HPD matrices.
 
     The Riemannian NaN-mean is the masked Riemannian mean applied to SPD/HPD
     matrices potentially corrupted by symmetric NaN values [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n, n)
+    X : ndarray, shape (n_matrices, n, n)
         Set of SPD/HPD matrices, corrupted by symmetric NaN values [1]_.
     tol : float, default=10e-9
         The tolerance to stop the gradient descent.
     maxiter : int, default=100
         The maximum number of iteration.
     init : None | ndarray, shape (n, n), default=None
         A SPD/HPD matrix used to initialize the gradient descent.
         If None, a regularized Euclidean NaN-mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n, n)
+    M : ndarray, shape (n, n)
         Riemannian NaN-mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
@@ -815,22 +826,23 @@
     ----------
     .. [1] `Geodesically-convex optimization for averaging partially observed
         covariance matrices
         <https://hal.archives-ouvertes.fr/hal-02984423>`_
         F. Yger, S. Chevallier, Q. Barthélemy, and S. Sra. Asian Conference on
         Machine Learning (ACML), Nov 2020, Bangkok, Thailand. pp.417 - 432.
     """
-    n_matrices, n, _ = covmats.shape
+    X = _deprecate_covmats(covmats, X)
+    n_matrices, n, _ = X.shape
     if init is None:
-        Cinit = np.nanmean(covmats, axis=0) + 1e-6 * np.eye(n)
+        Minit = np.nanmean(X, axis=0) + 1e-6 * np.eye(n)
     else:
-        Cinit = init
+        Minit = init
 
-    C = maskedmean_riemann(
-        np.nan_to_num(covmats),  # avoid nan contamination in matmul
-        _get_masks_from_nan(covmats),
+    M = maskedmean_riemann(
+        np.nan_to_num(X),  # avoid nan contamination in matmul
+        _get_masks_from_nan(X),
         tol=tol,
         maxiter=maxiter,
-        init=Cinit,
+        init=Minit,
         sample_weight=sample_weight
     )
-    return C
+    return M
```

### Comparing `pyriemann-0.5/pyriemann/utils/median.py` & `pyriemann-0.6/pyriemann/utils/median.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/pyriemann/utils/tangentspace.py` & `pyriemann-0.6/pyriemann/utils/tangentspace.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tangent space for SPD/HPD matrices."""
 
 import numpy as np
 
 from .base import sqrtm, invsqrtm, logm, expm
 from .mean import mean_covariance
+from .utils import check_function
 
 
 def _check_dimensions(X, Cref):
     n_1, n_2 = X.shape[-2:]
     n_3, n_4 = Cref.shape
     if not (n_1 == n_2 == n_3 == n_4):
         raise ValueError("Inputs have incompatible dimensions.")
@@ -24,15 +25,15 @@
         \mathbf{X}_\text{original} = \mathbf{X} + \mathbf{C}_\text{ref}
 
     Parameters
     ----------
     X : ndarray, shape (..., n, m)
         Matrices in tangent space.
     Cref : ndarray, shape (n, m)
-        The reference matrix.
+        Reference matrix.
 
     Returns
     -------
     X_original : ndarray, shape (..., n, m)
         Matrices in manifold.
 
     Notes
@@ -54,15 +55,15 @@
         \exp(\mathbf{X} + \log(\mathbf{C}_\text{ref}))
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         Matrices in tangent space.
     Cref : ndarray, shape (n, n)
-        The reference SPD/HPD matrix.
+        Reference SPD/HPD matrix.
 
     Returns
     -------
     X_original : ndarray, shape (..., n, n)
         Matrices in SPD/HPD manifold.
 
     Notes
@@ -91,15 +92,15 @@
         \mathbf{C}_\text{ref}^{-1/2}) \mathbf{C}_\text{ref}^{1/2}
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         Matrices in tangent space.
     Cref : ndarray, shape (n, n)
-        The reference SPD/HPD matrix.
+        Reference SPD/HPD matrix.
     Cm12 : bool, default=False
         If True, it returns the full Riemannian exponential map.
 
     Returns
     -------
     X_original : ndarray, shape (..., n, n)
         Matrices in SPD/HPD manifold.
@@ -124,17 +125,17 @@
 
     .. math::
         \mathbf{X}_\text{new} = \mathbf{X} - \mathbf{C}_\text{ref}
 
     Parameters
     ----------
     X : ndarray, shape (..., n, m)
-        Matrices in manidold.
+        Matrices in manifold.
     Cref : ndarray, shape (n, m)
-        The reference matrix.
+        Reference matrix.
 
     Returns
     -------
     X_new : ndarray, shape (..., n, m)
         Matrices projected in tangent space.
 
     Notes
@@ -153,17 +154,17 @@
 
     .. math::
         \mathbf{X}_\text{new} = \log(\mathbf{X}) - \log(\mathbf{C}_\text{ref})
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
-        Matrices in SPD/HPD manidold.
+        Matrices in SPD/HPD manifold.
     Cref : ndarray, shape (n, n)
-        The reference SPD matrix.
+        Reference SPD matrix.
 
     Returns
     -------
     X_new : ndarray, shape (..., n, n)
         Matrices projected in tangent space.
 
     Notes
@@ -191,17 +192,17 @@
         \mathbf{X}_\text{new} = \mathbf{C}_\text{ref}^{1/2}
         \log( \mathbf{C}_\text{ref}^{-1/2} \mathbf{X}
         \mathbf{C}_\text{ref}^{-1/2}) \mathbf{C}_\text{ref}^{1/2}
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
-        Matrices in SPD/HPD manidold.
+        Matrices in SPD/HPD manifold.
     Cref : ndarray, shape (n, n)
-        The reference SPD/HPD matrix.
+        Reference SPD/HPD matrix.
     C12 : bool, default=False
         If True, it returns the full Riemannian logarithmic map.
 
     Returns
     -------
     X_new : ndarray, shape (..., n, n)
         Matrices projected in tangent space.
@@ -288,107 +289,113 @@
     X[..., idx[0], idx[1]] = T
     idx = np.triu_indices_from(np.empty((n, n)), k=1)
     X[..., idx[0], idx[1]] /= np.sqrt(2)
     X[..., idx[1], idx[0]] = X[..., idx[0], idx[1]].conj()
     return X
 
 
-def tangent_space(X, Cref, *, metric='riemann'):
+log_map_functions = {
+    "euclid": log_map_euclid,
+    "logeuclid": log_map_logeuclid,
+    "riemann": log_map_riemann,
+}
+
+
+def tangent_space(X, Cref, *, metric="riemann"):
     """Transform matrices into tangent vectors.
 
     Transform matrices into tangent vectors, according to a reference
     matrix Cref and to a specific logarithmic map.
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
-        Matrices in manidold.
+        Matrices in manifold.
     Cref : ndarray, shape (n, n)
-        The reference matrix.
-    metric : string, default='riemann'
-        The metric used for logarithmic map, can be: 'euclid', 'logeuclid',
-        'riemann'.
+        Reference matrix.
+    metric : string | callable, default="riemann"
+        Metric used for logarithmic map, can be:
+        "euclid", "logeuclid", "riemann", or a callable function.
 
     Returns
     -------
     T : ndarray, shape (..., n * (n + 1) / 2)
         Tangent vectors.
 
     See Also
     --------
     log_map_euclid
     log_map_logeuclid
     log_map_riemann
     upper
     """
-    log_map_functions = {
-        'euclid': log_map_euclid,
-        'logeuclid': log_map_logeuclid,
-        'riemann': log_map_riemann,
-    }
-    X_ = log_map_functions[metric](X, Cref)
+    log_map_function = check_function(metric, log_map_functions)
+    X_ = log_map_function(X, Cref)
     T = upper(X_)
 
     return T
 
 
-def untangent_space(T, Cref, *, metric='riemann'):
+exp_map_functions = {
+    "euclid": exp_map_euclid,
+    "logeuclid": exp_map_logeuclid,
+    "riemann": exp_map_riemann,
+}
+
+
+def untangent_space(T, Cref, *, metric="riemann"):
     """Transform tangent vectors back to matrices.
 
     Transform tangent vectors back to matrices, according to a reference
     matrix Cref and to a specific exponential map.
 
     Parameters
     ----------
     T : ndarray, shape (..., n * (n + 1) / 2)
         Tangent vectors.
     Cref : ndarray, shape (n, n)
-        The reference matrix.
-    metric : string, default='riemann'
-        The metric used for exponential map, can be: 'euclid', 'logeuclid',
-        'riemann'.
+        Reference matrix.
+    metric : string | callable, default="riemann"
+        Metric used for exponential map, can be:
+        "euclid", "logeuclid", "riemann", or a callable function.
 
     Returns
     -------
     X : ndarray, shape (..., n, n)
-        Matrices in manidold.
+        Matrices in manifold.
 
     See Also
     --------
     unupper
     exp_map_euclid
     exp_map_logeuclid
     exp_map_riemann
     """
     X_ = unupper(T)
-    exp_map_functions = {
-        'euclid': exp_map_euclid,
-        'logeuclid': exp_map_logeuclid,
-        'riemann': exp_map_riemann,
-    }
-    X = exp_map_functions[metric](X_, Cref)
+    exp_map_function = check_function(metric, exp_map_functions)
+    X = exp_map_function(X_, Cref)
 
     return X
 
 
 ###############################################################################
 
 
 # NOT IN API
-def transport(Covs, Cref, metric='riemann'):
+def transport(Covs, Cref, metric="riemann"):
     """Parallel transport of a set of SPD matrices towards a reference matrix.
 
     Parameters
     ----------
     Covs : ndarray, shape (n_matrices, n, n)
         Set of SPD matrices.
     Cref : ndarray, shape (n, n)
         The reference SPD matrix.
-    metric : string, default='riemann'
-        The metric used for mean, can be: 'euclid', 'logeuclid', 'riemann'.
+    metric : string, default="riemann"
+        The metric used for mean, can be: "euclid", "logeuclid", "riemann".
 
     Returns
     -------
     out : ndarray, shape (n_matrices, n, n)
         Set of transported SPD matrices.
     """
     C = mean_covariance(Covs, metric=metric)
```

### Comparing `pyriemann-0.5/pyriemann/utils/test.py` & `pyriemann-0.6/pyriemann/utils/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if matrices are square.
     """
     return X.ndim >= 2 and X.shape[-2] == X.shape[-1]
 
 
 def is_sym(X):
     """Check if all matrices are symmetric.
@@ -29,15 +29,15 @@
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are symmetric.
     """
     return is_square(X) and np.allclose(X, np.swapaxes(X, -2, -1))
 
 
 def is_skew_sym(X):
     """Check if all matrices are skew-symmetric.
@@ -45,52 +45,101 @@
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are skew-symmetric.
     """
     return is_square(X) and np.allclose(X, -np.swapaxes(X, -2, -1))
 
 
+def is_hankel(X):
+    """Check if matrix is an Hankel matrix.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n, n)
+        Square matrix.
+
+    Returns
+    -------
+    ret : bool
+        True if Hankel matrix.
+    """
+    if not is_square(X) or X.ndim != 2:
+        return False
+    n, _ = X.shape
+
+    for i in range(n):
+        for j in range(n):
+            if (i + j < n):
+                if (X[i, j] != X[i + j, 0]):
+                    return False
+            else:
+                if (X[i, j] != X[i + j - n + 1, n - 1]):
+                    return False
+
+    return True
+
+
 def is_real(X):
     """Check if all matrices are strictly real.
 
     Better management of numerical imprecisions than np.all(np.isreal()).
 
     Parameters
     ----------
     X : ndarray, shape (..., n, m)
         The set of matrices.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are strictly real.
     """
     return np.allclose(X.imag, np.zeros_like(X.imag))
 
 
+def is_real_type(X):
+    """Check if matrices are real type.
+
+    Parameters
+    ----------
+    X : ndarray, shape (..., n, m)
+        The set of matrices.
+
+    Returns
+    -------
+    ret : bool
+        True if matrices are real type.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+    """
+    return np.isrealobj(X)
+
+
 def is_hermitian(X):
     """Check if all matrices are Hermitian.
 
     Check if all matrices are Hermitian, ie with a symmetric real part and
     a skew-symmetric imaginary part.
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are Hermitian.
     """
     return is_sym(X.real) and is_skew_sym(X.imag)
 
 
 def is_pos_def(X, tol=0.0, fast_mode=False):
     """Check if all matrices are positive definite (PD).
@@ -101,20 +150,20 @@
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
     tol : float, default 0.0
         Threshold below which eigen values are considered zero.
-    fast_mode : boolean, default=False
+    fast_mode : bool, default=False
         Use Cholesky decomposition to avoid computing all eigenvalues.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are positive definite.
     """
     if fast_mode:
         try:
             np.linalg.cholesky(X)
             return True
         except np.linalg.LinAlgError:
@@ -129,15 +178,15 @@
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are positive semi-definite.
     """
     return is_square(X) and np.all(_get_eigenvals(X) >= 0.0)
 
 
 def is_sym_pos_def(X, tol=0.0):
     """Check if all matrices are symmetric positive-definite (SPD).
@@ -147,15 +196,15 @@
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
     tol : float, default 0.0
         Threshold below which eigen values are considered zero.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are symmetric positive-definite.
     """
     return is_sym(X) and is_pos_def(X, tol=tol)
 
 
 def is_sym_pos_semi_def(X):
     """Check if all matrices are symmetric positive semi-definite (SPSD).
@@ -163,15 +212,15 @@
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are symmetric positive semi-definite.
     """
     return is_sym(X) and is_pos_semi_def(X)
 
 
 def is_herm_pos_def(X, tol=0.0):
     """Check if all matrices are Hermitian positive-definite (HPD).
@@ -181,15 +230,15 @@
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
     tol : float, default 0.0
         Threshold below which eigen values are considered zero.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are Hermitian positive-definite.
     """
     return is_hermitian(X) and is_pos_def(X, tol=tol)
 
 
 def is_herm_pos_semi_def(X):
     """Check if all matrices are Hermitian positive semi-definite (HPSD).
@@ -197,11 +246,11 @@
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
-    ret : boolean
+    ret : bool
         True if all matrices are Hermitian positive semi-definite.
     """
     return is_hermitian(X) and is_pos_semi_def(X)
```

### Comparing `pyriemann-0.5/pyriemann/utils/viz.py` & `pyriemann-0.6/pyriemann/utils/viz.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,149 @@
 """Helpers for vizualization."""
+import matplotlib.pyplot as plt
+from matplotlib.patches import Ellipse
+import matplotlib.transforms as transforms
 import numpy as np
+
 from ..embedding import SpectralEmbedding, LocallyLinearEmbedding
 
 
 def plot_embedding(X,
                    y=None,
                    *,
                    metric="riemann",
                    title="Embedding of covariances",
-                   embd_type='Spectral',
+                   embd_type="Spectral",
                    normalize=True):
     """Plot 2D embedding of SPD matrices.
 
     Parameters
     ----------
     X : ndarray, shape (n_matrices, n_channels, n_channels)
         Set of SPD matrices.
     y : None | ndarray, shape (n_matrices,), default=None
         Labels for each matrix.
-    metric : string, default='riemann'
-        Metric used in the embedding. Can be {'riemann' ,'logeuclid' ,
-        'euclid'} for Locally Linear Embedding and {'riemann' ,'logeuclid' ,
-        'euclid' , 'logdet', 'kullback', 'kullback_right', 'kullback_sym'}
+    metric : string, default="riemann"
+        Metric used in the embedding. Can be {"riemann", "logeuclid",
+        "euclid"} for Locally Linear Embedding, and {"riemann", "logeuclid",
+        "euclid", "logdet", "kullback", "kullback_right", "kullback_sym"}
         for Spectral Embedding.
     title : str, default="Embedding of covariances"
-        Title string for plot.
-    embd_type : {'Spectral' ,'LocallyLinear'}, default='Spectral'
+        Title of figure.
+    embd_type : {"Spectral", "LocallyLinear"}, default="Spectral"
         Embedding type.
     normalize : bool, default=True
         If True, the plot is normalized from -1 to +1.
 
     Returns
     -------
     fig : matplotlib figure
         Figure of embedding.
-    """
-    try:
-        import matplotlib.pyplot as plt
-    except ImportError:
-        raise ImportError("Install matplotlib to plot embeddings")
 
-    if embd_type == 'Spectral':
+    Notes
+    -----
+    .. versionadded:: 0.2.6
+    """
+    if embd_type == "Spectral":
         lapl = SpectralEmbedding(n_components=2, metric=metric)
-    elif embd_type == 'LocallyLinear':
+    elif embd_type == "LocallyLinear":
         lapl = LocallyLinearEmbedding(n_components=2,
                                       n_neighbors=X.shape[1],
                                       metric=metric)
     else:
-        raise ValueError("Invalid embedding type. Valid types are: 'Spectral',"
-                         " 'LocallyLinear'")
+        raise ValueError(f"Unknown embedding type {embd_type}. "
+                         "Valid types are: 'Spectral', 'LocallyLinear'.")
 
     embd = lapl.fit_transform(X)
 
     if y is None:
         y = np.ones(embd.shape[0])
 
     fig, ax = plt.subplots(figsize=(7, 7), facecolor="white")
     for label in np.unique(y):
         idx = y == label
         ax.scatter(embd[idx, 0], embd[idx, 1], s=36)
 
     ax.set_xlabel(r"$\varphi_1$", fontsize=16)
     ax.set_ylabel(r"$\varphi_2$", fontsize=16)
-    ax.set_title(f'{embd_type} {title}', fontsize=16)
+    ax.set_title(f"{embd_type} {title}", fontsize=16)
     ax.grid(False)
     if normalize:
         ax.set_xticks([-1.0, -0.5, 0.0, +0.5, 1.0])
         ax.set_yticks([-1.0, -0.5, 0.0, +0.5, 1.0])
     ax.legend(list(np.unique(y)))
 
     return fig
 
 
-def plot_cospectra(cosp, freqs, *, ylabels=None, title="Cospectra"):
+def plot_cospectra(X, freqs, *, ylabels=None, title="Cospectra"):
     """Plot cospectral matrices.
 
     Parameters
     ----------
-    cosp : ndarray, shape (n_freqs, n_channels, n_channels)
+    X : ndarray, shape (n_freqs, n_channels, n_channels)
         Cospectral matrices.
     freqs : ndarray, shape (n_freqs,)
         The frequencies associated to cospectra.
+    ylabels : list of str, default=None
+        ylabels of figure.
+    title : str, default="Cospectra"
+        Title of figure.
 
     Returns
     -------
     fig : matplotlib figure
         Figure of cospectra.
 
     Notes
     -----
     .. versionadded:: 0.2.7
     """
-    try:
-        import matplotlib.pyplot as plt
-    except ImportError:
-        raise ImportError("Install matplotlib to plot cospectra")
-
-    if cosp.ndim != 3:
-        raise Exception('Input cosp has not 3 dimensions')
-    n_freqs, n_channels, _ = cosp.shape
+    if X.ndim != 3:
+        raise ValueError("Input X has not 3 dimensions")
+    n_freqs, n_channels, _ = X.shape
     if freqs.shape != (n_freqs,):
-        raise Exception(
-            'Input freqs has not the same number of frequencies as cosp')
+        raise ValueError(
+            "Input freqs has not the same number of frequencies as X")
 
     fig = plt.figure(figsize=(12, 7))
     fig.suptitle(title)
     for f in range(n_freqs):
         ax = plt.subplot((n_freqs - 1) // 8 + 1, 8, f + 1)
-        plt.imshow(cosp[f], cmap=plt.get_cmap("Reds"))
+        plt.imshow(X[f], cmap=plt.get_cmap("Reds"))
         plt.title("{} Hz".format(freqs[f]))
         plt.xticks([])
         if ylabels and f == 0:
             plt.yticks(np.arange(0, len(ylabels), 2), ylabels[::2])
             ax.tick_params(axis="both", which="major", labelsize=7)
         elif ylabels and f == 8:
             plt.yticks(np.arange(1, len(ylabels), 2), ylabels[1::2])
             ax.tick_params(axis="both", which="major", labelsize=7)
         else:
             plt.yticks([])
 
     return fig
 
 
-def plot_waveforms(X, display, *, times=None, color='gray', alpha=0.5,
-                   linewidth=1.5, color_mean='k', color_std='gray', n_bins=50,
+def plot_waveforms(X, display, *, times=None, color="gray", alpha=0.5,
+                   linewidth=1.5, color_mean="k", color_std="gray", n_bins=50,
                    cmap=None):
-    """ Display repetitions of a multichannel waveform.
+    """Plot repetitions of a multichannel waveform.
 
     Parameters
     ----------
     X : ndarray, shape (n_reps, n_channels, n_times)
         Repetitions of the multichannel waveform.
-    display : {'all', 'mean', 'mean+/-std', 'hist'}
+    display : {"all", "mean", "mean+/-std", "hist"}
         Type of display:
 
-        * 'all' for all the repetitions;
-        * 'mean' for the mean of the repetitions;
-        * 'mean+/-std' for the mean +/- standard deviation of the repetitions;
-        * 'hist' for the 2D histogram of the repetitions.
+        * "all" for all the repetitions;
+        * "mean" for the mean of the repetitions;
+        * "mean+/-std" for the mean +/- standard deviation of the repetitions;
+        * "hist" for the 2D histogram of the repetitions.
     time : None | ndarray, shape (n_times,), default=None
         Values to display on x-axis.
     color : matplotlib color, optional
         Color of the lines, when ``display=all``.
     alpha : float, optional
         Alpha value used to cumulate repetitions, when ``display=all``.
     linewidth : float, optional
@@ -160,56 +162,51 @@
     fig : matplotlib figure
         Figure of waveform (one subplot by channel).
 
     Notes
     -----
     .. versionadded:: 0.3
     """
-    try:
-        import matplotlib.pyplot as plt
-    except ImportError:
-        raise ImportError("Install matplotlib to plot waveforms")
-
     if X.ndim != 3:
-        raise Exception('Input X has not 3 dimensions')
+        raise ValueError("Input X has not 3 dimensions")
     n_reps, n_channels, n_times = X.shape
     if times is None:
         times = np.arange(n_times)
     elif times.shape != (n_times,):
-        raise Exception(
-            'Parameter times has not the same number of values as X')
+        raise ValueError(
+            "Parameter times has not the same number of values as X")
 
     fig, axes = plt.subplots(nrows=n_channels, ncols=1)
     if n_channels == 1:
         axes = [axes]
     channels = np.arange(n_channels)
 
-    if display == 'all':
+    if display == "all":
         for (channel, ax) in zip(channels, axes):
             for i_rep in range(n_reps):
                 ax.plot(times, X[i_rep, channel], c=color, alpha=alpha)
 
-    elif display in ['mean', 'mean+/-std']:
+    elif display in ["mean", "mean+/-std"]:
         mean = np.mean(X, axis=0)
         for (channel, ax) in zip(channels, axes):
             ax.plot(times, mean[channel], c=color_mean, lw=linewidth)
-        if display == 'mean+/-std':
+        if display == "mean+/-std":
             std = np.std(X, axis=0)
             for (channel, ax) in zip(channels, axes):
                 ax.fill_between(times, mean[channel] - std[channel],
                                 mean[channel] + std[channel], color=color_std)
 
-    elif display == 'hist':
+    elif display == "hist":
         times_rep = np.repeat(times[np.newaxis, :], n_reps, axis=0)
         for (channel, ax) in zip(channels, axes):
             ax.hist2d(times_rep.ravel(), X[:, channel, :].ravel(),
                       bins=(n_times, n_bins), cmap=cmap)
 
     else:
-        raise Exception('Parameter display unknown %s' % display)
+        raise ValueError(f"Unknown parameter display {display}")
 
     if n_channels > 1:
         for ax in axes[:-1]:
             ax.set_xticklabels([])  # remove xticklabels
     return fig
 
 
@@ -218,7 +215,154 @@
     try:
         from matplotlib.colors import to_rgb
     except ImportError:
         raise ImportError("Install matplotlib to add alpha")
 
     cols = [to_rgb(c) for c in colors]
     return [(c[0], c[1], c[2], a) for c, a in zip(cols, alphas[-len(cols):])]
+
+
+def plot_cov_ellipse(ax, X, n_std=2.5, **kwds):
+    """Plot 2x2 covariance matrix as an ellipse.
+
+    Parameters
+    ----------
+    ax : matplotlib axis
+        Axis of figure.
+    X : ndarray, shape (2, 2)
+        Covariance matrix.
+    n_std : float, default=2.5
+        Number of standard deviations.
+    **kwds : dict
+        Any further parameters are passed directly to the Ellipse.
+
+    Returns
+    -------
+    ax : matplotlib axis
+        Axis of figure.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+
+    References
+    ----------
+    .. [1] https://matplotlib.org/stable/gallery/statistics/confidence_ellipse.html
+    """  # noqa
+    if X.shape != (2, 2):
+        raise ValueError("Input X must be a 2x2 covariance matrix")
+
+    pearson = X[0, 1] / np.sqrt(X[0, 0] * X[1, 1])
+    ell_radius_x = np.sqrt(1 + pearson)
+    ell_radius_y = np.sqrt(1 - pearson)
+    ellipse = Ellipse((0, 0), width=ell_radius_x * 2, height=ell_radius_y * 2,
+                      facecolor='none', **kwds)
+    scale_x = np.sqrt(X[0, 0]) * n_std
+    scale_y = np.sqrt(X[1, 1]) * n_std
+    transf = transforms.Affine2D().rotate_deg(45).scale(scale_x, scale_y)
+    ellipse.set_transform(transf + ax.transData)
+
+    return ax.add_patch(ellipse)
+
+
+def plot_bihist(X, y, n_bins=10, title="Histogram"):
+    """Plot histogram of bi-class predictions.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices, 2)
+        Predictions, distances or probabilities.
+    y : ndarray, shape (n_matrices,)
+        Labels for each matrix.
+    n_bins : int, default=10
+        Number of bins of histogram.
+    title : str, default="Histogram"
+        Title of figure.
+
+    Returns
+    -------
+    fig : matplotlib figure
+        Figure of histogram.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+    """
+    if X.ndim != 2:
+        raise ValueError("Input X has not 2 dimensions")
+    if X.shape[1] != 2:
+        raise ValueError("Input X has not 2 classes")
+
+    classes = np.unique(y)
+    if classes.shape[0] != 2:
+        raise ValueError("Input y has not 2 labels")
+
+    X = X / np.sum(X, axis=1, keepdims=True)
+    X0 = X[y == classes[0], 0]
+    X1 = 1 - X[y == classes[1], 1]
+
+    def get_bins(X, n_bins, target=0.5):
+        """Estimate bins with the garantee to have target value in bin edges"""
+        bins = np.histogram_bin_edges(X, bins=n_bins)
+        idx = (np.abs(bins - target)).argmin()
+        bins[idx] = target
+        return bins
+
+    fig, ax = plt.subplots(figsize=(6, 5))
+    ax.axvline(x=0.5, c="k", linestyle=":")
+    ax.hist(X0, bins=get_bins(X0, n_bins), label=classes[0], alpha=0.5)
+    ax.hist(X1, bins=get_bins(X1, n_bins), label=classes[1], alpha=0.5)
+
+    (Xmin, Xmax) = ax.get_xlim()
+    Xm = min(Xmin, 1 - Xmax)
+    ax.set_xlim(Xm, 1 - Xm)
+    ax.set(xlabel="Rescaled predictions", ylabel="Frequency", title=title)
+    ax.legend(title="Classes", loc="upper left")
+
+    return fig
+
+
+def plot_biscatter(X, y):
+    """Plot scatter of bi-class predictions.
+
+    Parameters
+    ----------
+    X : ndarray, shape (n_matrices, 2)
+        Predictions, distances or probabilities.
+    y : ndarray, shape (n_matrices,)
+        Labels for each matrix.
+
+    Returns
+    -------
+    fig : matplotlib figure
+        Figure of scatter plot.
+
+    Notes
+    -----
+    .. versionadded:: 0.6
+    """
+
+    if X.ndim != 2:
+        raise ValueError("Input X has not 2 dimensions")
+    if X.shape[1] != 2:
+        raise ValueError("Input X has not 2 classes")
+
+    classes = np.unique(y)
+    if classes.shape[0] != 2:
+        raise ValueError("Input y has not 2 labels")
+
+    X0 = X[y == classes[0]]
+    X1 = X[y == classes[1]]
+
+    fig, ax = plt.subplots(figsize=(7, 7))
+    ax.scatter(X0[:, 0], X0[:, 1], label=classes[0], alpha=1)
+    ax.scatter(X1[:, 0], X1[:, 1], label=classes[1], alpha=0.5)
+    ax.legend(title="Classes", loc="upper left")
+
+    (Xmin, Xmax) = ax.get_xlim()
+    (Ymin, Ymax) = ax.get_ylim()
+    XYmin, XYmax = min(Xmin, Ymin), max(Xmax, Ymax)
+    ax.plot([XYmin, XYmax], [XYmin, XYmax], c="k", linestyle=":")
+    ax.set_xlim([XYmin, XYmax])
+    ax.set_ylim([XYmin, XYmax])
+
+    return fig
```

### Comparing `pyriemann-0.5/pyriemann.egg-info/PKG-INFO` & `pyriemann-0.6/pyriemann.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,78 @@
 Metadata-Version: 2.1
 Name: pyriemann
-Version: 0.5
+Version: 0.6
 Summary: Biosignals classification with Riemannian geometry
 Home-page: https://pyriemann.readthedocs.io
 Author: Alexandre Barachant
 Author-email: alexandre.barachant@gmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://pyriemann.readthedocs.io
 Project-URL: Source, https://github.com/pyRiemann/pyRiemann
 Project-URL: Tracker, https://github.com/pyRiemann/pyRiemann/issues/
 Platform: any
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy!=1.24.0
+Requires-Dist: scipy
+Requires-Dist: scikit-learn>=0.24
+Requires-Dist: joblib
+Requires-Dist: matplotlib
 Provides-Extra: docs
+Requires-Dist: sphinx<=7.0.1,>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-gallery; extra == "docs"
+Requires-Dist: sphinx-bootstrap_theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: mne; extra == "docs"
+Requires-Dist: seaborn; extra == "docs"
+Requires-Dist: pandas; extra == "docs"
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: seaborn; extra == "tests"
+Requires-Dist: flake8; extra == "tests"
 
 # pyRiemann
 
-[![Code PythonVersion](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
+[![Code PythonVersion](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
 [![PyPI version](https://badge.fury.io/py/pyriemann.svg)](https://badge.fury.io/py/pyriemann)
 [![Build Status](https://github.com/pyRiemann/pyRiemann/workflows/testing/badge.svg?branch=master&event=push)](https://github.com/pyRiemann/pyRiemann/actions)
 [![codecov](https://codecov.io/gh/pyRiemann/pyRiemann/branch/master/graph/badge.svg)](https://codecov.io/gh/pyRiemann/pyRiemann)
 [![Documentation Status](https://readthedocs.org/projects/pyriemann/badge/?version=latest)](http://pyriemann.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.593816.svg)](https://doi.org/10.5281/zenodo.593816)
 [![Downloads](https://pepy.tech/badge/pot)](https://pepy.tech/project/pyriemann)
 
 pyRiemann is a Python machine learning package based on [scikit-learn](http://scikit-learn.org/stable/modules/classes.html) API.
-It provides a high-level interface for processing and classification of multivariate time series
-through the Riemannian geometry of symmetric positive definite (SPD) matrices.
-
-pyRiemann aims at being a generic package for multivariate time series classification
-but has been designed around multichannel biosignals (like EEG, MEG or EMG) manipulation applied to brain-computer interface (BCI),
-transforming multichannel time series into covariance matrices, and classifying them using the Riemannian geometry of SPD matrices [[1]](#1).
+It provides a high-level interface for processing and classification of real (*resp*. complex)-valued multivariate data
+through the Riemannian geometry of symmetric (*resp*. Hermitian) 
+[positive definite](https://en.wikipedia.org/wiki/Definite_matrix) (SPD) (*resp*. HPD) matrices.
+
+pyRiemann aims at being a generic package for multivariate data analysis
+but has been designed around [biosignals](https://en.wikipedia.org/wiki/Biosignal) (like EEG, MEG or EMG)
+manipulation applied to [brain-computer interface](https://en.wikipedia.org/wiki/Brain%E2%80%93computer_interface) (BCI),
+estimating [covariance matrices](https://en.wikipedia.org/wiki/Covariance_matrix) from multichannel time series,
+and classifying them using the Riemannian geometry of SPD matrices [[1]](#1).
 
 For BCI applications, studied paradigms are motor imagery [[2]](#2) [[3]](#3), event-related potentials (ERP) [[4]](#4) and steady-state visually evoked potentials (SSVEP) [[5]](#5).
 Using extended labels, API allows transfer learning between sessions or subjects [[6]](#6).
 
-This code is BSD-licenced (3 clause).
+This code is BSD-licensed (3 clause).
 
 ## Documentation
 
 The documentation is available on http://pyriemann.readthedocs.io/en/latest/
 
-## Install
+# Installation
 
 #### Using PyPI
 
 ```
 pip install pyriemann
 ```
-or using pip+git for the latest version of the code :
+or using pip+git for the latest version of the code:
 
 ```
 pip install git+https://github.com/pyRiemann/pyRiemann
 ```
 
 #### Using conda
 
@@ -75,15 +93,15 @@
 
 or in editable mode to be able to modify the sources:
 
 ```shell
 pip install -e .
 ```
 
-## How to use it
+# How to use
 
 Most of the functions mimic the scikit-learn API, and therefore can be directly used with sklearn.
 For example, for cross-validation classification of EEG signal using the MDM algorithm described in [[2]](#2), it is easy as:
 
 ```python
 import pyriemann
 from sklearn.model_selection import cross_val_score
@@ -128,15 +146,15 @@
 # cross validation
 accuracy = cross_val_score(clf, X, y)
 
 print(accuracy.mean())
 
 ```
 
-**Check out the example folder for more examples !**
+**Check out the example folder for more examples.**
 
 # Contribution Guidelines
 
 The package aims at adopting the [scikit-learn](http://scikit-learn.org/stable/developers/contributing.html#contributing-code)
 and [MNE-Python](https://mne.tools/stable/install/contributing.html) conventions as much as possible.
 See their contribution guidelines before contributing to the repository.
 
@@ -163,21 +181,21 @@
                   Gabriel Wagner vom Berg and
                   Ghiles Reguig and
                   Arthur Lebeurrier and
                   Erik Bjäreholt and
                   Maria Sayu Yamamoto and
                   Pierre Clisson and
                   Marie-Constance Corsi},
-  title        = {pyRiemann/pyRiemann: v0.3},
-  month        = jul,
-  year         = 2022,
+  title        = {pyRiemann/pyRiemann: v0.5},
+  month        = june,
+  year         = 2023,
   publisher    = {Zenodo},
-  version      = {v0.3},
-  doi          = {10.5281/zenodo.7547583},
-  url          = {https://doi.org/10.5281/zenodo.7547583}
+  version      = {v0.5},
+  doi          = {10.5281/zenodo.8059038},
+  url          = {https://doi.org/10.5281/zenodo.8059038}
 }
 ```
 
 # References
 
 <a id="1">[1]</a>
 M. Congedo, A. Barachant and R. Bhatia, "Riemannian geometry for EEG-based brain-computer interfaces; a primer and a review".
```

### Comparing `pyriemann-0.5/pyriemann.egg-info/SOURCES.txt` & `pyriemann-0.6/pyriemann.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyriemann-0.5/setup.py` & `pyriemann-0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import sys
 import os.path as op
+import sys
 
-from setuptools import setup, find_packages
-
+from setuptools import find_packages, setup
 
-# get the version (don't import mne here, so dependencies are not needed)
 version = None
 with open(op.join("pyriemann", "_version.py"), "r") as fid:
     for line in (line.strip() for line in fid):
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().strip("'")
             break
 if version is None:
@@ -32,27 +30,33 @@
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://pyriemann.readthedocs.io",
         "Source": "https://github.com/pyRiemann/pyRiemann",
         "Tracker": "https://github.com/pyRiemann/pyRiemann/issues/",
     },
     platforms="any",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "numpy!=1.24.0",
         "scipy",
-        "scikit-learn",
+        "scikit-learn>=0.24",
         "joblib",
+        "matplotlib",
     ],
     extras_require={
         "docs": [
+            "sphinx>=6.0.0,<=7.0.1",
             "sphinx-gallery",
             "sphinx-bootstrap_theme",
             "numpydoc",
             "mne",
             "seaborn",
             "pandas",
         ],
-        "tests": ["pytest", "seaborn", "flake8"],
+        "tests": [
+            "pytest",
+            "seaborn",
+            "flake8"
+        ],
     },
     zip_safe=False,
 )
```

### Comparing `pyriemann-0.5/tests/test_channelselection.py` & `pyriemann-0.6/tests/test_channelselection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from numpy.testing import assert_array_equal
+
 from pyriemann.channelselection import ElectrodeSelection, FlatChannelRemover
 
 
-def test_electrodeselection(get_covmats, get_labels):
+def test_electrodeselection(get_mats, get_labels):
     """Test transform of channelselection."""
     n_matrices, n_channels, n_classes = 10, 30, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     se = ElectrodeSelection()
     se.fit(covmats, labels)
     se.transform(covmats)
 
 
-def test_electrodeselection_nonelabel(get_covmats):
+def test_electrodeselection_nonelabel(get_mats):
     n_matrices, n_channels = 1, 3
-    covmats, labels = get_covmats(n_matrices, n_channels), None
+    covmats, labels = get_mats(n_matrices, n_channels, "spd"), None
     se = ElectrodeSelection()
     se.fit(covmats, labels)
     se.transform(covmats)
 
 
 def test_flatchannelremover(rndstate):
     n_matrices, n_channels, n_times = 10, 3, 100
```

### Comparing `pyriemann-0.5/tests/test_classification.py` & `pyriemann-0.6/tests/test_classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,72 @@
 import pickle
 
 import numpy as np
 from numpy.testing import assert_array_equal
 import pytest
 from pytest import approx
+from scipy.stats import mode
 from sklearn.dummy import DummyClassifier
 
 from conftest import get_distances, get_means, get_metrics
 from pyriemann.estimation import Covariances
 from pyriemann.utils.kernel import kernel
 from pyriemann.utils.mean import mean_covariance
 from pyriemann.classification import (
+    _mode_2d,
     MDM,
     FgMDM,
     KNearestNeighbor,
     TSclassifier,
     SVC,
     MeanField,
     class_distinctiveness,
 )
 
 rclf = [MDM, FgMDM, KNearestNeighbor, TSclassifier, SVC, MeanField]
 
 
+@pytest.mark.parametrize(
+    "X, axis, expected",
+    [
+        (
+            np.array([[0, 5], [1, 7], [0, 6], [2, 7]]),
+            0,
+            np.array([0, 7]),
+        ),
+        (
+            np.array([[0, 1, 2, 1, 1, 0], [7, 5, 7, 6, 7, 6]]),
+            1,
+            np.array([1, 7]),
+        ),
+        (
+            np.array([['a', 'b', 'a', 'c', 'a'], ['d', 'e', 'f', 'e', 'e']]),
+            1,
+            np.array(['a', 'e']),
+        ),
+    ],
+)
+def test_mode(X, axis, expected):
+    actual = _mode_2d(X, axis=axis)
+    assert_array_equal(actual, expected)
+
+    if np.issubdtype(X.dtype, np.number):
+        sp, _ = mode(X, axis=axis)
+        assert_array_equal(actual, sp.ravel())
+
+
 @pytest.mark.parametrize("n_classes", [2, 3])
 @pytest.mark.parametrize("classif", rclf)
-def test_classifier(n_classes, classif, get_covmats, get_labels):
+def test_classifier(n_classes, classif, get_mats, get_labels):
     if n_classes == 2:
         n_matrices, n_channels = 6, 3
     else:
         assert n_classes == 3
         n_matrices, n_channels = 9, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
 
     clf_predict(classif, covmats, labels)
     clf_fit_independence(classif, covmats, labels)
     clf_predict_proba(classif, covmats, labels)
     clf_score(classif, covmats, labels)
     clf_populate_classes(classif, covmats, labels)
@@ -114,111 +145,114 @@
     clf = classif(tsupdate=True)
     clf.fit(covmats, labels).predict(covmats)
 
 
 @pytest.mark.parametrize("classif", rclf)
 @pytest.mark.parametrize("mean", ["faulty", 42])
 @pytest.mark.parametrize("dist", ["not_real", 27])
-def test_metric_dict_error(classif, mean, dist, get_covmats, get_labels):
+def test_metric_dict_error(classif, mean, dist, get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = classif(metric={"mean": mean, "distance": dist})
     with pytest.raises((TypeError, KeyError, ValueError)):
         clf.fit(covmats, labels).predict(covmats)
 
 
 @pytest.mark.parametrize("classif", rclf)
 @pytest.mark.parametrize("metric", [42, "faulty", {"foo": "bar"}])
-def test_metric_errors(classif, metric, get_covmats, get_labels):
+def test_metric_errors(classif, metric, get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = classif(metric=metric)
     with pytest.raises((TypeError, KeyError, ValueError)):
         clf.fit(covmats, labels).predict(covmats)
 
 
 @pytest.mark.parametrize("classif", rclf)
 @pytest.mark.parametrize("metric", get_metrics())
-def test_metric_str(classif, metric, get_covmats, get_labels):
+def test_metric_str(classif, metric, get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = classif(metric=metric)
 
     if classif in [SVC, FgMDM, TSclassifier] \
             and metric not in ['riemann', 'euclid', 'logeuclid']:
         with pytest.raises((KeyError, ValueError)):
             clf.fit(covmats, labels).predict(covmats)
     else:
         clf.fit(covmats, labels).predict(covmats)
 
 
 @pytest.mark.parametrize("metric_mean", get_means())
 @pytest.mark.parametrize("metric_dist", get_distances())
-def test_metric_mdm(metric_mean, metric_dist, get_covmats, get_labels):
-    n_matrices, n_channels, n_classes = 4, 3, 2
+@pytest.mark.parametrize("n_classes", [2, 3, 4])
+def test_metric_mdm(metric_mean, metric_dist, n_classes, get_mats, get_labels):
+    n_matrices, n_channels = 4 * n_classes, 3
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = MDM(metric={"mean": metric_mean, "distance": metric_dist})
     clf.fit(covmats, labels).predict(covmats)
+    assert clf.classes_.shape == (n_classes,)
+    assert clf.covmeans_.shape == (n_classes, n_channels, n_channels)
 
 
 @pytest.mark.parametrize("metric_mean", get_means())
 @pytest.mark.parametrize("metric_dist", get_distances())
 @pytest.mark.parametrize("metric_map", ["euclid", "logeuclid", "riemann"])
-def test_metric_fgmdm(metric_mean, metric_dist, metric_map, get_covmats,
+def test_metric_fgmdm(metric_mean, metric_dist, metric_map, get_mats,
                       get_labels):
     n_matrices, n_channels, n_classes = 4, 3, 2
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = FgMDM(metric={
         "mean": metric_mean,
         "distance": metric_dist,
         "map": metric_map
     })
     clf.fit(covmats, labels).predict(covmats)
 
 
 @pytest.mark.parametrize("metric_mean", get_means())
 @pytest.mark.parametrize("metric_map", ["euclid", "logeuclid", "riemann"])
-def test_metric_tsclassifier(metric_mean, metric_map, get_covmats, get_labels):
+def test_metric_tsclassifier(metric_mean, metric_map, get_mats, get_labels):
     n_matrices, n_channels, n_classes = 4, 3, 2
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = TSclassifier(metric={"mean": metric_mean, "map": metric_map})
     clf.fit(covmats, labels).predict(covmats)
 
 
-def test_1nn(get_covmats, get_labels):
+def test_1nn(get_mats, get_labels):
     """Test KNearestNeighbor with K=1"""
     n_matrices, n_channels, n_classes = 9, 3, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
 
     knn = KNearestNeighbor(1, metric="riemann")
     knn.fit(covmats, labels)
     preds = knn.predict(covmats)
     assert_array_equal(labels, preds)
 
 
-def test_tsclassifier_fit(get_covmats, get_labels):
+def test_tsclassifier_fit(get_mats, get_labels):
     """Test TS Classifier"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     clf = TSclassifier(clf=DummyClassifier())
     clf.fit(covmats, labels).predict(covmats)
 
 
-def test_tsclassifier_clf_error(get_covmats, get_labels):
+def test_tsclassifier_clf_error(get_mats, get_labels):
     """Test TS if not Classifier"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     with pytest.raises(TypeError):
         TSclassifier(clf=Covariances()).fit(covmats, labels)
 
 
 def test_svc_params():
     rsvc = SVC()
@@ -227,42 +261,42 @@
     rsvc.set_params(**{'metric': 'logeuclid'})
     assert rsvc.metric == 'logeuclid'
 
     rsvc.set_params(**{'max_iter': 501})
     assert rsvc.max_iter == 501
 
 
-def test_svc_params_error(get_covmats, get_labels):
+def test_svc_params_error(get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
 
     with pytest.raises(TypeError):
         SVC(C='hello').fit(covmats, labels)
 
     with pytest.raises(TypeError):
         SVC(foo=5)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_cref_metric(get_covmats, get_labels, metric):
+def test_svc_cref_metric(get_mats, get_labels, metric):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     Cref = mean_covariance(covmats, metric=metric)
 
     rsvc = SVC(Cref=Cref).fit(covmats, labels)
     rsvc_1 = SVC(Cref=None, metric=metric).fit(covmats, labels)
     assert np.array_equal(rsvc.Cref_, rsvc_1.Cref_)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_cref_callable(get_covmats, get_labels, metric):
+def test_svc_cref_callable(get_mats, get_labels, metric):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     def Cref(X): return mean_covariance(X, metric=metric)
 
     rsvc = SVC(Cref=Cref).fit(covmats, labels)
     rsvc_1 = SVC(metric=metric).fit(covmats, labels)
     assert np.array_equal(rsvc.Cref_, rsvc_1.Cref_)
 
@@ -270,84 +304,99 @@
     rsvc.predict(covmats)
     rsvc_1 = SVC(metric=metric).fit(covmats, labels)
     rsvc_1.predict(covmats)
     assert np.array_equal(rsvc.Cref_, rsvc_1.Cref_)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_cref_error(get_covmats, get_labels, metric):
+def test_svc_cref_error(get_mats, get_labels, metric):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     def Cref(X, met): mean_covariance(X, metric=met)
 
     with pytest.raises(TypeError):
         SVC(Cref=Cref).fit(covmats, labels)
 
     Cref = metric
 
     with pytest.raises(TypeError):
         SVC(Cref=Cref).fit(covmats, labels)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_kernel_callable(get_covmats, get_labels, metric):
+def test_svc_kernel_callable(get_mats, get_labels, metric):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
 
-    rsvc = SVC(kernel_fct=kernel,
-               metric=metric).fit(covmats, labels)
+    rsvc = SVC(kernel_fct=kernel, metric=metric).fit(covmats, labels)
     rsvc_1 = SVC(metric=metric).fit(covmats, labels)
     p1 = rsvc.predict(covmats[:-1])
     p2 = rsvc_1.predict(covmats[:-1])
     assert np.array_equal(p1, p2)
 
     def custom_kernel(X, Y, Cref, metric):
         return np.ones((len(X), len(Y)))
     SVC(kernel_fct=custom_kernel,
         metric=metric).fit(covmats, labels).predict(covmats[:-1])
 
+    # check if pickleable
+    pickle.dumps(rsvc)
+    pickle.dumps(rsvc_1)
+
+
+@pytest.mark.parametrize("kernel_fct", [None, "precomputed"])
+@pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
+def test_svc_kernel_precomputed(get_mats, get_labels, kernel_fct, metric):
+    n_matrices, n_channels, n_classes = 6, 3, 2
+    covmats = get_mats(n_matrices, n_channels, "spd")
+    labels = get_labels(n_matrices, n_classes)
+
+    SVC(kernel_fct=kernel_fct, metric=metric).fit(covmats, labels)
+
+
+def test_svc_kernel_error(get_mats, get_labels):
+    n_matrices, n_channels, n_classes = 4, 2, 2
+    covmats = get_mats(n_matrices, n_channels, "spd")
+    labels = get_labels(n_matrices, n_classes)
+
     def custom_kernel(X, Y, Cref):
         return np.ones((len(X), len(Y)))
     with pytest.raises(TypeError):
-        SVC(kernel_fct=custom_kernel, metric=metric).fit(covmats, labels)
+        SVC(kernel_fct=custom_kernel, metric="euclid").fit(covmats, labels)
 
     custom_kernel = np.array([1, 2])
     with pytest.raises(TypeError):
-        SVC(kernel_fct=custom_kernel, metric=metric).fit(covmats, labels)
-
-    # check if pickleable
-    pickle.dumps(rsvc)
-    pickle.dumps(rsvc_1)
+        SVC(kernel_fct=custom_kernel, metric="riemann").fit(covmats, labels)
 
 
 @pytest.mark.parametrize("method_label", ["sum_means", "inf_means"])
-def test_meanfield(get_covmats, get_labels, method_label):
+def test_meanfield(get_mats, get_labels, method_label):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     mf = MeanField(method_label=method_label).fit(covmats, labels)
     pred = mf.predict(covmats)
     assert pred.shape == (n_matrices,)
     proba = mf.predict_proba(covmats)
     assert proba.shape == (n_matrices, n_classes)
     transf = mf.transform(covmats)
     assert transf.shape == (n_matrices, n_classes)
 
 
 @pytest.mark.parametrize("n_classes", [1, 2, 3])
 @pytest.mark.parametrize("metric_mean", get_means())
 @pytest.mark.parametrize("metric_dist", get_distances())
 @pytest.mark.parametrize("exponent", [1, 2])
-def test_class_distinctiveness(get_covmats, get_labels,
+def test_class_distinctiveness(get_mats, get_labels,
                                n_classes, metric_mean, metric_dist, exponent):
     """Test function for class distinctiveness measure for two class problem"""
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     if n_classes == 1:
         with pytest.raises(ValueError):
             class_distinctiveness(covmats, labels)
         return
 
     class_dis, num, denom = class_distinctiveness(
```

### Comparing `pyriemann-0.5/tests/test_clustering.py` & `pyriemann-0.6/tests/test_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from conftest import get_metrics
 import numpy as np
 from numpy.testing import assert_array_equal
 import pytest
-from pyriemann.clustering import (Kmeans, KmeansPerClassTransform, Potato,
-                                  PotatoField)
+
+from conftest import get_metrics
+from pyriemann.clustering import (
+    Kmeans,
+    KmeansPerClassTransform,
+    Potato,
+    PotatoField,
+)
 
 
 @pytest.mark.parametrize(
     "clust", [Kmeans, KmeansPerClassTransform, Potato, PotatoField]
 )
 class ClusteringTestCase:
-    def test_two_clusters(self, clust, get_covmats, get_labels):
+    def test_two_clusters(self, clust, get_mats, get_labels):
         n_clusters = 2
         n_matrices, n_channels = 6, 4
-        covmats = get_covmats(n_matrices, n_channels)
+        covmats = get_mats(n_matrices, n_channels, "spd")
         if clust is Kmeans:
             self.clf_predict(clust, covmats, n_clusters)
             self.clf_transform(clust, covmats, n_clusters)
             self.clf_jobs(clust, covmats, n_clusters)
             self.clf_centroids(clust, covmats, n_clusters)
             self.clf_fit_independence(clust, covmats)
         if clust is KmeansPerClassTransform:
@@ -30,27 +35,27 @@
             self.clf_transform(clust, covmats)
             self.clf_predict(clust, covmats)
             self.clf_predict_proba(clust, covmats)
             self.clf_partial_fit(clust, covmats)
             self.clf_fit_independence(clust, covmats)
         if clust is PotatoField:
             n_potatoes = 3
-            covmats = [get_covmats(n_matrices, n_channels),
-                       get_covmats(n_matrices, n_channels + 2),
-                       get_covmats(n_matrices, n_channels + 1)]
+            covmats = [get_mats(n_matrices, n_channels, "spd"),
+                       get_mats(n_matrices, n_channels + 2, "spd"),
+                       get_mats(n_matrices, n_channels + 1, "spd")]
             self.clf_transform(clust, covmats, n_potatoes)
             self.clf_predict(clust, covmats, n_potatoes)
             self.clf_predict_proba(clust, covmats, n_potatoes)
             self.clf_partial_fit(clust, covmats, n_potatoes)
             self.clf_fit_independence(clust, covmats, n_potatoes)
 
-    def test_three_clusters(self, clust, get_covmats, get_labels):
+    def test_three_clusters(self, clust, get_mats, get_labels):
         n_clusters = 3
         n_matrices, n_channels = 6, 3
-        covmats = get_covmats(n_matrices, n_channels)
+        covmats = get_mats(n_matrices, n_channels, "spd")
         if clust is Kmeans:
             self.clf_predict(clust, covmats, n_clusters)
             self.clf_transform(clust, covmats, n_clusters)
             self.clf_jobs(clust, covmats, n_clusters)
             self.clf_centroids(clust, covmats, n_clusters)
             self.clf_fit_independence(clust, covmats)
         if clust is KmeansPerClassTransform:
@@ -160,17 +165,17 @@
         clf.fit(new_covmats, labels).transform(new_covmats)
 
 
 @pytest.mark.parametrize("clust", [Kmeans, KmeansPerClassTransform])
 @pytest.mark.parametrize("init", ["random", "ndarray"])
 @pytest.mark.parametrize("n_init", [1, 5])
 @pytest.mark.parametrize("metric", get_metrics())
-def test_km_init_metric(clust, init, n_init, metric, get_covmats, get_labels):
+def test_km_init_metric(clust, init, n_init, metric, get_mats, get_labels):
     n_clusters, n_matrices, n_channels = 2, 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_clusters)
     if init == "ndarray":
         clf = clust(
             n_clusters=n_clusters,
             metric=metric,
             init=covmats[:n_clusters],
             n_init=n_init,
@@ -180,95 +185,95 @@
             n_clusters=n_clusters, metric=metric, init=init, n_init=n_init
         )
     clf.fit(covmats, labels)
     transformed = clf.transform(covmats)
     assert len(transformed) == n_matrices
 
 
-def test_potato_fit_equal_labels(get_covmats):
+def test_potato_fit_equal_labels(get_mats):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         Potato(pos_label=0).fit(covmats)
 
 
 @pytest.mark.parametrize("y_fail", [[1], [0] * 6, [0] * 7, [0, 1, 2] * 2])
-def test_potato_fit_error(y_fail, get_covmats):
+def test_potato_fit_error(y_fail, get_mats):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         Potato().fit(covmats, y=y_fail)
 
 
-def test_potato_partial_fit_not_fitted(get_covmats):
+def test_potato_partial_fit_not_fitted(get_mats):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):  # potato not fitted
         Potato().partial_fit(covmats)
 
 
-def test_potato_partial_fit_diff_channels(get_covmats, get_labels):
+def test_potato_partial_fit_diff_channels(get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     pt = Potato().fit(covmats, labels)
     with pytest.raises(ValueError):  # unequal # of chans
-        pt.partial_fit(get_covmats(2, n_channels + 1))
+        pt.partial_fit(get_mats(2, n_channels + 1, "spd"))
 
 
-def test_potato_partial_fit_no_poslabel(get_covmats, get_labels):
+def test_potato_partial_fit_no_poslabel(get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     pt = Potato().fit(covmats, labels)
     with pytest.raises(ValueError):  # no positive labels
         pt.partial_fit(covmats, [0] * n_matrices)
 
 
 @pytest.mark.parametrize("alpha", [-0.1, 1.1])
-def test_potato_partial_fit_alpha(alpha, get_covmats, get_labels):
+def test_potato_partial_fit_alpha(alpha, get_mats, get_labels):
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     pt = Potato().fit(covmats, labels)
     with pytest.raises(ValueError):
         pt.partial_fit(covmats, labels, alpha=alpha)
 
 
-def test_potato_1channel(get_covmats):
+def test_potato_1channel(get_mats):
     n_matrices, n_channels = 6, 1
-    covmats_1chan = get_covmats(n_matrices, n_channels)
+    covmats_1chan = get_mats(n_matrices, n_channels, "spd")
     pt = Potato()
     pt.fit_transform(covmats_1chan)
     pt.predict(covmats_1chan)
     pt.predict_proba(covmats_1chan)
 
 
-def test_potato_threshold(get_covmats):
+def test_potato_threshold(get_mats):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     pt = Potato(threshold=2.5)
     pt.fit(covmats)
 
 
-def test_potato_specific_labels(get_covmats):
+def test_potato_specific_labels(get_mats):
     n_matrices, n_channels = 10, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     covmats[-1] = 10 * np.eye(n_channels)
     pt = Potato(threshold=2.0, pos_label=2, neg_label=7)
     pt.fit(covmats)
     assert_array_equal(np.unique(pt.predict(covmats)), [2, 7])
     # fit with custom positive label
     pt.fit(covmats, y=[2] * n_matrices)
 
 
-def test_potato_field_fit(get_covmats):
+def test_potato_field_fit(get_mats):
     n_potatoes, n_matrices, n_channels = 2, 6, 3
-    covmats1 = get_covmats(n_matrices, n_channels)
-    covmats2 = get_covmats(n_matrices, n_channels + 1)
+    covmats1 = get_mats(n_matrices, n_channels, "spd")
+    covmats2 = get_mats(n_matrices, n_channels + 1, "spd")
     covmats = [covmats1, covmats2]
     with pytest.raises(ValueError):  # n_potatoes too low
         PotatoField(n_potatoes=0).fit(covmats)
     with pytest.raises(ValueError):   # p_threshold out of bounds
         PotatoField(p_threshold=0).fit(covmats)
     with pytest.raises(ValueError):  # p_threshold out of bounds
         PotatoField(p_threshold=1).fit(covmats)
@@ -277,17 +282,17 @@
         pf.fit([covmats1, covmats1, covmats2])
     with pytest.raises(ValueError):  # n_matrices not equal
         pf.fit([covmats1, covmats2[:1]])
 
 
 @pytest.mark.parametrize("method",
                          ["partial_fit", "transform", "predict_proba"])
-def test_potato_field_method(get_covmats, method):
+def test_potato_field_method(get_mats, method):
     n_potatoes, n_matrices, n_channels = 2, 6, 3
-    covmats1 = get_covmats(n_matrices, n_channels)
-    covmats2 = get_covmats(n_matrices, n_channels + 1)
+    covmats1 = get_mats(n_matrices, n_channels, "spd")
+    covmats2 = get_mats(n_matrices, n_channels + 1, "spd")
     covmats = [covmats1, covmats2]
     pf = PotatoField(n_potatoes=n_potatoes).fit(covmats)
     with pytest.raises(ValueError):  # n_potatoes not equal to input length
         getattr(pf, method)([covmats1, covmats1, covmats2])
     with pytest.raises(ValueError):  # n_matrices not equal
         getattr(pf, method)([covmats1, covmats2[:1]])
```

### Comparing `pyriemann-0.5/tests/test_embedding.py` & `pyriemann-0.6/tests/test_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from conftest import get_metrics
 import numpy as np
+import pytest
 from sklearn.neighbors import NearestCentroid
 
+from conftest import get_metrics
 from pyriemann.datasets import make_gaussian_blobs
-from pyriemann.embedding import (SpectralEmbedding,
-                                 LocallyLinearEmbedding,
-                                 barycenter_weights,
-                                 locally_linear_embedding)
-import pytest
+from pyriemann.embedding import (
+    SpectralEmbedding,
+    LocallyLinearEmbedding,
+    barycenter_weights,
+    locally_linear_embedding,
+)
 
 rembd = [SpectralEmbedding, LocallyLinearEmbedding]
-n_comp = [2, 4, 100]
 
 
 @pytest.mark.parametrize("embd", rembd)
 class EmbeddingTestCase:
-    def test_embedding_build(self, embd, get_covmats):
+    def test_embedding_build(self, embd, get_mats):
         n_matrices, n_channels, n_comp = 8, 3, 4
-        covmats = get_covmats(n_matrices, n_channels)
+        covmats = get_mats(n_matrices, n_channels, "spd")
 
         self.embd_fit(embd, covmats, n_comp)
         self.embd_fit_transform(embd, covmats, n_comp)
         self.embd_fit_independence(embd, covmats, n_comp)
         if 'transform' in embd.__dict__.keys():
             self.embd_transform(embd, covmats, n_comp)
             self.embd_transform_error(embd, covmats, n_comp)
@@ -77,45 +78,45 @@
 
         embd = embedding(n_components=1)
         X_ = embd.fit_transform(X)
         score = NearestCentroid().fit(X_, y).score(X_, y)
         assert score == 1.
 
 
-@pytest.mark.parametrize("n_components", n_comp)
+@pytest.mark.parametrize("n_components", [2, 4, 100])
 @pytest.mark.parametrize("embd", rembd)
-def embd_n_comp(n_components, embd, get_covmats):
+def embd_n_comp(n_components, embd, get_mats):
     n_matrices, n_channels = 8, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     embd = embd(n_components=n_components)
     if n_matrices <= n_components:
         with pytest.raises(AssertionError):
             embd.fit(covmats)
     else:
         embd.fit(covmats)
 
 
 @pytest.mark.parametrize("metric", get_metrics())
 @pytest.mark.parametrize("eps", [None, 0.1])
-def test_spectral_embedding_parameters(metric, eps, get_covmats):
+def test_spectral_embedding_parameters(metric, eps, get_mats):
     """Test SpectralEmbedding."""
     n_matrices, n_channels, n_comp = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     embd = SpectralEmbedding(metric=metric, n_components=n_comp, eps=eps)
     covembd = embd.fit_transform(covmats)
     assert covembd.shape == (n_matrices, n_comp)
 
 
 @pytest.mark.parametrize("metric", ['riemann', 'euclid', 'logeuclid'])
 @pytest.mark.parametrize("n_neighbors", [2, 4, 8, 16])
 @pytest.mark.parametrize("reg", [1e-3, 0])
-def test_locally_linear_parameters(metric, n_neighbors, reg, get_covmats):
-    """Test SpectralEmbedding."""
+def test_locally_linear_parameters(metric, n_neighbors, reg, get_mats):
+    """Test LocallyLinearEmbedding."""
     n_matrices, n_channels, n_comp = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
 
     if n_matrices <= n_neighbors:
         with pytest.raises(AssertionError):
             embd = LocallyLinearEmbedding(metric=metric,
                                           n_components=n_comp,
                                           n_neighbors=n_neighbors)
             embd.fit(covmats)
@@ -123,25 +124,25 @@
         embd = LocallyLinearEmbedding(metric=metric,
                                       n_components=n_comp,
                                       n_neighbors=n_neighbors)
         covembd = embd.fit_transform(covmats)
         assert covembd.shape == (n_matrices, n_comp)
 
 
-def test_barycenter_weights(get_covmats):
+def test_barycenter_weights(get_mats):
     """Test barycenter_weights helper function."""
     n_matrices, n_channels = 4, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     weights = barycenter_weights(covmats, covmats, np.array([[1, 2], [2, 3],
                                                              [3, 0], [0, 1]]))
     assert weights.shape == (n_matrices, 2)
 
 
-def test_locally_linear_embedding(get_covmats):
+def test_locally_linear_embedding(get_mats):
     """Test locally_linear_embedding helper function."""
     n_matrices, n_channels, n_comps, n_neighbors = 4, 3, 2, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     embedding, error = locally_linear_embedding(covmats,
                                                 n_neighbors=n_neighbors,
                                                 n_components=n_comps)
     assert embedding.shape == (n_matrices, n_comps)
     assert isinstance(error, float)
```

### Comparing `pyriemann-0.5/tests/test_estimation.py` & `pyriemann-0.6/tests/test_estimation.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,29 @@
 )
 import pytest
 
 from pyriemann.estimation import (
     Covariances,
     ERPCovariances,
     XdawnCovariances,
+    CrossSpectra,
+    CoSpectra,
     CospCovariances,
+    TimeDelayCovariances,
     HankelCovariances,
     Coherences,
     Shrinkage,
     BlockCovariances,
     Kernels,
 )
 from pyriemann.utils.test import (
     is_sym_pos_def as is_spd,
     is_sym_pos_semi_def as is_spsd,
+    is_herm_pos_semi_def as is_hpsd,
+    is_hankel
 )
 
 estim = ['corr', 'cov', 'lwf', 'mcd', 'oas', 'sch', 'scm']
 m_estim = ['hub', 'stu', 'tyl']
 coh = ["ordinary", "instantaneous", "lagged", "imaginary"]
 
 
@@ -58,28 +63,57 @@
     covs_none = Covariances(estimator=estimator).fit_transform(x)
     covs_kwds = Covariances(estimator=estimator, **kwds).fit_transform(x)
     assert_raises(
         AssertionError, assert_array_equal, covs_none, covs_kwds
     )
 
 
-@pytest.mark.parametrize("delays", [4, [1, 2]])
-def test_hankel_covariances_delays(delays, rndstate):
+def test_time_delay_covariances_xtd():
+    x = np.array([
+        [[1, 2, 3, 4, 5], [11, 12, 13, 14, 15]],
+        [[-1, -2, -3, -4, -5], [-11, -12, -13, -14, -15]]
+    ])
+    cov = TimeDelayCovariances(delays=[1])
+    cov.fit_transform(x)
+
+    xtd = np.array([
+        [[1, 2, 3, 4, 5], [11, 12, 13, 14, 15],
+         [5, 1, 2, 3, 4], [15, 11, 12, 13, 14]],
+        [[-1, -2, -3, -4, -5], [-11, -12, -13, -14, -15],
+         [-5, -1, -2, -3, -4], [-15, -11, -12, -13, -14]]
+    ])
+    assert_array_equal(cov.Xtd_, xtd)
+
+
+@pytest.mark.parametrize("delays", [4, [1, 5]])
+def test_time_delay_covariances(delays, rndstate):
     n_matrices, n_channels, n_times = 2, 3, 100
     x = rndstate.randn(n_matrices, n_channels, n_times)
-    cov = HankelCovariances(delays=delays).fit(x)
+    cov = TimeDelayCovariances(delays=delays)
     covmats = cov.fit_transform(x)
     assert cov.get_params() == dict(estimator="scm", delays=delays)
-    if isinstance(delays, list):
-        n_delays = 1 + len(delays)
-    elif isinstance(delays, int):
+    if isinstance(delays, int):
         n_delays = delays
+    elif isinstance(delays, list):
+        n_delays = 1 + len(delays)
+
     assert covmats.shape == (n_matrices, n_delays * n_channels,
                              n_delays * n_channels)
+    assert cov.Xtd_.shape == (n_matrices, n_delays * n_channels, n_times)
     assert is_spd(covmats)
+    assert ~is_hankel(covmats[0])
+
+
+def test_hankel_covariances():
+    import warnings
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        HankelCovariances()
+        assert len(w) == 1
+        assert issubclass(w[-1].category, DeprecationWarning)
 
 
 @pytest.mark.parametrize("estimator", estim)
 @pytest.mark.parametrize("svd", [None, 2, 3, 4])
 @pytest.mark.parametrize("n_classes", [2, 3, 4])
 def test_erp_covariances(estimator, svd, n_classes, rndstate, get_labels):
     """Test fit ERPCovariances"""
@@ -229,27 +263,39 @@
     n_matrices, n_channels, n_times = 2, 12, 100
     x = rndstate.randn(n_matrices, n_channels, n_times)
     cov = BlockCovariances(block_size='[4, 4, 5]')
     with pytest.raises(ValueError):
         cov.fit_transform(x)
 
 
-def test_cosp_covariances(rndstate):
-    """Test fit CospCovariances"""
+@pytest.mark.parametrize("estim", [CrossSpectra, CoSpectra])
+def test_xspectra(estim, rndstate):
+    """Test CrossSpectra and CoSpectra"""
     n_matrices, n_channels, n_times = 2, 3, 1000
     x = rndstate.randn(n_matrices, n_channels, n_times)
-    cov = CospCovariances()
-    cov.fit(x)
-    covmats = cov.transform(x)
-    assert cov.get_params() == dict(
+    spectra = estim().fit(x)
+    mats = spectra.transform(x)
+    assert spectra.get_params() == dict(
         window=128, overlap=0.75, fmin=None, fmax=None, fs=None
     )
     n_freqs = 65
-    assert covmats.shape == (n_matrices, n_channels, n_channels, n_freqs)
-    assert is_spsd(covmats.transpose(0, 3, 1, 2))
+    assert mats.shape == (n_matrices, n_channels, n_channels, n_freqs)
+    if estim is CoSpectra:
+        assert is_spsd(mats.transpose(0, 3, 1, 2))
+    else:
+        assert is_hpsd(mats.transpose(0, 3, 1, 2))
+
+
+def test_cosp_covariances():
+    import warnings
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        CospCovariances()
+        assert len(w) == 1
+        assert issubclass(w[-1].category, DeprecationWarning)
 
 
 @pytest.mark.parametrize("coh", coh)
 def test_coherences(coh, rndstate):
     """Test fit Coherences"""
     n_matrices, n_channels, n_times = 2, 5, 200
     x = rndstate.randn(n_matrices, n_channels, n_times)
```

### Comparing `pyriemann-0.5/tests/test_preprocessing.py` & `pyriemann-0.6/tests/test_preprocessing.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 def test_whitening_init():
     whit = Whitening()
     assert whit.metric == "euclid"
     assert whit.dim_red is None
     assert not whit.verbose
 
 
-def test_whitening_error(rndstate, get_covmats):
+def test_whitening_error(rndstate, get_mats):
     """Test Whitening"""
     n_matrices, n_channels = 20, 6
-    cov = get_covmats(n_matrices, n_channels)
+    cov = get_mats(n_matrices, n_channels, "spd")
     # Test Fit
     with pytest.raises(ValueError):  # len dim_red not equal to 1
         Whitening(dim_red={"n_components": 2, "expl_var": 0.5}).fit(cov)
     with pytest.raises(ValueError):  # n_components not superior to 1
         Whitening(dim_red={"n_components": 0}).fit(cov)
     with pytest.raises(ValueError):  # n_components not a int
         Whitening(dim_red={"n_components": 2.5}).fit(cov)
@@ -46,18 +46,18 @@
         Whitening(dim_red="max_cond").fit(cov)
     with pytest.raises(ValueError):  # unknown type
         Whitening(dim_red=20).fit(cov)
 
 
 @pytest.mark.parametrize("dim_red", dim_red)
 @pytest.mark.parametrize("metric", ["euclid", "logeuclid", "riemann"])
-def test_whitening_fit(dim_red, metric, rndstate, get_covmats):
+def test_whitening_fit(dim_red, metric, rndstate, get_mats):
     """Test Whitening fit"""
     n_matrices, n_channels = 20, 6
-    cov = get_covmats(n_matrices, n_channels)
+    cov = get_mats(n_matrices, n_channels, "spd")
 
     w = rndstate.rand(n_matrices)
     whit = Whitening(dim_red=dim_red, metric=metric).fit(cov, sample_weight=w)
     if dim_red is None:
         n_comp = n_channels
     else:
         n_comp = whit.n_components_
@@ -68,18 +68,18 @@
         assert whit.n_components_ == n_comp
     assert whit.filters_.shape == (n_channels, n_comp)
     assert whit.inv_filters_.shape == (n_comp, n_channels)
 
 
 @pytest.mark.parametrize("dim_red", dim_red)
 @pytest.mark.parametrize("metric", ["euclid", "logeuclid", "riemann"])
-def test_whitening_transform(dim_red, metric, rndstate, get_covmats):
+def test_whitening_transform(dim_red, metric, rndstate, get_mats):
     """Test Whitening transform"""
     n_matrices, n_channels = 20, 6
-    cov = get_covmats(n_matrices, n_channels)
+    cov = get_mats(n_matrices, n_channels, "spd")
     whit = Whitening(metric=metric).fit(cov)
     cov_w = whit.transform(cov)
     if dim_red is None:
         n_comp = n_channels
     else:
         n_comp = whit.n_components_
     assert cov_w.shape == (n_matrices, n_comp, n_comp)
@@ -91,16 +91,16 @@
     )
     if dim_red is not None and "max_cond" in dim_red.keys():
         assert np.linalg.cond(cov_w.mean(axis=0)) <= max_cond
 
 
 @pytest.mark.parametrize("dim_red", dim_red)
 @pytest.mark.parametrize("metric", ["euclid", "logeuclid", "riemann"])
-def test_whitening_inverse_transform(dim_red, metric, rndstate, get_covmats):
+def test_whitening_inverse_transform(dim_red, metric, rndstate, get_mats):
     """Test Whitening inverse transform"""
     n_matrices, n_channels = 20, 6
-    cov = get_covmats(n_matrices, n_channels)
+    cov = get_mats(n_matrices, n_channels, "spd")
     whit = Whitening(dim_red=dim_red, metric=metric).fit(cov)
     cov_iw = whit.inverse_transform(whit.transform(cov))
     assert cov_iw.shape == (n_matrices, n_channels, n_channels)
     if dim_red is None:
         assert_array_almost_equal(cov, cov_iw)
```

### Comparing `pyriemann-0.5/tests/test_regression.py` & `pyriemann-0.6/tests/test_regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from pyriemann.utils.mean import mean_covariance
 
 regs = [SVR, KNearestNeighborRegressor]
 
 
 @pytest.mark.parametrize("regres", regs)
 class RegressorTestCase:
-    def test_regression(self, regres, get_covmats, get_targets):
+    def test_regression(self, regres, get_mats, get_targets):
         n_matrices, n_channels = 6, 3
-        covmats = get_covmats(n_matrices, n_channels)
+        covmats = get_mats(n_matrices, n_channels, "spd")
         targets = get_targets(n_matrices)
 
         self.reg_predict(regres, covmats, targets)
         self.reg_fit_independence(regres, covmats, targets)
         self.reg_score(regres, covmats, targets)
 
 
@@ -43,75 +43,75 @@
         clf.fit(covmats, targets)
         clf.score(covmats, targets)
 
 
 @pytest.mark.parametrize("regres", [KNearestNeighborRegressor])
 @pytest.mark.parametrize("mean", ["faulty", 42])
 @pytest.mark.parametrize("dist", ["not_real", 27])
-def test_metric_dict_error(regres, mean, dist, get_covmats, get_targets):
+def test_metric_dict_error(regres, mean, dist, get_mats, get_targets):
     n_matrices, n_channels = 6, 3
     targets = get_targets(n_matrices)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         clf = regres(metric={"mean": mean, "distance": dist})
         clf.fit(covmats, targets).predict(covmats)
 
 
 @pytest.mark.parametrize("regres", [KNearestNeighborRegressor])
 @pytest.mark.parametrize("mean", get_means())
 @pytest.mark.parametrize("dist", get_distances())
-def test_metric_dist(regres, mean, dist, get_covmats, get_targets):
+def test_metric_dist(regres, mean, dist, get_mats, get_targets):
     n_matrices, n_channels = 4, 3
     targets = get_targets(n_matrices)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = regres(metric={"mean": mean, "distance": dist})
     clf.fit(covmats, targets).predict(covmats)
 
 
 @pytest.mark.parametrize("regres", regs)
 @pytest.mark.parametrize("metric", [42, "faulty", {"foo": "bar"}])
-def test_metric_wrong_keys(regres, metric, get_covmats, get_targets):
+def test_metric_wrong_keys(regres, metric, get_mats, get_targets):
     n_matrices, n_channels = 6, 3
     targets = get_targets(n_matrices)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises((TypeError, KeyError, ValueError)):
         clf = regres(metric=metric)
         clf.fit(covmats, targets).predict(covmats)
 
 
 @pytest.mark.parametrize("regres", regs)
 @pytest.mark.parametrize("metric", get_metrics())
-def test_metric_str(regres, metric, get_covmats, get_targets):
+def test_metric_str(regres, metric, get_mats, get_targets):
     n_matrices, n_channels = 6, 3
     targets = get_targets(n_matrices)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     clf = regres(metric=metric)
 
     if regres is SVR and metric not in ['riemann', 'euclid', 'logeuclid']:
         with pytest.raises(ValueError):
             clf.fit(covmats, targets).predict(covmats)
 
     else:
         clf.fit(covmats, targets).predict(covmats)
 
 
 @pytest.mark.parametrize("dist", ["not_real", 42])
-def test_knn_dict_dist(dist, get_covmats, get_targets):
+def test_knn_dict_dist(dist, get_mats, get_targets):
     n_matrices, n_channels = 6, 3
     targets = get_targets(n_matrices)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(KeyError):
         clf = KNearestNeighborRegressor(metric={"distance": dist})
         clf.fit(covmats, targets).predict(covmats)
 
 
-def test_1NN(get_covmats, get_targets):
+def test_1NN(get_mats, get_targets):
     """Test KNearestNeighborRegressor with K=1"""
     n_matrices, n_channels = 9, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     targets = get_targets(n_matrices)
 
     knn = KNearestNeighborRegressor(1, metric="riemann")
     knn.fit(covmats, targets)
     preds = knn.predict(covmats[:-1])
     assert_array_equal(targets[:-1], preds)
 
@@ -123,42 +123,42 @@
     rsvr.set_params(**{'metric': 'logeuclid'})
     assert rsvr.metric == 'logeuclid'
 
     rsvr.set_params(**{'max_iter': 501})
     assert rsvr.max_iter == 501
 
 
-def test_svr_params_error(get_covmats, get_targets):
+def test_svr_params_error(get_mats, get_targets):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     targets = get_targets(n_matrices)
 
     with pytest.raises(TypeError):
         SVR(C='hello').fit(covmats, targets)
 
     with pytest.raises(TypeError):
         SVR(foo=5)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svr_cref_metric(get_covmats, get_targets, metric):
+def test_svr_cref_metric(get_mats, get_targets, metric):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     targets = get_targets(n_matrices)
     Cref = mean_covariance(covmats, metric=metric)
 
     rsvc = SVR(Cref=Cref).fit(covmats, targets)
     rsvc_1 = SVR(Cref=None, metric=metric).fit(covmats, targets)
     assert np.array_equal(rsvc.Cref_, rsvc_1.Cref_)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_cref_callable(get_covmats, get_targets, metric):
+def test_svc_cref_callable(get_mats, get_targets, metric):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     targets = get_targets(n_matrices)
     def Cref(X): return mean_covariance(X, metric=metric)
 
     rsvc = SVR(Cref=Cref).fit(covmats, targets)
     rsvc_1 = SVR(metric=metric).fit(covmats, targets)
     assert np.array_equal(rsvc.Cref_, rsvc_1.Cref_)
 
@@ -166,33 +166,33 @@
     rsvc.predict(covmats)
     rsvc_1 = SVR(metric=metric).fit(covmats, targets)
     rsvc_1.predict(covmats)
     assert np.array_equal(rsvc.Cref_, rsvc_1.Cref_)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_cref_error(get_covmats, get_targets, metric):
+def test_svc_cref_error(get_mats, get_targets, metric):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     targets = get_targets(n_matrices)
     def Cref(X, met): mean_covariance(X, metric=met)
 
     with pytest.raises(TypeError):
         SVR(Cref=Cref).fit(covmats, targets)
 
     Cref = metric
 
     with pytest.raises(TypeError):
         SVR(Cref=Cref).fit(covmats, targets)
 
 
 @pytest.mark.parametrize("metric", ["riemann", "euclid", "logeuclid"])
-def test_svc_kernel_callable(get_covmats, get_targets, metric):
+def test_svc_kernel_callable(get_mats, get_targets, metric):
     n_matrices, n_channels = 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     targets = get_targets(n_matrices)
 
     rsvc = SVR(kernel_fct=kernel,
                metric=metric).fit(covmats, targets)
     rsvc_1 = SVR(metric=metric).fit(covmats, targets)
     p1 = rsvc.predict(covmats[:-1])
     p2 = rsvc_1.predict(covmats[:-1])
```

### Comparing `pyriemann-0.5/tests/test_sampling.py` & `pyriemann-0.6/tests/test_sampling.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pytest
 import numpy as np
+import pytest
 
 from pyriemann.datasets.sampling import (sample_gaussian_spd,
                                          generate_random_spd_matrix)
 from pyriemann.utils.distance import distance_riemann
 from pyriemann.utils.test import is_sym_pos_def as is_spd
```

### Comparing `pyriemann-0.5/tests/test_simulated.py` & `pyriemann-0.6/tests/test_simulated.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,27 @@
-import pytest
 import numpy as np
 from numpy.testing import assert_array_almost_equal
+import pytest
 
 from pyriemann.datasets.sampling import generate_random_spd_matrix
 from pyriemann.datasets.simulated import (
-    make_covariances,
     make_matrices,
     make_masks,
     make_gaussian_blobs,
     make_outliers,
 )
 from pyriemann.utils.test import (
     is_real,
     is_sym_pos_def as is_spd,
     is_sym_pos_semi_def as is_spsd,
     is_herm_pos_def as is_hpd,
     is_herm_pos_semi_def as is_hpsd,
 )
 
 
-def test_make_covariances(rndstate):
-    """Test function for make covariances."""
-    n_matrices, n_channels = 5, 4
-    X, evals, evecs = make_covariances(n_matrices=n_matrices,
-                                       n_channels=n_channels,
-                                       return_params=True,
-                                       rs=rndstate)
-    assert X.shape == (n_matrices, n_channels, n_channels)  # X shape mismatch
-    assert evals.shape == (n_matrices, n_channels)  # evals shape mismatch
-    assert evecs.shape == (n_channels, n_channels)  # evecs shape mismatch
-
-
 @pytest.mark.parametrize(
     "kind", ["real", "comp", "spd", "spsd", "hpd", "hpsd"]
 )
 def test_make_matrices(rndstate, kind):
     """Test function for make matrices."""
     n_matrices, n_dim = 5, 4
     X = make_matrices(
```

### Comparing `pyriemann-0.5/tests/test_spatialfilters.py` & `pyriemann-0.6/tests/test_spatialfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from conftest import get_metrics
-import pytest
 import numpy as np
 from numpy.testing import assert_array_equal
+import pytest
 
+from conftest import get_metrics
 from pyriemann.spatialfilters import Xdawn, CSP, SPoC, BilinearFilter, AJDC
 
 
 @pytest.mark.parametrize("spfilt", [Xdawn, CSP, SPoC, BilinearFilter, AJDC])
 @pytest.mark.parametrize("n_channels", [3, 5, 7])
 @pytest.mark.parametrize("n_classes", [2, 3])
 def test_spatial_filters(spfilt, n_channels,
-                         get_covmats, rndstate, get_labels, n_classes):
+                         get_mats, rndstate, get_labels, n_classes):
     if n_classes == 2:
         n_matrices, n_times = 10, 256
     else:
         n_matrices, n_times = 9, 256
     labels = get_labels(n_matrices, n_classes)
     if spfilt is Xdawn:
         X = rndstate.randn(n_matrices, n_channels, n_times)
     elif spfilt in (CSP, SPoC, BilinearFilter):
-        X = get_covmats(n_matrices, n_channels)
+        X = get_mats(n_matrices, n_channels, "spd")
     elif spfilt is AJDC:
         n_subjects, n_conditions = 2, 2
         X = rndstate.randn(n_subjects, n_conditions, n_channels, n_times)
 
     clf_fit(spfilt, X, labels, n_channels, n_times)
     clf_fit_independence(spfilt, X, labels, n_channels)
     if spfilt is CSP:
@@ -150,50 +150,50 @@
     n_components = min(n_channels, xd.nfilter)
     assert xd.filters_.shape == (n_classes * n_components, n_channels)
 
 
 @pytest.mark.parametrize("n_filters", [3, 4, 5])
 @pytest.mark.parametrize("metric", get_metrics())
 @pytest.mark.parametrize("log", [True, False])
-def test_csp_init(n_filters, metric, log, get_covmats, get_labels):
+def test_csp_init(n_filters, metric, log, get_mats, get_labels):
     n_classes, n_matrices, n_channels = 2, 6, 4
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     csp = CSP(nfilter=n_filters, metric=metric, log=log)
     Xtr = csp.fit(covmats, labels).transform(covmats)
     n_components = min(n_channels, n_filters)
     if log:
         assert Xtr.shape == (n_matrices, n_components)
     else:
         assert Xtr.shape == (n_matrices, n_components, n_components)
     assert csp.filters_.shape == (n_components, n_channels)
     assert csp.patterns_.shape == (n_components, n_channels)
 
 
-def test_bilinearfilter_filter_error(get_covmats, get_labels):
+def test_bilinearfilter_filter_error(get_mats, get_labels):
     n_classes, n_matrices, n_channels = 2, 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     with pytest.raises(TypeError):
         BilinearFilter("foo").fit(covmats, labels)
 
 
-def test_bilinearfilter_log_error(get_covmats, get_labels):
+def test_bilinearfilter_log_error(get_mats, get_labels):
     n_classes, n_matrices, n_channels = 2, 6, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     with pytest.raises(TypeError):
         BilinearFilter(np.eye(3), log="foo").fit(covmats, labels)
 
 
 @pytest.mark.parametrize("n_filters", [3, 4])
 @pytest.mark.parametrize("log", [True, False])
-def test_bilinearfilter_log(n_filters, log, get_covmats, get_labels):
+def test_bilinearfilter_log(n_filters, log, get_mats, get_labels):
     n_classes, n_matrices, n_channels = 2, 6, 4
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     bf = BilinearFilter(np.eye(n_filters, n_channels), log=log)
     Xtr = bf.fit(covmats, labels).transform(covmats)
     if log:
         assert Xtr.shape == (n_matrices, n_filters)
     else:
         assert Xtr.shape == (n_matrices, n_filters, n_filters)
```

### Comparing `pyriemann-0.5/tests/test_stats.py` & `pyriemann-0.6/tests/test_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,76 @@
-from conftest import requires_matplotlib
 import numpy as np
+import pytest
+
+from conftest import requires_matplotlib
 from pyriemann.stats import PermutationDistance, PermutationModel
 from pyriemann.spatialfilters import CSP
-import pytest
 
 
 def test_permutation_badmode():
     """Test one way permutation test"""
     with pytest.raises(ValueError):
         PermutationDistance(mode="badmode")
 
 
 @pytest.mark.parametrize("mode", ["ttest", "ftest"])
-def test_permutation_mode(mode, get_covmats, get_labels):
+def test_permutation_mode(mode, get_mats, get_labels):
     """Test one way permutation test"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     p = PermutationDistance(100, mode=mode)
     p.test(covmats, labels)
 
 
-def test_permutation_pairwise(get_covmats, get_labels):
+def test_permutation_pairwise(get_mats, get_labels):
     """Test one way permutation pairwise test"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     groups = np.array([0] * 3 + [1] * 3)
     # pairwise
     p = PermutationDistance(100, mode="pairwise")
     p.test(covmats, labels)
     # with group
     p.test(covmats, labels, groups=groups)
 
 
-def test_permutation_pairwise_estimator(get_covmats, get_labels):
+def test_permutation_pairwise_estimator(get_mats, get_labels):
     """Test one way permutation with estimator"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     # with custom estimator
     p = PermutationDistance(10, mode="pairwise", estimator=CSP(2, log=False))
     p.test(covmats, labels)
 
 
-def test_permutation_pairwise_unique(get_covmats, get_labels):
+def test_permutation_pairwise_unique(get_mats, get_labels):
     """Test one way permutation with estimator"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     # unique perms
     p = PermutationDistance(1000)
     p.test(covmats, labels)
 
 
 @requires_matplotlib
-def test_permutation_pairwise_plot(get_covmats, get_labels):
+def test_permutation_pairwise_plot(get_mats, get_labels):
     """Test one way permutation with estimator"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     p = PermutationDistance(100, mode="pairwise")
     p.test(covmats, labels)
     p.plot(nbins=2)
 
 
-def test_permutation_model(get_covmats, get_labels):
+def test_permutation_model(get_mats, get_labels):
     """Test one way permutation test"""
     n_matrices, n_channels, n_classes = 6, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     labels = get_labels(n_matrices, n_classes)
     # pairwise
     p = PermutationModel(10)
     p.test(covmats, labels)
```

### Comparing `pyriemann-0.5/tests/test_tangentspace.py` & `pyriemann-0.6/tests/test_tangentspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from conftest import get_metrics
 import numpy as np
-from pyriemann.tangentspace import TangentSpace, FGDA
 import pytest
 from pytest import approx
 
+from conftest import get_metrics
+from pyriemann.tangentspace import TangentSpace, FGDA
+
 
 @pytest.mark.parametrize("tspace", [TangentSpace, FGDA])
 class TangentSpaceTestCase:
-    def test_tangentspace(self, tspace, get_covmats, get_labels):
+    def test_tangentspace(self, tspace, get_mats, get_labels):
         n_classes, n_matrices, n_channels = 2, 6, 3
-        covmats = get_covmats(n_matrices, n_channels)
+        covmats = get_mats(n_matrices, n_channels, "spd")
         labels = get_labels(n_matrices, n_classes)
         self.clf_transform(tspace, covmats, labels)
         self.clf_fit_transform(tspace, covmats, labels)
         self.clf_fit_transform_independence(tspace, covmats, labels)
         if tspace is TangentSpace:
             self.clf_transform_wo_fit(tspace, covmats)
             self.clf_inversetransform(tspace, covmats)
@@ -65,65 +66,64 @@
         assert covinv == approx(covmats)
 
 
 @pytest.mark.parametrize("fit", [True, False])
 @pytest.mark.parametrize("tsupdate", [True, False])
 @pytest.mark.parametrize("metric_mean", get_metrics())
 @pytest.mark.parametrize("metric_map", ["euclid", "logeuclid", "riemann"])
-def test_TangentSpace_init(fit, tsupdate, metric_mean, metric_map,
-                           get_covmats):
+def test_TangentSpace_init(fit, tsupdate, metric_mean, metric_map, get_mats):
     n_matrices, n_channels = 4, 3
     n_ts = (n_channels * (n_channels + 1)) // 2
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     ts = TangentSpace(
         metric={"mean": metric_mean, "map": metric_map},
         tsupdate=tsupdate
     )
     if fit:
         ts.fit(covmats)
     Xtr = ts.transform(covmats)
     assert Xtr.shape == (n_matrices, n_ts)
 
 
 @pytest.mark.parametrize("tsupdate", [True, False])
 @pytest.mark.parametrize("metric_mean", get_metrics())
 @pytest.mark.parametrize("metric_map", ["euclid", "logeuclid", "riemann"])
-def test_FGDA_init(tsupdate, metric_mean, metric_map, get_covmats, get_labels):
+def test_FGDA_init(tsupdate, metric_mean, metric_map, get_mats, get_labels):
     n_classes, n_matrices, n_channels = 2, 6, 3
     labels = get_labels(n_matrices, n_classes)
-    covmats = get_covmats(n_matrices, n_channels)
+    covmats = get_mats(n_matrices, n_channels, "spd")
     ts = FGDA(
         metric={"mean": metric_mean, "map": metric_map},
         tsupdate=tsupdate
     )
     ts.fit(covmats, labels)
     Xtr = ts.transform(covmats)
     assert Xtr.shape == (n_matrices, n_channels, n_channels)
 
 
 @pytest.mark.parametrize("tspace", [TangentSpace, FGDA])
 @pytest.mark.parametrize("metric", [42, "faulty", {"foo": "bar"}])
-def test_metric_wrong_keys(tspace, metric, get_covmats, get_labels):
+def test_metric_wrong_keys(tspace, metric, get_mats, get_labels):
     with pytest.raises((TypeError, KeyError, ValueError)):
         n_classes, n_matrices, n_channels = 2, 6, 3
         labels = get_labels(n_matrices, n_classes)
-        covmats = get_covmats(n_matrices, n_channels)
+        covmats = get_mats(n_matrices, n_channels, "spd")
         clf = tspace(metric=metric)
         clf.fit(covmats, labels).transform(covmats)
 
 
-def test_TS_vecdim_error(get_covmats, rndstate):
+def test_TS_vecdim_error():
     n_matrices, n_ts = 4, 6
     ts = TangentSpace()
     with pytest.raises(ValueError):
         tsvectors_wrong = np.empty((n_matrices, n_ts + 1))
         ts.transform(tsvectors_wrong)
 
 
-def test_TS_matdim_error(get_covmats):
+def test_TS_matdim_error():
     n_matrices, n_channels = 4, 3
     ts = TangentSpace()
     with pytest.raises(ValueError):
         not_square_mat = np.empty((n_matrices, n_channels, n_channels + 1))
         ts.transform(not_square_mat)
     with pytest.raises(ValueError):
         too_many_dim = np.empty((1, 2, 3, 4))
```

### Comparing `pyriemann-0.5/tests/test_transfer.py` & `pyriemann-0.6/tests/test_transfer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
-import pytest
-from pytest import approx
 import numpy as np
 from numpy.testing import assert_array_equal
+import pytest
+from pytest import approx
 from sklearn.model_selection import KFold, StratifiedShuffleSplit
 from sklearn.pipeline import make_pipeline, Pipeline
 
 from pyriemann.datasets.simulated import (
     make_classification_transfer,
     make_matrices,
 )
@@ -28,14 +27,15 @@
     TLSplitter,
     TLClassifier,
     TLRegressor,
     MDWM,
 )
 from pyriemann.utils.distance import distance, distance_riemann
 from pyriemann.utils.mean import mean_covariance, mean_riemann
+from pyriemann.utils.utils import check_weights
 
 rndstate = 1234
 
 
 def test_encode_decode_domains(rndstate):
     """Test encoding and decoding of domains for data points"""
     n_matrices, n_channels = 4, 2
@@ -51,75 +51,115 @@
 
     _, y_dec, d_dec = decode_domains(X_enc, y_enc)
     assert (y == y_dec).all()
     assert (domain == d_dec).all()
 
 
 @pytest.mark.parametrize("metric", ["riemann"])
-def test_tlcenter(rndstate, metric):
+@pytest.mark.parametrize("sample_weight", [True, False])
+def test_tlcenter(rndstate, metric, sample_weight):
     """Test pipeline for recentering data to Identity"""
     # check if the global mean of the domains is indeed Identity
     rct = TLCenter(target_domain='target_domain', metric=metric)
     X, y_enc = make_classification_transfer(
         n_matrices=25, random_state=rndstate)
-    X_rct = rct.fit_transform(X, y_enc)
+    if sample_weight:
+        sample_weight_ = rndstate.rand(len(y_enc))
+    else:
+        sample_weight_ = None
+    X_rct = rct.fit_transform(X, y_enc, sample_weight_)
     _, _, domain = decode_domains(X_rct, y_enc)
     for d in np.unique(domain):
-        Xd = X_rct[domain == d]
-        Md = mean_covariance(Xd, metric=metric)
+        idx = domain == d
+        Xd = X_rct[idx]
+        if sample_weight:
+            sample_weight_d = check_weights(sample_weight_[idx], np.sum(idx))
+            Md = mean_covariance(Xd, metric='riemann',
+                                 sample_weight=sample_weight_d)
+        else:
+            Md = mean_covariance(Xd, metric='riemann')
         assert Md == pytest.approx(np.eye(2))
 
 
 @pytest.mark.parametrize("centered_data", [True, False])
 @pytest.mark.parametrize("metric", ["riemann"])
-def test_tlstretch(rndstate, centered_data, metric):
+@pytest.mark.parametrize("sample_weight", [True, False])
+def test_tlstretch(rndstate, centered_data, metric, sample_weight):
     """Test pipeline for stretching data"""
     # check if the dispersion of the dataset indeed decreases to 1
     tlstr = TLStretch(
         target_domain='target_domain',
         final_dispersion=1.0,
         centered_data=centered_data,
         metric=metric
     )
     X, y_enc = make_classification_transfer(
         n_matrices=25, class_disp=2.0, random_state=rndstate)
+
+    if sample_weight:
+        sample_weight_ = rndstate.rand(len(y_enc))
+    else:
+        sample_weight_ = None
     if centered_data:  # ensure that data is indeed centered on each domain
         tlrct = TLCenter(target_domain='target_domain', metric=metric)
-        X = tlrct.fit_transform(X, y_enc)
-    X_str = tlstr.fit_transform(X, y_enc)
+        X = tlrct.fit_transform(X, y_enc, sample_weight=sample_weight_)
+
+    X_str = tlstr.fit_transform(X, y_enc, sample_weight=sample_weight_)
+
     _, _, domain = decode_domains(X_str, y_enc)
     for d in np.unique(domain):
-        Xd = X_str[domain == d]
-        Md = mean_riemann(Xd)
-        disp = np.sum(distance(Xd, Md, metric=metric)**2)
+        idx = domain == d
+        Xd = X_str[idx]
+        if sample_weight:
+            sample_weight_d = check_weights(sample_weight_[idx], np.sum(idx))
+            Md = mean_riemann(Xd, sample_weight=sample_weight_d)
+            dist = distance(Xd, Md, metric=metric, squared=True)
+            disp = np.sum(sample_weight_d * np.squeeze(dist))
+        else:
+            Md = mean_riemann(Xd)
+            disp = np.mean(distance(Xd, Md, metric=metric, squared=True))
         assert np.isclose(disp, 1.0)
 
 
 @pytest.mark.parametrize("metric", ["euclid", "riemann"])
-def test_tlrotate(rndstate, metric):
-    """Test pipeline for rotating the datasets"""
+@pytest.mark.parametrize("sample_weight", [True, False])
+def test_tlrotate(rndstate, metric, sample_weight):
+    """Test fit_transform method for rotating the datasets"""
     # check if the distance between the classes of each domain is reduced
     X, y_enc = make_classification_transfer(
-        n_matrices=50, class_sep=3, class_disp=1.0, random_state=rndstate)
-    rct = TLCenter(target_domain='target_domain')
-    X_rct = rct.fit_transform(X, y_enc)
+        n_matrices=50, class_sep=3, class_disp=1.0, theta=np.pi/2,
+        random_state=rndstate)
+
+    if sample_weight:
+        sample_weight_ = rndstate.rand(len(y_enc))
+    else:
+        sample_weight_ = None
+    sample_weight_ = check_weights(sample_weight_, len(y_enc))
+
+    rct = TLCenter(target_domain='target_domain', metric=metric)
+    X_rct = rct.fit_transform(X, y_enc, sample_weight=sample_weight_)
     rot = TLRotate(target_domain='target_domain', metric=metric)
-    X_rot = rot.fit_transform(X_rct, y_enc)
+    X_rot = rot.fit_transform(X_rct, y_enc, sample_weight=sample_weight_)
+
     _, y, domain = decode_domains(X_rot, y_enc)
     for label in np.unique(y):
         d = 'source_domain'
         M_rct_label_source = mean_riemann(
-            X_rct[domain == d][y[domain == d] == label])
+            X_rct[domain == d][y[domain == d] == label],
+            sample_weight=sample_weight_[domain == d][y[domain == d] == label])
         M_rot_label_source = mean_riemann(
-            X_rot[domain == d][y[domain == d] == label])
+            X_rot[domain == d][y[domain == d] == label],
+            sample_weight=sample_weight_[domain == d][y[domain == d] == label])
         d = 'target_domain'
         M_rct_label_target = mean_riemann(
-            X_rct[domain == d][y[domain == d] == label])
+            X_rct[domain == d][y[domain == d] == label],
+            sample_weight=sample_weight_[domain == d][y[domain == d] == label])
         M_rot_label_target = mean_riemann(
-            X_rot[domain == d][y[domain == d] == label])
+            X_rot[domain == d][y[domain == d] == label],
+            sample_weight=sample_weight_[domain == d][y[domain == d] == label])
         d_rct = distance_riemann(M_rct_label_source, M_rct_label_target)
         d_rot = distance_riemann(M_rot_label_source, M_rot_label_target)
         assert d_rot <= d_rct
 
 
 @pytest.mark.parametrize(
     "cv",
@@ -312,14 +352,15 @@
         metric=metric,
         n_jobs=n_jobs,
     )
 
     # test fit
     clf.fit(X, y_enc)
     assert_array_equal(clf.classes_, ['1', '2'])
+    assert clf.covmeans_.shape == (n_classes, 2, 2)
 
     X, y, domain = decode_domains(X, y_enc)
     X_source = X[domain == 'source_domain']
     y_source = y[domain == 'source_domain']
     X_target = X[domain == 'target_domain']
     y_target = y[domain == 'target_domain']
 
@@ -344,7 +385,25 @@
     # test predict_proba
     probabilities = clf.predict_proba(X)
     assert probabilities.shape == (n_matrices, n_classes)
     assert probabilities.sum(axis=1) == approx(np.ones(n_matrices))
 
     # test score
     clf.score(X, y_enc)
+
+
+def test_mdwm_weights(rndstate):
+    n_classes, n_matrices = 2, 40
+    X, y_enc = make_classification_transfer(
+        n_matrices=n_matrices // 4,
+        class_sep=5,
+        class_disp=1.0,
+        random_state=rndstate,
+    )
+    weights = rndstate.rand(n_matrices // n_classes)
+
+    clf = MDWM(
+        domain_tradeoff=0.5,
+        target_domain='target_domain',
+        metric="riemann",
+    )
+    clf.fit(X, y_enc, sample_weight=weights)
```

### Comparing `pyriemann-0.5/tests/test_utils_ajd.py` & `pyriemann-0.6/tests/test_utils_ajd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,109 @@
-from numpy.testing import assert_array_equal
 import numpy as np
+from numpy.testing import assert_array_equal
 import pytest
 from pytest import approx
 
-from pyriemann.utils.ajd import rjd, ajd_pham, uwedge
+from pyriemann.utils.ajd import ajd, rjd, ajd_pham, uwedge
 
 
-@pytest.mark.parametrize("ajd", [rjd, ajd_pham, uwedge])
-@pytest.mark.parametrize("init", [True, False])
-def test_ajd(ajd, init, get_covmats_params):
+@pytest.mark.parametrize(
+    "method, algo",
+    [
+        ("rjd", rjd),
+        ("ajd_pham", ajd_pham),
+        ("uwedge", uwedge),
+        (uwedge, uwedge),
+    ]
+)
+def test_ajd(method, algo, get_mats):
     """Test ajd algos"""
-    n_matrices, n_channels = 5, 3
-    covmats, _, evecs = get_covmats_params(n_matrices, n_channels)
-    if init:
-        V, D = ajd(covmats)
-    else:
-        V, D = ajd(covmats, init=evecs)
+    eps, n_iter_max = 1e-6, 100
+    n_matrices, n_channels = 10, 3
+    mats = get_mats(n_matrices, n_channels, "spd")
+
+    V, D = ajd(mats, method=method, eps=eps, n_iter_max=n_iter_max)
     assert V.shape == (n_channels, n_channels)
     assert D.shape == (n_matrices, n_channels, n_channels)
 
-    if ajd is rjd:
+    if method == "rjd":
+        assert D == approx(V.T @ mats @ V)
         assert V.T @ V == approx(np.eye(n_channels))  # check orthogonality
+    else:
+        assert D == approx(V @ mats @ V.T)
+
+    V_, D_ = algo(mats, eps=eps, n_iter_max=n_iter_max)
+    assert np.all(V == V_)
+    assert np.all(D == D_)
 
 
-@pytest.mark.parametrize("ajd", [rjd, ajd_pham, uwedge])
-def test_ajd_init_error(ajd, get_covmats):
+@pytest.mark.parametrize("method", ["rjd", "ajd_pham", "uwedge"])
+@pytest.mark.parametrize("init", [True, False])
+def test_ajd_init(method, init, get_mats_params):
     """Test init for ajd algos"""
-    n_matrices, n_channels = 5, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    n_matrices, n_channels = 9, 4
+    mats, _, evecs = get_mats_params(n_matrices, n_channels, "spd")
+    if init:
+        ajd(mats, method=method, init=evecs)
+    else:
+        ajd(mats, method=method)
+
+
+@pytest.mark.parametrize("method", ["rjd", "ajd_pham", "uwedge"])
+def test_ajd_init_error(method, get_mats):
+    """Test init errors for ajd algos"""
+    n_matrices, n_channels = 4, 3
+    mats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):  # not 2D array
-        ajd(covmats, init=np.ones((3, 2, 2)))
+        ajd(mats, method=method, init=np.ones((3, 2, 2)))
     with pytest.raises(ValueError):  # not square array
-        ajd(covmats, init=np.ones((3, 2)))
+        ajd(mats, method=method, init=np.ones((3, 2)))
     with pytest.raises(ValueError):  # shape not equal to n_channels
-        ajd(covmats, init=np.ones((2, 2)))
+        ajd(mats, method=method, init=np.ones((2, 2)))
 
 
-def test_pham_weight_none_equivalent_uniform(get_covmats):
-    """Test pham's ajd weights: none is equivalent to uniform values"""
-    n_matrices, n_channels, w_val = 5, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
-    V, D = ajd_pham(covmats)
-    assert V.shape == (n_channels, n_channels)
-    assert D.shape == (n_matrices, n_channels, n_channels)
+@pytest.mark.parametrize("method", ["abc", 42])
+def test_ajd_method_error(method):
+    with pytest.raises(ValueError):
+        ajd(np.ones((3, 2, 2)), method=method)
 
-    Vw, Dw = ajd_pham(covmats, sample_weight=w_val * np.ones(n_matrices))
+
+def test_ajd_pham(get_mats):
+    """Test pham's ajd"""
+    n_matrices, n_channels = 7, 4
+    mats = get_mats(n_matrices, n_channels, "spd")
+    V, D = ajd_pham(mats)
+    assert D == approx(V @ mats @ V.conj().T)
+
+
+def test_ajd_pham_weight_none_equivalent_uniform(get_mats):
+    """Test pham's ajd weights: none is equivalent to uniform values"""
+    n_matrices, n_channels = 5, 3
+    mats = get_mats(n_matrices, n_channels, "spd")
+    V, D = ajd_pham(mats)
+    Vw, Dw = ajd_pham(mats, sample_weight=np.ones(n_matrices))
     assert_array_equal(V, Vw)  # same result as ajd_pham without weight
     assert_array_equal(D, Dw)
 
+    ajd(mats, method="ajd_pham", sample_weight=np.ones(n_matrices))
+
 
-def test_pham_weight_positive(get_covmats):
+def test_ajd_pham_weight_positive(get_mats):
     """Test pham's ajd weights: must be strictly positive"""
-    n_matrices, n_channels, w_val = 5, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
-    w = w_val * np.ones(n_matrices)
+    n_matrices, n_channels = 4, 2
+    mats = get_mats(n_matrices, n_channels, "spd")
+    w = 1.23 * np.ones(n_matrices)
     with pytest.raises(ValueError):  # not strictly positive weight
         w[0] = 0
-        ajd_pham(covmats, sample_weight=w)
+        ajd_pham(mats, sample_weight=w)
 
 
-def test_pham_weight_zero(get_covmats):
+def test_ajd_pham_weight_zero(get_mats):
     """Setting one weight to almost 0 it's almost like not passing the mat"""
-    n_matrices, n_channels, w_val = 5, 3, 2
-    covmats = get_covmats(n_matrices, n_channels)
-    w = w_val * np.ones(n_matrices)
-    V, D = ajd_pham(covmats[1:], sample_weight=w[1:])
+    n_matrices, n_channels = 5, 4
+    mats = get_mats(n_matrices, n_channels, "spd")
+    w = 4.32 * np.ones(n_matrices)
+    V, D = ajd_pham(mats[1:], sample_weight=w[1:])
     w[0] = 1e-12
-    Vw, Dw = ajd_pham(covmats, sample_weight=w)
+    Vw, Dw = ajd_pham(mats, sample_weight=w)
     assert V == approx(Vw, rel=1e-4, abs=1e-8)
     assert D == approx(Dw[1:], rel=1e-4, abs=1e-8)
```

### Comparing `pyriemann-0.5/tests/test_utils_base.py` & `pyriemann-0.6/tests/test_utils_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import pytest
 import numpy as np
 from numpy.testing import assert_array_almost_equal
+import pytest
 
 from pyriemann.utils.base import (
     expm,
     invsqrtm,
     logm,
     powm,
     sqrtm,
@@ -145,16 +145,16 @@
     # This is an indirect check, the riemannian mean must crash when the
     # matrices are not SPD.
     with pytest.warns(RuntimeWarning):
         with pytest.raises(ValueError):
             mean_riemann(C)
 
 
-def test_nearest_sym_pos_def(get_covmats):
+def test_nearest_sym_pos_def(get_mats):
     n_matrices = 3
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     D = mats.diagonal(axis1=1, axis2=2)
     psd = np.array([mat - np.diag(d) for mat, d in zip(mats, D)])
 
     assert not is_pos_def(psd)
     assert is_sym_pos_def(nearest_sym_pos_def(mats))
     assert is_sym_pos_def(nearest_sym_pos_def(psd))
```

### Comparing `pyriemann-0.5/tests/test_utils_covariance.py` & `pyriemann-0.6/tests/test_utils_covariance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from numpy.testing import assert_array_almost_equal
 import numpy as np
+from numpy.testing import assert_array_almost_equal
+import pytest
 from scipy.linalg import block_diag
 from scipy.signal import welch, csd, coherence as coherence_sp
-import pytest
+from sklearn.covariance import empirical_covariance
+
 
 from pyriemann.utils.covariance import (
     covariances, covariances_EP, covariances_X, eegtocov,
     cross_spectrum, cospectrum, coherence,
-    normalize, get_nondiag_weight, block_covariances
+    normalize, get_nondiag_weight, block_covariances, _complex_estimator
 )
 from pyriemann.utils.test import (
     is_real,
     is_hermitian,
     is_sym_pos_def,
     is_herm_pos_def
 )
@@ -48,18 +50,47 @@
         elif estimator == 'tyl':
             assert_array_almost_equal(
                 np.trace(cov, axis1=-2, axis2=-1),
                 np.full(n_matrices, n_channels)
             )
 
 
-@pytest.mark.parametrize('estimator', ['corr', 'cov'] + m_estimators)
+@pytest.mark.parametrize('assume_centered', [True, False])
+def test_covariance_scm_real(rndstate, assume_centered):
+    """Test equivalence between pyriemann and sklearn estimator on real data"""
+    n_matrices, n_channels, n_times = 3, 4, 50
+    x = rndstate.randn(n_matrices, n_channels, n_times)
+
+    cov = covariances(x, estimator='scm', assume_centered=assume_centered)
+    cov_sklearn = np.asarray([
+        empirical_covariance(x_.T, assume_centered=assume_centered)
+        for x_ in x
+    ])
+    assert_array_almost_equal(cov, cov_sklearn, 10)
+
+
+def test_covariance_scm_complex(rndstate):
+    """ Test correctness of decorator for complex estimator on complex data"""
+    n_matrices, n_channels, n_times = 4, 3, 60
+    x = rndstate.randn(n_matrices, n_channels, n_times) \
+        + 1j * rndstate.randn(n_matrices, n_channels, n_times)
+
+    cov = covariances(x, estimator='scm', assume_centered=True)
+
+    @_complex_estimator
+    def complex_scm_sklearn(x):
+        return empirical_covariance(x.T, assume_centered=True)
+    cov_decorator = np.asarray([complex_scm_sklearn(x_) for x_ in x])
+    assert_array_almost_equal(cov, cov_decorator, 10)
+
+
+@pytest.mark.parametrize('estimator', estimators + m_estimators)
 def test_covariances_complex(estimator, rndstate):
     """Test covariance for complex inputs"""
-    n_matrices, n_channels, n_times = 2, 3, 100
+    n_matrices, n_channels, n_times = 3, 4, 50
     x = rndstate.randn(n_matrices, n_channels, n_times) \
         + 1j * rndstate.randn(n_matrices, n_channels, n_times)
 
     cov = covariances(x, estimator=estimator)
     assert cov.shape == (n_matrices, n_channels, n_channels)
     assert is_herm_pos_def(cov)
 
@@ -68,15 +99,32 @@
     'estimator', estimators + [None]
 )
 def test_covariances_EP(estimator, rndstate):
     """Test covariance_EP for multiple estimators"""
     n_matrices, n_channels_x, n_channels_p, n_times = 2, 3, 3, 100
     x = rndstate.randn(n_matrices, n_channels_x, n_times)
     p = rndstate.randn(n_channels_p, n_times)
+    if estimator is None:
+        cov = covariances_EP(x, p)
+    else:
+        cov = covariances_EP(x, p, estimator=estimator)
+    n_dim_cov = n_channels_x + n_channels_p
+    assert cov.shape == (n_matrices, n_dim_cov, n_dim_cov)
+
 
+@pytest.mark.parametrize(
+    'estimator', estimators + [None]
+)
+def test_covariances_EP_complex(estimator, rndstate):
+    """Test covariance_EP for complex input"""
+    n_matrices, n_channels_x, n_channels_p, n_times = 2, 3, 3, 100
+    x = rndstate.randn(n_matrices, n_channels_x, n_times) \
+        + 1j * rndstate.randn(n_matrices, n_channels_x, n_times)
+    p = rndstate.randn(n_channels_p, n_times) \
+        + 1j * rndstate.randn(n_channels_p, n_times)
     if estimator is None:
         cov = covariances_EP(x, p)
     else:
         cov = covariances_EP(x, p, estimator=estimator)
     n_dim_cov = n_channels_x + n_channels_p
     assert cov.shape == (n_matrices, n_dim_cov, n_dim_cov)
 
@@ -84,15 +132,14 @@
 @pytest.mark.parametrize(
     'estimator', estimators + [None]
 )
 def test_covariances_X(estimator, rndstate):
     """Test covariance_X for multiple estimators"""
     n_matrices, n_channels, n_times = 3, 5, 15
     x = rndstate.randn(n_matrices, n_channels, n_times)
-
     if estimator is None:
         cov = covariances_X(x, alpha=5.)
     else:
         cov = covariances_X(x, estimator=estimator, alpha=5.)
     n_dim_cov = n_channels + n_times
     assert cov.shape == (n_matrices, n_dim_cov, n_dim_cov)
 
@@ -367,20 +414,20 @@
     assert mat.shape == mat_n.shape
     # test a 4d array, ie a group of groups of square matrices
     mat = rndstate.randn(n_conds, n_matrices, n_channels, n_channels)
     mat_n = normalize(mat, norm)
     assert mat.shape == mat_n.shape
 
 
-def test_normalize_values(rndstate, get_covmats):
+def test_normalize_values(rndstate, get_mats):
     """Test normalize values"""
     n_matrices, n_channels = 20, 3
 
     # after corr-normalization => diags = 1 and values in [-1, 1]
-    mat = get_covmats(n_channels, n_channels)
+    mat = get_mats(n_channels, n_channels, "spd")
     mat_cn = normalize(mat, "corr")
     assert_array_almost_equal(np.ones(mat_cn.shape[:-1]),
                               np.diagonal(mat_cn, axis1=-2, axis2=-1))
     assert np.all(-1 <= mat_cn) and np.all(mat_cn <= 1)
 
     # after trace-normalization => trace equal to 1
     mat = rndstate.randn(n_matrices, n_channels, n_channels)
```

### Comparing `pyriemann-0.5/tests/test_utils_distance.py` & `pyriemann-0.6/tests/test_utils_distance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from conftest import get_distances
 import numpy as np
 from numpy.testing import assert_array_almost_equal
-from scipy.spatial.distance import euclidean, mahalanobis
 import pytest
 from pytest import approx
+from scipy.spatial.distance import euclidean, mahalanobis
 
+from conftest import get_distances
 from pyriemann.utils.distance import (
     distance_euclid,
     distance_harmonic,
     distance_kullback,
     distance_kullback_right,
     distance_kullback_sym,
     distance_logdet,
@@ -62,21 +62,21 @@
 )
 def test_distances_metric(kind, metric, dist, get_mats):
     """Test distance for metric"""
     n_matrices, n_channels = 2, 3
     mats = get_mats(n_matrices, n_channels, kind)
     A, B = mats[0], mats[1]
     d = distance(A, B, metric=metric)
-    dtrue = dist(A, B)
-    assert d == approx(dtrue)
+    assert d == approx(dist(A, B))
+    assert np.isreal(d)
 
 
-def test_distances_metric_error(get_covmats):
+def test_distances_metric_error(get_mats):
     n_matrices, n_channels = 2, 2
-    A = get_covmats(n_matrices, n_channels)
+    A = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         distance(A[0], A[1], metric="universe")
     with pytest.raises(ValueError):
         distance(A[0], A[1], metric=42)
 
 
 @pytest.mark.parametrize("kind", ["spd", "hpd"])
@@ -85,26 +85,26 @@
     n_matrices, n_channels = 2, 5
     mats = get_mats(n_matrices, n_channels, kind)
     A, B = mats[0], mats[1]
     assert dist(A, B, squared=True) == approx(dist(A, B) ** 2)
 
 
 @pytest.mark.parametrize("dist", get_dist_func())
-def test_distances_all_error(dist, get_covmats):
+def test_distances_all_error(dist, get_mats):
     n_matrices, n_channels = 3, 3
-    A = get_covmats(n_matrices, n_channels)
+    A = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         dist(A, A[0])
 
 
 @pytest.mark.parametrize("dist", get_dist_func())
-def test_distances_all_ndarray(dist, get_covmats):
+def test_distances_all_ndarray(dist, get_mats):
     n_matrices, n_channels = 5, 3
-    A = get_covmats(n_matrices, n_channels)
-    B = get_covmats(n_matrices, n_channels)
+    A = get_mats(n_matrices, n_channels, "spd")
+    B = get_mats(n_matrices, n_channels, "spd")
     assert isinstance(dist(A[0], B[0]), float)  # 2D arrays
     assert dist(A, B).shape == (n_matrices,)  # 3D arrays
 
     n_sets = 5
     C = np.asarray([A for _ in range(n_sets)])
     D = np.asarray([B for _ in range(n_sets)])
     assert dist(C, D).shape == (n_sets, n_matrices,)  # 4D arrays
@@ -173,30 +173,30 @@
     """Test harmonic distance for invertible matrices"""
     n_matrices, n_channels = 2, 5
     mats = get_mats(n_matrices, n_channels, kind)
     A, B = mats[0], mats[1]
     distance_harmonic(A, B)
 
 
-def test_distance_kullback_implementation(get_covmats):
+def test_distance_kullback_implementation(get_mats):
     n_matrices, n_channels = 2, 6
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     A, B = mats[0], mats[1]
-    dist = 0.5*(np.trace(np.linalg.inv(B) @ A) - n_channels
-                + np.log(np.linalg.det(B) / np.linalg.det(A)))
-    assert distance_kullback(A, B) == approx(dist)
+    d = 0.5*(np.trace(np.linalg.inv(B) @ A) - n_channels
+             + np.log(np.linalg.det(B) / np.linalg.det(A)))
+    assert distance_kullback(A, B) == approx(d)
 
 
-def test_distance_logdet_implementation(get_covmats):
+def test_distance_logdet_implementation(get_mats):
     n_matrices, n_channels = 2, 6
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     A, B = mats[0], mats[1]
-    dist = np.sqrt(np.log(np.linalg.det((A + B) / 2.0))
-                   - 0.5 * np.log(np.linalg.det(A)*np.linalg.det(B)))
-    assert distance_logdet(A, B) == approx(dist)
+    d = np.sqrt(np.log(np.linalg.det((A + B) / 2.0))
+                - 0.5 * np.log(np.linalg.det(A)*np.linalg.det(B)))
+    assert distance_logdet(A, B) == approx(d)
 
 
 @pytest.mark.parametrize("kind", ["spd", "hpd"])
 def test_distance_riemann_properties(kind, get_mats):
     n_channels = 6
     mats = get_mats(2, n_channels, kind)
     A, B = mats[0], mats[1]
@@ -219,69 +219,82 @@
     alpha = np.random.uniform()
     dist_1 = distance_riemann(A, geodesic(A, B, alpha, metric='riemann'))
     dist_2 = alpha * distance_riemann(A, B)
     assert dist_1 == approx(dist_2)
 
 
 @pytest.mark.parametrize("dist, dfunc", zip(get_distances(), get_dist_func()))
-def test_distance_wrapper(dist, dfunc, get_covmats):
+def test_distance_wrapper(dist, dfunc, get_mats):
     n_matrices, n_channels = 2, 5
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     A, B = mats[0], mats[1]
     assert distance(A, B, metric=dist) == dfunc(A, B)
 
 
 @pytest.mark.parametrize("dist", get_dist_func())
-def test_distance_wrapper_between_set_and_matrix(dist, get_covmats):
+def test_distance_wrapper_between_set_and_matrix(dist, get_mats):
     n_matrices, n_channels = 10, 4
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     assert distance(mats, mats[-1], metric=dist).shape == (n_matrices, 1)
 
     n_sets = 5
     covs_4d = np.asarray([mats for _ in range(n_sets)])
     with pytest.raises(ValueError):
         distance(covs_4d, mats, metric=dist)
 
 
 @pytest.mark.parametrize("dist", get_distances())
 @pytest.mark.parametrize("Y", [None, True])
-def test_pairwise_distance_matrix(get_covmats, dist, Y):
+@pytest.mark.parametrize("squared", [False, True])
+def test_pairwise_distance_matrix(get_mats, dist, Y, squared):
     n_matrices_X, n_matrices_Y, n_channels = 6, 4, 5
-    X = get_covmats(n_matrices_X, n_channels)
+    X = get_mats(n_matrices_X, n_channels, "spd")
     if Y is None:
         n_matrices_Y = n_matrices_X
+        Y_ = X
     else:
-        Y = get_covmats(n_matrices_Y, n_channels)
+        Y = get_mats(n_matrices_Y, n_channels, "spd")
+        Y_ = Y
 
-    pdist = pairwise_distance(X, Y, metric=dist)
+    pdist = pairwise_distance(X, Y, metric=dist, squared=squared)
     assert pdist.shape == (n_matrices_X, n_matrices_Y)
 
+    for i in range(n_matrices_X):
+        for j in range(n_matrices_Y):
+            assert np.isclose(pdist[i, j],
+                              distance(X[i],
+                                       Y_[j],
+                                       metric=dist,
+                                       squared=squared),
+                              atol=1e-5,
+                              rtol=1e-5)
+
     if Y is None and dist not in ["kullback", "kullback_right"]:
         assert is_sym(pdist)
     else:
         assert not is_sym(pdist)
 
 
 @pytest.mark.parametrize("complex_valued", [True, False])
 def test_distance_mahalanobis(rndstate, complex_valued):
     n_channels, n_times = 3, 100
     X = rndstate.randn(n_channels, n_times)
     if complex_valued:
         X = X + 1j * rndstate.randn(n_channels, n_times)
-    dist = distance_mahalanobis(X, np.cov(X))
-    assert dist.shape == (n_times,)
-    assert np.all(np.isreal(dist))
+    d = distance_mahalanobis(X, np.cov(X))
+    assert d.shape == (n_times,)
+    assert np.all(np.isreal(d))
 
 
 @pytest.mark.parametrize("mean", [True, None])
-def test_distance_mahalanobis_scipy(rndstate, get_covmats, mean):
+def test_distance_mahalanobis_scipy(rndstate, get_mats, mean):
     """Test equivalence between pyriemann and scipy for real data"""
     n_channels, n_times = 3, 100
     X = rndstate.randn(n_channels, n_times)
-    C = get_covmats(1, n_channels)[0]
+    C = get_mats(1, n_channels, "spd")[0]
 
     Cinv = np.linalg.inv(C)
     y = np.zeros(n_channels)
     dist_sp = [mahalanobis(x, y, Cinv) for x in X.T]
 
     if mean:
         mean = np.zeros((n_channels, 1))
```

### Comparing `pyriemann-0.5/tests/test_utils_geodesic.py` & `pyriemann-0.6/tests/test_utils_geodesic.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     if complex_valued:
         mats = mats + 1j * rndstate.randn(n_matrices, n_dim0, n_dim1)
     A, B = mats[0], mats[1]
     assert geodesic_euclid(A, B).shape == A.shape
 
 
 @pytest.mark.parametrize("metric", get_geod_name())
-def test_geodesic_wrapper_ndarray(metric, get_covmats):
+def test_geodesic_wrapper_ndarray(metric, get_mats):
     n_matrices, n_channels = 5, 3
-    A = get_covmats(n_matrices, n_channels)
-    B = get_covmats(n_matrices, n_channels)
+    A = get_mats(n_matrices, n_channels, "spd")
+    B = get_mats(n_matrices, n_channels, "spd")
     assert geodesic(A[0], B[0], .3, metric=metric).shape == A[0].shape
     assert geodesic(A, B, .2, metric=metric).shape == A.shape  # 3D arrays
 
     n_sets = 4
     C = np.asarray([A for _ in range(n_sets)])
     D = np.asarray([B for _ in range(n_sets)])
     assert geodesic(C, D, .7, metric=metric).shape == C.shape  # 4D arrays
@@ -105,17 +105,17 @@
         B = 1.5 * np.eye(n_channels)
     else:
         B = 2.0 * np.eye(n_channels)
     assert geodesic(A, B, 0.5, metric=metric) == approx(np.eye(n_channels))
 
 
 @pytest.mark.parametrize("metric, gfun", zip(get_geod_name(), get_geod_func()))
-def test_geodesic_wrapper_random(metric, gfun, get_covmats):
+def test_geodesic_wrapper_random(metric, gfun, get_mats):
     n_matrices, n_channels = 2, 5
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     A, B = mats[0], mats[1]
     if gfun is geodesic_euclid:
         Ctrue = mean_euclid(mats)
     elif gfun is geodesic_logeuclid:
         Ctrue = mean_logeuclid(mats)
     elif gfun is geodesic_riemann:
         Ctrue = mean_riemann(mats)
```

### Comparing `pyriemann-0.5/tests/test_utils_kernel.py` & `pyriemann-0.6/tests/test_utils_kernel.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,70 +13,70 @@
 from pyriemann.utils.test import is_sym_pos_semi_def as is_spsd
 
 rker_str = ['euclid', 'logeuclid', 'riemann']
 rker_fct = [kernel_euclid, kernel_logeuclid, kernel_riemann]
 
 
 @pytest.mark.parametrize("ker", rker_fct)
-def test_kernel_x_x(ker, get_covmats):
+def test_kernel_x_x(ker, get_mats):
     """Test kernel build"""
     n_matrices, n_channels = 7, 3
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     K = ker(X, X)
     assert K.shape == (n_matrices, n_matrices)
     assert is_spsd(K)
     assert_array_almost_equal(K, ker(X))
 
 
 @pytest.mark.parametrize("ker", rker_str)
-def test_kernel_cref(ker, get_covmats):
+def test_kernel_cref(ker, get_mats):
     """Test kernel reference"""
     n_matrices, n_channels = 5, 3
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     cref = mean_covariance(X, metric=ker)
     K = kernel(X, X, metric=ker)
     K1 = kernel(X, X, Cref=cref, metric=ker)
     assert_array_equal(K, K1)
 
 
 @pytest.mark.parametrize("ker", rker_str)
-def test_kernel_x_y(ker, get_covmats):
+def test_kernel_x_y(ker, get_mats):
     """Test kernel for different X and Y"""
     n_matrices_X, n_matrices_Y, n_channels = 6, 5, 3
-    X = get_covmats(n_matrices_X, n_channels)
-    Y = get_covmats(n_matrices_Y, n_channels)
+    X = get_mats(n_matrices_X, n_channels, "spd")
+    Y = get_mats(n_matrices_Y, n_channels, "spd")
     K = kernel(X, Y, metric=ker)
     assert K.shape == (n_matrices_X, n_matrices_Y)
 
 
 @pytest.mark.parametrize("ker", rker_str)
-def test_metric_string(ker, get_covmats):
+def test_metric_string(ker, get_mats):
     """Test generic kernel function"""
     n_matrices, n_channels = 5, 3
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     K = globals()[f'kernel_{ker}'](X)
     K1 = kernel(X, metric=ker)
     assert_array_equal(K, K1)
 
 
-def test_metric_string_error(get_covmats):
+def test_metric_string_error(get_mats):
     """Test generic kernel function error raise"""
     n_matrices, n_channels = 5, 3
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         kernel(X, metric='foo')
 
 
 @pytest.mark.parametrize("ker", rker_str)
-def test_input_dimension_error(ker, get_covmats):
+def test_input_dimension_error(ker, get_mats):
     """Test errors for incorrect dimension"""
     n_matrices, n_channels = 5, 3
-    X = get_covmats(n_matrices, n_channels)
-    Y = get_covmats(n_matrices, n_channels + 1)
-    cref = get_covmats(1, n_channels + 1)[0]
+    X = get_mats(n_matrices, n_channels, "spd")
+    Y = get_mats(n_matrices, n_channels + 1, "spd")
+    cref = get_mats(1, n_channels + 1, "spd")[0]
     if ker == 'riemann':
         with pytest.raises(AssertionError):
             kernel(X, Cref=cref, metric=ker)
     with pytest.raises(AssertionError):
         kernel(X, Y, metric=ker)
 
 
@@ -86,23 +86,26 @@
     n_matrices_X, n_matrices_Y = 2, 3
     X = rndstate.randn(n_matrices_X, n_dim0, n_dim1)
     Y = rndstate.randn(n_matrices_Y, n_dim0, n_dim1)
     K = kernel_euclid(X, Y)
     assert K.shape == (n_matrices_X, n_matrices_Y)
 
     K1 = np.empty((n_matrices_X, n_matrices_Y))
+    K2 = np.empty((n_matrices_X, n_matrices_Y))
     for i in range(n_matrices_X):
         for j in range(n_matrices_Y):
             K1[i, j] = np.trace(X[i].T @ Y[j])
+            K2[i, j] = np.dot(X[i].flatten(), Y[j].flatten())
     assert_array_almost_equal(K, K1)
+    assert_array_almost_equal(K, K2)
 
 
-def test_riemann_correctness(get_covmats):
+def test_riemann_correctness(get_mats):
     """Test Riemannian kernel correctness"""
     n_matrices, n_channels = 5, 3
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     K = kernel_riemann(X, Cref=np.eye(n_channels), reg=0)
 
     log_X = logm(X)
     tensor = np.tensordot(log_X, log_X.T, axes=1)
     K1 = np.trace(tensor, axis1=1, axis2=2)
     assert_array_almost_equal(K, K1)
```

### Comparing `pyriemann-0.5/tests/test_utils_mean.py` & `pyriemann-0.6/tests/test_utils_mean.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from scipy.stats import gmean
 import pytest
 from pytest import approx
+from scipy.stats import gmean
 
 from pyriemann.utils.geodesic import geodesic_riemann
 from pyriemann.utils.mean import (
     mean_covariance,
     mean_ale,
     mean_alm,
     mean_euclid,
@@ -39,14 +39,16 @@
         nanmean_riemann,
     ],
 )
 def test_mean_shape(kind, mean, get_mats):
     """Test the shape of mean"""
     n_matrices, n_channels = 5, 3
     mats = get_mats(n_matrices, n_channels, kind)
+    if mean is mean_ale and kind == "hpd":
+        pytest.skip()
     if mean == mean_power:
         C = mean(mats, 0.42)
     else:
         C = mean(mats)
     assert C.shape == (n_channels, n_channels)
 
 
@@ -96,17 +98,17 @@
         mean_logdet,
         mean_logeuclid,
         mean_riemann,
         mean_wasserstein,
         nanmean_riemann,
     ],
 )
-def test_mean_weight_len_error(mean, get_covmats):
+def test_mean_weight_len_error(mean, get_mats):
     n_matrices, n_channels = 3, 2
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         mean(mats, sample_weight=np.ones(n_matrices + 1))
 
 
 @pytest.mark.parametrize(
     "mean", [
         mean_ale,
@@ -114,18 +116,18 @@
         mean_logdet,
         mean_power,
         mean_riemann,
         mean_wasserstein,
         nanmean_riemann
     ]
 )
-def test_mean_warning_convergence(mean, get_covmats):
+def test_mean_warning_convergence(mean, get_mats):
     """Test warning for convergence not reached """
     n_matrices, n_channels = 3, 2
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     with pytest.warns(UserWarning):
         if mean == mean_power:
             mean(mats, 0.3, maxiter=0)
         else:
             mean(mats, maxiter=0)
 
 
@@ -146,15 +148,15 @@
     ],
 )
 def test_mean_of_means(kind, mean, get_mats):
     """Test mean of submeans equal to grand mean"""
     n_matrices, n_channels = 10, 3
     mats = get_mats(n_matrices, n_channels, kind)
     if mean is mean_ale and kind == "hpd":
-        return True
+        pytest.skip()
     if mean == mean_power:
         p = -0.42
         C = mean(mats, p)
         C1 = mean(mats[:n_matrices//2], p)
         C2 = mean(mats[n_matrices//2:], p)
         C3 = mean(np.array([C1, C2]), p)
     else:
@@ -191,36 +193,36 @@
     n_matrices, n_dim0, n_dim1 = 10, 3, 4
     mats = rndstate.randn(n_matrices, n_dim0, n_dim1)
     if complex_valued:
         mats = mats + 1j * rndstate.randn(n_matrices, n_dim0, n_dim1)
     assert mean_euclid(mats) == approx(mats.mean(axis=0))
 
 
-def test_mean_identity(get_covmats):
+def test_mean_identity(get_mats):
     """Test the identity mean"""
     n_matrices, n_channels = 2, 3
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     C = mean_identity(mats)
     assert np.all(C == np.eye(n_channels))
 
 
 @pytest.mark.parametrize("kind", ["spd", "hpd"])
 def test_mean_power(kind, get_mats):
     """Test the power mean"""
     n_matrices, n_channels = 3, 3
     mats = get_mats(n_matrices, n_channels, kind)
     assert mean_power(mats, 1) == approx(mean_euclid(mats))
     assert mean_power(mats, 0) == approx(mean_riemann(mats))
     assert mean_power(mats, -1) == approx(mean_harmonic(mats))
 
 
-def test_mean_power_errors(get_covmats):
+def test_mean_power_errors(get_mats):
     """Test the power mean errors"""
     n_matrices, n_channels = 3, 2
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
 
     with pytest.raises(ValueError):  # exponent is not a scalar
         mean_power(mats, [1])
     with pytest.raises(ValueError):  # exponent is not in [-1,1]
         mean_power(mats, 3)
 
 
@@ -253,49 +255,49 @@
     assert C == approx(np.linalg.inv(mean_riemann(np.linalg.inv(mats))))
 
     # determinant identity, P9 in [Nakamura2009]
     assert np.linalg.det(C) == approx(gmean(np.linalg.det(mats)))
 
 
 @pytest.mark.parametrize("init", [True, False])
-def test_mean_masked_riemann_shape(init, get_covmats, get_masks):
+def test_mean_masked_riemann_shape(init, get_mats, get_masks):
     """Test the masked Riemannian mean"""
     n_matrices, n_channels = 5, 3
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     masks = get_masks(n_matrices, n_channels)
     if init:
         C = maskedmean_riemann(mats, masks, tol=10e-3, init=mats[0])
     else:
         C = maskedmean_riemann(mats, masks, tol=10e-3)
     assert C.shape == (n_channels, n_channels)
 
 
 @pytest.mark.parametrize("init", [True, False])
-def test_mean_nan_riemann_shape(init, get_covmats, rndstate):
+def test_mean_nan_riemann_shape(init, get_mats, rndstate):
     """Test the Riemannian NaN-mean"""
     n_matrices, n_channels = 10, 6
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     emean = np.mean(mats, axis=0)
     for i in range(n_matrices):
         corrup_channels = rndstate.choice(
             np.arange(0, n_channels), size=n_channels // 3, replace=False)
         for j in corrup_channels:
             mats[i, j] = np.nan
             mats[i, :, j] = np.nan
     if init:
         C = nanmean_riemann(mats, tol=10e-3, init=emean)
     else:
         C = nanmean_riemann(mats, tol=10e-3)
     assert C.shape == (n_channels, n_channels)
 
 
-def test_mean_nan_riemann_errors(get_covmats):
+def test_mean_nan_riemann_errors(get_mats):
     """Test the Riemannian NaN-mean errors"""
     n_matrices, n_channels = 5, 4
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
 
     with pytest.raises(ValueError):  # not symmetric NaN values
         mats_ = mats.copy()
         mats_[0, 0] = np.nan  # corrup only a row, not its corresp column
         nanmean_riemann(mats_)
     with pytest.raises(ValueError):  # not rows and columns NaN values
         mats_ = mats.copy()
@@ -319,23 +321,23 @@
         ("logdet", mean_logdet),
         ("logeuclid", mean_logeuclid),
         ("riemann", mean_riemann),
         ("wasserstein", mean_wasserstein),
         (callable_np_average, mean_euclid),
     ],
 )
-def test_mean_covariance_metric(metric, mean, get_covmats):
+def test_mean_covariance_metric(metric, mean, get_mats):
     """Test mean_covariance for metric"""
     n_matrices, n_channels = 3, 3
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     C = mean_covariance(mats, metric=metric)
     Ctrue = mean(mats)
     assert np.all(C == Ctrue)
 
 
-def test_mean_covariance_args(get_covmats):
+def test_mean_covariance_args(get_mats):
     """Test mean_covariance with different arguments"""
     n_matrices, n_channels = 3, 3
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     mean_covariance(mats, metric='ale', maxiter=5)
     mean_covariance(mats, metric='logdet', tol=10e-3)
     mean_covariance(mats, metric='riemann', init=np.eye(n_channels))
```

### Comparing `pyriemann-0.5/tests/test_utils_median.py` & `pyriemann-0.6/tests/test_utils_median.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,18 @@
     C = median(mats[1:], weights=w[1:])
     w[0] = 1e-12
     Cw = median(mats, weights=w)
     assert C == approx(Cw, rel=1e-6, abs=1e-8)
 
 
 @pytest.mark.parametrize("median", [median_euclid, median_riemann])
-def test_median_warning_convergence(median, get_covmats):
+def test_median_warning_convergence(median, get_mats):
     """Test warning for convergence not reached"""
     n_matrices, n_channels = 3, 2
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     with pytest.warns(UserWarning):
         median(mats, maxiter=0)
 
 
 @pytest.mark.parametrize("n_values", [3, 5, 7])
 def test_median_euclid_1d(n_values, rndstate):
     """Compare geometric Euclidean median to marginal median in 1D"""
@@ -66,12 +66,12 @@
     mats = rndstate.randn(n_matrices, n_dim0, n_dim1)
     if complex_valued:
         mats = mats + 1j * rndstate.randn(n_matrices, n_dim0, n_dim1)
     assert median_euclid(mats).shape == (n_dim0, n_dim1)
 
 
 @pytest.mark.parametrize("step_size", [0, 2.5])
-def test_median_riemann_stepsize_error(step_size, get_covmats):
+def test_median_riemann_stepsize_error(step_size, get_mats):
     n_matrices, n_channels = 1, 2
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
         median_riemann(mats, step_size=step_size)
```

### Comparing `pyriemann-0.5/tests/test_utils_tangent_space.py` & `pyriemann-0.6/tests/test_utils_tangent_space.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from conftest import get_metrics
 import numpy as np
 import pytest
 from pytest import approx
 
+from conftest import get_metrics
 from pyriemann.utils.distance import distance_riemann
 from pyriemann.utils.tangentspace import (
     exp_map_euclid, exp_map_logeuclid, exp_map_riemann,
     log_map_euclid, log_map_logeuclid, log_map_riemann,
     upper, unupper, tangent_space, untangent_space, transport
 )
 
 
 @pytest.mark.parametrize(
     "fun_map", [exp_map_euclid, exp_map_logeuclid, exp_map_riemann,
                 log_map_euclid, log_map_logeuclid, log_map_riemann]
 )
-def test_maps_ndarray(fun_map, get_covmats):
+def test_maps_ndarray(fun_map, get_mats):
     """Test log and exp maps"""
     n_matrices, n_channels = 6, 3
-    mats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     Xt = fun_map(mats, np.eye(n_channels))
     assert Xt.shape == (n_matrices, n_channels, n_channels)
 
     n_sets = 2
     covmats_4d = np.asarray([mats for _ in range(n_sets)])
     Xt = fun_map(covmats_4d, np.eye(n_channels))
     assert Xt.shape == (n_sets, n_matrices, n_channels, n_channels)
@@ -35,50 +35,47 @@
         [exp_map_euclid, exp_map_logeuclid, exp_map_riemann]
     )
 )
 def test_maps_log_exp(kind, log_map, exp_map, get_mats):
     """Test log then exp maps should be identity"""
     n_matrices, n_channels = 10, 3
     mats = get_mats(n_matrices, n_channels, kind)
-    X, C = mats[:n_matrices - 1], mats[-1]
-    X_log_exp = exp_map(log_map(X, C), C)
-    assert X_log_exp == approx(X)
+    X, C = mats[:-1], mats[-1]
+    assert exp_map(log_map(X, C), C) == approx(X)
 
 
 @pytest.mark.parametrize("complex_valued", [True, False])
 def test_map_euclid(rndstate, complex_valued):
-    """Test Euclidean maps for generic matrices"""
+    """Test Euclidean map for generic matrices"""
     n_matrices, n_dim0, n_dim1 = 5, 3, 4
     mats = rndstate.randn(n_matrices, n_dim0, n_dim1)
     if complex_valued:
         mats = mats + 1j * rndstate.randn(n_matrices, n_dim0, n_dim1)
     X, C = mats[:n_matrices - 1], mats[-1]
     assert exp_map_euclid(log_map_euclid(X, C), C) == approx(X)
 
 
 @pytest.mark.parametrize("kind", ["spd", "hpd"])
 def test_upper_and_unupper(kind, get_mats):
     """Test upper then unupper should be identity"""
     n_matrices, n_channels = 7, 3
     mats = get_mats(n_matrices, n_channels, kind)
-    mats_ut = unupper(upper(mats))
-    assert mats_ut == approx(mats)
+    assert unupper(upper(mats)) == approx(mats)
 
     n_sets = 2
     mats_4d = np.asarray([mats for _ in range(n_sets)])
-    mats_4d_ut = unupper(upper(mats_4d))
-    assert mats_4d_ut == approx(mats_4d)
+    assert unupper(upper(mats_4d)) == approx(mats_4d)
 
 
 @pytest.mark.parametrize("metric", ["euclid", "logeuclid", "riemann"])
-def test_tangent_space_ndarray(metric, get_covmats):
+def test_tangent_space_ndarray(metric, get_mats):
     """Test tangent space projection"""
     n_matrices, n_channels = 6, 3
     n_ts = (n_channels * (n_channels + 1)) // 2
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     Xts = tangent_space(X, np.eye(n_channels), metric=metric)
     assert Xts.shape == (n_matrices, n_ts)
 
     n_sets = 2
     X_4d = np.asarray([X for _ in range(n_sets)])
     Xts = tangent_space(X_4d, np.eye(n_channels), metric=metric)
     assert Xts.shape == (n_sets, n_matrices, n_ts)
@@ -120,12 +117,12 @@
     X, C = mats[:n_matrices - 1], mats[-1]
     X_t = tangent_space(X, C, metric=metric)
     X_ut = untangent_space(X_t, C, metric=metric)
     assert X_ut == approx(X)
 
 
 @pytest.mark.parametrize("metric", get_metrics())
-def test_transport(metric, get_covmats):
+def test_transport(metric, get_mats):
     n_matrices, n_channels = 10, 3
-    X = get_covmats(n_matrices, n_channels)
+    X = get_mats(n_matrices, n_channels, "spd")
     X_tr = transport(X, np.eye(n_channels), metric=metric)
     assert X_tr.shape == (n_matrices, n_channels, n_channels)
```

### Comparing `pyriemann-0.5/tests/test_utils_test.py` & `pyriemann-0.6/tests/test_utils_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pytest
 
 from pyriemann.utils.test import (
-    is_square, is_sym, is_skew_sym, is_real, is_hermitian,
+    is_square, is_sym, is_skew_sym, is_hankel,
+    is_real, is_real_type, is_hermitian,
     is_pos_def, is_pos_semi_def,
     is_sym_pos_def, is_sym_pos_semi_def,
     is_herm_pos_def, is_herm_pos_semi_def,
 )
 
 
 n = 3
@@ -30,31 +31,45 @@
     A = rndstate.randn(n, n)
     assert is_skew_sym(A - A.T)
     assert not is_skew_sym(np.eye(n))
     assert not is_skew_sym(A + A.T)
     assert not is_skew_sym(np.ones((n, n + 1)))
 
 
+def test_is_hankel():
+    assert is_hankel(np.array([[1, 2, 3], [2, 3, 4], [3, 4, 5]]))
+    assert not is_hankel(np.array([[1, 2, 3], [1, 3, 4], [3, 4, 5]]))
+    assert not is_hankel(np.array([[1, 2, 3], [2, 3, 3], [3, 4, 5]]))
+
+
 def test_is_real(rndstate):
     A = rndstate.randn(n, n + 2)
     assert is_real(A)
 
     B = np.zeros((n, n + 2), dtype=complex)
     B.real = A
     assert is_real(B)
     B.imag = A / 1000.0
     assert not is_real(B)
 
 
+def test_is_real_type(rndstate):
+    A = np.zeros((n, n + 1))
+    assert is_real_type(A)
+
+    B = np.zeros((n, n + 2), dtype=complex)
+    assert not is_real_type(B)
+
+
 def test_is_hermitian(rndstate):
     A = rndstate.randn(n, n)
     B = np.zeros((n, n), dtype=complex)
     B.real, B.imag = A + A.T, A - A.T
     assert is_hermitian(B)
-    assert not is_hermitian(np.ones((n, n + 1)))
+    assert not is_hermitian(np.ones((n, n)) + 1j * np.ones((n, n)))
 
 
 @pytest.mark.parametrize("fast_mode", [True, False])
 def test_is_pos_def(rndstate, fast_mode):
     assert is_pos_def(np.eye(n), fast_mode=fast_mode)
 
     A = rndstate.randn(n, 100)
```

### Comparing `pyriemann-0.5/tests/test_utils_viz.py` & `pyriemann-0.6/tests/test_utils_viz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from conftest import requires_matplotlib
 import numpy as np
 import pytest
 
+from conftest import requires_matplotlib
 from pyriemann.utils.viz import (
     plot_embedding,
     plot_cospectra,
     plot_waveforms
 )
 
 
 @requires_matplotlib
-def test_embedding(get_covmats):
+def test_embedding(get_mats):
     """Test ."""
     n_matrices, n_channels = 5, 3
-    covmats = get_covmats(n_matrices, n_channels)
-    plot_embedding(covmats, y=None, metric="euclid")
-    y = np.ones(covmats.shape[0])
-    plot_embedding(covmats, y=y, metric="euclid")
+    mats = get_mats(n_matrices, n_channels, "spd")
+    plot_embedding(mats, y=None, metric="euclid")
+    y = np.ones(mats.shape[0])
+    plot_embedding(mats, y=y, metric="euclid")
 
 
 @requires_matplotlib
-def test_embedding_error_raise(get_covmats):
+def test_embedding_error_raise(get_mats):
     """Test ValueError for unknown embedding type."""
     n_matrices, n_channels = 5, 3
-    covmats = get_covmats(n_matrices, n_channels)
+    mats = get_mats(n_matrices, n_channels, "spd")
     with pytest.raises(ValueError):
-        plot_embedding(covmats, y=None, metric="euclid", embd_type='foo')
+        plot_embedding(mats, y=None, metric="euclid", embd_type='foo')
 
 
 @requires_matplotlib
 def test_cospectra():
     """Test plot_cospectra"""
     n_freqs, n_channels = 16, 3
     cosp = np.random.randn(n_freqs, n_channels, n_channels)
```

