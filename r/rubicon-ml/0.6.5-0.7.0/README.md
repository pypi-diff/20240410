# Comparing `tmp/rubicon-ml-0.6.5.tar.gz` & `tmp/rubicon-ml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-ml-0.6.5.tar", last modified: Wed Mar 13 17:36:48 2024, max compression
+gzip compressed data, was "rubicon-ml-0.7.0.tar", last modified: Tue Apr  9 18:50:00 2024, max compression
```

## Comparing `rubicon-ml-0.6.5.tar` & `rubicon-ml-0.7.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/rubicon_ml/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/rubicon_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.930609 rubicon-ml-0.6.5/rubicon_ml/client/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    27487 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18269 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/rubicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/rubicon_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/client/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/utils/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/client/utils/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/utils/training_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/domain/utils/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/repository/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49100 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/repository/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/repository/utils/slugify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.934609 rubicon-ml-0.6.5/rubicon_ml/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.938609 rubicon-ml-0.6.5/rubicon_ml/schema/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OGeneralizedLinearEstimator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OGradientBoostingEstimator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2ORandomForestEstimator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OTargetEncoderEstimator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OXGBoostEstimator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/lightgbm__LGBMClassifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/lightgbm__LGBMModel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/lightgbm__LGBMRegressor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/sklearn__RandomForestClassifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/xgboost__DaskXGBClassifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/xgboost__DaskXGBRegressor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/xgboost__XGBClassifier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/xgboost__XGBModel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/schema/schema/xgboost__XGBRegressor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.938609 rubicon-ml-0.6.5/rubicon_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/sklearn/estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/sklearn/filter_estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/sklearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.938609 rubicon-ml-0.6.5/rubicon_ml/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.926609 rubicon-ml-0.6.5/rubicon_ml/viz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.938609 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/common.css
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/dropdown-header.css
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/experiments-table.css
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/frame.css
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/metric-correlation-plot.css
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/metric-lists-comparison.css
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/css/plots-comparison.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.938609 rubicon-ml-0.6.5/rubicon_ml/viz/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/rubicon_ml/viz/common/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/common/dropdown_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/dataframe_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/experiments_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/metric_correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/viz/metric_lists_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/rubicon_ml/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/rubicon_ml/workflow/prefect/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/workflow/prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/rubicon_ml/workflow/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.930609 rubicon-ml-0.6.5/rubicon_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 17:36:48.000000 rubicon-ml-0.6.5/rubicon_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:48.942609 rubicon-ml-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-03-13 17:36:40.000000 rubicon-ml-0.6.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.233100 rubicon-ml-0.7.0/rubicon_ml/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27487 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/rubicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/rubicon_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.233100 rubicon-ml-0.7.0/rubicon_ml/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/utils/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/client/utils/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.237100 rubicon-ml-0.7.0/rubicon_ml/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.237100 rubicon-ml-0.7.0/rubicon_ml/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/utils/training_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/domain/utils/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.237100 rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.237100 rubicon-ml-0.7.0/rubicon_ml/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49100 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.237100 rubicon-ml-0.7.0/rubicon_ml/repository/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/repository/utils/slugify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.237100 rubicon-ml-0.7.0/rubicon_ml/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.241100 rubicon-ml-0.7.0/rubicon_ml/schema/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OGeneralizedLinearEstimator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OGradientBoostingEstimator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2ORandomForestEstimator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OTargetEncoderEstimator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OXGBoostEstimator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/lightgbm__LGBMClassifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/lightgbm__LGBMModel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/lightgbm__LGBMRegressor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/sklearn__RandomForestClassifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/xgboost__DaskXGBClassifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/xgboost__DaskXGBRegressor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/xgboost__XGBClassifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/xgboost__XGBModel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/schema/schema/xgboost__XGBRegressor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.241100 rubicon-ml-0.7.0/rubicon_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/sklearn/estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/sklearn/filter_estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/sklearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.241100 rubicon-ml-0.7.0/rubicon_ml/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.229100 rubicon-ml-0.7.0/rubicon_ml/viz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/dropdown-header.css
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/experiments-table.css
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/frame.css
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/metric-correlation-plot.css
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/metric-lists-comparison.css
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/css/plots-comparison.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/viz/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/viz/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/common/dropdown_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/dataframe_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/experiments_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/metric_correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/viz/metric_lists_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/rubicon_ml/workflow/prefect/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/workflow/prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/rubicon_ml/workflow/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.233100 rubicon-ml-0.7.0/rubicon_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 18:50:00.000000 rubicon-ml-0.7.0/rubicon_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:50:00.245100 rubicon-ml-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-09 18:49:51.000000 rubicon-ml-0.7.0/versioneer.py
```

### Comparing `rubicon-ml-0.6.5/LICENSE` & `rubicon-ml-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/PKG-INFO` & `rubicon-ml-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.6.5
+Version: 0.7.0
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.6.5/README.md` & `rubicon-ml-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/__init__.py` & `rubicon-ml-0.7.0/rubicon_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/cli.py` & `rubicon-ml-0.7.0/rubicon_ml/cli.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/__init__.py` & `rubicon-ml-0.7.0/rubicon_ml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/artifact.py` & `rubicon-ml-0.7.0/rubicon_ml/client/artifact.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/base.py` & `rubicon-ml-0.7.0/rubicon_ml/client/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/config.py` & `rubicon-ml-0.7.0/rubicon_ml/client/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Parameters
     ----------
     persistence : str, optional
         The persistence type. Can be one of ["filesystem", "memory"].
     root_dir : str, optional
         Absolute or relative filepath. Defaults to using the local
         filesystem. Prefix with s3:// to use s3 instead.
-    auto_git_enabled : bool, optional
+    is_auto_git_enabled : bool, optional
         True to use the `git` command to automatically log relevant repository
         information to projects and experiments logged with this client instance,
         False otherwise. Defaults to False.
     storage_options : dict, optional
         Additional keyword arguments specific to the protocol being chosen. They
         are passed directly to the underlying filesystem class.
     """
```

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/dataframe.py` & `rubicon-ml-0.7.0/rubicon_ml/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/experiment.py` & `rubicon-ml-0.7.0/rubicon_ml/client/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/feature.py` & `rubicon-ml-0.7.0/rubicon_ml/client/feature.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/metric.py` & `rubicon-ml-0.7.0/rubicon_ml/client/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/mixin.py` & `rubicon-ml-0.7.0/rubicon_ml/client/mixin.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/parameter.py` & `rubicon-ml-0.7.0/rubicon_ml/client/parameter.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/project.py` & `rubicon-ml-0.7.0/rubicon_ml/client/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         branch_name,
         commit_hash,
         training_metadata,
         tags,
         comments,
     ):
         """Instantiates and returns an experiment domain object."""
-        if self.is_auto_git_enabled:
+        if self.is_auto_git_enabled():
             if branch_name is None:
                 branch_name = self._get_branch_name()
             if commit_hash is None:
                 commit_hash = self._get_commit_hash()
 
         if training_metadata is not None:
             training_metadata = domain.utils.TrainingMetadata(training_metadata)
```

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/rubicon.py` & `rubicon-ml-0.7.0/rubicon_ml/client/rubicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,28 @@
         **storage_options,
     ):
         if composite_config is not None:
             self.configs = [
                 Config(
                     persistence=config["persistence"],
                     root_dir=config["root_dir"],
-                    auto_git_enabled=auto_git_enabled,
+                    is_auto_git_enabled=auto_git_enabled,
                     **storage_options,
                 )
                 for config in composite_config
             ]
         else:
-            self.configs = [Config(persistence, root_dir, auto_git_enabled, **storage_options)]
+            self.configs = [
+                Config(
+                    persistence=persistence,
+                    root_dir=root_dir,
+                    is_auto_git_enabled=auto_git_enabled,
+                    **storage_options,
+                ),
+            ]
 
     @property
     def config(self):
         """
         Returns a single config.
 
         Exists to promote backwards compatibility.
@@ -112,15 +119,15 @@
         self,
         name: str,
         description: Optional[str],
         github_url: Optional[str],
         training_metadata: Optional[Union[List[Tuple], Tuple]],
     ):
         """Instantiates and returns a project domain object."""
-        if self.is_auto_git_enabled and github_url is None:
+        if self.is_auto_git_enabled() and github_url is None:
             github_url = self._get_github_url()
 
         if training_metadata is not None:
             training_metadata_class = TrainingMetadata(training_metadata)
         else:
             training_metadata_class = None
```

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/rubicon_json.py` & `rubicon-ml-0.7.0/rubicon_ml/client/rubicon_json.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/utils/exception_handling.py` & `rubicon-ml-0.7.0/rubicon_ml/client/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/client/utils/tags.py` & `rubicon-ml-0.7.0/rubicon_ml/client/utils/tags.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/__init__.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/artifact.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/artifact.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/dataframe.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/dataframe.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/experiment.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/feature.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/feature.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/metric.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/mixin.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/mixin.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/parameter.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/parameter.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/domain/utils/training_metadata.py` & `rubicon-ml-0.7.0/rubicon_ml/domain/utils/training_metadata.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/base.py` & `rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/experiment.py` & `rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/intake_rubicon/publish.py` & `rubicon-ml-0.7.0/rubicon_ml/intake_rubicon/publish.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/repository/base.py` & `rubicon-ml-0.7.0/rubicon_ml/repository/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/repository/local.py` & `rubicon-ml-0.7.0/rubicon_ml/repository/local.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/repository/memory.py` & `rubicon-ml-0.7.0/rubicon_ml/repository/memory.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/repository/s3.py` & `rubicon-ml-0.7.0/rubicon_ml/repository/s3.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/repository/utils/json.py` & `rubicon-ml-0.7.0/rubicon_ml/repository/utils/json.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/logger.py` & `rubicon-ml-0.7.0/rubicon_ml/schema/logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/registry.py` & `rubicon-ml-0.7.0/rubicon_ml/schema/registry.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OGeneralizedLinearEstimator.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OGeneralizedLinearEstimator.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OGradientBoostingEstimator.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OGradientBoostingEstimator.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2ORandomForestEstimator.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2ORandomForestEstimator.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OTargetEncoderEstimator.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OTargetEncoderEstimator.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/h2o__H2OXGBoostEstimator.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/h2o__H2OXGBoostEstimator.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/lightgbm__LGBMModel.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/lightgbm__LGBMModel.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/sklearn__RandomForestClassifier.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/sklearn__RandomForestClassifier.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/schema/schema/xgboost__XGBModel.yaml` & `rubicon-ml-0.7.0/rubicon_ml/schema/schema/xgboost__XGBModel.yaml`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/sklearn/estimator_logger.py` & `rubicon-ml-0.7.0/rubicon_ml/sklearn/estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/sklearn/filter_estimator_logger.py` & `rubicon-ml-0.7.0/rubicon_ml/sklearn/filter_estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/sklearn/pipeline.py` & `rubicon-ml-0.7.0/rubicon_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/assets/images/rubicon-logo-dark.png` & `rubicon-ml-0.7.0/rubicon_ml/viz/assets/images/rubicon-logo-dark.png`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/base.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/common/dropdown_header.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/common/dropdown_header.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/dashboard.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/dataframe_plot.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/dataframe_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/experiments_table.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/experiments_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                 "name": experiment.name,
                 "created_at": experiment.created_at,
                 "model_name": experiment.model_name,
                 "commit_hash": None,
                 "tags": ", ".join(str(tag) for tag in experiment.tags),
             }
 
-            if experiment.commit_hash is not None:
+            if experiment.commit_hash:
                 experiment_record["commit_hash"] = experiment.commit_hash[:7]
 
                 commit_hashes.add(experiment.commit_hash)
                 show_columns.add("commit_hash")
 
             if experiment.model_name is not None:
                 show_columns.add("model_name")
```

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/metric_correlation_plot.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/metric_correlation_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/viz/metric_lists_comparison.py` & `rubicon-ml-0.7.0/rubicon_ml/viz/metric_lists_comparison.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/workflow/prefect/__init__.py` & `rubicon-ml-0.7.0/rubicon_ml/workflow/prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml/workflow/prefect/tasks.py` & `rubicon-ml-0.7.0/rubicon_ml/workflow/prefect/tasks.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml.egg-info/PKG-INFO` & `rubicon-ml-0.7.0/rubicon_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.6.5
+Version: 0.7.0
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.6.5/rubicon_ml.egg-info/SOURCES.txt` & `rubicon-ml-0.7.0/rubicon_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/rubicon_ml.egg-info/requires.txt` & `rubicon-ml-0.7.0/rubicon_ml.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 click<=8.1.7,>=7.1
-fsspec<=2024.2.0,>=2021.4.0
-intake[dataframe]<=2.0.3,>=0.5.2
+fsspec<=2024.3.1,>=2021.4.0
+intake<=2.0.4,>=0.5.2
 jsonpath-ng<=1.6.1,>=1.5.3
 numpy<=1.26.4,>=1.22.0
 pandas<=2.2.1,>=1.0.0
-pyarrow<=15.0.0,>=14.0.1
+pyarrow<=15.0.2,>=14.0.1
 PyYAML<=6.0.1,>=5.4.0
 scikit-learn<=1.4.1.post1,>=0.22.0
 
 [all]
-dash<=2.15.0,>=2.11.0
+dash<=2.16.1,>=2.11.0
 dash-bootstrap-components<=1.5.0,>=1.0.0
 prefect<=1.2.4,>=0.12.0
-s3fs<=2024.2.0,>=0.4
+s3fs<=2024.3.1,>=0.4
 
 [prefect]
 prefect<=1.2.4,>=0.12.0
 
 [s3]
-s3fs<=2024.2.0,>=0.4
+s3fs<=2024.3.1,>=0.4
 
 [ui]
-dash<=2.15.0,>=2.11.0
+dash<=2.16.1,>=2.11.0
 dash-bootstrap-components<=1.5.0,>=1.0.0
 
 [viz]
-dash<=2.15.0,>=2.11.0
+dash<=2.16.1,>=2.11.0
 dash-bootstrap-components<=1.5.0,>=1.0.0
```

### Comparing `rubicon-ml-0.6.5/setup.cfg` & `rubicon-ml-0.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -25,39 +25,39 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	click<=8.1.7,>=7.1
-	fsspec<=2024.2.0,>=2021.4.0
-	intake[dataframe]<=2.0.3,>=0.5.2
+	fsspec<=2024.3.1,>=2021.4.0
+	intake<=2.0.4,>=0.5.2
 	jsonpath-ng<=1.6.1,>=1.5.3
 	numpy<=1.26.4,>=1.22.0
 	pandas<=2.2.1,>=1.0.0
-	pyarrow<=15.0.0,>=14.0.1
+	pyarrow<=15.0.2,>=14.0.1
 	PyYAML<=6.0.1,>=5.4.0
 	scikit-learn<=1.4.1.post1,>=0.22.0
 
 [options.extras_require]
 prefect = 
 	prefect<=1.2.4,>=0.12.0
 s3 = 
-	s3fs<=2024.2.0,>=0.4
+	s3fs<=2024.3.1,>=0.4
 ui = 
-	dash<=2.15.0,>=2.11.0
+	dash<=2.16.1,>=2.11.0
 	dash-bootstrap-components<=1.5.0,>=1.0.0
 viz = 
-	dash<=2.15.0,>=2.11.0
+	dash<=2.16.1,>=2.11.0
 	dash-bootstrap-components<=1.5.0,>=1.0.0
 all = 
-	dash<=2.15.0,>=2.11.0
+	dash<=2.16.1,>=2.11.0
 	dash-bootstrap-components<=1.5.0,>=1.0.0
 	prefect<=1.2.4,>=0.12.0
-	s3fs<=2024.2.0,>=0.4
+	s3fs<=2024.3.1,>=0.4
 
 [options.entry_points]
 console_scripts = 
 	rubicon_ml = rubicon_ml.cli:cli
 intake.drivers = 
 	rubicon_ml_experiment = rubicon_ml.intake_rubicon.experiment:ExperimentSource
 
@@ -95,15 +95,16 @@
 addopts = --cov=./rubicon_ml --cov-report=term-missing --cov-fail-under=90 -m="not write_files"
 minversion = 3.2
 xfail_strict = True
 
 [edgetest.envs.core]
 python_version = 3.9
 deps = 
-	dask
+	dask[dataframe]
+	h2o
 	jupyterlab
 	kaleido
 	lightgbm
 	nodejs
 	nbconvert
 	nbformat
 	palmerpenguins
@@ -115,15 +116,15 @@
 extras = 
 	all
 upgrade = 
 	click
 	dash
 	dash-bootstrap-components
 	fsspec
-	intake[dataframe]
+	intake
 	jsonpath-ng
 	numpy
 	pandas
 	pyarrow
 	PyYAML
 	s3fs
 	scikit-learn
```

### Comparing `rubicon-ml-0.6.5/tests/fixtures.py` & `rubicon-ml-0.7.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.6.5/versioneer.py` & `rubicon-ml-0.7.0/versioneer.py`

 * *Files identical despite different names*

