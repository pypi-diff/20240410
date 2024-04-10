# Comparing `tmp/apax-0.3.0.tar.gz` & `tmp/apax-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apax-0.3.0.tar", max compression
+gzip compressed data, was "apax-0.4.0.tar", max compression
```

## Comparing `apax-0.3.0.tar` & `apax-0.4.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1089 2024-04-08 13:35:11.000000 apax-0.3.0/LICENSE
--rw-r--r--   0        0        0     4360 2024-04-10 14:48:13.000000 apax-0.3.0/README.md
--rw-r--r--   0        0        0      214 2024-04-08 13:39:05.000000 apax-0.3.0/apax/__init__.py
--rw-r--r--   0        0        0       74 2023-10-04 12:28:17.000000 apax-0.3.0/apax/bal/__init__.py
--rw-r--r--   0        0        0     5051 2024-04-10 14:48:13.000000 apax-0.3.0/apax/bal/api.py
--rw-r--r--   0        0        0     2852 2024-04-10 14:48:13.000000 apax-0.3.0/apax/bal/feature_maps.py
--rw-r--r--   0        0        0      770 2023-10-04 12:28:17.000000 apax-0.3.0/apax/bal/kernel.py
--rw-r--r--   0        0        0     1267 2024-04-10 14:48:13.000000 apax-0.3.0/apax/bal/selection.py
--rw-r--r--   0        0        0     1154 2024-04-10 14:48:13.000000 apax-0.3.0/apax/bal/transforms.py
--rw-r--r--   0        0        0        0 2024-04-08 13:35:11.000000 apax-0.3.0/apax/cli/__init__.py
--rw-r--r--   0        0        0     7653 2024-04-08 13:39:05.000000 apax-0.3.0/apax/cli/apax_app.py
--rw-r--r--   0        0        0        0 2024-04-08 13:35:11.000000 apax-0.3.0/apax/cli/templates/__init__.py
--rw-r--r--   0        0        0      481 2024-04-10 15:40:31.000000 apax-0.3.0/apax/cli/templates/md_config_minimal.yaml
--rw-r--r--   0        0        0     1565 2024-04-10 15:40:31.000000 apax-0.3.0/apax/cli/templates/train_config_full.yaml
--rw-r--r--   0        0        0      319 2023-09-15 10:49:47.000000 apax-0.3.0/apax/cli/templates/train_config_minimal.yaml
--rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.3.0/apax/config/__init__.py
--rw-r--r--   0        0        0      402 2023-09-18 15:23:15.000000 apax-0.3.0/apax/config/__init__.pyi
--rw-r--r--   0        0        0     1488 2024-04-10 15:40:31.000000 apax-0.3.0/apax/config/common.py
--rw-r--r--   0        0        0     4951 2024-04-10 15:40:31.000000 apax-0.3.0/apax/config/md_config.py
--rw-r--r--   0        0        0    14278 2024-04-10 15:40:31.000000 apax-0.3.0/apax/config/train_config.py
--rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.3.0/apax/data/__init__.py
--rw-r--r--   0        0        0      121 2023-06-14 20:43:10.000000 apax-0.3.0/apax/data/__init__.pyi
--rw-r--r--   0        0        0     1479 2024-04-10 15:40:31.000000 apax-0.3.0/apax/data/initialization.py
--rw-r--r--   0        0        0    11188 2024-04-10 15:40:31.000000 apax-0.3.0/apax/data/input_pipeline.py
--rw-r--r--   0        0        0     3239 2024-04-10 15:40:31.000000 apax-0.3.0/apax/data/preprocessing.py
--rw-r--r--   0        0        0     5512 2024-04-08 13:39:05.000000 apax-0.3.0/apax/data/statistics.py
--rw-r--r--   0        0        0      133 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/__init__.py
--rw-r--r--   0        0        0       89 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/activation.py
--rw-r--r--   0        0        0      127 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/descriptor/__init__.py
--rw-r--r--   0        0        0     3318 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/descriptor/basis_functions.py
--rw-r--r--   0        0        0     3998 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/descriptor/gaussian_moment_descriptor.py
--rw-r--r--   0        0        0     1127 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/descriptor/moments.py
--rw-r--r--   0        0        0     1326 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/descriptor/triangular_indices.py
--rw-r--r--   0        0        0     2635 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/empirical.py
--rw-r--r--   0        0        0      676 2024-04-08 13:39:05.000000 apax-0.3.0/apax/layers/initializers.py
--rw-r--r--   0        0        0      357 2024-04-08 11:05:45.000000 apax-0.3.0/apax/layers/masking.py
--rw-r--r--   0        0        0     1116 2024-04-08 11:05:45.000000 apax-0.3.0/apax/layers/ntk_linear.py
--rw-r--r--   0        0        0     1145 2024-04-10 14:48:27.000000 apax-0.3.0/apax/layers/properties.py
--rw-r--r--   0        0        0      915 2024-04-10 14:48:13.000000 apax-0.3.0/apax/layers/readout.py
--rw-r--r--   0        0        0     1326 2024-04-08 11:05:45.000000 apax-0.3.0/apax/layers/scaling.py
--rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.3.0/apax/md/__init__.py
--rw-r--r--   0        0        0       99 2023-06-14 20:43:10.000000 apax-0.3.0/apax/md/__init__.pyi
--rw-r--r--   0        0        0    13218 2024-04-10 15:40:31.000000 apax-0.3.0/apax/md/ase_calc.py
--rw-r--r--   0        0        0     2807 2024-04-10 15:40:31.000000 apax-0.3.0/apax/md/function_transformations.py
--rw-r--r--   0        0        0     3788 2024-04-08 13:39:05.000000 apax-0.3.0/apax/md/io.py
--rw-r--r--   0        0        0      589 2023-12-27 15:40:25.000000 apax-0.3.0/apax/md/md_checkpoint.py
--rw-r--r--   0        0        0    13504 2024-04-10 15:40:31.000000 apax-0.3.0/apax/md/nvt.py
--rw-r--r--   0        0        0     1128 2024-04-08 13:39:05.000000 apax-0.3.0/apax/md/sim_utils.py
--rw-r--r--   0        0        0       97 2024-04-10 14:48:13.000000 apax-0.3.0/apax/model/__init__.py
--rw-r--r--   0        0        0      189 2023-06-19 10:07:44.000000 apax-0.3.0/apax/model/__init__.pyi
--rw-r--r--   0        0        0     3818 2024-04-10 14:48:27.000000 apax-0.3.0/apax/model/builder.py
--rw-r--r--   0        0        0     5357 2024-04-10 14:48:27.000000 apax-0.3.0/apax/model/gmnn.py
--rw-r--r--   0        0        0      113 2024-04-09 11:07:12.000000 apax-0.3.0/apax/nodes/__init__.py
--rw-r--r--   0        0        0     2405 2024-04-10 15:40:31.000000 apax-0.3.0/apax/nodes/md.py
--rw-r--r--   0        0        0     4622 2024-04-10 15:40:31.000000 apax-0.3.0/apax/nodes/model.py
--rw-r--r--   0        0        0      777 2024-04-09 11:07:12.000000 apax-0.3.0/apax/nodes/utils.py
--rw-r--r--   0        0        0       72 2023-06-01 09:13:14.000000 apax-0.3.0/apax/optimizer/__init__.py
--rw-r--r--   0        0        0     2848 2024-01-08 21:00:06.000000 apax-0.3.0/apax/optimizer/get_optimizer.py
--rw-r--r--   0        0        0      163 2023-11-23 08:20:22.000000 apax-0.3.0/apax/train/__init__.py
--rw-r--r--   0        0        0      178 2023-06-14 20:43:10.000000 apax-0.3.0/apax/train/__init__.pyi
--rw-r--r--   0        0        0     3645 2024-04-10 15:40:31.000000 apax-0.3.0/apax/train/callbacks.py
--rw-r--r--   0        0        0     6467 2024-03-27 12:52:22.000000 apax-0.3.0/apax/train/checkpoints.py
--rw-r--r--   0        0        0     5736 2024-04-10 15:40:31.000000 apax-0.3.0/apax/train/eval.py
--rw-r--r--   0        0        0     4564 2024-04-08 13:39:05.000000 apax-0.3.0/apax/train/loss.py
--rw-r--r--   0        0        0     2775 2024-03-27 12:52:29.000000 apax-0.3.0/apax/train/metrics.py
--rw-r--r--   0        0        0     6291 2024-04-10 15:40:31.000000 apax-0.3.0/apax/train/run.py
--rw-r--r--   0        0        0    10236 2024-04-10 15:40:31.000000 apax-0.3.0/apax/train/trainer.py
--rw-r--r--   0        0        0      178 2024-03-27 12:52:34.000000 apax-0.3.0/apax/transfer_learning/__init__.py
--rw-r--r--   0        0        0     1135 2024-03-27 12:52:35.000000 apax-0.3.0/apax/transfer_learning/parameter_transfer.py
--rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.3.0/apax/utils/__init__.py
--rw-r--r--   0        0        0      145 2024-04-10 14:48:13.000000 apax-0.3.0/apax/utils/__init__.pyi
--rw-r--r--   0        0        0     4283 2024-04-09 11:07:12.000000 apax-0.3.0/apax/utils/convert.py
--rw-r--r--   0        0        0     3093 2024-04-10 15:40:31.000000 apax-0.3.0/apax/utils/data.py
--rw-r--r--   0        0        0     3088 2024-04-10 14:48:27.000000 apax-0.3.0/apax/utils/datasets.py
--rw-r--r--   0        0        0     1464 2024-04-10 14:48:27.000000 apax-0.3.0/apax/utils/helpers.py
--rw-r--r--   0        0        0      726 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/README.md
--rw-r--r--   0        0        0      222 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/__init__.py
--rw-r--r--   0        0        0     2548 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/dataclasses.py
--rw-r--r--   0        0        0    31390 2024-04-10 15:40:31.000000 apax-0.3.0/apax/utils/jax_md_reduced/partition.py
--rw-r--r--   0        0        0    26600 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/quantity.py
--rw-r--r--   0        0        0    62016 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/simulate.py
--rw-r--r--   0        0        0    37595 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/smap.py
--rw-r--r--   0        0        0    11931 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/space.py
--rw-r--r--   0        0        0     2864 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/jax_md_reduced/util.py
--rw-r--r--   0        0        0      702 2024-04-08 13:39:05.000000 apax-0.3.0/apax/utils/math.py
--rw-r--r--   0        0        0      170 2024-03-27 12:52:42.000000 apax-0.3.0/apax/utils/random.py
--rw-r--r--   0        0        0     1935 2024-04-10 16:01:53.000000 apax-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 apax-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-08 13:35:11.000000 apax-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4360 2024-04-10 21:06:48.377449 apax-0.4.0/README.md
+-rw-r--r--   0        0        0      214 2024-04-10 21:06:48.377449 apax-0.4.0/apax/__init__.py
+-rw-r--r--   0        0        0       74 2023-10-04 12:28:17.000000 apax-0.4.0/apax/bal/__init__.py
+-rw-r--r--   0        0        0     5053 2024-04-10 21:06:48.377449 apax-0.4.0/apax/bal/api.py
+-rw-r--r--   0        0        0     2852 2024-04-10 21:06:48.377449 apax-0.4.0/apax/bal/feature_maps.py
+-rw-r--r--   0        0        0      770 2023-10-04 12:28:17.000000 apax-0.4.0/apax/bal/kernel.py
+-rw-r--r--   0        0        0     1267 2024-04-10 21:06:48.377449 apax-0.4.0/apax/bal/selection.py
+-rw-r--r--   0        0        0     1154 2024-04-10 21:06:48.377449 apax-0.4.0/apax/bal/transforms.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:35:11.000000 apax-0.4.0/apax/cli/__init__.py
+-rw-r--r--   0        0        0     7653 2024-04-10 21:06:48.377449 apax-0.4.0/apax/cli/apax_app.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:35:11.000000 apax-0.4.0/apax/cli/templates/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-10 21:06:48.377449 apax-0.4.0/apax/cli/templates/md_config_minimal.yaml
+-rw-r--r--   0        0        0     1565 2024-04-10 21:06:48.377449 apax-0.4.0/apax/cli/templates/train_config_full.yaml
+-rw-r--r--   0        0        0      319 2023-09-15 10:49:47.000000 apax-0.4.0/apax/cli/templates/train_config_minimal.yaml
+-rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.4.0/apax/config/__init__.py
+-rw-r--r--   0        0        0      402 2023-09-18 15:23:15.000000 apax-0.4.0/apax/config/__init__.pyi
+-rw-r--r--   0        0        0     1488 2024-04-10 21:06:48.377449 apax-0.4.0/apax/config/common.py
+-rw-r--r--   0        0        0     4951 2024-04-10 21:06:48.377449 apax-0.4.0/apax/config/md_config.py
+-rw-r--r--   0        0        0    14279 2024-04-10 21:06:48.377449 apax-0.4.0/apax/config/train_config.py
+-rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.4.0/apax/data/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-14 20:43:10.000000 apax-0.4.0/apax/data/__init__.pyi
+-rw-r--r--   0        0        0     1479 2024-04-10 21:06:48.377449 apax-0.4.0/apax/data/initialization.py
+-rw-r--r--   0        0        0    11189 2024-04-10 21:06:48.377449 apax-0.4.0/apax/data/input_pipeline.py
+-rw-r--r--   0        0        0     3239 2024-04-10 21:06:48.377449 apax-0.4.0/apax/data/preprocessing.py
+-rw-r--r--   0        0        0     5512 2024-04-10 21:06:48.377449 apax-0.4.0/apax/data/statistics.py
+-rw-r--r--   0        0        0      133 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/activation.py
+-rw-r--r--   0        0        0      127 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/descriptor/__init__.py
+-rw-r--r--   0        0        0     3318 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/descriptor/basis_functions.py
+-rw-r--r--   0        0        0     3998 2024-04-10 21:06:48.377449 apax-0.4.0/apax/layers/descriptor/gaussian_moment_descriptor.py
+-rw-r--r--   0        0        0     1127 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/descriptor/moments.py
+-rw-r--r--   0        0        0     1326 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/descriptor/triangular_indices.py
+-rw-r--r--   0        0        0     2635 2024-04-10 21:06:48.377449 apax-0.4.0/apax/layers/empirical.py
+-rw-r--r--   0        0        0      676 2024-04-10 21:06:48.377449 apax-0.4.0/apax/layers/initializers.py
+-rw-r--r--   0        0        0      357 2024-04-08 11:05:45.000000 apax-0.4.0/apax/layers/masking.py
+-rw-r--r--   0        0        0     1116 2024-04-08 11:05:45.000000 apax-0.4.0/apax/layers/ntk_linear.py
+-rw-r--r--   0        0        0     1145 2024-04-10 21:06:48.377449 apax-0.4.0/apax/layers/properties.py
+-rw-r--r--   0        0        0      915 2024-04-10 14:48:13.000000 apax-0.4.0/apax/layers/readout.py
+-rw-r--r--   0        0        0     1326 2024-04-08 11:05:45.000000 apax-0.4.0/apax/layers/scaling.py
+-rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.4.0/apax/md/__init__.py
+-rw-r--r--   0        0        0       99 2023-06-14 20:43:10.000000 apax-0.4.0/apax/md/__init__.pyi
+-rw-r--r--   0        0        0    13217 2024-04-10 21:06:48.377449 apax-0.4.0/apax/md/ase_calc.py
+-rw-r--r--   0        0        0     2807 2024-04-10 21:06:48.377449 apax-0.4.0/apax/md/function_transformations.py
+-rw-r--r--   0        0        0     3788 2024-04-10 21:06:48.377449 apax-0.4.0/apax/md/io.py
+-rw-r--r--   0        0        0      589 2023-12-27 15:40:25.000000 apax-0.4.0/apax/md/md_checkpoint.py
+-rw-r--r--   0        0        0    13504 2024-04-10 21:06:48.377449 apax-0.4.0/apax/md/nvt.py
+-rw-r--r--   0        0        0     1128 2024-04-10 21:06:48.377449 apax-0.4.0/apax/md/sim_utils.py
+-rw-r--r--   0        0        0       97 2024-04-10 14:48:13.000000 apax-0.4.0/apax/model/__init__.py
+-rw-r--r--   0        0        0      189 2023-06-19 10:07:44.000000 apax-0.4.0/apax/model/__init__.pyi
+-rw-r--r--   0        0        0     3818 2024-04-10 21:06:48.377449 apax-0.4.0/apax/model/builder.py
+-rw-r--r--   0        0        0     5357 2024-04-10 21:06:48.377449 apax-0.4.0/apax/model/gmnn.py
+-rw-r--r--   0        0        0      113 2024-04-09 11:07:12.000000 apax-0.4.0/apax/nodes/__init__.py
+-rw-r--r--   0        0        0     2405 2024-04-10 21:06:48.377449 apax-0.4.0/apax/nodes/md.py
+-rw-r--r--   0        0        0     4622 2024-04-10 21:06:48.377449 apax-0.4.0/apax/nodes/model.py
+-rw-r--r--   0        0        0      777 2024-04-09 11:07:12.000000 apax-0.4.0/apax/nodes/utils.py
+-rw-r--r--   0        0        0       72 2023-06-01 09:13:14.000000 apax-0.4.0/apax/optimizer/__init__.py
+-rw-r--r--   0        0        0     2848 2024-01-08 21:00:06.000000 apax-0.4.0/apax/optimizer/get_optimizer.py
+-rw-r--r--   0        0        0      163 2023-11-23 08:20:22.000000 apax-0.4.0/apax/train/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-14 20:43:10.000000 apax-0.4.0/apax/train/__init__.pyi
+-rw-r--r--   0        0        0     3645 2024-04-10 21:06:48.377449 apax-0.4.0/apax/train/callbacks.py
+-rw-r--r--   0        0        0     6467 2024-03-27 12:52:22.000000 apax-0.4.0/apax/train/checkpoints.py
+-rw-r--r--   0        0        0     5736 2024-04-10 21:06:48.377449 apax-0.4.0/apax/train/eval.py
+-rw-r--r--   0        0        0     4564 2024-04-10 21:06:48.377449 apax-0.4.0/apax/train/loss.py
+-rw-r--r--   0        0        0     2775 2024-03-27 12:52:29.000000 apax-0.4.0/apax/train/metrics.py
+-rw-r--r--   0        0        0     6290 2024-04-10 21:06:48.377449 apax-0.4.0/apax/train/run.py
+-rw-r--r--   0        0        0    10236 2024-04-10 21:06:48.377449 apax-0.4.0/apax/train/trainer.py
+-rw-r--r--   0        0        0      178 2024-03-27 12:52:34.000000 apax-0.4.0/apax/transfer_learning/__init__.py
+-rw-r--r--   0        0        0     1135 2024-03-27 12:52:35.000000 apax-0.4.0/apax/transfer_learning/parameter_transfer.py
+-rw-r--r--   0        0        0       97 2024-04-08 13:35:11.000000 apax-0.4.0/apax/utils/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/__init__.pyi
+-rw-r--r--   0        0        0     4283 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/convert.py
+-rw-r--r--   0        0        0     3093 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/data.py
+-rw-r--r--   0        0        0     3088 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/datasets.py
+-rw-r--r--   0        0        0     1464 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/helpers.py
+-rw-r--r--   0        0        0      726 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/jax_md_reduced/README.md
+-rw-r--r--   0        0        0      222 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/jax_md_reduced/__init__.py
+-rw-r--r--   0        0        0     2548 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/jax_md_reduced/dataclasses.py
+-rw-r--r--   0        0        0    31392 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/jax_md_reduced/partition.py
+-rw-r--r--   0        0        0    26600 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/jax_md_reduced/quantity.py
+-rw-r--r--   0        0        0    62016 2024-04-10 21:06:48.377449 apax-0.4.0/apax/utils/jax_md_reduced/simulate.py
+-rw-r--r--   0        0        0    37596 2024-04-10 21:06:48.381450 apax-0.4.0/apax/utils/jax_md_reduced/smap.py
+-rw-r--r--   0        0        0    11931 2024-04-10 21:06:48.381450 apax-0.4.0/apax/utils/jax_md_reduced/space.py
+-rw-r--r--   0        0        0     2864 2024-04-10 21:06:48.381450 apax-0.4.0/apax/utils/jax_md_reduced/util.py
+-rw-r--r--   0        0        0      702 2024-04-10 21:06:48.381450 apax-0.4.0/apax/utils/math.py
+-rw-r--r--   0        0        0      170 2024-03-27 12:52:42.000000 apax-0.4.0/apax/utils/random.py
+-rw-r--r--   0        0        0     1935 2024-04-10 21:06:48.385450 apax-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 apax-0.4.0/PKG-INFO
```

### Comparing `apax-0.3.0/LICENSE` & `apax-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/README.md` & `apax-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/bal/api.py` & `apax-0.4.0/apax/bal/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,17 @@
     pool_atoms: List[Atoms]
         List of `ase.Atoms` to select new data from.
     base_fm_options:
         Settings for the base feature map.
     selection_method:
         Currently only "max_dist" is supported.
     feature_transforms:
-        Feature tranforms to be applied on top of the
+        Feature transforms to be applied on top of the
         base feature map transform.
-        Examples would include multiplcation with or addition of a constant.
+        Examples would include multiplication with or addition of a constant.
     selection_batch_size:
         Amount of new data points to be selected from `pool_atoms`.
     processing_batch_size:
         Amount of data points to compute the features for at once.
         Does not effect results, just the speed of processing.
     """
     selection_fn = {
```

### Comparing `apax-0.3.0/apax/bal/feature_maps.py` & `apax-0.4.0/apax/bal/feature_maps.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/bal/kernel.py` & `apax-0.4.0/apax/bal/kernel.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/bal/selection.py` & `apax-0.4.0/apax/bal/selection.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/bal/transforms.py` & `apax-0.4.0/apax/bal/transforms.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/cli/apax_app.py` & `apax-0.4.0/apax/cli/apax_app.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/cli/templates/train_config_full.yaml` & `apax-0.4.0/apax/cli/templates/train_config_full.yaml`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/config/common.py` & `apax-0.4.0/apax/config/common.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/config/md_config.py` & `apax-0.4.0/apax/config/md_config.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/config/train_config.py` & `apax-0.4.0/apax/config/train_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
     ckpt_interval: PositiveInt = 1
     base_model_checkpoint: Optional[str] = None
     reset_layers: List[str] = []
 
 
 class Config(BaseModel, frozen=True, extra="forbid"):
     """
-    Main configuration of a apax training run. Parameter that are cofig classes will
+    Main configuration of a apax training run. Parameter that are config classes will
     be generated by parsing the config.yaml file and are specified
     as shown :ref:`here <train_config>`:
 
     Example
     -------
     .. code-block:: yaml
 
@@ -381,15 +381,15 @@
         | Number of epochs without improvement before trainings gets terminated.
     seed : int, default = 1
         | Random seed.
     n_models : int, default = 1
         | Number of models to be trained at once.
     n_jitted_steps : int, default = 1
         | Number of train batches to be processed in a compiled loop.
-        | Can yield singificant speedups for small structures or small batch sizes.
+        | Can yield significant speedups for small structures or small batch sizes.
     data : :class:`.DataConfig`
         | Data configuration.
     model : :class:`.ModelConfig`
         | Model configuration.
     metrics : List of :class:`.MetricsConfig`
         | Metrics configuration.
     loss : List of :class:`.LossConfig`
```

### Comparing `apax-0.3.0/apax/data/initialization.py` & `apax-0.4.0/apax/data/initialization.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/data/input_pipeline.py` & `apax-0.4.0/apax/data/input_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from apax.utils.convert import atoms_to_inputs, atoms_to_labels, unit_dict
 
 log = logging.getLogger(__name__)
 
 
 def pad_nl(idx, offsets, max_neighbors):
     """
-    Pad the neighbor list arrays to the maximal number of neighbors occuring.
+    Pad the neighbor list arrays to the maximal number of neighbors occurring.
 
     Parameters
     ----------
     idx : np.ndarray
         Neighbor indices array.
     offsets : np.ndarray
         Offset array.
```

### Comparing `apax-0.3.0/apax/data/preprocessing.py` & `apax-0.4.0/apax/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/data/statistics.py` & `apax-0.4.0/apax/data/statistics.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/descriptor/basis_functions.py` & `apax-0.4.0/apax/layers/descriptor/basis_functions.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/descriptor/gaussian_moment_descriptor.py` & `apax-0.4.0/apax/layers/descriptor/gaussian_moment_descriptor.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/descriptor/moments.py` & `apax-0.4.0/apax/layers/descriptor/moments.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/descriptor/triangular_indices.py` & `apax-0.4.0/apax/layers/descriptor/triangular_indices.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/empirical.py` & `apax-0.4.0/apax/layers/empirical.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/initializers.py` & `apax-0.4.0/apax/layers/initializers.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/ntk_linear.py` & `apax-0.4.0/apax/layers/ntk_linear.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/properties.py` & `apax-0.4.0/apax/layers/properties.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/readout.py` & `apax-0.4.0/apax/layers/readout.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/layers/scaling.py` & `apax-0.4.0/apax/layers/scaling.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/md/ase_calc.py` & `apax-0.4.0/apax/md/ase_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
                 inputs["idx"],
                 inputs["box"],
                 inputs["offsets"],
             )
             unpadded_results = unpack_results(results, inputs)
 
             # for the last batch, the number of structures may be less
-            # than the batch_size,  which is why we check this explicitely
+            # than the batch_size,  which is why we check this explicitly
             num_strucutres_in_batch = results["energy"].shape[0]
             for j in range(num_strucutres_in_batch):
                 atoms = atoms_list[i].copy()
                 atoms.calc = SinglePointCalculator(atoms=atoms, **unpadded_results[j])
                 evaluated_atoms_list.append(atoms)
             pbar.update(batch_size)
         pbar.close()
```

### Comparing `apax-0.3.0/apax/md/function_transformations.py` & `apax-0.4.0/apax/md/function_transformations.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/md/io.py` & `apax-0.4.0/apax/md/io.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/md/md_checkpoint.py` & `apax-0.4.0/apax/md/md_checkpoint.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/md/nvt.py` & `apax-0.4.0/apax/md/nvt.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/md/sim_utils.py` & `apax-0.4.0/apax/md/sim_utils.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/model/builder.py` & `apax-0.4.0/apax/model/builder.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/model/gmnn.py` & `apax-0.4.0/apax/model/gmnn.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/nodes/md.py` & `apax-0.4.0/apax/nodes/md.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/nodes/model.py` & `apax-0.4.0/apax/nodes/model.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/nodes/utils.py` & `apax-0.4.0/apax/nodes/utils.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/optimizer/get_optimizer.py` & `apax-0.4.0/apax/optimizer/get_optimizer.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/train/callbacks.py` & `apax-0.4.0/apax/train/callbacks.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/train/checkpoints.py` & `apax-0.4.0/apax/train/checkpoints.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/train/eval.py` & `apax-0.4.0/apax/train/eval.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/train/loss.py` & `apax-0.4.0/apax/train/loss.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/train/metrics.py` & `apax-0.4.0/apax/train/metrics.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/train/run.py` & `apax-0.4.0/apax/train/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 def run(user_config: Union[str, os.PathLike, dict], log_level="error"):
     """
     Starts the training of a model with parameters provided by a the config.
 
     Parameters
     ----------
     user_config : str | os.PathLike | dict
-        training config full exmaple can be finde :ref:`here <train_config>`:
+        training config full example can be find :ref:`here <train_config>`:
 
     """
     config = parse_config(user_config)
 
     seed_py_np_tf(config.seed)
     rng_key = jax.random.PRNGKey(config.seed)
```

### Comparing `apax-0.3.0/apax/train/trainer.py` & `apax-0.4.0/apax/train/trainer.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/transfer_learning/parameter_transfer.py` & `apax-0.4.0/apax/transfer_learning/parameter_transfer.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/convert.py` & `apax-0.4.0/apax/utils/convert.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/data.py` & `apax-0.4.0/apax/utils/data.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/datasets.py` & `apax-0.4.0/apax/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/helpers.py` & `apax-0.4.0/apax/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/README.md` & `apax-0.4.0/apax/utils/jax_md_reduced/README.md`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/dataclasses.py` & `apax-0.4.0/apax/utils/jax_md_reduced/dataclasses.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/partition.py` & `apax-0.4.0/apax/utils/jax_md_reduced/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         cl_data = (self.cell_capacity, self.did_buffer_overflow, self.update_fn)
         return self.update_fn(position, cl_data, **kwargs)
 
     @property
     def kwarg_buffers(self):
         logging.warning(
             "kwarg_buffers renamed to named_buffer. The name "
-            "kwarg_buffers will be depricated."
+            "kwarg_buffers will be deprecated."
         )
         return self.named_buffer
 
 
 class PartitionErrorCode(IntEnum):
     """An enum specifying different error codes.
 
@@ -175,15 +175,15 @@
         enough to contain all of the particles. This should indicate that it is
         necessary to allocate a new neighbor list.
       CELL_LIST_OVERFLOW: Indicates that the cell list was not large enough to
         contain all of the particles. This should indicate that it is necessary
         to allocate a new cell list.
       CELL_SIZE_TOO_SMALL: Indicates that the size of cells in a cell list was
         not large enough to properly capture particle interactions. This
-        indicates that it is necessary to allcoate a new cell list with larger
+        indicates that it is necessary to allocate a new cell list with larger
         cells.
       MALFORMED_BOX: Indicates that a box matrix was not properly upper
         triangular.
     """
 
     NONE = 0
     NEIGHBOR_LIST_OVERFLOW = 1 << 0
@@ -238,15 +238,15 @@
 
     Attributes:
       idx: For an N particle system this is an `[N, max_occupancy]` array of
         integers such that `idx[i, j]` is the j-th neighbor of particle i.
       reference_position: The positions of particles when the neighbor list was
         constructed. This is used to decide whether the neighbor list ought to be
         updated.
-      error: An error code that is used to identify errors that occured during
+      error: An error code that is used to identify errors that occurred during
         neighbor list construction. See `PartitionError` and `PartitionErrorCode`
         for details.
       cell_list_capacity: An optional integer specifying the capacity of the cell
         list used as an intermediate step in the creation of the neighbor list.
       max_occupancy: A static integer specifying the maximum size of the
         neighbor list. Changing this will invoke a recompilation.
       format: A NeighborListFormat enum specifying the format of the neighbor
@@ -313,15 +313,15 @@
 
     Attributes:
       idx: For an N particle system this is an `[N, max_occupancy]` array of
         integers such that `idx[i, j]` is the j-th neighbor of particle i.
       reference_position: The positions of particles when the neighbor list was
         constructed. This is used to decide whether the neighbor list ought to be
         updated.
-      error: An error code that is used to identify errors that occured during
+      error: An error code that is used to identify errors that occurred during
         neighbor list construction. See `PartitionError` and `PartitionErrorCode`
         for details.
       cell_list_capacity: An optional integer specifying the capacity of the cell
         list used as an intermediate step in the creation of the neighbor list.
       max_occupancy: A static integer specifying the maximum size of the
         neighbor list. Changing this will invoke a recompilation.
       format: A NeighborListFormat enum specifying the format of the neighbor
```

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/quantity.py` & `apax-0.4.0/apax/utils/jax_md_reduced/quantity.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/simulate.py` & `apax-0.4.0/apax/utils/jax_md_reduced/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1586,16 +1586,16 @@
     tau: float,
     **sim_kwargs,
 ) -> Simulator:
     """Simulation using the canonical sampling through velocity rescaling (CSVR) thermostat.
 
     Samples from the canonical ensemble in which the number of particles (N),
     the system volume (V), and the temperature (T) are held constant. CSVR
-    algorithmn samples the canonical distribution by rescaling the velocities
-    by a appropritely chosen random factor. At each timestep (dt) the rescaling
+    algorithm samples the canonical distribution by rescaling the velocities
+    by a appropriately chosen random factor. At each timestep (dt) the rescaling
     takes place and the rescaling factor is calculated using
     A7 Bussi et al. [#bussi2007]_. CSVR updates to the velocity are stochastic in
     nature and unlike the Berendsen thermostat it samples the true canonical
     distribution [#Braun2018]_.
 
     Args:
       energy_or_force: A function that produces either an energy or a force from
```

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/smap.py` & `apax-0.4.0/apax/utils/jax_md_reduced/smap.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         specifying parameters for the function. `fn` returns an ndarray of
         evaluations of shape `[n, m, d_out]`.
       metric: A function that takes two ndarray of positions of shape
         `[spatial_dimension]` and `[spatial_dimension]` respectively and returns
         an ndarray of distances or displacements of shape `[]` or `[d_in]`
         respectively. The metric can optionally take a floating point time as a
         third argument.
-      static_bonds: An ndarray of integer pairs wth shape `[b, 2]` where each
+      static_bonds: An ndarray of integer pairs with shape `[b, 2]` where each
         pair specifies a bond. `static_bonds` are baked into the returned compute
         function statically and cannot be changed after the fact.
       static_bond_types: An ndarray of integers of shape `[b]` specifying the
         type of each bond. Only specify bond types if you want to specify bond
         parameters by type. One can also specify constant or per-bond parameters
         (see below).
       ignore_unused_parameters: A boolean that denotes whether dynamically
```

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/space.py` & `apax-0.4.0/apax/utils/jax_md_reduced/space.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/jax_md_reduced/util.py` & `apax-0.4.0/apax/utils/jax_md_reduced/util.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/apax/utils/math.py` & `apax-0.4.0/apax/utils/math.py`

 * *Files identical despite different names*

### Comparing `apax-0.3.0/pyproject.toml` & `apax-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apax"
-version = "0.3.0"
+version = "0.4.0"
 description = "Atomistic Learned Potential Package in JAX"
 authors = ["Moritz René Schäfer <schaefer@theochem.uni-stuttgart.de>", "Nico Segreto <segreto@theochem.uni-stuttgart.de>"]
 keywords=["machine-learning", "interatomic potentials", "molecular-dynamics"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "apax"}]
 documentation = "https://apax.readthedocs.io/en/latest/"
```

### Comparing `apax-0.3.0/PKG-INFO` & `apax-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apax
-Version: 0.3.0
+Version: 0.4.0
 Summary: Atomistic Learned Potential Package in JAX
 License: MIT
 Keywords: machine-learning,interatomic potentials,molecular-dynamics
 Author: Moritz René Schäfer
 Author-email: schaefer@theochem.uni-stuttgart.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

