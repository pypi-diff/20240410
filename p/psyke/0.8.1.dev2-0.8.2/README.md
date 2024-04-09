# Comparing `tmp/psyke-0.8.1.dev2.tar.gz` & `tmp/psyke-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.1.dev2.tar", last modified: Thu Mar 28 19:36:47 2024, max compression
+gzip compressed data, was "psyke-0.8.2.tar", last modified: Tue Apr  9 16:01:11 2024, max compression
```

## Comparing `psyke-0.8.1.dev2.tar` & `psyke-0.8.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.611039 psyke-0.8.1.dev2/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-03-28 19:36:45.000000 psyke-0.8.1.dev2/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.611039 psyke-0.8.1.dev2/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.611039 psyke-0.8.1.dev2/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.611039 psyke-0.8.1.dev2/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.611039 psyke-0.8.1.dev2/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21894 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.615039 psyke-0.8.1.dev2/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 19:36:47.000000 psyke-0.8.1.dev2/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.611039 psyke-0.8.1.dev2/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.619039 psyke-0.8.1.dev2/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-28 19:35:38.000000 psyke-0.8.1.dev2/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 19:35:40.000000 psyke-0.8.1.dev2/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-28 19:35:40.000000 psyke-0.8.1.dev2/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-28 19:35:40.000000 psyke-0.8.1.dev2/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:36:47.623039 psyke-0.8.1.dev2/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 19:35:40.000000 psyke-0.8.1.dev2/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-09 16:00:04.000000 psyke-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 16:00:04.000000 psyke-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-09 16:01:11.588844 psyke-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-09 16:00:04.000000 psyke-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 16:01:11.000000 psyke-0.8.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.576844 psyke-0.8.2/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-09 16:01:09.000000 psyke-0.8.2/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21894 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.580844 psyke-0.8.2/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 16:00:04.000000 psyke-0.8.2/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-09 16:01:11.000000 psyke-0.8.2/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-09 16:01:11.000000 psyke-0.8.2/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:01:11.000000 psyke-0.8.2/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:01:11.000000 psyke-0.8.2/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 16:01:11.000000 psyke-0.8.2/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 16:01:11.000000 psyke-0.8.2/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 16:00:04.000000 psyke-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:01:11.588844 psyke-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-09 16:00:04.000000 psyke-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.576844 psyke-0.8.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.584844 psyke-0.8.2/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-09 16:00:04.000000 psyke-0.8.2/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 16:00:06.000000 psyke-0.8.2/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 16:00:06.000000 psyke-0.8.2/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 16:00:06.000000 psyke-0.8.2/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:01:11.588844 psyke-0.8.2/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 16:00:07.000000 psyke-0.8.2/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.1.dev2/LICENSE` & `psyke-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/PKG-INFO` & `psyke-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.1.dev2
+Version: 0.8.2
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.1.dev2/README.md` & `psyke-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/__init__.py` & `psyke-0.8.2/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/clustering/__init__.py` & `psyke-0.8.2/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/clustering/cream/__init__.py` & `psyke-0.8.2/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/clustering/exact/__init__.py` & `psyke-0.8.2/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/clustering/utils.py` & `psyke-0.8.2/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/__init__.py` & `psyke-0.8.2/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/cart/__init__.py` & `psyke-0.8.2/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/cart/predictor.py` & `psyke-0.8.2/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         surrounding.update(dataframe, self.predictor)
         root = HEx.Node(surrounding, threshold=self.threshold)
         current = [root]
 
         for iteration in self.grid.iterate():
             next_iteration = []
             for node in current:
+                if node.cube.diversity < self.threshold:
+                    continue
                 children, fake = self._cubes_to_split(node.cube, surrounding, iteration, dataframe, fake, True)
                 node.children = [HEx.Node(c, node, threshold=self.threshold) for c in children]
                 cleaned = node.update(fake, self.predictor, False)
                 node.children = [HEx.Node(c, node, threshold=self.threshold) for c in self._merge(
                     [c for c, _ in cleaned], fake)]
                 next_iteration += [n for n in node.children]
```

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.2/psyke/extraction/hypercubic/hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.2/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.2/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.2/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/real/__init__.py` & `psyke-0.8.2/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/real/utils.py` & `psyke-0.8.2/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/trepan/__init__.py` & `psyke-0.8.2/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/extraction/trepan/utils.py` & `psyke-0.8.2/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/hypercubepredictor.py` & `psyke-0.8.2/psyke/hypercubepredictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/schema/__init__.py` & `psyke-0.8.2/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/tuning/__init__.py` & `psyke-0.8.2/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/tuning/crash/__init__.py` & `psyke-0.8.2/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/tuning/orchid/__init__.py` & `psyke-0.8.2/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/tuning/pedro/__init__.py` & `psyke-0.8.2/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/utils/__init__.py` & `psyke-0.8.2/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/utils/dataframe.py` & `psyke-0.8.2/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/utils/logic.py` & `psyke-0.8.2/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/utils/metrics.py` & `psyke-0.8.2/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/utils/plot.py` & `psyke-0.8.2/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke/utils/sorted.py` & `psyke-0.8.2/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/psyke.egg-info/PKG-INFO` & `psyke-0.8.2/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.1.dev2
+Version: 0.8.2
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.1.dev2/psyke.egg-info/SOURCES.txt` & `psyke-0.8.2/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/setup.py` & `psyke-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/__init__.py` & `psyke-0.8.2/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.2/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.2/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.2/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.2/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.2/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/real/test_real.py` & `psyke-0.8.2/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.2/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.2/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.2/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.2/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/utils/test_prune.py` & `psyke-0.8.2/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/utils/test_simplify.py` & `psyke-0.8.2/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.2/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.1.dev2/test/resources/tests/__init__.py` & `psyke-0.8.2/test/resources/tests/__init__.py`

 * *Files identical despite different names*

