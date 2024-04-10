# Comparing `tmp/autogluon.timeseries-1.0.1b20240408.tar.gz` & `tmp/autogluon.timeseries-1.1.0b20240409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.0.1b20240408.tar", last modified: Mon Apr  8 09:05:42 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.0b20240409.tar", last modified: Tue Apr  9 09:06:08 2024, max compression
```

## Comparing `autogluon.timeseries-1.0.1b20240408.tar` & `autogluon.timeseries-1.1.0b20240409.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.742568 autogluon.timeseries-1.0.1b20240408/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:05:42.742568 autogluon.timeseries-1.0.1b20240408/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.730568 autogluon.timeseries-1.0.1b20240408/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.730568 autogluon.timeseries-1.0.1b20240408/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/chronos/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.734568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.738568 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-08 09:04:26.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:05:42.730568 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:05:42.000000 autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.545612 autogluon.timeseries-1.1.0b20240409/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.545612 autogluon.timeseries-1.1.0b20240409/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.0.1b20240408/PKG-INFO` & `autogluon.timeseries-1.1.0b20240409/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.0.1b20240408
+Version: 1.1.0b20240409
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.0.1b20240408/setup.py` & `autogluon.timeseries-1.1.0b20240409/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,25 +52,24 @@
         "ruff>=0.0.285",
         "flaky>=3.7,<4",
         "pytest-timeout>=2.1,<3",
         "isort>=5.10",
         "black~=23.0",
     ],
     "chronos-openvino": [  # for faster CPU inference in pretrained models with OpenVINO
-        "optimum-intel[openvino,nncf]>=1.16,<1.17",
-        "optimum[openvino,nncf]>=1.18,<1.19",
+        "optimum-intel[openvino,nncf]>=1.15,<1.17",
+        "optimum[openvino,nncf]>=1.17,<1.19",
     ],
     "chronos-onnx": [  # for faster CPU inference in pretrained models with ONNX
-        "optimum[onnxruntime]>=1.18,<1.19",
+        "optimum[onnxruntime]>=1.17,<1.19",
     ],
 }
 
-extras_require["all"] = list(
-    set.union(*(set(extras_require[extra]) for extra in ["chronos-onnx", "chronos-openvino"]))
-)
+# TODO: add openvino back to "all" after dependency versions are relaxed
+extras_require["all"] = list(set.union(*(set(extras_require[extra]) for extra in ["chronos-onnx"])))
 
 install_requires = ag.get_dependency_version_ranges(install_requires)
 
 if __name__ == "__main__":
     ag.create_version_file(version=version, submodule=submodule)
     setup_args = ag.default_setup_args(version=version, submodule=submodule)
     setup(
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,21 +369,22 @@
         return self._score_with_predictions(data=data, predictions=predictions, metric=metric)
 
     def score_and_cache_oof(
         self,
         val_data: TimeSeriesDataFrame,
         store_val_score: bool = False,
         store_predict_time: bool = False,
+        **predict_kwargs,
     ) -> None:
         """Compute val_score, predict_time and cache out-of-fold (OOF) predictions."""
         past_data, known_covariates = val_data.get_model_inputs_for_scoring(
             prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates
         )
         predict_start_time = time.time()
-        oof_predictions = self.predict(past_data, known_covariates=known_covariates)
+        oof_predictions = self.predict(past_data, known_covariates=known_covariates, **predict_kwargs)
         self._oof_predictions = [oof_predictions]
         if store_predict_time:
             self.predict_time = time.time() - predict_start_time
         if store_val_score:
             self.val_score = self._score_with_predictions(val_data, oof_predictions)
 
     def _get_hpo_train_fn_kwargs(self, **train_fn_kwargs) -> dict:
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,50 +49,14 @@
     "mini": "amazon/chronos-t5-mini",
     "small": "amazon/chronos-t5-small",
     "base": "amazon/chronos-t5-base",
     "large": "amazon/chronos-t5-large",
 }
 
 
-class ChronosInferenceDataset:
-    """A container for time series datasets that implements the ``torch.utils.data.Dataset`` interface"""
-
-    def __init__(
-        self,
-        target_df: TimeSeriesDataFrame,
-        context_length: int,
-        target_column: str = "target",
-    ):
-        assert context_length > 0
-        self.context_length = context_length
-        self.target_array = target_df[target_column].to_numpy(dtype=np.float32)
-        self.freq = target_df.freq
-
-        # store pointer to start:end of each time series
-        cum_sizes = target_df.num_timesteps_per_item().values.cumsum()
-        self.indptr = np.append(0, cum_sizes).astype(np.int32)
-
-    def __len__(self):
-        return len(self.indptr) - 1  # noqa
-
-    def _get_context(self, a: np.ndarray, pad_value=np.nan):
-        a = a[-self.context_length :]
-        pad_size = self.context_length - len(a)
-        if pad_size > 0:
-            pad = np.full(shape=(pad_size,), fill_value=pad_value)
-            a = np.concatenate((pad, a))
-        return a
-
-    def __getitem__(self, idx) -> np.ndarray:
-        start_idx = self.indptr[idx]
-        end_idx = self.indptr[idx + 1]
-
-        return self._get_context(self.target_array[start_idx:end_idx])
-
-
 class ChronosModel(AbstractTimeSeriesModel):
     """Chronos pretrained time series forecasting models, based on the original
     `ChronosModel <https://github.com/amazon-science/chronos-forecasting>`_ implementation.
 
     Chronos is family of pretrained models, based on the T5 family, with number of parameters ranging between 8M and 710M.
     The full collection of Chronos models is available on
     `Hugging Face <https://huggingface.co/collections/amazon/chronos-models-65f1791d630a8d57cb718444>`_. For Chronos small,
@@ -192,14 +156,15 @@
             name=name,
             eval_metric=eval_metric,
             hyperparameters=hyperparameters,
             **kwargs,
         )
 
         self.model_pipeline: Optional[Any] = None  # of type OptimizedChronosPipeline
+        self.time_limit: Optional[float] = None
 
     def save(self, path: str = None, verbose: bool = True) -> str:
         pipeline = self.model_pipeline
         self.model_pipeline = None
         path = super().save(path=path, verbose=verbose)
         self.model_pipeline = pipeline
 
@@ -284,34 +249,37 @@
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: int = None,
         **kwargs,
     ) -> None:
         self._check_fit_params()
+        self.time_limit = time_limit
 
     def _get_inference_data_loader(
         self,
         data: TimeSeriesDataFrame,
         context_length: int,
         num_workers: int = 0,
+        time_limit: Optional[float] = None,
     ):
-        import torch
+        from .utils import ChronosInferenceDataLoader, ChronosInferenceDataset, timeout_callback
 
         chronos_dataset = ChronosInferenceDataset(
             target_df=data,
             target_column=self.target,
             context_length=context_length,
         )
 
-        return torch.utils.data.DataLoader(
+        return ChronosInferenceDataLoader(
             chronos_dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=num_workers,
+            on_batch=timeout_callback(seconds=time_limit),
         )
 
     def _predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         **kwargs,
@@ -329,31 +297,33 @@
         with warning_filter(all_warnings=True):
             import torch
 
             if self.model_pipeline is None:
                 # load model pipeline to device memory
                 self.load_model_pipeline(context_length=context_length)
 
+            inference_data_loader = self._get_inference_data_loader(
+                data=data,
+                num_workers=self.data_loader_num_workers,
+                context_length=context_length,
+                time_limit=kwargs.get("time_limit"),
+            )
             self.model_pipeline.model.eval()
             with torch.inference_mode():
                 prediction_samples = [
                     self.model_pipeline.predict(
                         batch,
                         prediction_length=self.prediction_length,
                         num_samples=self.num_samples,
                         limit_prediction_length=False,
                     )
                     .detach()
                     .cpu()
                     .numpy()
-                    for batch in self._get_inference_data_loader(
-                        data=data,
-                        num_workers=self.data_loader_num_workers,
-                        context_length=context_length,
-                    )
+                    for batch in inference_data_loader
                 ]
 
         samples = np.concatenate(prediction_samples, axis=0).swapaxes(1, 2).reshape(-1, self.num_samples)
 
         mean = samples.mean(axis=-1, keepdims=True)
         quantiles = np.quantile(samples, self.quantile_levels, axis=-1).T
 
@@ -363,7 +333,20 @@
             index=get_forecast_horizon_index_ts_dataframe(data, self.prediction_length),
         )
 
         return TimeSeriesDataFrame(df)
 
     def _more_tags(self) -> Dict:
         return {"allow_nan": True}
+
+    def score_and_cache_oof(
+        self,
+        val_data: TimeSeriesDataFrame,
+        store_val_score: bool = False,
+        store_predict_time: bool = False,
+        **predict_kwargs,
+    ) -> None:
+        # All computation happens during inference, so we provide the time_limit at prediction time
+        # TODO: Once custom predict_kwargs is allowed, make sure that `time_limit` is not among the keys
+        super().score_and_cache_oof(
+            val_data, store_val_score, store_predict_time, time_limit=self.time_limit, **predict_kwargs
+        )
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,18 @@
             data = data.groupby(level=ITEMID, sort=False).tail(self.max_ts_length)
 
         df = pd.DataFrame(data).reset_index(level=ITEMID)
         all_series = (ts for _, ts in df.groupby(by=ITEMID, as_index=False, sort=False)[self.target])
 
         # timeout ensures that no individual job takes longer than time_limit
         # TODO: a job started late may still exceed time_limit - how to prevent that?
-        timeout = None if self.n_jobs == 1 else self.time_limit
+        time_limit = kwargs.get("time_limit")
+        timeout = None if self.n_jobs == 1 else time_limit
         # end_time ensures that no new jobs are started after time_limit is exceeded
-        end_time = None if self.time_limit is None else time.time() + self.time_limit
+        end_time = None if time_limit is None else time.time() + time_limit
         executor = Parallel(self.n_jobs, timeout=timeout)
 
         try:
             with warning_filter():
                 predictions_with_flags = executor(
                     delayed(self._predict_wrapper)(ts, end_time=end_time) for ts in all_series
                 )
@@ -165,19 +166,24 @@
                 f"({fraction_failed_models:.1%}). Fallback model SeasonalNaive was used for these time series."
             )
         predictions_df = pd.concat([pred for pred, _ in predictions_with_flags])
         predictions_df.index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
         return TimeSeriesDataFrame(predictions_df)
 
     def score_and_cache_oof(
-        self, val_data: TimeSeriesDataFrame, store_val_score: bool = False, store_predict_time: bool = False
+        self,
+        val_data: TimeSeriesDataFrame,
+        store_val_score: bool = False,
+        store_predict_time: bool = False,
+        **predict_kwargs,
     ) -> None:
-        super().score_and_cache_oof(val_data, store_val_score, store_predict_time)
-        # Remove time_limit for future predictions
-        self.time_limit = None
+        # All computation happens during inference, so we provide the time_limit at prediction time
+        super().score_and_cache_oof(
+            val_data, store_val_score, store_predict_time, time_limit=self.time_limit, **predict_kwargs
+        )
 
     def _predict_wrapper(self, time_series: pd.Series, end_time: Optional[float] = None) -> Tuple[pd.DataFrame, bool]:
         if end_time is not None and time.time() >= end_time:
             raise TimeLimitExceeded
 
         if time_series.isna().all():
             result = self._dummy_forecast.copy()
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         return self.most_recent_model.predict(data, known_covariates=known_covariates, **kwargs)
 
     def score_and_cache_oof(
         self,
         val_data: TimeSeriesDataFrame,
         store_val_score: bool = False,
         store_predict_time: bool = False,
+        **predict_kwargs,
     ) -> None:
         # self.val_score, self.predict_time, self._oof_predictions already saved during _fit()
         assert self._oof_predictions is not None
         if store_val_score:
             assert self.val_score is not None
         if store_predict_time:
             assert self.predict_time is not None
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.0.1b20240408
+Version: 1.1.0b20240409
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/autogluon/timeseries/models/abstract/model_trial.py
 src/autogluon/timeseries/models/autogluon_tabular/__init__.py
 src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
 src/autogluon/timeseries/models/autogluon_tabular/utils.py
 src/autogluon/timeseries/models/chronos/__init__.py
 src/autogluon/timeseries/models/chronos/model.py
 src/autogluon/timeseries/models/chronos/pipeline.py
+src/autogluon/timeseries/models/chronos/utils.py
 src/autogluon/timeseries/models/ensemble/__init__.py
 src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
 src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
 src/autogluon/timeseries/models/gluonts/__init__.py
 src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
 src/autogluon/timeseries/models/gluonts/torch/__init__.py
 src/autogluon/timeseries/models/gluonts/torch/models.py
```

### Comparing `autogluon.timeseries-1.0.1b20240408/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.0.1b20240408
-autogluon.common==1.0.1b20240408
-autogluon.tabular[catboost,lightgbm,xgboost]==1.0.1b20240408
+autogluon.core[raytune]==1.1.0b20240409
+autogluon.common==1.1.0b20240409
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240409
 
 [all]
-optimum[onnxruntime]<1.19,>=1.18
-optimum-intel[nncf,openvino]<1.17,>=1.16
-optimum[nncf,openvino]<1.19,>=1.18
+optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
-optimum[onnxruntime]<1.19,>=1.18
+optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-openvino]
-optimum-intel[nncf,openvino]<1.17,>=1.16
-optimum[nncf,openvino]<1.19,>=1.18
+optimum-intel[nncf,openvino]<1.17,>=1.15
+optimum[nncf,openvino]<1.19,>=1.17
 
 [tests]
 pytest
 ruff>=0.0.285
 flaky<4,>=3.7
 pytest-timeout<3,>=2.1
 isort>=5.10
```

