# Comparing `tmp/mljar-supervised-1.1.6.tar.gz` & `tmp/mljar-supervised-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mljar-supervised-1.1.6.tar", last modified: Fri Mar  8 09:44:37 2024, max compression
+gzip compressed data, was "mljar-supervised-1.1.7.tar", last modified: Wed Apr 10 12:39:36 2024, max compression
```

## Comparing `mljar-supervised-1.1.6.tar` & `mljar-supervised-1.1.7.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.804365 mljar-supervised-1.1.6/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.1.6/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26122 2024-03-08 09:44:37.804365 mljar-supervised-1.1.6/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    25334 2024-01-08 08:57:51.000000 mljar-supervised-1.1.6/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.796365 mljar-supervised-1.1.6/mljar_supervised.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26122 2024-03-08 09:44:37.000000 mljar-supervised-1.1.6/mljar_supervised.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3493 2024-03-08 09:44:37.000000 mljar-supervised-1.1.6/mljar_supervised.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-03-08 09:44:37.000000 mljar-supervised-1.1.6/mljar_supervised.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      319 2024-03-08 09:44:37.000000 mljar-supervised-1.1.6/mljar_supervised.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-03-08 09:44:37.000000 mljar-supervised-1.1.6/mljar_supervised.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      319 2024-01-22 10:03:14.000000 mljar-supervised-1.1.6/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       33 2023-09-21 12:45:57.000000 mljar-supervised-1.1.6/requirements_dev.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-03-08 09:44:37.804365 mljar-supervised-1.1.6/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1506 2024-03-08 09:44:11.000000 mljar-supervised-1.1.6/setup.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2024-03-08 09:44:11.000000 mljar-supervised-1.1.6/supervised/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/algorithms/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/algorithms/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4174 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/algorithms/algorithm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2475 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/baseline.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    14679 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9190 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/decision_tree.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5161 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-12-01 11:37:16.000000 mljar-supervised-1.1.6/supervised/algorithms/factory.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3710 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12349 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5833 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/linear.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4842 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5282 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/algorithms/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-04 09:46:14.000000 mljar-supervised-1.1.6/supervised/algorithms/registry.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6245 2023-12-01 11:37:16.000000 mljar-supervised-1.1.6/supervised/algorithms/sklearn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12532 2024-03-04 13:30:52.000000 mljar-supervised-1.1.6/supervised/algorithms/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26170 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/automl.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    99509 2024-03-08 09:41:43.000000 mljar-supervised-1.1.6/supervised/base_automl.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/callbacks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/callbacks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/callbacks/callback.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/callbacks/callback_list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9018 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/callbacks/early_stopping.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1701 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/callbacks/learner_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      568 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/callbacks/max_iters_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1847 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/callbacks/metric_logger.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      933 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/callbacks/terminate_on_nan.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3353 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/callbacks/total_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    22911 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/ensemble.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      547 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/exceptions.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/fairness/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.1.6/supervised/fairness/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26141 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/fairness/metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15001 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/fairness/optimization.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.1.6/supervised/fairness/plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4975 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/fairness/report.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.1.6/supervised/fairness/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    29288 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/model_framework.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/preprocessing/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/preprocessing/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3535 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/datetime_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12603 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/eda.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2023-12-01 11:37:16.000000 mljar-supervised-1.1.6/supervised/preprocessing/encoding_selector.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1488 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/exclude_missing_target.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10807 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/goldenfeatures_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3819 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/kmeans_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2446 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/label_binarizer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1793 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/label_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1555 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/loo_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26388 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/preprocessing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4616 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/preprocessing_categorical.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/preprocessing_missing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/preprocessing/preprocessing_utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3646 2024-03-04 12:03:16.000000 mljar-supervised-1.1.6/supervised/preprocessing/scale.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2557 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/preprocessing/text_transformer.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/tuner/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/tuner/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2361 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/data_info.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/hill_climbing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    59416 2024-03-04 11:50:15.000000 mljar-supervised-1.1.6/supervised/tuner/mljar_tuner.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.800365 mljar-supervised-1.1.6/supervised/tuner/optuna/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5539 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2510 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1910 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5896 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2122 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2511 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11606 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4727 2024-03-04 13:31:00.000000 mljar-supervised-1.1.6/supervised/tuner/optuna/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6273 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/preprocessing_tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/tuner/random_parameters.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8944 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/tuner/time_controller.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.804365 mljar-supervised-1.1.6/supervised/utils/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      259 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    37054 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/additional_metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8148 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/additional_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5352 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/automl_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/utils/common.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2023-09-21 12:19:11.000000 mljar-supervised-1.1.6/supervised/utils/config.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/utils/constants.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.1.6/supervised/utils/data_validation.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3015 2024-03-04 10:30:50.000000 mljar-supervised-1.1.6/supervised/utils/importance.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      823 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/jsonencoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4951 2023-09-20 06:26:40.000000 mljar-supervised-1.1.6/supervised/utils/leaderboard_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4972 2024-03-04 12:16:25.000000 mljar-supervised-1.1.6/supervised/utils/learning_curves.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    13465 2024-03-04 11:46:43.000000 mljar-supervised-1.1.6/supervised/utils/metric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12128 2024-03-04 11:50:51.000000 mljar-supervised-1.1.6/supervised/utils/shap.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      424 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/subsample.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      589 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/utils/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-08 09:44:37.804365 mljar-supervised-1.1.6/supervised/validation/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/validation/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1210 2023-09-20 06:26:41.000000 mljar-supervised-1.1.6/supervised/validation/validation_step.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.1.6/supervised/validation/validator_base.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4075 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/validation/validator_custom.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5505 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/validation/validator_kfold.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4708 2024-03-01 11:22:55.000000 mljar-supervised-1.1.6/supervised/validation/validator_split.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.1.7/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26122 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    25334 2024-01-08 08:57:51.000000 mljar-supervised-1.1.7/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/mljar_supervised.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26122 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3493 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2024-04-10 12:39:36.000000 mljar-supervised-1.1.7/mljar_supervised.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      325 2024-04-10 12:35:04.000000 mljar-supervised-1.1.7/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       33 2023-09-21 12:45:57.000000 mljar-supervised-1.1.7/requirements_dev.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1506 2024-04-10 12:38:52.000000 mljar-supervised-1.1.7/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2024-04-10 12:39:15.000000 mljar-supervised-1.1.7/supervised/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/algorithms/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/algorithms/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4174 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/algorithms/algorithm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2475 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/baseline.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    14679 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9190 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/decision_tree.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5161 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-12-01 11:37:16.000000 mljar-supervised-1.1.7/supervised/algorithms/factory.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3710 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12349 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5833 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/linear.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4842 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5282 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/algorithms/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-04 09:46:14.000000 mljar-supervised-1.1.7/supervised/algorithms/registry.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6245 2023-12-01 11:37:16.000000 mljar-supervised-1.1.7/supervised/algorithms/sklearn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12532 2024-03-04 13:30:52.000000 mljar-supervised-1.1.7/supervised/algorithms/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26170 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/automl.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    99509 2024-03-08 09:41:43.000000 mljar-supervised-1.1.7/supervised/base_automl.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/callbacks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/callbacks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/callbacks/callback.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/callbacks/callback_list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9018 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/callbacks/early_stopping.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1701 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/callbacks/learner_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      568 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/callbacks/max_iters_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1847 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/callbacks/metric_logger.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      933 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/callbacks/terminate_on_nan.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3353 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/callbacks/total_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    22911 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/ensemble.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      547 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/exceptions.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/fairness/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.1.7/supervised/fairness/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26141 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/fairness/metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15001 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/fairness/optimization.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.1.7/supervised/fairness/plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4975 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/fairness/report.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.1.7/supervised/fairness/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29288 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/model_framework.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.873661 mljar-supervised-1.1.7/supervised/preprocessing/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/preprocessing/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3535 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/datetime_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12603 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/eda.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2023-12-01 11:37:16.000000 mljar-supervised-1.1.7/supervised/preprocessing/encoding_selector.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1488 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/exclude_missing_target.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10807 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/goldenfeatures_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3819 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/kmeans_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2446 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/label_binarizer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1793 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/label_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1555 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/loo_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26388 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4616 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_categorical.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_missing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3646 2024-03-04 12:03:16.000000 mljar-supervised-1.1.7/supervised/preprocessing/scale.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2557 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/preprocessing/text_transformer.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/tuner/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/tuner/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2361 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/data_info.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2346 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/hill_climbing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    59416 2024-03-04 11:50:15.000000 mljar-supervised-1.1.7/supervised/tuner/mljar_tuner.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/tuner/optuna/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5539 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2510 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1910 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5896 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2122 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2511 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11606 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4727 2024-03-04 13:31:00.000000 mljar-supervised-1.1.7/supervised/tuner/optuna/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6273 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/preprocessing_tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/tuner/random_parameters.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8944 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/tuner/time_controller.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/utils/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      259 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    37054 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/additional_metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8148 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/additional_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5352 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/automl_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/utils/common.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2023-09-21 12:19:11.000000 mljar-supervised-1.1.7/supervised/utils/config.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/utils/constants.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.1.7/supervised/utils/data_validation.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3015 2024-03-04 10:30:50.000000 mljar-supervised-1.1.7/supervised/utils/importance.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      823 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/jsonencoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4951 2023-09-20 06:26:40.000000 mljar-supervised-1.1.7/supervised/utils/leaderboard_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4972 2024-03-04 12:16:25.000000 mljar-supervised-1.1.7/supervised/utils/learning_curves.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    13465 2024-03-04 11:46:43.000000 mljar-supervised-1.1.7/supervised/utils/metric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12128 2024-03-04 11:50:51.000000 mljar-supervised-1.1.7/supervised/utils/shap.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      424 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/subsample.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      589 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/utils/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-04-10 12:39:36.877661 mljar-supervised-1.1.7/supervised/validation/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/validation/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1210 2023-09-20 06:26:41.000000 mljar-supervised-1.1.7/supervised/validation/validation_step.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.1.7/supervised/validation/validator_base.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4075 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/validation/validator_custom.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5505 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/validation/validator_kfold.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4708 2024-03-01 11:22:55.000000 mljar-supervised-1.1.7/supervised/validation/validator_split.py
```

### Comparing `mljar-supervised-1.1.6/LICENSE` & `mljar-supervised-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/PKG-INFO` & `mljar-supervised-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.1.6
+Version: 1.1.7
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar,random forest,decision tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features selection,features engineering
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.6 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.7 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Keywords: automated machine learning,automl,machine learning,data
 science,data mining,mljar,random forest,decision
 tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features
 selection,features engineering Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `mljar-supervised-1.1.6/README.md` & `mljar-supervised-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/mljar_supervised.egg-info/PKG-INFO` & `mljar-supervised-1.1.7/mljar_supervised.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.1.6
+Version: 1.1.7
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar,random forest,decision tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features selection,features engineering
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.6 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.1.7 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Keywords: automated machine learning,automl,machine learning,data
 science,data mining,mljar,random forest,decision
 tree,xgboost,lightgbm,catboost,neural network,extra trees,linear model,features
 selection,features engineering Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `mljar-supervised-1.1.6/mljar_supervised.egg-info/SOURCES.txt` & `mljar-supervised-1.1.7/mljar_supervised.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/setup.py` & `mljar-supervised-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mljar-supervised",
-    version="1.1.6",
+    version="1.1.7",
     description="Automated Machine Learning for Humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mljar/mljar-supervised",
     author="MLJAR, Sp. z o.o.",
     author_email="contact@mljar.com",
     license="MIT",
```

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/algorithm.py` & `mljar-supervised-1.1.7/supervised/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/baseline.py` & `mljar-supervised-1.1.7/supervised/algorithms/baseline.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/catboost.py` & `mljar-supervised-1.1.7/supervised/algorithms/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/decision_tree.py` & `mljar-supervised-1.1.7/supervised/algorithms/decision_tree.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/extra_trees.py` & `mljar-supervised-1.1.7/supervised/algorithms/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/factory.py` & `mljar-supervised-1.1.7/supervised/algorithms/factory.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/knn.py` & `mljar-supervised-1.1.7/supervised/algorithms/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/lightgbm.py` & `mljar-supervised-1.1.7/supervised/algorithms/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/linear.py` & `mljar-supervised-1.1.7/supervised/algorithms/linear.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/nn.py` & `mljar-supervised-1.1.7/supervised/algorithms/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/random_forest.py` & `mljar-supervised-1.1.7/supervised/algorithms/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/registry.py` & `mljar-supervised-1.1.7/supervised/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/sklearn.py` & `mljar-supervised-1.1.7/supervised/algorithms/sklearn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/algorithms/xgboost.py` & `mljar-supervised-1.1.7/supervised/algorithms/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/automl.py` & `mljar-supervised-1.1.7/supervised/automl.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/base_automl.py` & `mljar-supervised-1.1.7/supervised/base_automl.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/callback.py` & `mljar-supervised-1.1.7/supervised/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/callback_list.py` & `mljar-supervised-1.1.7/supervised/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/early_stopping.py` & `mljar-supervised-1.1.7/supervised/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/learner_time_constraint.py` & `mljar-supervised-1.1.7/supervised/callbacks/learner_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/max_iters_constraint.py` & `mljar-supervised-1.1.7/supervised/callbacks/max_iters_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/metric_logger.py` & `mljar-supervised-1.1.7/supervised/callbacks/metric_logger.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/terminate_on_nan.py` & `mljar-supervised-1.1.7/supervised/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/callbacks/total_time_constraint.py` & `mljar-supervised-1.1.7/supervised/callbacks/total_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/ensemble.py` & `mljar-supervised-1.1.7/supervised/ensemble.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/exceptions.py` & `mljar-supervised-1.1.7/supervised/exceptions.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/fairness/metrics.py` & `mljar-supervised-1.1.7/supervised/fairness/metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/fairness/optimization.py` & `mljar-supervised-1.1.7/supervised/fairness/optimization.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/fairness/plots.py` & `mljar-supervised-1.1.7/supervised/fairness/plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/fairness/report.py` & `mljar-supervised-1.1.7/supervised/fairness/report.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/fairness/utils.py` & `mljar-supervised-1.1.7/supervised/fairness/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/model_framework.py` & `mljar-supervised-1.1.7/supervised/model_framework.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/datetime_transformer.py` & `mljar-supervised-1.1.7/supervised/preprocessing/datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/eda.py` & `mljar-supervised-1.1.7/supervised/preprocessing/eda.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/encoding_selector.py` & `mljar-supervised-1.1.7/supervised/preprocessing/encoding_selector.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/exclude_missing_target.py` & `mljar-supervised-1.1.7/supervised/preprocessing/exclude_missing_target.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/goldenfeatures_transformer.py` & `mljar-supervised-1.1.7/supervised/preprocessing/goldenfeatures_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/kmeans_transformer.py` & `mljar-supervised-1.1.7/supervised/preprocessing/kmeans_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/label_binarizer.py` & `mljar-supervised-1.1.7/supervised/preprocessing/label_binarizer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/label_encoder.py` & `mljar-supervised-1.1.7/supervised/preprocessing/label_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/loo_encoder.py` & `mljar-supervised-1.1.7/supervised/preprocessing/loo_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/preprocessing.py` & `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/preprocessing_categorical.py` & `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_categorical.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/preprocessing_missing.py` & `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_missing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/preprocessing_utils.py` & `mljar-supervised-1.1.7/supervised/preprocessing/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/scale.py` & `mljar-supervised-1.1.7/supervised/preprocessing/scale.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/preprocessing/text_transformer.py` & `mljar-supervised-1.1.7/supervised/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/data_info.py` & `mljar-supervised-1.1.7/supervised/tuner/data_info.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/hill_climbing.py` & `mljar-supervised-1.1.7/supervised/tuner/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/mljar_tuner.py` & `mljar-supervised-1.1.7/supervised/tuner/mljar_tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/catboost.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/extra_trees.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/knn.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/lightgbm.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/nn.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/random_forest.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/tuner.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/optuna/xgboost.py` & `mljar-supervised-1.1.7/supervised/tuner/optuna/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/preprocessing_tuner.py` & `mljar-supervised-1.1.7/supervised/tuner/preprocessing_tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/random_parameters.py` & `mljar-supervised-1.1.7/supervised/tuner/random_parameters.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/tuner/time_controller.py` & `mljar-supervised-1.1.7/supervised/tuner/time_controller.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/additional_metrics.py` & `mljar-supervised-1.1.7/supervised/utils/additional_metrics.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/additional_plots.py` & `mljar-supervised-1.1.7/supervised/utils/additional_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/automl_plots.py` & `mljar-supervised-1.1.7/supervised/utils/automl_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/common.py` & `mljar-supervised-1.1.7/supervised/utils/common.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/config.py` & `mljar-supervised-1.1.7/supervised/utils/config.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/data_validation.py` & `mljar-supervised-1.1.7/supervised/utils/data_validation.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/importance.py` & `mljar-supervised-1.1.7/supervised/utils/importance.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/jsonencoder.py` & `mljar-supervised-1.1.7/supervised/utils/jsonencoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/leaderboard_plots.py` & `mljar-supervised-1.1.7/supervised/utils/leaderboard_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/learning_curves.py` & `mljar-supervised-1.1.7/supervised/utils/learning_curves.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/metric.py` & `mljar-supervised-1.1.7/supervised/utils/metric.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/shap.py` & `mljar-supervised-1.1.7/supervised/utils/shap.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/utils/utils.py` & `mljar-supervised-1.1.7/supervised/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/validation/validation_step.py` & `mljar-supervised-1.1.7/supervised/validation/validation_step.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/validation/validator_custom.py` & `mljar-supervised-1.1.7/supervised/validation/validator_custom.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/validation/validator_kfold.py` & `mljar-supervised-1.1.7/supervised/validation/validator_kfold.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.1.6/supervised/validation/validator_split.py` & `mljar-supervised-1.1.7/supervised/validation/validator_split.py`

 * *Files identical despite different names*

