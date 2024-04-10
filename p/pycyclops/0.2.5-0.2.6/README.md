# Comparing `tmp/pycyclops-0.2.5.tar.gz` & `tmp/pycyclops-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycyclops-0.2.5.tar", max compression
+gzip compressed data, was "pycyclops-0.2.6.tar", max compression
```

## Comparing `pycyclops-0.2.5.tar` & `pycyclops-0.2.6.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0    11347 2024-03-18 13:05:00.856252 pycyclops-0.2.5/LICENSE.md
--rw-r--r--   0        0        0     6433 2024-03-18 13:05:00.856252 pycyclops-0.2.5/README.md
--rw-r--r--   0        0        0       23 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/__init__.py
--rw-r--r--   0        0        0      192 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/__init__.py
--rw-r--r--   0        0        0    25741 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/aggregate.py
--rw-r--r--   0        0        0     4344 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/clean.py
--rw-r--r--   0        0        0     3469 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/constants.py
--rw-r--r--   0        0        0       39 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/df/__init__.py
--rw-r--r--   0        0        0    26086 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/df/feature.py
--rw-r--r--   0        0        0    26171 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/df/handle_types.py
--rw-r--r--   0        0        0    17267 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/df/normalize.py
--rw-r--r--   0        0        0    12116 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/df/split.py
--rw-r--r--   0        0        0    30240 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/df/vectorized.py
--rw-r--r--   0        0        0     3295 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/diagnoses.py
--rw-r--r--   0        0        0      118 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/features/__init__.py
--rw-r--r--   0        0        0     9640 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/features/medical_image.py
--rw-r--r--   0        0        0    17072 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/impute.py
--rw-r--r--   0        0        0     3228 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/loader.py
--rw-r--r--   0        0        0      638 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/packaged_loading_scripts/__init__.py
--rw-r--r--   0        0        0       36 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
--rw-r--r--   0        0        0     2110 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
--rw-r--r--   0        0        0      881 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/preprocess.py
--rw-r--r--   0        0        0    32163 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/slicer.py
--rw-r--r--   0        0        0     6471 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/string_ops.py
--rw-r--r--   0        0        0     3027 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/transforms.py
--rw-r--r--   0        0        0    13157 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/data/utils.py
--rw-r--r--   0        0        0      139 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/__init__.py
--rw-r--r--   0        0        0    12362 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/evaluator.py
--rw-r--r--   0        0        0      159 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/fairness/__init__.py
--rw-r--r--   0        0        0     1104 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/fairness/config.py
--rw-r--r--   0        0        0    36125 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/fairness/evaluator.py
--rw-r--r--   0        0        0     1837 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0    13476 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0    13702 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/auroc.py
--rw-r--r--   0        0        0     4899 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/average_precision.py
--rw-r--r--   0        0        0     2484 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/__init__.py
--rw-r--r--   0        0        0     7774 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/_stat_scores.py
--rw-r--r--   0        0        0     7217 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/accuracy.py
--rw-r--r--   0        0        0    11290 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/auroc.py
--rw-r--r--   0        0        0    11136 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/average_precision.py
--rw-r--r--   0        0        0    12934 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/confusion_matrix.py
--rw-r--r--   0        0        0     1349 2024-03-18 13:05:00.860252 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
--rw-r--r--   0        0        0     2066 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
--rw-r--r--   0        0        0     3491 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
--rw-r--r--   0        0        0     1062 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
--rw-r--r--   0        0        0     3916 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
--rw-r--r--   0        0        0    17182 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/f_score.py
--rw-r--r--   0        0        0     2614 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/__init__.py
--rw-r--r--   0        0        0    17136 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
--rw-r--r--   0        0        0    17396 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/accuracy.py
--rw-r--r--   0        0        0    24663 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/auroc.py
--rw-r--r--   0        0        0    26373 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/average_precision.py
--rw-r--r--   0        0        0    27914 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
--rw-r--r--   0        0        0    33936 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/f_score.py
--rw-r--r--   0        0        0     2559 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/mae.py
--rw-r--r--   0        0        0     3551 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/mape.py
--rw-r--r--   0        0        0    12370 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
--rw-r--r--   0        0        0     4101 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/mse.py
--rw-r--r--   0        0        0    16833 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
--rw-r--r--   0        0        0    32246 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
--rw-r--r--   0        0        0    45978 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    25481 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/roc.py
--rw-r--r--   0        0        0     3612 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/smape.py
--rw-r--r--   0        0        0    16929 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/specificity.py
--rw-r--r--   0        0        0     3253 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/wmape.py
--rw-r--r--   0        0        0     1858 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/mae.py
--rw-r--r--   0        0        0     2498 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/mape.py
--rw-r--r--   0        0        0     6089 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
--rw-r--r--   0        0        0    26623 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/metric.py
--rw-r--r--   0        0        0    21975 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/metric_dict.py
--rw-r--r--   0        0        0     3290 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/mse.py
--rw-r--r--   0        0        0     7802 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
--rw-r--r--   0        0        0    33336 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/precision_recall.py
--rw-r--r--   0        0        0    19586 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
--rw-r--r--   0        0        0     9557 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/roc.py
--rw-r--r--   0        0        0     2597 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/smape.py
--rw-r--r--   0        0        0    13798 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/specificity.py
--rw-r--r--   0        0        0      546 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/__init__.py
--rw-r--r--   0        0        0    35848 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/ops.py
--rw-r--r--   0        0        0     9057 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/types.py
--rw-r--r--   0        0        0     4589 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/validation.py
--rw-r--r--   0        0        0     2727 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/wmape.py
--rw-r--r--   0        0        0    26187 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/f_beta.py
--rw-r--r--   0        0        0     1815 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/factory.py
--rw-r--r--   0        0        0     1933 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/__init__.py
--rw-r--r--   0        0        0    16824 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/accuracy.py
--rw-r--r--   0        0        0    22142 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/auroc.py
--rw-r--r--   0        0        0     5544 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/average_precision.py
--rw-r--r--   0        0        0    26687 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/f_beta.py
--rw-r--r--   0        0        0    27455 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/precision_recall.py
--rw-r--r--   0        0        0    37364 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    21633 2024-03-18 13:05:00.864251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/roc.py
--rw-r--r--   0        0        0    11342 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/sensitivity.py
--rw-r--r--   0        0        0    16029 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/specificity.py
--rw-r--r--   0        0        0    26592 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/functional/stat_scores.py
--rw-r--r--   0        0        0    32052 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/metric.py
--rw-r--r--   0        0        0    26995 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/precision_recall.py
--rw-r--r--   0        0        0    23073 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/precision_recall_curve.py
--rw-r--r--   0        0        0    13622 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/roc.py
--rw-r--r--   0        0        0    12350 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/sensitivity.py
--rw-r--r--   0        0        0    14376 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/specificity.py
--rw-r--r--   0        0        0    16991 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/stat_scores.py
--rw-r--r--   0        0        0    10157 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/metrics/utils.py
--rw-r--r--   0        0        0     2388 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/evaluate/utils.py
--rw-r--r--   0        0        0     1658 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/__init__.py
--rw-r--r--   0        0        0     7660 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/catalog.py
--rw-r--r--   0        0        0      727 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/densenet.yaml
--rw-r--r--   0        0        0      647 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/gru.yaml
--rw-r--r--   0        0        0       34 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/logistic_regression.yaml
--rw-r--r--   0        0        0      647 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/lstm.yaml
--rw-r--r--   0        0        0      117 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/mlp_classifier.yaml
--rw-r--r--   0        0        0      577 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/mlp_pt.yaml
--rw-r--r--   0        0        0      512 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/resnet.yaml
--rw-r--r--   0        0        0       53 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/rf_classifier.yaml
--rw-r--r--   0        0        0      590 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/rnn.yaml
--rw-r--r--   0        0        0       91 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/sgd_classifier.yaml
--rw-r--r--   0        0        0      180 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/configs/xgb_classifier.yaml
--rw-r--r--   0        0        0     1791 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/data.py
--rw-r--r--   0        0        0      266 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/neural_nets/__init__.py
--rw-r--r--   0        0        0     2226 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/neural_nets/gru.py
--rw-r--r--   0        0        0     2436 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/neural_nets/lstm.py
--rw-r--r--   0        0        0     3013 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/neural_nets/mlp.py
--rw-r--r--   0        0        0     2214 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/neural_nets/rnn.py
--rw-r--r--   0        0        0     2588 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/plotter.py
--rw-r--r--   0        0        0     7171 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/torch_utils.py
--rw-r--r--   0        0        0     4371 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/utils.py
--rw-r--r--   0        0        0      372 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/wrappers/__init__.py
--rw-r--r--   0        0        0    10026 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/wrappers/base.py
--rw-r--r--   0        0        0    49399 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/wrappers/pt_model.py
--rw-r--r--   0        0        0    39968 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/wrappers/sk_model.py
--rw-r--r--   0        0        0     9899 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/models/wrappers/utils.py
--rw-r--r--   0        0        0      468 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/__init__.py
--rw-r--r--   0        0        0    16172 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/clinical_applicator.py
--rw-r--r--   0        0        0    13248 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/detector.py
--rw-r--r--   0        0        0     2554 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/explainer.py
--rw-r--r--   0        0        0    13859 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/plotter.py
--rw-r--r--   0        0        0     9566 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/reductor.py
--rw-r--r--   0        0        0     9118 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/synthetic_applicator.py
--rw-r--r--   0        0        0    37496 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/tester.py
--rw-r--r--   0        0        0    18561 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/monitor/utils.py
--rw-r--r--   0        0        0       81 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/__init__.py
--rw-r--r--   0        0        0      100 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/model_card/__init__.py
--rw-r--r--   0        0        0     6005 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/model_card/base.py
--rw-r--r--   0        0        0    18872 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/model_card/fields.py
--rw-r--r--   0        0        0     3054 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/model_card/model_card.py
--rw-r--r--   0        0        0     6166 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/model_card/sections.py
--rw-r--r--   0        0        0       37 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/plot/__init__.py
--rw-r--r--   0        0        0     3275 2024-03-18 13:05:00.868251 pycyclops-0.2.5/cyclops/report/plot/base.py
--rw-r--r--   0        0        0    43311 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/plot/classification.py
--rw-r--r--   0        0        0     5463 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/plot/utils.py
--rw-r--r--   0        0        0    39651 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/report.py
--rw-r--r--   0        0        0     1828 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/templates/model_report/button.js
--rw-r--r--   0        0        0    15741 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/templates/model_report/macros.jinja
--rw-r--r--   0        0        0    14849 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/templates/model_report/model_report.jinja
--rw-r--r--   0        0        0    30509 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/templates/model_report/plot.js
--rw-r--r--   0        0        0    32211 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/report/utils.py
--rw-r--r--   0        0        0      143 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/tasks/__init__.py
--rw-r--r--   0        0        0     7278 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/tasks/base.py
--rw-r--r--   0        0        0    22027 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/tasks/classification.py
--rw-r--r--   0        0        0     4211 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/tasks/utils.py
--rw-r--r--   0        0        0       23 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/__init__.py
--rw-r--r--   0        0        0     4966 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/common.py
--rw-r--r--   0        0        0    10240 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/file.py
--rw-r--r--   0        0        0     2423 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/index.py
--rw-r--r--   0        0        0     3611 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/log.py
--rw-r--r--   0        0        0     1701 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/optional.py
--rw-r--r--   0        0        0     5571 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/plot.py
--rw-r--r--   0        0        0      874 2024-03-18 13:05:00.872251 pycyclops-0.2.5/cyclops/utils/profile.py
--rw-r--r--   0        0        0     6354 2024-03-18 13:05:00.880251 pycyclops-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     8821 1970-01-01 00:00:00.000000 pycyclops-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-04-10 21:12:46.385642 pycyclops-0.2.6/LICENSE.md
+-rw-r--r--   0        0        0     6433 2024-04-10 21:12:46.385642 pycyclops-0.2.6/README.md
+-rw-r--r--   0        0        0       23 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/__init__.py
+-rw-r--r--   0        0        0    25741 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/aggregate.py
+-rw-r--r--   0        0        0     4344 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/clean.py
+-rw-r--r--   0        0        0     3469 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/constants.py
+-rw-r--r--   0        0        0       39 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/__init__.py
+-rw-r--r--   0        0        0    26086 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/feature.py
+-rw-r--r--   0        0        0    26171 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/handle_types.py
+-rw-r--r--   0        0        0    17267 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/normalize.py
+-rw-r--r--   0        0        0    12116 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/split.py
+-rw-r--r--   0        0        0    30240 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/vectorized.py
+-rw-r--r--   0        0        0     3295 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/diagnoses.py
+-rw-r--r--   0        0        0      118 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/features/__init__.py
+-rw-r--r--   0        0        0     9640 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/features/medical_image.py
+-rw-r--r--   0        0        0    17072 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/impute.py
+-rw-r--r--   0        0        0     3228 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/loader.py
+-rw-r--r--   0        0        0      638 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/__init__.py
+-rw-r--r--   0        0        0       36 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
+-rw-r--r--   0        0        0      881 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/preprocess.py
+-rw-r--r--   0        0        0    32163 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/slicer.py
+-rw-r--r--   0        0        0     6471 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/string_ops.py
+-rw-r--r--   0        0        0     3027 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/transforms.py
+-rw-r--r--   0        0        0    13157 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/utils.py
+-rw-r--r--   0        0        0      139 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/evaluate/__init__.py
+-rw-r--r--   0        0        0    12362 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/evaluate/evaluator.py
+-rw-r--r--   0        0        0      159 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/evaluate/fairness/__init__.py
+-rw-r--r--   0        0        0     1104 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/fairness/config.py
+-rw-r--r--   0        0        0    36125 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/fairness/evaluator.py
+-rw-r--r--   0        0        0     1837 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0    13476 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0    13702 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/auroc.py
+-rw-r--r--   0        0        0     4899 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/average_precision.py
+-rw-r--r--   0        0        0     2484 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/__init__.py
+-rw-r--r--   0        0        0     7774 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/_stat_scores.py
+-rw-r--r--   0        0        0     7217 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/accuracy.py
+-rw-r--r--   0        0        0    11290 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/auroc.py
+-rw-r--r--   0        0        0    11136 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/average_precision.py
+-rw-r--r--   0        0        0    12934 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/confusion_matrix.py
+-rw-r--r--   0        0        0     1349 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
+-rw-r--r--   0        0        0     2066 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
+-rw-r--r--   0        0        0     3491 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
+-rw-r--r--   0        0        0     1062 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
+-rw-r--r--   0        0        0     3916 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
+-rw-r--r--   0        0        0    17182 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/f_score.py
+-rw-r--r--   0        0        0     2614 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/__init__.py
+-rw-r--r--   0        0        0    17136 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
+-rw-r--r--   0        0        0    17396 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/accuracy.py
+-rw-r--r--   0        0        0    25070 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/auroc.py
+-rw-r--r--   0        0        0    26707 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/average_precision.py
+-rw-r--r--   0        0        0    27926 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
+-rw-r--r--   0        0        0    34008 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/f_score.py
+-rw-r--r--   0        0        0     2631 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mae.py
+-rw-r--r--   0        0        0     3551 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mape.py
+-rw-r--r--   0        0        0    12394 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
+-rw-r--r--   0        0        0     4101 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mse.py
+-rw-r--r--   0        0        0    16833 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
+-rw-r--r--   0        0        0    32246 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
+-rw-r--r--   0        0        0    45990 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    25481 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/roc.py
+-rw-r--r--   0        0        0     3612 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/smape.py
+-rw-r--r--   0        0        0    16929 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/specificity.py
+-rw-r--r--   0        0        0     3253 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/wmape.py
+-rw-r--r--   0        0        0     1858 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mae.py
+-rw-r--r--   0        0        0     2498 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mape.py
+-rw-r--r--   0        0        0     6089 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
+-rw-r--r--   0        0        0    26623 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric.py
+-rw-r--r--   0        0        0    21975 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric_dict.py
+-rw-r--r--   0        0        0     3290 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mse.py
+-rw-r--r--   0        0        0     7802 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
+-rw-r--r--   0        0        0    33336 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall.py
+-rw-r--r--   0        0        0    19586 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
+-rw-r--r--   0        0        0     9557 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/roc.py
+-rw-r--r--   0        0        0     2597 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/smape.py
+-rw-r--r--   0        0        0    13798 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/specificity.py
+-rw-r--r--   0        0        0      546 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/__init__.py
+-rw-r--r--   0        0        0    36009 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/ops.py
+-rw-r--r--   0        0        0     9057 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/types.py
+-rw-r--r--   0        0        0     4589 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/validation.py
+-rw-r--r--   0        0        0     2727 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/wmape.py
+-rw-r--r--   0        0        0    26187 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/f_beta.py
+-rw-r--r--   0        0        0     1815 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/factory.py
+-rw-r--r--   0        0        0     1933 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/__init__.py
+-rw-r--r--   0        0        0    16824 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/accuracy.py
+-rw-r--r--   0        0        0    22142 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/auroc.py
+-rw-r--r--   0        0        0     5544 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/average_precision.py
+-rw-r--r--   0        0        0    26687 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/f_beta.py
+-rw-r--r--   0        0        0    27455 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall.py
+-rw-r--r--   0        0        0    37364 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    21633 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/roc.py
+-rw-r--r--   0        0        0    11342 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/sensitivity.py
+-rw-r--r--   0        0        0    16029 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/specificity.py
+-rw-r--r--   0        0        0    26592 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/stat_scores.py
+-rw-r--r--   0        0        0    32052 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/metric.py
+-rw-r--r--   0        0        0    26995 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall.py
+-rw-r--r--   0        0        0    23073 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall_curve.py
+-rw-r--r--   0        0        0    13622 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/roc.py
+-rw-r--r--   0        0        0    12350 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/sensitivity.py
+-rw-r--r--   0        0        0    14376 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/specificity.py
+-rw-r--r--   0        0        0    16991 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/stat_scores.py
+-rw-r--r--   0        0        0    10157 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/utils.py
+-rw-r--r--   0        0        0     2388 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/utils.py
+-rw-r--r--   0        0        0     1658 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/__init__.py
+-rw-r--r--   0        0        0     7660 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/catalog.py
+-rw-r--r--   0        0        0      727 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/densenet.yaml
+-rw-r--r--   0        0        0      647 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/gru.yaml
+-rw-r--r--   0        0        0       34 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/logistic_regression.yaml
+-rw-r--r--   0        0        0      647 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/lstm.yaml
+-rw-r--r--   0        0        0      117 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/mlp_classifier.yaml
+-rw-r--r--   0        0        0      577 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/mlp_pt.yaml
+-rw-r--r--   0        0        0      512 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/resnet.yaml
+-rw-r--r--   0        0        0       53 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/rf_classifier.yaml
+-rw-r--r--   0        0        0      590 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/rnn.yaml
+-rw-r--r--   0        0        0       91 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/sgd_classifier.yaml
+-rw-r--r--   0        0        0      180 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/xgb_classifier.yaml
+-rw-r--r--   0        0        0     1791 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/data.py
+-rw-r--r--   0        0        0      266 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/__init__.py
+-rw-r--r--   0        0        0     2226 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/gru.py
+-rw-r--r--   0        0        0     2436 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/lstm.py
+-rw-r--r--   0        0        0     3013 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/mlp.py
+-rw-r--r--   0        0        0     2214 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/rnn.py
+-rw-r--r--   0        0        0     2588 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/plotter.py
+-rw-r--r--   0        0        0     7171 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/torch_utils.py
+-rw-r--r--   0        0        0     4371 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/utils.py
+-rw-r--r--   0        0        0      372 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/__init__.py
+-rw-r--r--   0        0        0    10026 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/base.py
+-rw-r--r--   0        0        0    49399 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/pt_model.py
+-rw-r--r--   0        0        0    39968 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/sk_model.py
+-rw-r--r--   0        0        0     9899 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/utils.py
+-rw-r--r--   0        0        0      468 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/monitor/__init__.py
+-rw-r--r--   0        0        0    16172 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/monitor/clinical_applicator.py
+-rw-r--r--   0        0        0    13248 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/detector.py
+-rw-r--r--   0        0        0     2554 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/explainer.py
+-rw-r--r--   0        0        0    13859 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/plotter.py
+-rw-r--r--   0        0        0     9566 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/reductor.py
+-rw-r--r--   0        0        0     9118 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/synthetic_applicator.py
+-rw-r--r--   0        0        0    37496 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/tester.py
+-rw-r--r--   0        0        0    18561 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/utils.py
+-rw-r--r--   0        0        0       81 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/__init__.py
+-rw-r--r--   0        0        0     6005 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/base.py
+-rw-r--r--   0        0        0    18872 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/fields.py
+-rw-r--r--   0        0        0     3054 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/model_card.py
+-rw-r--r--   0        0        0     6166 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/sections.py
+-rw-r--r--   0        0        0       37 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/__init__.py
+-rw-r--r--   0        0        0     3275 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/base.py
+-rw-r--r--   0        0        0    47331 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/classification.py
+-rw-r--r--   0        0        0     5463 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/utils.py
+-rw-r--r--   0        0        0    39651 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/report.py
+-rw-r--r--   0        0        0     1828 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/button.js
+-rw-r--r--   0        0        0    15741 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/macros.jinja
+-rw-r--r--   0        0        0    14849 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/model_report.jinja
+-rw-r--r--   0        0        0    30509 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/plot.js
+-rw-r--r--   0        0        0    33209 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/utils.py
+-rw-r--r--   0        0        0      143 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/__init__.py
+-rw-r--r--   0        0        0     7447 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/base.py
+-rw-r--r--   0        0        0    22027 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/classification.py
+-rw-r--r--   0        0        0     4211 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/utils.py
+-rw-r--r--   0        0        0       23 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/__init__.py
+-rw-r--r--   0        0        0     4966 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/common.py
+-rw-r--r--   0        0        0    10240 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/file.py
+-rw-r--r--   0        0        0     2423 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/index.py
+-rw-r--r--   0        0        0     3611 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/log.py
+-rw-r--r--   0        0        0     1701 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/optional.py
+-rw-r--r--   0        0        0     5571 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/plot.py
+-rw-r--r--   0        0        0      874 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/profile.py
+-rw-r--r--   0        0        0     6350 2024-04-10 21:12:46.409643 pycyclops-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     8864 1970-01-01 00:00:00.000000 pycyclops-0.2.6/PKG-INFO
```

### Comparing `pycyclops-0.2.5/LICENSE.md` & `pycyclops-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/README.md` & `pycyclops-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/aggregate.py` & `pycyclops-0.2.6/cyclops/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/clean.py` & `pycyclops-0.2.6/cyclops/data/clean.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/constants.py` & `pycyclops-0.2.6/cyclops/data/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/df/feature.py` & `pycyclops-0.2.6/cyclops/data/df/feature.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/df/handle_types.py` & `pycyclops-0.2.6/cyclops/data/df/handle_types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/df/normalize.py` & `pycyclops-0.2.6/cyclops/data/df/normalize.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/df/split.py` & `pycyclops-0.2.6/cyclops/data/df/split.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/df/vectorized.py` & `pycyclops-0.2.6/cyclops/data/df/vectorized.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/diagnoses.py` & `pycyclops-0.2.6/cyclops/data/diagnoses.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/features/medical_image.py` & `pycyclops-0.2.6/cyclops/data/features/medical_image.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/impute.py` & `pycyclops-0.2.6/cyclops/data/impute.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/loader.py` & `pycyclops-0.2.6/cyclops/data/loader.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/packaged_loading_scripts/__init__.py` & `pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py` & `pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/preprocess.py` & `pycyclops-0.2.6/cyclops/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/slicer.py` & `pycyclops-0.2.6/cyclops/data/slicer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/string_ops.py` & `pycyclops-0.2.6/cyclops/data/string_ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/transforms.py` & `pycyclops-0.2.6/cyclops/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/data/utils.py` & `pycyclops-0.2.6/cyclops/data/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/evaluator.py` & `pycyclops-0.2.6/cyclops/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/fairness/config.py` & `pycyclops-0.2.6/cyclops/evaluate/fairness/config.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/fairness/evaluator.py` & `pycyclops-0.2.6/cyclops/evaluate/fairness/evaluator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/__init__.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/accuracy.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/auroc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/average_precision.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/__init__.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/_stat_scores.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/accuracy.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/auroc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/average_precision.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/confusion_matrix.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/base.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/f_score.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/__init__.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/accuracy.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/auroc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/auroc.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,19 @@
     state: Union[Array, Tuple[Array, Array]],
     thresholds: Optional[Array],
     max_fpr: Optional[float] = None,
     pos_label: int = 1,
 ) -> Array:
     """Compute the area under the ROC curve for binary classification tasks."""
     fpr, tpr, _ = _binary_roc_compute(state, thresholds, pos_label)
-    xp = apc.array_namespace(state)
+    xp = (
+        apc.array_namespace(*state)
+        if isinstance(state, tuple)
+        else apc.array_namespace(state)
+    )
     if max_fpr is None or max_fpr == 1 or xp.sum(fpr) == 0 or xp.sum(tpr) == 0:
         return _auc_compute(fpr, tpr, 1.0)
 
     _device = apc.device(fpr) if apc.is_array_api_obj(fpr) else apc.device(fpr[0])
     max_area = xp.asarray(max_fpr, dtype=xp.float32, device=_device)
 
     # Add a single point at max_fpr and interpolate its tpr value
@@ -279,22 +283,28 @@
     state: Union[Array, Tuple[Array, Array]],
     num_classes: int,
     thresholds: Optional[Array] = None,
     average: Optional[Literal["macro", "weighted", "none"]] = "macro",
 ) -> Array:
     """Compute the area under the ROC curve for multiclass classification tasks."""
     fpr, tpr, _ = _multiclass_roc_compute(state, num_classes, thresholds=thresholds)
-    xp = apc.array_namespace(state)
+    xp = (
+        apc.array_namespace(*state)
+        if isinstance(state, tuple)
+        else apc.array_namespace(state)
+    )
     return _reduce_auroc(
         fpr,
         tpr,
         average=average,
-        weights=xp.astype(bincount(state[0], minlength=num_classes), xp.float32)
-        if thresholds is None
-        else xp.sum(state[0, ...][:, 1, :], axis=-1),  # type: ignore[call-overload]
+        weights=(
+            xp.astype(bincount(state[0], minlength=num_classes), xp.float32, copy=False)
+            if thresholds is None
+            else xp.sum(state[0, ...][:, 1, :], axis=-1)  # type: ignore[call-overload]
+        ),
         xp=xp,
     )
 
 
 def multiclass_auroc(
     target: Array,
     preds: Array,
@@ -484,25 +494,32 @@
         target = flatten(state[0])
         preds = flatten(state[1])
         if ignore_index is not None:
             target, preds = remove_ignore_index(target, preds, ignore_index)
         return _binary_auroc_compute((target, preds), thresholds, max_fpr=None)
 
     fpr, tpr, _ = _multilabel_roc_compute(state, num_labels, thresholds, ignore_index)
-    xp = apc.array_namespace(state)
+    xp = (
+        apc.array_namespace(*state)
+        if isinstance(state, tuple)
+        else apc.array_namespace(state)
+    )
     return _reduce_auroc(
         fpr,
         tpr,
         average,
-        weights=xp.astype(
-            xp.sum(xp.astype(state[0] == 1, xp.int32), axis=0),
-            xp.float32,
-        )
-        if thresholds is None
-        else xp.sum(state[0, ...][:, 1, :], axis=-1),  # type: ignore[call-overload]
+        weights=(
+            xp.astype(
+                xp.sum(xp.astype(state[0] == 1, xp.int32, copy=False), axis=0),
+                xp.float32,
+                copy=False,
+            )
+            if thresholds is None
+            else xp.sum(state[0, ...][:, 1, :], axis=-1)  # type: ignore[call-overload]
+        ),
         xp=xp,
     )
 
 
 def multilabel_auroc(
     target: Array,
     preds: Array,
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/average_precision.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/average_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,22 +287,28 @@
     """Compute the average precision score for multiclass classification task."""
     precision, recall, _ = _multiclass_precision_recall_curve_compute(
         state,
         num_classes,
         thresholds=thresholds,
         average=None,
     )
-    xp = apc.array_namespace(state)
+    xp = (
+        apc.array_namespace(*state)
+        if isinstance(state, tuple)
+        else apc.array_namespace(state)
+    )
     return _reduce_average_precision(
         precision,
         recall,
         average=average,
-        weights=xp.astype(bincount(state[0], minlength=num_classes), xp.float32)
-        if thresholds is None
-        else xp.sum(state[0, ...][:, 1, :], axis=-1, dtype=xp.float32),  # type: ignore
+        weights=(
+            xp.astype(bincount(state[0], minlength=num_classes), xp.float32, copy=False)
+            if thresholds is None
+            else xp.sum(state[0, ...][:, 1, :], axis=-1, dtype=xp.float32)  # type: ignore[call-overload]
+        ),
         xp=xp,
     )
 
 
 def multiclass_average_precision(
     target: Array,
     preds: Array,
@@ -501,15 +507,19 @@
     state: Union[Tuple[Array, Array], Array],
     num_labels: int,
     thresholds: Optional[Array],
     average: Optional[Literal["micro", "macro", "weighted", "none"]] = "macro",
     ignore_index: Optional[int] = None,
 ) -> Array:
     """Compute the average precision score for multilabel classification task."""
-    xp = apc.array_namespace(state)
+    xp = (
+        apc.array_namespace(*state)
+        if isinstance(state, tuple)
+        else apc.array_namespace(state)
+    )
     if average == "micro":
         if apc.is_array_api_obj(state) and thresholds is not None:
             state = xp.sum(state, axis=1)
         else:
             target, preds = flatten(state[0]), flatten(state[1])
             target, preds = remove_ignore_index(target, preds, ignore_index)
             state = (target, preds)
@@ -521,17 +531,21 @@
         thresholds=thresholds,
         ignore_index=ignore_index,
     )
     return _reduce_average_precision(
         precision,
         recall,
         average=average,
-        weights=xp.sum(xp.astype(state[0] == 1, xp.int32), axis=0, dtype=xp.float32)
-        if thresholds is None
-        else xp.sum(state[0, ...][:, 1, :], axis=-1),  # type: ignore
+        weights=(
+            xp.sum(
+                xp.astype(state[0] == 1, xp.int32, copy=False), axis=0, dtype=xp.float32
+            )
+            if thresholds is None
+            else xp.sum(state[0, ...][:, 1, :], axis=-1)  # type: ignore[call-overload]
+        ),
         xp=xp,
     )
 
 
 def multilabel_average_precision(
     target: Array,
     preds: Array,
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     confmat: Array,
     normalize: Optional[str] = None,
     *,
     xp: ModuleType,
 ) -> Array:
     """Normalize the confusion matrix."""
     if normalize in ["true", "pred", "all"]:
-        confmat = xp.astype(confmat, xp.float32)
+        confmat = xp.astype(confmat, xp.float32, copy=False)
 
     if normalize == "pred":
         return safe_divide(confmat, xp.sum(confmat, axis=-2, keepdims=True))
     if normalize == "true":
         return safe_divide(confmat, xp.sum(confmat, axis=-1, keepdims=True))
     if normalize == "all":
         return safe_divide(confmat, xp.sum(confmat, axis=(-1, -2), keepdims=True))
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/f_score.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/f_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     fp: Array,
     fn: Array,
     tp: Array,
 ) -> Array:
     """Compute the F-beta score for binary classification tasks."""
     beta2 = beta**2
     xp = apc.array_namespace(fp, fn, tp)
-    tp = xp.astype(tp, xp.float32)
-    fp = xp.astype(fp, xp.float32)
-    fn = xp.astype(fn, xp.float32)
+    tp = xp.astype(tp, xp.float32, copy=False)
+    fp = xp.astype(fp, xp.float32, copy=False)
+    fn = xp.astype(fn, xp.float32, copy=False)
     return squeeze_all(
         safe_divide(
             numerator=(1 + beta2) * tp,
             denominator=(1 + beta2) * tp + beta2 * fn + fp,
         ),
     )
 
@@ -86,17 +86,17 @@
         fn = xp.sum(fn, axis=0, dtype=xp.float32)
         fp = xp.sum(fp, axis=0, dtype=xp.float32)
         return safe_divide(
             numerator=(1 + beta2) * tp,
             denominator=(1 + beta2) * tp + beta2 * fn + fp,
         )
 
-    tp = xp.astype(tp, xp.float32)
-    fp = xp.astype(fp, xp.float32)
-    fn = xp.astype(fn, xp.float32)
+    tp = xp.astype(tp, xp.float32, copy=False)
+    fp = xp.astype(fp, xp.float32, copy=False)
+    fn = xp.astype(fn, xp.float32, copy=False)
     score = safe_divide(
         numerator=(1 + beta2) * tp,
         denominator=(1 + beta2) * tp + beta2 * fn + fp,
     )
 
     return _adjust_weight_apply_average(
         score,
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/mae.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mae.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,22 @@
 
 def _mean_absolute_error_update(target: Array, preds: Array) -> Tuple[Array, int]:
     """Update and return variables required to compute Mean Absolute Error."""
     _basic_input_array_checks(target, preds)
     _check_same_shape(target, preds)
     xp = apc.array_namespace(target, preds)
 
-    target = target if is_floating_point(target) else xp.astype(target, xp.float32)
-    preds = preds if is_floating_point(preds) else xp.astype(preds, xp.float32)
+    target = (
+        target
+        if is_floating_point(target)
+        else xp.astype(target, xp.float32, copy=False)
+    )
+    preds = (
+        preds if is_floating_point(preds) else xp.astype(preds, xp.float32, copy=False)
+    )
 
     sum_abs_error = xp.sum(xp.abs(preds - target), dtype=xp.float32)
     num_obs = int(apc.size(target) or 0)
     return sum_abs_error, num_obs
 
 
 def _mean_absolute_error_compute(
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/mape.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,24 @@
     xp = apc.array_namespace(confmat)
 
     # convert multilabel into binary
     confmat = xp.sum(confmat, axis=0) if confmat.ndim == 3 else confmat
 
     if int(apc.size(confmat) or 0) == 4:  # binary case
         # convert tp, tn, fp, fn to float32 for type promotion rules to work
-        tn, fp, fn, tp = xp.reshape(xp.astype(confmat, xp.float32), (-1,))
+        tn, fp, fn, tp = xp.reshape(xp.astype(confmat, xp.float32, copy=False), (-1,))
         if tp + tn != 0 and fp + fn == 0:
             return xp.asarray(1.0, dtype=confmat.dtype, device=apc.device(confmat))  # type: ignore[no-any-return]
 
         if tp + tn == 0 and fp + fn != 0:
             return xp.asarray(-1.0, dtype=confmat.dtype, device=apc.device(confmat))  # type: ignore[no-any-return]
 
     tk = xp.sum(confmat, axis=-1, dtype=xp.float64)  # tn + fp and tp + fn
     pk = xp.sum(confmat, axis=-2, dtype=xp.float64)  # tn + fn and tp + fp
-    c = xp.astype(xp.linalg.trace(confmat), xp.float64)  # tn and tp
+    c = xp.astype(xp.linalg.trace(confmat), xp.float64, copy=False)  # tn and tp
     s = xp.sum(confmat, dtype=xp.float64)  # tn + tp + fn + fp
 
     cov_ytyp = c * s - sum(tk * pk)
     cov_ypyp = s**2 - sum(pk * pk)
     cov_ytyt = s**2 - sum(tk * tk)
 
     numerator = cov_ytyp
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/mse.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/precision_recall.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     target = xp.astype(target == pos_label, xp.float32, copy=False)
     tps = _array_indexing(_cumsum(target * weight, axis=0), threshold_idxs)
     if sample_weights is not None:
         # express fps as a cumsum to ensure fps is increasing even in
         # the presence of floating point errors
         fps = _array_indexing(_cumsum((1 - target) * weight, axis=0), threshold_idxs)
     else:
-        fps = 1 + xp.astype(threshold_idxs, xp.float32) - tps
+        fps = 1 + xp.astype(threshold_idxs, xp.float32, copy=False) - tps
 
     return fps, tps, _array_indexing(preds, threshold_idxs)
 
 
 def _binary_precision_recall_curve_compute(
     state: Union[Array, Tuple[Array, Array]],
     thresholds: Optional[Array],
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/roc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/smape.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/specificity.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/functional/wmape.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/mae.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/mape.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/metric.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/metric_dict.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric_dict.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/mse.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/negative_predictive_value.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/precision_recall.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/precision_recall_curve.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/roc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/smape.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/specificity.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/__init__.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/ops.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Tuple,
     Union,
     cast,
 )
 
 import array_api_compat as apc
 import numpy as np
-from array_api_compat.common._helpers import _is_numpy_array, _is_torch_array
+from array_api_compat.common._helpers import is_numpy_array, is_torch_array
 
 from cyclops.evaluate.metrics.experimental.utils.types import Array
 from cyclops.evaluate.metrics.experimental.utils.validation import (
     _get_int_dtypes,
     is_floating_point,
 )
 
@@ -163,14 +163,15 @@
     size = int(xp.max(array)) + 1
     size = max(size, int(minlength))
     device = apc.device(array)
 
     bincount = xp.astype(
         array == xp.arange(size, device=device)[:, None],
         weights.dtype if weights is not None else xp.int32,
+        copy=False,
     )
     return xp.sum(bincount * (weights if weights is not None else 1), axis=1)
 
 
 def clone(array: Array) -> Array:
     """Create a copy of an array.
 
@@ -241,15 +242,15 @@
     xp = apc.array_namespace(x)
     return xp.max(x, axis=0)
 
 
 def dim_zero_mean(x: Array) -> Array:
     """Average along the zero dimension."""
     xp = apc.array_namespace(x)
-    x = x if is_floating_point(x) else xp.astype(x, xp.float32)
+    x = x if is_floating_point(x) else xp.astype(x, xp.float32, copy=False)
     return xp.mean(x, axis=0)
 
 
 def dim_zero_min(x: Array) -> Array:
     """Min along the zero dimension."""
     xp = apc.array_namespace(x)
     return xp.min(x, axis=0)
@@ -509,20 +510,22 @@
     >>> safe_divide(x, y)
     Array([1., 0., 1.], dtype=float64)
 
     """
     xp = apc.array_namespace(numerator, denominator)
 
     numerator = (
-        numerator if is_floating_point(numerator) else xp.astype(numerator, xp.float32)
+        numerator
+        if is_floating_point(numerator)
+        else xp.astype(numerator, xp.float32, copy=False)
     )
     denominator = (
         denominator
         if is_floating_point(denominator)
-        else xp.astype(denominator, xp.float32)
+        else xp.astype(denominator, xp.float32, copy=False)
     )
 
     return xp.where(
         denominator == 0,
         xp.asarray(0, dtype=xp.float32, device=apc.device(numerator)),
         numerator / denominator,
     )
@@ -550,15 +553,17 @@
     Array([0.75026011, 0.88079708, 0.95257413], dtype=float64)
 
     """
     xp = apc.array_namespace(array)
     if apc.size(array) == 0:
         return xp.asarray([], dtype=xp.float32, device=apc.device(array))
 
-    array = array if is_floating_point(array) else xp.astype(array, xp.float32)
+    array = (
+        array if is_floating_point(array) else xp.astype(array, xp.float32, copy=False)
+    )
 
     exp_array = xp.exp(array)
     return xp.where(
         array >= 0,
         1 / (1 + xp.exp(-array)),
         exp_array / (1 + exp_array),
     )
@@ -671,15 +676,15 @@
     if average == "weighted":
         weights = tp + fn
     else:  # average == "macro"
         weights = xp.ones_like(score)
         if not is_multilabel:
             weights[tp + fp + fn == 0] = 0.0
 
-    weights = xp.astype(weights, xp.float32)
+    weights = xp.astype(weights, xp.float32, copy=False)
     return xp.sum(  # type: ignore[no-any-return]
         safe_divide(
             weights * score,
             xp.sum(weights, axis=-1, dtype=score.dtype, keepdims=True),
         ),
         axis=-1,
         dtype=score.dtype,
@@ -736,15 +741,15 @@
                 raise ValueError(
                     "The array `x` is neither increasing or decreasing. "
                     "Try setting the reorder argument to `True`.",
                 )
         else:
             direction = 1.0
 
-    return xp.astype(_trapz(y, x, axis=axis) * direction, xp.float32)
+    return xp.astype(_trapz(y, x, axis=axis) * direction, xp.float32, copy=False)
 
 
 def _cumsum(x: Array, axis: Optional[int] = None, dtype: Optional[Any] = None) -> Array:
     """Compute the cumulative sum of an array along a given axis.
 
     Parameters
     ----------
@@ -906,15 +911,15 @@
     Array
         The interpolated values.
     """
     xp = apc.array_namespace(x, xcoords, ycoords)
     if hasattr(xp, "interp"):
         return xp.interp(x, xcoords, ycoords)
 
-    if _is_torch_array(x):
+    if is_torch_array(x):
         weight = (x - xcoords[0]) / (xcoords[-1] - xcoords[0])
         return xp.lerp(ycoords[0], ycoords[-1], weight)
 
     if xcoords.ndim != 1 or ycoords.ndim != 1:
         raise ValueError(
             "Expected `xcoords` and `ycoords` to be 1D arrays. "
             f"Got xcoords.ndim={xcoords.ndim} and ycoords.ndim={ycoords.ndim}.",
@@ -926,15 +931,18 @@
         )
 
     m = safe_divide(ycoords[1:] - ycoords[:-1], xcoords[1:] - xcoords[:-1])
     b = ycoords[:-1] - (m * xcoords[:-1])
 
     # create slices to work for any ndim of x and xcoords
     indices = (
-        xp.sum(xp.astype(x[..., None] >= xcoords[None, ...], xp.int32), axis=1) - 1
+        xp.sum(
+            xp.astype(x[..., None] >= xcoords[None, ...], xp.int32, copy=False), axis=1
+        )
+        - 1
     )
     _min_val = xp.asarray(0, dtype=xp.int32, device=apc.device(x))
     _max_val = xp.asarray(
         m.shape[0] if m.ndim > 0 else 1 - 1,
         dtype=xp.int32,
         device=apc.device(x),
     )
@@ -1018,17 +1026,17 @@
         topk_indices = xp.argsort(scores, axis=axis, descending=True, stable=False)
         slice_indices = [slice(None)] * scores.ndim
         slice_indices[axis] = slice(None, top_k)
         topk_indices = topk_indices[tuple(slice_indices)]
 
     zeros = xp.zeros_like(scores, dtype=xp.int32)
 
-    if _is_torch_array(scores):
+    if is_torch_array(scores):
         return zeros.scatter(axis, topk_indices, 1)
-    if _is_numpy_array(scores):
+    if is_numpy_array(scores):
         xp.put_along_axis(zeros, topk_indices, 1, axis)
         return zeros
 
     result = np.zeros(scores.shape, dtype=np.int32)
     topk_indices = np.from_dlpack(apc.to_device(topk_indices, "cpu"))
     np.put_along_axis(result, topk_indices, 1, axis)
```

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/types.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/utils/validation.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/experimental/wmape.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/f_beta.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/factory.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/__init__.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/accuracy.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/auroc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/average_precision.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/f_beta.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/precision_recall.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/precision_recall_curve.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/roc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/sensitivity.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/specificity.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/functional/stat_scores.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/metric.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/precision_recall.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/precision_recall_curve.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/roc.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/sensitivity.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/specificity.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/stat_scores.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/metrics/utils.py` & `pycyclops-0.2.6/cyclops/evaluate/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/evaluate/utils.py` & `pycyclops-0.2.6/cyclops/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/__init__.py` & `pycyclops-0.2.6/cyclops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/catalog.py` & `pycyclops-0.2.6/cyclops/models/catalog.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/configs/densenet.yaml` & `pycyclops-0.2.6/cyclops/models/configs/densenet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/configs/gru.yaml` & `pycyclops-0.2.6/cyclops/models/configs/gru.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/configs/lstm.yaml` & `pycyclops-0.2.6/cyclops/models/configs/lstm.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/configs/mlp_pt.yaml` & `pycyclops-0.2.6/cyclops/models/configs/mlp_pt.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/configs/resnet.yaml` & `pycyclops-0.2.6/cyclops/models/configs/resnet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/configs/rnn.yaml` & `pycyclops-0.2.6/cyclops/models/configs/rnn.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/data.py` & `pycyclops-0.2.6/cyclops/models/data.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/neural_nets/gru.py` & `pycyclops-0.2.6/cyclops/models/neural_nets/gru.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/neural_nets/lstm.py` & `pycyclops-0.2.6/cyclops/models/neural_nets/lstm.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/neural_nets/mlp.py` & `pycyclops-0.2.6/cyclops/models/neural_nets/mlp.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/neural_nets/rnn.py` & `pycyclops-0.2.6/cyclops/models/neural_nets/rnn.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/plotter.py` & `pycyclops-0.2.6/cyclops/models/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/torch_utils.py` & `pycyclops-0.2.6/cyclops/models/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/utils.py` & `pycyclops-0.2.6/cyclops/models/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/wrappers/base.py` & `pycyclops-0.2.6/cyclops/models/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/wrappers/pt_model.py` & `pycyclops-0.2.6/cyclops/models/wrappers/pt_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/wrappers/sk_model.py` & `pycyclops-0.2.6/cyclops/models/wrappers/sk_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/models/wrappers/utils.py` & `pycyclops-0.2.6/cyclops/models/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/clinical_applicator.py` & `pycyclops-0.2.6/cyclops/monitor/clinical_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/detector.py` & `pycyclops-0.2.6/cyclops/monitor/detector.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/explainer.py` & `pycyclops-0.2.6/cyclops/monitor/explainer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/plotter.py` & `pycyclops-0.2.6/cyclops/monitor/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/reductor.py` & `pycyclops-0.2.6/cyclops/monitor/reductor.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/synthetic_applicator.py` & `pycyclops-0.2.6/cyclops/monitor/synthetic_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/tester.py` & `pycyclops-0.2.6/cyclops/monitor/tester.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/monitor/utils.py` & `pycyclops-0.2.6/cyclops/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/model_card/base.py` & `pycyclops-0.2.6/cyclops/report/model_card/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/model_card/fields.py` & `pycyclops-0.2.6/cyclops/report/model_card/fields.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/model_card/model_card.py` & `pycyclops-0.2.6/cyclops/report/model_card/model_card.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/model_card/sections.py` & `pycyclops-0.2.6/cyclops/report/model_card/sections.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/plot/base.py` & `pycyclops-0.2.6/cyclops/report/plot/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/plot/classification.py` & `pycyclops-0.2.6/cyclops/report/plot/classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Classification plotter."""
 
 from collections import defaultdict
 from typing import Any, Dict, List, Literal, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
+from sklearn.calibration import calibration_curve
 
 from cyclops.evaluate.metrics.experimental.functional import PRCurve as PRCurveExp
 from cyclops.evaluate.metrics.experimental.functional import ROCCurve as ROCCurveExp
 from cyclops.evaluate.metrics.functional import PRCurve, ROCCurve
 from cyclops.report.plot.base import Plotter
 from cyclops.report.plot.utils import (
     bar_plot,
@@ -89,14 +91,133 @@
             ), "class_names must be equal to class_num"
         elif self.task_type == "multilabel":
             class_names = [f"Label_{i+1}" for i in range(self.class_num)]
         else:
             class_names = [f"Class_{i+1}" for i in range(self.class_num)]
         self.class_names = class_names
 
+    def calibration(
+        self,
+        data: pd.DataFrame,
+        y_true_col: str,
+        y_prob_col: str,
+        group_col: Optional[str] = None,
+        title: Optional[str] = "Calibration Plot",
+        layout: Optional[go.Layout] = None,
+        n_bins: Optional[int] = 10,
+        n_bins_hist: Optional[int] = 100,
+        **plot_kwargs: Any,
+    ) -> go.Figure:
+        """Plot calibration curve for binary classification.
+
+        Parameters
+        ----------
+        data : pd.DataFrame
+            Dataframe containing true labels and predicted probabilities
+        y_true_col : str
+            Column name for true labels
+        y_prob_col : str
+            Column name for predicted probabilities
+        group_col : str, optional
+            Column name for grouping the data, by default None
+        title: str, optional
+            Plot title, by default "Calibration Plot"
+        layout : go.Layout, optional
+            Customized figure layout, by default None
+        n_bins : int, optional
+            Number of bins for calibration curve, by default 10
+        n_bins_hist : int, optional
+            Number of bins for histogram, by default 100
+        **plot_kwargs : dict
+            Additional keyword arguments
+
+        Returns
+        -------
+        go.Figure
+            Plotly figure object
+
+        """
+        if self.task_type != "binary":
+            raise ValueError(
+                "Calibration plot is only available for binary classification"
+            )
+        # Create subplots: 1 plot for calibration curve, 1 plot for histogram
+        fig = make_subplots(
+            rows=2,
+            cols=1,
+            shared_xaxes=True,
+            vertical_spacing=0.02,
+            row_heights=[0.8, 0.2],
+        )
+        if group_col:
+            # Plot a calibration curve for each level of the grouping variable
+            unique_groups = data[group_col].unique()
+            for group in unique_groups:
+                group_df = data[data[group_col] == group]
+                prob_true, prob_pred = calibration_curve(
+                    group_df[y_true_col], group_df[y_prob_col], n_bins=n_bins
+                )
+                fig.add_trace(
+                    go.Scatter(
+                        x=prob_pred, y=prob_true, mode="markers+lines", name=f"{group}"
+                    ),
+                    row=1,
+                    col=1,
+                )
+        else:
+            # Plot a single calibration curve
+            prob_true, prob_pred = calibration_curve(
+                data[y_true_col], data[y_prob_col], n_bins=n_bins
+            )
+            fig.add_trace(
+                go.Scatter(
+                    x=prob_pred, y=prob_true, mode="markers+lines", name="Model"
+                ),
+                row=1,
+                col=1,
+            )
+        # Add perfectly calibrated line to the calibration curve
+        fig.add_trace(
+            go.Scatter(
+                x=[0, 1],
+                y=[0, 1],
+                mode="lines",
+                name="Perfectly calibrated",
+                line={"dash": "dot"},
+            ),
+            row=1,
+            col=1,
+        )
+        # Plot histogram if no grouping variable is provided
+        fig.add_trace(
+            go.Histogram(
+                x=data[y_prob_col],
+                nbinsx=n_bins_hist,
+                name="Probabilities",
+                showlegend=False,
+            ),
+            row=2,
+            col=1,
+        )
+        # Update layout
+        legend_title = group_col if group_col else None
+        fig.update_layout(
+            height=800,
+            title=title,
+            yaxis_title="Fraction of Positives",
+            legend_title=legend_title,
+        )
+        fig.update_xaxes(title_text="Mean Predicted Probability", row=2, col=1)
+        fig.update_yaxes(title_text="Count", row=2, col=1)
+
+        if layout is not None:
+            fig.update_layout(layout)
+
+        return fig
+
     def threshperf(
         self,
         roc_curve: ROCCurve,
         ppv: npt.NDArray[np.float_],
         npv: npt.NDArray[np.float_],
         pred_probs: npt.NDArray[np.float_],
         title: Optional[str] = "Diagnostic Performance Metrics by Thresholds",
@@ -135,107 +256,95 @@
             == len(roc_curve.fpr)
             == len(roc_curve.thresholds)
             == len(ppv)
             == len(npv)
         ), "Length mismatch between ROC curve, PPV, NPV. All curves need to be computed using the same thresholds"
         # Define hover template to show three decimal places
         hover_template = "Threshold: %{x:.3f}<br>Metric Value: %{y:.3f}<extra></extra>"
-
         # Create a subplot for each metric
         fig = make_subplots(rows=5, cols=1, shared_xaxes=True, vertical_spacing=0.02)
-
         # Sensitivity plot (True Positive Rate)
         fig.add_trace(
             go.Scatter(
                 x=roc_curve.thresholds,
                 y=roc_curve.tpr,
                 mode="lines",
                 name="Sensitivity",
                 hovertemplate=hover_template,
             ),
             row=1,
             col=1,
         )
-
         # Specificity plot (1 - False Positive Rate)
         fig.add_trace(
             go.Scatter(
                 x=roc_curve.thresholds,
                 y=1 - roc_curve.fpr,
                 mode="lines",
                 name="1 - Specificity",
                 hovertemplate=hover_template,
             ),
             row=2,
             col=1,
         )
-
         # PPV plot (Positive Predictive Value)
         fig.add_trace(
             go.Scatter(
                 x=roc_curve.thresholds,
                 y=ppv,
                 mode="lines",
                 name="PPV",
                 hovertemplate=hover_template,
             ),
             row=3,
             col=1,
         )
-
         # NPV plot (Negative Predictive Value)
         fig.add_trace(
             go.Scatter(
                 x=roc_curve.thresholds,
                 y=npv,
                 mode="lines",
                 name="NPV",
                 hovertemplate=hover_template,
             ),
             row=4,
             col=1,
         )
-
         # Add histogram of predicted probabilities
         fig.add_trace(
             go.Histogram(x=pred_probs, nbinsx=80, name="Predicted Probabilities"),
             row=5,
             col=1,
         )
-
         # Update layout
         fig.update_layout(
             height=1200,
             width=1024,
             title_text=title,
             legend={
                 "orientation": "h",
                 "yanchor": "bottom",
                 "y": -0.2,
                 "xanchor": "center",
                 "x": 0.5,
             },
         )
-
         # Remove subplot titles
         for i in fig["layout"]["annotations"]:
             i["text"] = ""
-
         # Remove the plot background color, keep gridlines, show y-axis ticks and labels
         fig.update_xaxes(showgrid=True)
         fig.update_yaxes(showgrid=True, showticklabels=True)
-
         # Only show the x-axis line and labels on the bottommost plot
         fig.update_xaxes(showline=True, linewidth=1, linecolor="black", mirror=True)
         fig.update_xaxes(showticklabels=True, row=4, col=1)
         fig.update_yaxes(showline=True, linewidth=1, linecolor="black", mirror=True)
-
         fig.update_xaxes(showline=False, row=5, col=1, showticklabels=False)
         fig.update_yaxes(showline=False, row=5, col=1)
-
         if layout is not None:
             fig.update_layout(layout)
 
         return fig
 
     def roc_curve(
         self,
@@ -1140,15 +1249,15 @@
 
             fig.update_layout(title={"text": title}, height=rows * 450)
 
         if layout is not None:
             fig.update_layout(layout)
         return fig
 
-    def plot_confusion_matrix(
+    def confusion_matrix(
         self,
         confusion_matrix: np.typing.NDArray[Any],
     ) -> go.Figure:
         """Plot confusion matrix.
 
         Parameters
         ----------
```

### Comparing `pycyclops-0.2.5/cyclops/report/plot/utils.py` & `pycyclops-0.2.6/cyclops/report/plot/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/report.py` & `pycyclops-0.2.6/cyclops/report/report.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/templates/model_report/button.js` & `pycyclops-0.2.6/cyclops/report/templates/model_report/button.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/templates/model_report/macros.jinja` & `pycyclops-0.2.6/cyclops/report/templates/model_report/macros.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/templates/model_report/model_report.jinja` & `pycyclops-0.2.6/cyclops/report/templates/model_report/model_report.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/templates/model_report/plot.js` & `pycyclops-0.2.6/cyclops/report/templates/model_report/plot.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/report/utils.py` & `pycyclops-0.2.6/cyclops/report/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,23 @@
     GraphicsCollection,
     MetricCard,
     PerformanceMetric,
     Test,
 )
 
 
+_METRIC_NAMES_DISPLAY_MAP = {
+    "PositivePredictiveValue": "Positive Predictive Value (PPV)",
+    "NegativePredictiveValue": "Negative Predictive Value (NPV)",
+    "FalsePositiveRate": "False Positive Rate (FPR)",
+    "FalseNegativeRate": "False Negative Rate (FNR)",
+    "F1Score": "F1 Score",
+}
+
+
 def str_to_snake_case(string: str) -> str:
     """Convert a string to snake_case.
 
     Parameters
     ----------
     string : str
         The string to convert.
@@ -572,26 +581,30 @@
         pass
     else:
         for itr, metric_card in enumerate(model_card.overview.metric_cards.collection):
             timestamps[itr] = metric_card.timestamps
     return json.dumps(timestamps)
 
 
-def create_metric_cards(  # noqa: PLR0912 PLR0915
+def _extract_slices_and_values(
     current_metrics: List[PerformanceMetric],
-    timestamp: str,
-    last_metric_cards: Optional[List[MetricCard]] = None,
-) -> Tuple[
-    List[str],
-    List[Optional[str]],
-    List[str],
-    List[List[str]],
-    List[MetricCard],
-]:
-    """Create metric cards for each metric."""
+) -> Tuple[List[str], List[List[str]]]:
+    """Extract slice and value names from a list of performance metrics.
+
+    Parameters
+    ----------
+    current_metrics : List[PerformanceMetric]
+        The list of performance metrics to extract slice and value names from.
+
+    Returns
+    -------
+    Tuple[List[str], List[List[str]]]
+        A tuple of lists of slice and value names.
+
+    """
     slices_values = []
     for current_metric in current_metrics:
         if current_metric.slice is not None:
             for slice_val in current_metric.slice.split("&"):
                 if slice_val not in slices_values and slice_val != "overall":
                     slices_values.append(slice_val)
     slices = [
@@ -601,235 +614,351 @@
     ]
     slices = list(dict.fromkeys(slices))
     values_all = [
         slice_val.split(":")[1]
         for slice_val in slices_values
         if slice_val.split(":")[0] != "overall"
     ]
-
     values: List[List[str]] = [[] for _ in range(len(slices))]
-
     for i, slice_name in enumerate(slices):
         for j, slice_val in enumerate(slices_values):
             if slice_val.startswith(slice_name):
                 values[i].append(values_all[j])
 
+    return slices, values
+
+
+def _gather_metrics(
+    current_metrics: List[PerformanceMetric],
+    last_metric_cards: Optional[List[MetricCard]] = None,
+) -> List[Dict[str, Any]]:
+    """Gather all metrics from current metrics and last metric cards.
+
+    Parameters
+    ----------
+    current_metrics : List[PerformanceMetric]
+        The current performance metrics.
+    last_metric_cards : Optional[List[MetricCard]], optional
+        The last metric cards, by default None.
+
+    Returns
+    -------
+    List[Dict[str, Any]]
+        A list of dictionaries with keys type, slice, current_metric,
+        and last_metric_card.
+
+    """
     all_metrics = []
-    # gather overall metrics with matching type
     for current_metric in current_metrics:
-        if last_metric_cards is None:
-            last_metric_card_match = None
-        else:
-            last_metric_card_match = None
-            for last_metric_card in last_metric_cards:
-                if (
-                    current_metric.type == last_metric_card.type
-                    and current_metric.slice == last_metric_card.slice
-                ):
-                    last_metric_card_match = last_metric_card
+        last_metric_card_match = next(
+            (
+                last_metric_card
+                for last_metric_card in last_metric_cards or []
+                if current_metric.type == last_metric_card.type
+                and current_metric.slice == last_metric_card.slice
+            ),
+            None,
+        )
         all_metrics.append(
             {
                 "type": current_metric.type,
                 "slice": current_metric.slice,
                 "current_metric": current_metric,
                 "last_metric_card": last_metric_card_match,
-            },
+            }
         )
-
-    # find metric cards that are not in current metrics
     if last_metric_cards is not None:
         for last_metric_card in last_metric_cards:
-            current_metric_match = None
-            for current_metric in current_metrics:
-                if (
-                    current_metric.type == last_metric_card.type
+            current_metric_match = next(
+                (
+                    current_metric
+                    for current_metric in current_metrics
+                    if current_metric.type == last_metric_card.type
                     and current_metric.slice == last_metric_card.slice
-                ):
-                    current_metric_match = current_metric
-
+                ),
+                None,
+            )
             if current_metric_match is None:
                 all_metrics.append(
                     {
                         "type": last_metric_card.type,
                         "slice": last_metric_card.slice,
                         "current_metric": None,
                         "last_metric_card": last_metric_card,
-                    },
+                    }
                 )
 
-    # create dict to populate metrics cards
+    return all_metrics
+
+
+def _process_metric_name(
+    metric: Dict[str, Any],
+) -> str:
+    """Process a metric name.
+
+    Parameters
+    ----------
+    metric : Dict[str, Any]
+        Metric dictionary.
+
+    Returns
+    -------
+    str
+        The processed metric name.
+
+    """
+    if isinstance(metric["type"], str):
+        # Check if name has prefix "Binary", "Multiclass", or "Multilabel"
+        if metric["type"].startswith("Binary"):
+            name = metric["type"][6:]
+        elif metric["type"].startswith("Multiclass") or metric["type"].startswith(
+            "Multilabel",
+        ):
+            name = metric["type"][10:]
+        for key, value in _METRIC_NAMES_DISPLAY_MAP.items():
+            name = name.replace(key, value)
+    else:
+        raise ValueError(f"Invalid metric type: {metric['type']}")
+
+    return name
+
+
+def _create_metric_card(
+    metric: Dict[str, Any],
+    name: str,
+    history: List[float],
+    timestamps: List[str],
+    threshold: Union[float, None],
+    passed: Union[bool, None],
+) -> MetricCard:
+    """Create a metric card.
+
+    Parameters
+    ----------
+    metric : Dict[str, Any]
+        Metric dictionary.
+    name : str
+        The name for the metric card.
+    history : List[float]
+        The history for the metric card.
+    timestamps : List[str]
+        The timestamps for the metric card.
+    threshold : Union[float, None]
+        The threshold for the metric card.
+    passed : Union[bool, None]
+        Whether or not the metric card passed.
+
+    Returns
+    -------
+    MetricCard
+        The created metric card.
+
+    """
+    return MetricCard(
+        name=name,
+        type=metric["current_metric"].type
+        if isinstance(metric["current_metric"], PerformanceMetric)
+        else None,
+        slice=metric["current_metric"].slice
+        if isinstance(metric["current_metric"], PerformanceMetric)
+        else None,
+        tooltip=metric["current_metric"].description
+        if isinstance(metric["current_metric"], PerformanceMetric)
+        else None,
+        value=metric["current_metric"].value
+        if isinstance(metric["current_metric"], PerformanceMetric)
+        and isinstance(metric["current_metric"].value, float)
+        else None,
+        threshold=threshold,
+        passed=passed,
+        history=history,
+        timestamps=timestamps,
+    )
+
+
+def _get_metric_card(
+    metric: Dict[str, Any],
+    name: str,
+    timestamp: str,
+) -> MetricCard:
+    """Get a metric card.
+
+    Parameters
+    ----------
+    metric : Dict[str, Any]
+        Metric dictionary.
+    name : str
+        The name for the metric card.
+    timestamp : str
+        The timestamp for the current metric card.
+
+    Returns
+    -------
+    Tuple[List[float], List[str], MetricCard]
+        The history, timestamps, and metric card.
+
+    """
+    metric_card = None
+    if (
+        metric["current_metric"] is None
+        and metric["last_metric_card"]
+        and isinstance(
+            metric["last_metric_card"],
+            MetricCard,
+        )
+    ):
+        history = metric["last_metric_card"].history
+        history.append(np.nan)
+        timestamps = metric["last_metric_card"].timestamps
+        if timestamps is not None:
+            timestamps.append(timestamp)
+        metric["last_metric_card"].timestamps = timestamps
+        metric_card = metric["last_metric_card"]
+    elif (
+        metric["current_metric"] is not None
+        and metric["last_metric_card"]
+        and isinstance(
+            metric["last_metric_card"],
+            MetricCard,
+        )
+    ):
+        history = metric["last_metric_card"].history
+        if (isinstance(metric["current_metric"], PerformanceMetric)) and (
+            isinstance(metric["current_metric"].value, float)
+        ):
+            history.append(metric["current_metric"].value)
+        timestamps = metric["last_metric_card"].timestamps
+        if timestamps is not None:
+            timestamps.append(timestamp)
+    else:
+        history = [
+            metric["current_metric"].value
+            if isinstance(
+                metric["current_metric"],
+                PerformanceMetric,
+            )
+            and isinstance(metric["current_metric"].value, float)
+            else 0,
+        ]
+        timestamps = [timestamp]
+    if metric_card is None:
+        metric_card = _create_metric_card(
+            metric,
+            name,
+            history,
+            timestamps,
+            _get_threshold(metric),
+            _get_passed(metric),
+        )
+
+    return metric_card
+
+
+def _get_threshold(metric: Dict[str, Any]) -> Union[float, None]:
+    """Get the threshold for a metric card.
+
+    Parameters
+    ----------
+    metric : Dict[str, Any]
+        Metric dictionary.
+
+    Returns
+    -------
+    Union[float, None]
+        The threshold for the metric card.
+
+    """
+    return (
+        metric["current_metric"].tests[0].threshold
+        if (
+            isinstance(metric["current_metric"], PerformanceMetric)
+            and (metric["current_metric"].tests is not None)
+            and (isinstance(metric["current_metric"].tests[0], Test))
+            and (metric["current_metric"].tests[0].threshold is not None)
+        )
+        else None
+    )
+
+
+def _get_passed(metric: Dict[str, Any]) -> Union[bool, None]:
+    """Get whether or not a metric card test passed.
+
+    Parameters
+    ----------
+    metric : Dict[str, Any]
+        Metric dictionary.
+
+    Returns
+    -------
+    Union[bool, None]
+        Whether or not the metric card passed.
+
+    """
+    return (
+        metric["current_metric"].tests[0].passed
+        if (
+            isinstance(metric["current_metric"], PerformanceMetric)
+            and (metric["current_metric"].tests is not None)
+            and (isinstance(metric["current_metric"].tests[0], Test))
+            and (metric["current_metric"].tests[0].passed is not None)
+        )
+        else None
+    )
+
+
+def create_metric_cards(
+    current_metrics: List[PerformanceMetric],
+    timestamp: str,
+    last_metric_cards: Optional[List[MetricCard]] = None,
+) -> Tuple[
+    List[str],
+    List[Optional[str]],
+    List[str],
+    List[List[str]],
+    List[MetricCard],
+]:
+    """Create metric cards for each metric.
+
+    Parameters
+    ----------
+    current_metrics : List[PerformanceMetric]
+        The current performance metrics.
+    timestamp : str
+        The timestamp for the current metric card.
+    last_metric_cards : Optional[List[MetricCard]], optional
+        The last metric cards, by default None.
+
+    Returns
+    -------
+    Tuple[
+        List[str],
+        List[Optional[str]],
+        List[str],
+        List[List[str]],
+        List[MetricCard]
+    ]
+        A tuple of lists of metrics, tooltips, slices, values, and metric cards.
+
+    """
+    slices, values = _extract_slices_and_values(current_metrics)
+    all_metrics = _gather_metrics(current_metrics, last_metric_cards)
+    # Create dict to populate metrics cards
     metric_cards = []
     metrics = []
     tooltips = []
     for metric in all_metrics:
-        # split into words by camelcase
-        if isinstance(metric["type"], str):
-            # check if name has prefix "Binary", "Multiclass", or "Multilabel"
-            if metric["type"].startswith("Binary"):
-                name = metric["type"][6:]
-            elif metric["type"].startswith("Multiclass") or metric["type"].startswith(
-                "Multilabel",
-            ):
-                name = metric["type"][10:]
-            name = name.replace(
-                "PositivePredictiveValue",
-                "Positive Predictive Value (PPV)",
-            )
-            name = name.replace(
-                "NegativePredictiveValue",
-                "Negative Predictive Value (NPV)",
-            )
-            name = name.replace(
-                "FalsePositiveRate",
-                "False Positive Rate (FPR)",
-            )
-            name = name.replace(
-                "FalseNegativeRate",
-                "False Negative Rate (FNR)",
-            )
-            name = name.replace(
-                "F1Score",
-                "F1 Score",
-            )
+        name = _process_metric_name(metric)
         metrics.append(name)
         if isinstance(metric["current_metric"], PerformanceMetric):
             tooltips.append(metric["current_metric"].description)
-
-        if (
-            metric["current_metric"] is None
-            and metric["last_metric_card"]
-            and isinstance(
-                metric["last_metric_card"],
-                MetricCard,
-            )
-        ):
-            history = metric["last_metric_card"].history
-            history.append(np.nan)
-            metric["last_metric_card"].value = np.nan
-            timestamps = metric["last_metric_card"].timestamps
-            if timestamps is not None:
-                timestamps.append(timestamp)
-            metric["last_metric_card"].timestamps = timestamps
-            metric_cards.append(metric["last_metric_card"])
-
-        elif (
-            metric["current_metric"] is not None
-            and metric["last_metric_card"]
-            and isinstance(
-                metric["last_metric_card"],
-                MetricCard,
-            )
-        ):
-            history = metric["last_metric_card"].history
-            if (isinstance(metric["current_metric"], PerformanceMetric)) and (
-                isinstance(metric["current_metric"].value, float)
-            ):
-                history.append(metric["current_metric"].value)
-
-            timestamps = metric["last_metric_card"].timestamps
-            if timestamps is not None:
-                timestamps.append(timestamp)
-
-            metric_cards.append(
-                MetricCard(
-                    name=name,
-                    type=metric["current_metric"].type
-                    if isinstance(metric["current_metric"], PerformanceMetric)
-                    else None,
-                    slice=metric["current_metric"].slice
-                    if isinstance(metric["current_metric"], PerformanceMetric)
-                    else None,
-                    tooltip=metric["current_metric"].description
-                    if isinstance(metric["current_metric"], PerformanceMetric)
-                    else None,
-                    value=metric["current_metric"].value
-                    if isinstance(metric["current_metric"], PerformanceMetric)
-                    and isinstance(metric["current_metric"].value, float)
-                    else None,
-                    threshold=metric["current_metric"].tests[0].threshold
-                    if (
-                        isinstance(metric["current_metric"], PerformanceMetric)
-                        and (metric["current_metric"].tests is not None)
-                        and (isinstance(metric["current_metric"].tests[0], Test))
-                        and (metric["current_metric"].tests[0].threshold is not None)
-                    )
-                    else None,
-                    passed=metric["current_metric"].tests[0].passed
-                    if (
-                        isinstance(metric["current_metric"], PerformanceMetric)
-                        and (metric["current_metric"].tests is not None)
-                        and (isinstance(metric["current_metric"].tests[0], Test))
-                        and (metric["current_metric"].tests[0].passed is not None)
-                    )
-                    else None,
-                    history=history,
-                    timestamps=timestamps,
-                ),
-            )
-        else:
-            metric_cards.append(
-                MetricCard(
-                    name=name,
-                    type=metric["current_metric"].type
-                    if isinstance(
-                        metric["current_metric"],
-                        PerformanceMetric,
-                    )
-                    else None,
-                    slice=metric["current_metric"].slice
-                    if isinstance(
-                        metric["current_metric"],
-                        PerformanceMetric,
-                    )
-                    else None,
-                    tooltip=metric["current_metric"].description
-                    if isinstance(
-                        metric["current_metric"],
-                        PerformanceMetric,
-                    )
-                    else None,
-                    value=metric["current_metric"].value
-                    if isinstance(
-                        metric["current_metric"],
-                        PerformanceMetric,
-                    )
-                    and isinstance(metric["current_metric"].value, float)
-                    else None
-                    if isinstance(metric["current_metric"], PerformanceMetric)
-                    else None,
-                    threshold=metric["current_metric"].tests[0].threshold
-                    if (
-                        isinstance(metric["current_metric"], PerformanceMetric)
-                        and (metric["current_metric"].tests is not None)
-                        and (isinstance(metric["current_metric"].tests[0], Test))
-                        and (metric["current_metric"].tests[0].threshold is not None)
-                    )
-                    else None,
-                    passed=metric["current_metric"].tests[0].passed
-                    if (
-                        isinstance(metric["current_metric"], PerformanceMetric)
-                        and (metric["current_metric"].tests is not None)
-                        and (isinstance(metric["current_metric"].tests[0], Test))
-                        and (metric["current_metric"].tests[0].passed is not None)
-                    )
-                    else None,
-                    history=[
-                        metric["current_metric"].value
-                        if isinstance(
-                            metric["current_metric"],
-                            PerformanceMetric,
-                        )
-                        and isinstance(metric["current_metric"].value, float)
-                        else 0,
-                    ],
-                    timestamps=[timestamp],
-                ),
-            )
+        metric_card = _get_metric_card(metric, name, timestamp)
+        metric_cards.append(metric_card)
     metrics = list(dict.fromkeys(metrics))
     tooltips = list(dict.fromkeys(tooltips))
+
     return metrics, tooltips, slices, values, metric_cards
 
 
 def create_metric_card_plot(
     history: List[float],
     threshold: float,
 ) -> GraphicsCollection:
```

### Comparing `pycyclops-0.2.5/cyclops/tasks/base.py` & `pycyclops-0.2.6/cyclops/tasks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,69 @@
 """Base task class."""
 
 import logging
 import os
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
-from cyclops.models.torch_utils import get_device
 from cyclops.models.wrappers import WrappedModel
 from cyclops.tasks.utils import prepare_models
 from cyclops.utils.log import setup_logging
 
 
 LOGGER = logging.getLogger(__name__)
 setup_logging(print_level="INFO", logger=LOGGER)
 
 
 class BaseTask(ABC):
-    """Base task class."""
+    """Base task class.
+
+    Parameters
+    ----------
+    models
+        Models to use for the task. Can be a single model, a list of models, or a
+        dictionary of models.
+    task_features
+        Features to use for the task.
+    task_target
+        Target to use for the task.
+
+    Attributes
+    ----------
+    models
+        Models to use for the task.
+    task_features
+        Features to use for the task.
+    task_target
+        Target to use for the task.
+    trained_models
+        List of trained models.
+    pretrained_models
+        List of pretrained models.
+
+    """
 
     def __init__(
         self,
         models: Union[
             str,
             WrappedModel,
             Sequence[Union[str, WrappedModel]],
             Dict[str, WrappedModel],
         ],
         task_features: List[str],
         task_target: Union[str, List[str]],
     ) -> None:
-        """Initialize base task class.
-
-        Parameters
-        ----------
-        models
-            Models to use for the task. Can be a single model, a list of models, or a
-            dictionary of models.
-        task_features
-            Features to use for the task.
-        task_target
-            Target to use for the task.
-
-        """
+        """Initialize base task class."""
         self.models = prepare_models(models)
         self._validate_models()
         self.task_features = task_features
         self.task_target = (
             [task_target] if isinstance(task_target, str) else task_target
         )
-        self.device = get_device()
         self.trained_models: List[str] = []
         self.pretrained_models: List[str] = []
 
     @property
     def models_count(self) -> int:
         """Number of models in the task.
```

### Comparing `pycyclops-0.2.5/cyclops/tasks/classification.py` & `pycyclops-0.2.6/cyclops/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/tasks/utils.py` & `pycyclops-0.2.6/cyclops/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/common.py` & `pycyclops-0.2.6/cyclops/utils/common.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/file.py` & `pycyclops-0.2.6/cyclops/utils/file.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/index.py` & `pycyclops-0.2.6/cyclops/utils/index.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/log.py` & `pycyclops-0.2.6/cyclops/utils/log.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/optional.py` & `pycyclops-0.2.6/cyclops/utils/optional.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/plot.py` & `pycyclops-0.2.6/cyclops/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/cyclops/utils/profile.py` & `pycyclops-0.2.6/cyclops/utils/profile.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.5/pyproject.toml` & `pycyclops-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "pycyclops"
-version = "0.2.5"
+version = "0.2.6"
 description = "Framework for healthcare ML implementation"
 authors = ["Vector AI Engineering <cyclops@vectorinstitute.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/VectorInstitute/cyclops"
 documentation = "https://vectorinstitute.github.io/cyclops/"
 packages = [
     { include = "cyclops" },
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pandas = "^2.0"
 numpy = "^1.24.0"
-scikit-learn = "^1.2.2"
+scikit-learn = "^1.4.0"
 scipy = "^1.11.0"
+matplotlib = "^3.8.3"
 datasets = "^2.15.0"
 psutil = "^5.9.4"
 pyarrow = "^14.0.0"
 pydantic = "^1.10.11"
 Jinja2 = "^3.1.3"
 spdx-tools = "^0.8.1"
 pybtex = "^0.24.0"
 kaleido = "0.2.1"
 scour = "^0.38.2"
 plotly = "^5.7.0"
 pillow = "^10.0.0"
-array-api-compat = "1.4"
+array-api-compat = "1.6"
 hydra-core = "^1.2.0"
 
 # Optional dependencies
 monai = { version = "^1.3.0", extras = ["itk"], optional = true }
 torch = { version = "^1.11.0", optional = true }
 torchvision = { version = "^0.14.0", optional = true }
 torchxrayvision = { version = "^1.2.0", optional = true }
@@ -124,31 +125,30 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 cycquery = "^0.1.0"
 seaborn = "^0.11.2"
-matplotlib = "^3.5.1"
 jupyter = "^1.0.0"
 jupyterlab = "^3.4.2"
 ipympl = "^0.9.3"
 ipywidgets = "^8.0.6"
 torchmetrics = {version = "^1.2.0", extras = ["classification", "regression"]}
 cupy = "^12.2.0"
 mpi4py = {git = "https://github.com/mpi4py/mpi4py"}
-lightning = "^2.1.0"
-imbalanced-learn = "^0.11.0"
+imbalanced-learn = "^0.12.0"
+pyperf = "^2.6.3"
 
 [tool.poetry.group.deploy]
 optional = true
 
 [tool.poetry.group.deploy.dependencies]
 aiohttp = "^3.9.2"
-bentoml = { version = "^1.2.4", extras = ["triton"] }
+bentoml = { version = "1.2.0", extras = ["triton"] }
 torchxrayvision = "^1.2.1"
 kaggle = "^1.5.13"
 onnx = "^1.15.0"
 skl2onnx = "^1.16.0"
 
 [tool.poetry.extras]
 torch = ["torch"]
```

### Comparing `pycyclops-0.2.5/PKG-INFO` & `pycyclops-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyclops
-Version: 0.2.5
+Version: 0.2.6
 Summary: Framework for healthcare ML implementation
 Home-page: https://github.com/VectorInstitute/cyclops
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: cyclops@vectorinstitute.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,29 +19,30 @@
 Provides-Extra: torch
 Provides-Extra: torchvision
 Provides-Extra: torchxrayvision
 Provides-Extra: xgboost
 Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: alibi-detect[torch] (>=0.11.0,<0.12.0) ; extra == "alibi-detect" or extra == "all"
 Requires-Dist: alibi[shap] (>=0.9.4,<0.10.0) ; extra == "alibi" or extra == "all"
-Requires-Dist: array-api-compat (==1.4)
+Requires-Dist: array-api-compat (==1.6)
 Requires-Dist: datasets (>=2.15.0,<3.0.0)
 Requires-Dist: hydra-core (>=1.2.0,<2.0.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: llvmlite (>=0.40.0,<0.41.0) ; extra == "alibi" or extra == "alibi-detect" or extra == "all"
+Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: monai[itk] (>=1.3.0,<2.0.0) ; extra == "monai" or extra == "all"
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: plotly (>=5.7.0,<6.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
 Requires-Dist: pybtex (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
 Requires-Dist: scipy (>=1.11.0,<2.0.0)
 Requires-Dist: scour (>=0.38.2,<0.39.0)
 Requires-Dist: spdx-tools (>=0.8.1,<0.9.0)
 Requires-Dist: torch (>=1.11.0,<2.0.0) ; extra == "torch" or extra == "torchxrayvision" or extra == "monai" or extra == "alibi-detect" or extra == "all"
 Requires-Dist: torchvision (>=0.14.0,<0.15.0) ; extra == "torchvision" or extra == "all"
 Requires-Dist: torchxrayvision (>=1.2.0,<2.0.0) ; extra == "torchxrayvision" or extra == "all"
 Requires-Dist: xgboost (>=1.5.2,<2.0.0) ; extra == "xgboost" or extra == "all"
```

