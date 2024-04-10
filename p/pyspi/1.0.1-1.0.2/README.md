# Comparing `tmp/pyspi-1.0.1.tar.gz` & `tmp/pyspi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspi-1.0.1.tar", last modified: Fri Mar 15 20:48:15 2024, max compression
+gzip compressed data, was "pyspi-1.0.2.tar", last modified: Wed Apr 10 20:08:33 2024, max compression
```

## Comparing `pyspi-1.0.1.tar` & `pyspi-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.317611 pyspi-1.0.1/
--rw-r--r--   0 joshua     (501) staff       (20)    35137 2024-01-18 09:06:40.000000 pyspi-1.0.1/LICENSE.txt
--rw-r--r--   0 joshua     (501) staff       (20)    13215 2024-03-15 20:48:15.317303 pyspi-1.0.1/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)    11354 2024-03-15 02:59:54.000000 pyspi-1.0.1/README.md
--rw-r--r--   0 joshua     (501) staff       (20)     1229 2024-03-15 20:46:02.000000 pyspi-1.0.1/pyproject.toml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.305471 pyspi-1.0.1/pyspi/
--rw-r--r--   0 joshua     (501) staff       (20)      532 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     4511 2024-02-10 05:15:52.000000 pyspi-1.0.1/pyspi/base.py
--rw-r--r--   0 joshua     (501) staff       (20)    31205 2024-03-15 02:59:54.000000 pyspi-1.0.1/pyspi/calculator.py
--rw-r--r--   0 joshua     (501) staff       (20)    25298 2024-03-15 02:59:54.000000 pyspi-1.0.1/pyspi/config.yaml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.307650 pyspi-1.0.1/pyspi/data/
--rw-r--r--   0 joshua     (501) staff       (20)    40128 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/data/cml.npy
--rw-r--r--   0 joshua     (501) staff       (20)     5728 2024-03-13 19:42:57.000000 pyspi-1.0.1/pyspi/data/cml7.npy
--rw-r--r--   0 joshua     (501) staff       (20)    14128 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/data/forex.npy
--rw-r--r--   0 joshua     (501) staff       (20)     8128 2024-02-09 10:05:41.000000 pyspi-1.0.1/pyspi/data/standard_normal.npy
--rw-r--r--   0 joshua     (501) staff       (20)     9248 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/data.py
--rw-r--r--   0 joshua     (501) staff       (20)     1033 2024-03-15 02:59:54.000000 pyspi-1.0.1/pyspi/fabfour_config.yaml
--rw-r--r--   0 joshua     (501) staff       (20)    21771 2024-03-15 02:59:54.000000 pyspi-1.0.1/pyspi/fast_config.yaml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.307958 pyspi-1.0.1/pyspi/lib/
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.308081 pyspi-1.0.1/pyspi/lib/PhiToolbox/
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.310087 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2188 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)     3266 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m
--rw-r--r--   0 joshua     (501) staff       (20)     5053 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m
--rw-r--r--   0 joshua     (501) staff       (20)     4099 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)     1913 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_comp.m
--rw-r--r--   0 joshua     (501) staff       (20)     2181 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m
--rw-r--r--   0 joshua     (501) staff       (20)     3442 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/__init__.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.310696 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.311671 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/
--rw-r--r--   0 joshua     (501) staff       (20)     1539 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m
--rw-r--r--   0 joshua     (501) staff       (20)      321 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/Cov_cond.m
--rw-r--r--   0 joshua     (501) staff       (20)      420 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/H_gauss.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)      173 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/logdet.m
--rw-r--r--   0 joshua     (501) staff       (20)      740 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2699 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/data_to_probs.m
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/__init__.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.312024 pyspi-1.0.1/pyspi/lib/jidt/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/jidt/__init__.py
--rwxr-xr-x   0 joshua     (501) staff       (20)   613523 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/lib/jidt/infodynamics.jar
--rw-r--r--   0 joshua     (501) staff       (20)     3626 2024-03-15 02:59:54.000000 pyspi-1.0.1/pyspi/sonnet_config.yaml
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.315556 pyspi-1.0.1/pyspi/statistics/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/statistics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5759 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/statistics/basic.py
--rw-r--r--   0 joshua     (501) staff       (20)     5085 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/statistics/causal.py
--rw-r--r--   0 joshua     (501) staff       (20)     7425 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/statistics/distance.py
--rw-r--r--   0 joshua     (501) staff       (20)    20180 2024-03-15 02:59:54.000000 pyspi-1.0.1/pyspi/statistics/infotheory.py
--rw-r--r--   0 joshua     (501) staff       (20)     5235 2024-01-30 05:07:34.000000 pyspi-1.0.1/pyspi/statistics/misc.py
--rw-r--r--   0 joshua     (501) staff       (20)    14437 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/statistics/spectral.py
--rw-r--r--   0 joshua     (501) staff       (20)     6796 2024-01-18 09:06:41.000000 pyspi-1.0.1/pyspi/statistics/wavelet.py
--rw-r--r--   0 joshua     (501) staff       (20)     8458 2024-03-15 20:46:02.000000 pyspi-1.0.1/pyspi/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.316716 pyspi-1.0.1/pyspi.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)    13215 2024-03-15 20:48:15.000000 pyspi-1.0.1/pyspi.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     1524 2024-03-15 20:48:15.000000 pyspi-1.0.1/pyspi.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2024-03-15 20:48:15.000000 pyspi-1.0.1/pyspi.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      326 2024-03-15 20:48:15.000000 pyspi-1.0.1/pyspi.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)        6 2024-03-15 20:48:15.000000 pyspi-1.0.1/pyspi.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2024-03-15 20:48:15.317671 pyspi-1.0.1/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     3134 2024-03-15 20:46:02.000000 pyspi-1.0.1/setup.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-03-15 20:48:15.316356 pyspi-1.0.1/tests/
--rw-r--r--   0 joshua     (501) staff       (20)     3676 2024-03-15 02:59:54.000000 pyspi-1.0.1/tests/test_SPIs.py
--rw-r--r--   0 joshua     (501) staff       (20)    15412 2024-03-15 20:01:23.000000 pyspi-1.0.1/tests/test_calc.py
--rw-r--r--   0 joshua     (501) staff       (20)     5392 2024-03-15 20:46:02.000000 pyspi-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.999888 pyspi-1.0.2/
+-rw-r--r--   0 joshua     (501) staff       (20)    35137 2024-01-18 09:06:40.000000 pyspi-1.0.2/LICENSE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)    13215 2024-04-10 20:08:32.999410 pyspi-1.0.2/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)    11354 2024-03-15 02:59:54.000000 pyspi-1.0.2/README.md
+-rw-r--r--   0 joshua     (501) staff       (20)     1229 2024-04-10 19:05:24.000000 pyspi-1.0.2/pyproject.toml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.984723 pyspi-1.0.2/pyspi/
+-rw-r--r--   0 joshua     (501) staff       (20)      532 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     4511 2024-02-10 05:15:52.000000 pyspi-1.0.2/pyspi/base.py
+-rw-r--r--   0 joshua     (501) staff       (20)    31205 2024-03-15 02:59:54.000000 pyspi-1.0.2/pyspi/calculator.py
+-rw-r--r--   0 joshua     (501) staff       (20)    25487 2024-04-10 19:21:14.000000 pyspi-1.0.2/pyspi/config.yaml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.987139 pyspi-1.0.2/pyspi/data/
+-rw-r--r--   0 joshua     (501) staff       (20)    40128 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/data/cml.npy
+-rw-r--r--   0 joshua     (501) staff       (20)     5728 2024-03-13 19:42:57.000000 pyspi-1.0.2/pyspi/data/cml7.npy
+-rw-r--r--   0 joshua     (501) staff       (20)    14128 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/data/forex.npy
+-rw-r--r--   0 joshua     (501) staff       (20)     8128 2024-02-09 10:05:41.000000 pyspi-1.0.2/pyspi/data/standard_normal.npy
+-rw-r--r--   0 joshua     (501) staff       (20)     9248 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/data.py
+-rw-r--r--   0 joshua     (501) staff       (20)     1033 2024-03-15 02:59:54.000000 pyspi-1.0.2/pyspi/fabfour_config.yaml
+-rw-r--r--   0 joshua     (501) staff       (20)    21968 2024-04-10 19:22:42.000000 pyspi-1.0.2/pyspi/fast_config.yaml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.987467 pyspi-1.0.2/pyspi/lib/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.987598 pyspi-1.0.2/pyspi/lib/PhiToolbox/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.989668 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2188 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)     3266 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m
+-rw-r--r--   0 joshua     (501) staff       (20)     5053 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m
+-rw-r--r--   0 joshua     (501) staff       (20)     4099 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)     1913 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_comp.m
+-rw-r--r--   0 joshua     (501) staff       (20)     2181 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m
+-rw-r--r--   0 joshua     (501) staff       (20)     3442 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/__init__.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.990249 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.991469 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/
+-rw-r--r--   0 joshua     (501) staff       (20)     1539 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m
+-rw-r--r--   0 joshua     (501) staff       (20)      321 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/Cov_cond.m
+-rw-r--r--   0 joshua     (501) staff       (20)      420 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/H_gauss.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)      173 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/logdet.m
+-rw-r--r--   0 joshua     (501) staff       (20)      740 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2699 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/data_to_probs.m
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/__init__.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.991893 pyspi-1.0.2/pyspi/lib/jidt/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/jidt/__init__.py
+-rwxr-xr-x   0 joshua     (501) staff       (20)   613523 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/lib/jidt/infodynamics.jar
+-rw-r--r--   0 joshua     (501) staff       (20)     3626 2024-03-15 02:59:54.000000 pyspi-1.0.2/pyspi/sonnet_config.yaml
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.997544 pyspi-1.0.2/pyspi/statistics/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/statistics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5759 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/statistics/basic.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5085 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/statistics/causal.py
+-rw-r--r--   0 joshua     (501) staff       (20)     9231 2024-04-08 19:22:18.000000 pyspi-1.0.2/pyspi/statistics/distance.py
+-rw-r--r--   0 joshua     (501) staff       (20)    20180 2024-03-15 02:59:54.000000 pyspi-1.0.2/pyspi/statistics/infotheory.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5235 2024-01-30 05:07:34.000000 pyspi-1.0.2/pyspi/statistics/misc.py
+-rw-r--r--   0 joshua     (501) staff       (20)    14437 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/statistics/spectral.py
+-rw-r--r--   0 joshua     (501) staff       (20)     6796 2024-01-18 09:06:41.000000 pyspi-1.0.2/pyspi/statistics/wavelet.py
+-rw-r--r--   0 joshua     (501) staff       (20)     8458 2024-03-15 20:46:02.000000 pyspi-1.0.2/pyspi/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.998775 pyspi-1.0.2/pyspi.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)    13215 2024-04-10 20:08:32.000000 pyspi-1.0.2/pyspi.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     1524 2024-04-10 20:08:32.000000 pyspi-1.0.2/pyspi.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2024-04-10 20:08:32.000000 pyspi-1.0.2/pyspi.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      326 2024-04-10 20:08:32.000000 pyspi-1.0.2/pyspi.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        6 2024-04-10 20:08:32.000000 pyspi-1.0.2/pyspi.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2024-04-10 20:08:32.999954 pyspi-1.0.2/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     3134 2024-04-10 19:05:38.000000 pyspi-1.0.2/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-10 20:08:32.998398 pyspi-1.0.2/tests/
+-rw-r--r--   0 joshua     (501) staff       (20)     3571 2024-04-10 07:04:02.000000 pyspi-1.0.2/tests/test_SPIs.py
+-rw-r--r--   0 joshua     (501) staff       (20)    15412 2024-03-15 20:01:23.000000 pyspi-1.0.2/tests/test_calc.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5392 2024-03-15 20:46:02.000000 pyspi-1.0.2/tests/test_utils.py
```

### Comparing `pyspi-1.0.1/LICENSE.txt` & `pyspi-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/PKG-INFO` & `pyspi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for pairwise analysis of time series data.
 Home-page: https://github.com/DynamicsAndNeuralSystems/pyspi
 Author: Oliver M. Cliff
 Author-email: "Oliver M. Cliff" <oliver.m.cliff@gmail.com>
 Maintainer: Joshua B. Moore
 Maintainer-email: joshua.moore@sydney.edu.au
 License: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyspi Version: 1.0.1 Summary: Library for pairwise
+Metadata-Version: 2.1 Name: pyspi Version: 1.0.2 Summary: Library for pairwise
 analysis of time series data. Home-page: https://github.com/
 DynamicsAndNeuralSystems/pyspi Author: Oliver M. Cliff Author-email: "Oliver M.
 Cliff"
 gmail.com> Maintainer: Joshua B. Moore Maintainer-email:
 joshua.moore@sydney.edu.au License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/DynamicsAndNeuralSystems/pyspi
 Project-URL: Documentation, https://time-series-features.gitbook.io/pyspi/
```

### Comparing `pyspi-1.0.1/README.md` & `pyspi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyproject.toml` & `pyspi-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyspi"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name ="Oliver M. Cliff", email="oliver.m.cliff@gmail.com"},
 ]
 maintainers = [
     {name = "Joshua B. Moore"},
     {email = "joshua.moore@sydney.edu.au"},
 ]
```

### Comparing `pyspi-1.0.1/pyspi/__init__.py` & `pyspi-1.0.2/pyspi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/base.py` & `pyspi-1.0.2/pyspi/base.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/calculator.py` & `pyspi-1.0.2/pyspi/calculator.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/config.yaml` & `pyspi-1.0.2/pyspi/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,25 @@
         statistic: mean
         squared: True
 
       - mode: softdtw
         statistic: max
         squared: True
 
+  # Gromov-Wasserstain Distance
+  GromovWasserstainTau:
+    labels:
+      - unsigned
+      - distance
+      - unordered
+      - nonlinear
+      - undirected
+    dependencies:
+    configs:
+
 .statistics.causal:
   # Additive noise model
   AdditiveNoiseModel:
     labels:
       - directed
       - nonlinear
       - unsigned
```

### Comparing `pyspi-1.0.1/pyspi/data/cml.npy` & `pyspi-1.0.2/pyspi/data/cml.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/data/cml7.npy` & `pyspi-1.0.2/pyspi/data/cml7.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/data/forex.npy` & `pyspi-1.0.2/pyspi/data/forex.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/data/standard_normal.npy` & `pyspi-1.0.2/pyspi/data/standard_normal.npy`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/data.py` & `pyspi-1.0.2/pyspi/data.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/fabfour_config.yaml` & `pyspi-1.0.2/pyspi/fabfour_config.yaml`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/fast_config.yaml` & `pyspi-1.0.2/pyspi/fast_config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,25 @@
       - mode: euclidean
         statistic: mean
         squared: True
 
       - mode: euclidean
         statistic: max
         squared: True
+        
+  # Gromov-Wasserstain Distance
+  GromovWasserstainTau:
+    labels:
+      - unsigned
+      - distance
+      - unordered
+      - nonlinear
+      - undirected
+    dependencies:
+    configs:
 
 .statistics.causal:
   # Additive noise model
   AdditiveNoiseModel:
     labels:
       - directed
       - nonlinear
```

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_AL.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_G_Gauss_LBFGS.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_Gauss.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_comp.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_comp.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_comp_probs.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/Phi/phi_star_Gauss.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/Gauss/Cov_comp.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/I_s_I_s_d.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/PhiToolbox/utility/data_to_probs.m` & `pyspi-1.0.2/pyspi/lib/PhiToolbox/utility/data_to_probs.m`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/lib/jidt/infodynamics.jar` & `pyspi-1.0.2/pyspi/lib/jidt/infodynamics.jar`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/sonnet_config.yaml` & `pyspi-1.0.2/pyspi/sonnet_config.yaml`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/statistics/basic.py` & `pyspi-1.0.2/pyspi/statistics/basic.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/statistics/causal.py` & `pyspi-1.0.2/pyspi/statistics/causal.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/statistics/distance.py` & `pyspi-1.0.2/pyspi/statistics/distance.py`

 * *Files 16% similar despite different names*

```diff
@@ -255,7 +255,66 @@
             except AttributeError:
                 data.barycenter = {self._mode: {(i, j): bc}}
             except KeyError:
                 data.barycenter[self._mode] = {(i, j): bc}
             data.barycenter[self._mode][(j, i)] = data.barycenter[self._mode][(i, j)]
 
         return self._statfn(bc)
+
+
+class GromovWasserstainTau(Undirected, Unsigned):
+    """Gromov-Wasserstain distance (GWTau)"""
+
+    name = "Gromov-Wasserstain Distance"
+    identifier = "gwtau"
+    labels = ["unsigned", "distance", "unordered", "nonlinear", "undirected"]
+
+    @staticmethod
+    def vec_geo_dist(x):
+        diffs = np.diff(x, axis=0)
+        distances = np.linalg.norm(diffs, axis=1)
+        return np.cumsum(distances)
+    
+    @staticmethod
+    def wass_sorted(x1, x2):
+        x1 = np.sort(x1)[::-1] # sort in descending order
+        x2 = np.sort(x2)[::-1] 
+
+        if len(x1) == len(x2):
+            res = np.sqrt(np.mean((x1 - x2) ** 2))
+        else:
+            N, M = len(x1), len(x2)
+            i_ratios = np.arange(1, N + 1) / N
+            j_ratios = np.arange(1, M + 1) / M
+        
+        
+            min_values = np.minimum.outer(i_ratios, j_ratios)
+            max_values = np.maximum.outer(i_ratios - 1/N, j_ratios - 1/M)
+        
+            lam = np.where(min_values > max_values, min_values - max_values, 0)
+        
+            diffs_squared = (x1[:, None] - x2) ** 2
+            my_sum = np.sum(lam * diffs_squared)
+        
+            res = np.sqrt(my_sum)
+
+        return res
+    
+    @staticmethod
+    def gwtau(xi, xj):
+        timei = np.arange(len(xi))
+        timej = np.arange(len(xj))
+        traji = np.column_stack([timei, xi])
+        trajj = np.column_stack([timej, xj])
+
+        vi = GromovWasserstainTau.vec_geo_dist(traji)
+        vj = GromovWasserstainTau.vec_geo_dist(trajj)
+        gw = GromovWasserstainTau.wass_sorted(vi, vj)
+    
+        return gw
+
+    @parse_bivariate
+    def bivariate(self, data, i=None, j=None):
+        x, y = data.to_numpy()[[i, j]]
+        # insert compute SPI code here (computes on x and y)
+        stat = self.gwtau(x, y)
+        return stat
```

### Comparing `pyspi-1.0.1/pyspi/statistics/infotheory.py` & `pyspi-1.0.2/pyspi/statistics/infotheory.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/statistics/misc.py` & `pyspi-1.0.2/pyspi/statistics/misc.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/statistics/spectral.py` & `pyspi-1.0.2/pyspi/statistics/spectral.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/statistics/wavelet.py` & `pyspi-1.0.2/pyspi/statistics/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi/utils.py` & `pyspi-1.0.2/pyspi/utils.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/pyspi.egg-info/PKG-INFO` & `pyspi-1.0.2/pyspi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for pairwise analysis of time series data.
 Home-page: https://github.com/DynamicsAndNeuralSystems/pyspi
 Author: Oliver M. Cliff
 Author-email: "Oliver M. Cliff" <oliver.m.cliff@gmail.com>
 Maintainer: Joshua B. Moore
 Maintainer-email: joshua.moore@sydney.edu.au
 License: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyspi Version: 1.0.1 Summary: Library for pairwise
+Metadata-Version: 2.1 Name: pyspi Version: 1.0.2 Summary: Library for pairwise
 analysis of time series data. Home-page: https://github.com/
 DynamicsAndNeuralSystems/pyspi Author: Oliver M. Cliff Author-email: "Oliver M.
 Cliff"
 gmail.com> Maintainer: Joshua B. Moore Maintainer-email:
 joshua.moore@sydney.edu.au License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/DynamicsAndNeuralSystems/pyspi
 Project-URL: Documentation, https://time-series-features.gitbook.io/pyspi/
```

### Comparing `pyspi-1.0.1/pyspi.egg-info/SOURCES.txt` & `pyspi-1.0.2/pyspi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/setup.py` & `pyspi-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                         'lib/PhiToolbox/utility/Gauss/H_gauss.m',
                         'lib/PhiToolbox/utility/Gauss/logdet.m',
                         'data/cml.npy',
                         'data/forex.npy',
                         'data/standard_normal.npy',
                         'data/cml7.npy']},
     include_package_data=True,
-    version='1.0.1',
+    version='1.0.2',
     description='Library for pairwise analysis of time series data.',
     author='Oliver M. Cliff',
     author_email='oliver.m.cliff@gmail.com',
     url='https://github.com/DynamicsAndNeuralSystems/pyspi',
     long_description=long_description,
     classifiers=[
         "Programming Language :: Python",
```

### Comparing `pyspi-1.0.1/tests/test_SPIs.py` & `pyspi-1.0.2/tests/test_SPIs.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,46 +57,46 @@
     """Run the benchmarking tests."""
     zscore_threshold = 2 # 2 sigma
     
     # separate the the mean and std. dev tables for the benchmark
     mean_table = mpi_benchmark['mean']
     std_table = mpi_benchmark['std']
 
-    # check std stable for zeros and impute with smallest non-zero value
-    min_nonzero_std = np.nanmin(std_table[std_table > 0])
-    std_table[std_table == 0] = min_nonzero_std
-     
-
+    # check std table for zeros and impute with smallest non-zero value
+    std_table = np.where(std_table == 0, 1e-10, std_table)
+    
     # check that the shapes are equal
     assert mean_table.shape == mpi_new.shape, f"SPI: {est}| Different table shapes. "
 
     # convert NaNs to zeros before proeceeding - this will take care of diagonal and any null outputs
     mpi_new = np.nan_to_num(mpi_new)
     mpi_mean = np.nan_to_num(mean_table)
 
     # check if matrix is symmetric (undirected SPI) for num exceed correction
     isSymmetric = "undirected" in est_ob.labels 
 
     # get the module name for easy reference
     module_name = est_ob.__module__.split(".")[-1]
 
-    if (mpi_new == mpi_mean).all() == False:
+    if not np.allclose(mpi_new, mpi_mean):
         # tables are not equivalent, quantify the difference by z-scoring.
         diff = abs(mpi_new - mpi_mean)
         zscores = diff/std_table
+
         idxs_greater_than_thresh = np.argwhere(zscores > zscore_threshold)
+
         if len(idxs_greater_than_thresh) > 0:
-            sigs = list()
-            for idx in idxs_greater_than_thresh:
-                sigs.append(zscores[idx[0], idx[1]])
+            sigs = zscores[idxs_greater_than_thresh[:, 0], idxs_greater_than_thresh[:, 1]]
             # get the max
             max_z = max(sigs)
+
             # number of interactions
-            num_iteractions = (mpi_new.shape[0] * mpi_new.shape[1]) - mpi_new.shape[0]
+            num_interactions = mpi_new.size - mpi_new.shape[0]
             # count exceedances
             num_exceed = len(sigs)
+
             if isSymmetric:
                 # number of unique exceedences is half
-                num_exceed /= 2
-                num_iteractions /= 2
+                num_exceed //= 2
+                num_interactions //= 2
 
-            spi_warning_logger(est, module_name, max_z, int(num_exceed), int(num_iteractions))
+            spi_warning_logger(est, module_name, max_z, int(num_exceed), int(num_interactions))
```

### Comparing `pyspi-1.0.1/tests/test_calc.py` & `pyspi-1.0.2/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `pyspi-1.0.1/tests/test_utils.py` & `pyspi-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

