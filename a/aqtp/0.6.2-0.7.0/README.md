# Comparing `tmp/aqtp-0.6.2.tar.gz` & `tmp/aqtp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtp-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aqtp-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aqtp-0.6.2.tar` & `aqtp-0.7.0.tar`

### file list

```diff
@@ -1,263 +1,268 @@
--rw-r--r--   0        0        0       39 2024-02-07 19:51:57.211826 aqtp-0.6.2/.gitignore
--rw-r--r--   0        0        0      107 2024-02-07 19:51:57.211826 aqtp-0.6.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2024-02-07 19:51:57.211826 aqtp-0.6.2/LICENSE
--rw-r--r--   0        0        0    15432 2024-02-07 19:51:57.211826 aqtp-0.6.2/README.md
--rw-r--r--   0        0        0      641 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/__init__.py
--rw-r--r--   0        0        0      576 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/common/__init__.py
--rw-r--r--   0        0        0     4354 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/common/aqt_common.py
--rw-r--r--   0        0        0    16011 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/common/aqt_config.py
--rw-r--r--   0        0        0    13928 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/common/aqt_config_schedule_test.py
--rw-r--r--   0        0        0     5177 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/common/aqt_config_utils.py
--rw-r--r--   0        0        0    15655 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/common/emulated_floating_points.py
--rw-r--r--   0        0        0     5730 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/common/emulation_utils.py
--rw-r--r--   0        0        0    37847 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/g3doc/AQT favicon.png
--rw-r--r--   0        0        0    23437 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/g3doc/AQT logo.png
--rw-r--r--   0        0        0     1360 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/g3doc/aqt_development.md
--rw-r--r--   0        0        0     5938 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/g3doc/index.md
--rw-r--r--   0        0        0      381 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/g3doc/sitemap.md
--rw-r--r--   0        0        0      576 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/__init__.py
--rw-r--r--   0        0        0    13641 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_conv_general.py
--rw-r--r--   0        0        0    12151 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_conv_general_test.py
--rw-r--r--   0        0        0     8861 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_dot_general.py
--rw-r--r--   0        0        0    14977 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_dot_general_test.py
--rw-r--r--   0        0        0     3783 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_matmul.py
--rw-r--r--   0        0        0     3293 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_matmul_test.py
--rw-r--r--   0        0        0     1083 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_ops.py
--rw-r--r--   0        0        0    18180 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/aqt_tensor.py
--rw-r--r--   0        0        0     4751 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_tensor_test.py
--rw-r--r--   0        0        0     2705 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/aqt_utils.py
--rw-r--r--   0        0        0     4646 2024-03-11 23:38:05.874320 aqtp-0.6.2/aqt/jax/v2/aqt_conv_general.py
--rw-r--r--   0        0        0    28840 2024-03-12 00:31:18.035091 aqtp-0.6.2/aqt/jax/v2/aqt_dot_general.py
--rw-r--r--   0        0        0    37063 2024-03-11 23:38:05.874320 aqtp-0.6.2/aqt/jax/v2/aqt_dot_general_test.py
--rw-r--r--   0        0        0     4298 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/v2/aqt_quantizer.py
--rw-r--r--   0        0        0     9272 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/v2/aqt_tensor.py
--rw-r--r--   0        0        0     2568 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/v2/aqt_tensor_test.py
--rw-r--r--   0        0        0     2125 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/calibration.py
--rw-r--r--   0        0        0    19336 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/config.py
--rw-r--r--   0        0        0    29359 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/config_test.py
--rw-r--r--   0        0        0     5550 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax/v2/examples/examples.ipynb
--rw-r--r--   0        0        0     9645 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/v2/examples/flax_e2e_model.py
--rw-r--r--   0        0        0     8844 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/v2/examples/flax_e2e_model_test.py
--rw-r--r--   0        0        0    13367 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/v2/flax/aqt_flax.py
--rw-r--r--   0        0        0     4125 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/flax/aqt_flax_test.py
--rw-r--r--   0        0        0      906 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax/v2/flax/utils.py
--rw-r--r--   0        0        0     2680 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/numerics/fp8_numerics.py
--rw-r--r--   0        0        0     4887 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/numerics/fp8_numerics_test.py
--rw-r--r--   0        0        0     4451 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/numerics/int_numerics.py
--rw-r--r--   0        0        0     1426 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax/v2/numerics/no_numerics.py
--rw-r--r--   0        0        0     1338 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax/v2/numerics/numerics.py
--rw-r--r--   0        0        0     2030 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax/v2/pax/pax_base_ops.py
--rw-r--r--   0        0        0     2095 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/pax/pax_base_ops_test.py
--rw-r--r--   0        0        0     1846 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/stochastic_rounding.py
--rw-r--r--   0        0        0    10903 2024-03-12 00:31:18.035091 aqtp-0.6.2/aqt/jax/v2/tiled_dot_general.py
--rw-r--r--   0        0        0     7015 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/tiled_dot_general_test.py
--rw-r--r--   0        0        0     1629 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax/v2/utils.py
--rw-r--r--   0        0        0     1590 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/__init__.py
--rw-r--r--   0        0        0    14397 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
--rw-r--r--   0        0        0     1921 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/__init__.py
--rw-r--r--   0        0        0    17225 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/compute_cost_utils.py
--rw-r--r--   0        0        0    24127 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/compute_cost_utils_test.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/flax/__init__.py
--rw-r--r--   0        0        0     5671 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/flax/struct.py
--rw-r--r--   0        0        0    35156 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/flax_attention.py
--rw-r--r--   0        0        0    25400 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/flax_attention_test.py
--rw-r--r--   0        0        0    42938 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/flax_layers.py
--rw-r--r--   0        0        0    75454 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/flax_layers_test.py
--rw-r--r--   0        0        0     6897 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/fp_cast.py
--rw-r--r--   0        0        0     7682 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/fp_cast_test.py
--rw-r--r--   0        0        0     9842 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/get_bounds.py
--rw-r--r--   0        0        0    11477 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/get_bounds_test.py
--rw-r--r--   0        0        0     3477 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/hlo_utils.py
--rw-r--r--   0        0        0     2570 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/hlo_utils_test.py
--rw-r--r--   0        0        0    10045 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/__init__.py
--rw-r--r--   0        0        0     1963 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/check_config_util.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/__init__.py
--rw-r--r--   0        0        0     7382 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/base_config.py
--rw-r--r--   0        0        0     1207 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
--rw-r--r--   0        0        0      853 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
--rw-r--r--   0        0        0     1230 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
--rw-r--r--   0        0        0     1439 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
--rw-r--r--   0        0        0     1231 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
--rw-r--r--   0        0        0     2000 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
--rw-r--r--   0        0        0     6443 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
--rw-r--r--   0        0        0     1647 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
--rw-r--r--   0        0        0     7476 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
--rw-r--r--   0        0        0      855 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
--rw-r--r--   0        0        0      855 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
--rw-r--r--   0        0        0      925 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
--rw-r--r--   0        0        0     1439 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
--rw-r--r--   0        0        0     1440 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
--rw-r--r--   0        0        0     1390 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
--rw-r--r--   0        0        0     1514 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
--rw-r--r--   0        0        0     1383 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
--rw-r--r--   0        0        0     1025 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
--rw-r--r--   0        0        0      925 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
--rw-r--r--   0        0        0     1232 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
--rw-r--r--   0        0        0     6856 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
--rw-r--r--   0        0        0     9732 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
--rw-r--r--   0        0        0     2423 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_test.py
--rw-r--r--   0        0        0     2130 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/hparams_config.py
--rw-r--r--   0        0        0   331485 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/imagenet.png
--rw-r--r--   0        0        0     8129 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/input_pipeline.py
--rw-r--r--   0        0        0     7345 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/models.py
--rw-r--r--   0        0        0     9773 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/models_test.py
--rw-r--r--   0        0        0    15474 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/pokebnn.py
--rw-r--r--   0        0        0     3119 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
--rw-r--r--   0        0        0       62 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/requirements.txt
--rw-r--r--   0        0        0     5749 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
--rw-r--r--   0        0        0    19735 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train.py
--rw-r--r--   0        0        0     2611 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train_benchmark.py
--rw-r--r--   0        0        0     2547 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train_test.py
--rw-r--r--   0        0        0     7991 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train_utils.py
--rw-r--r--   0        0        0     5854 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/primitives.py
--rw-r--r--   0        0        0     6508 2024-02-07 19:51:57.227827 aqtp-0.6.2/aqt/jax_legacy/jax/primitives_test.py
--rw-r--r--   0        0        0     3927 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/quant_config.py
--rw-r--r--   0        0        0    63283 2024-03-14 21:30:03.195956 aqtp-0.6.2/aqt/jax_legacy/jax/quantization.py
--rw-r--r--   0        0        0    45534 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/quantization_test.py
--rw-r--r--   0        0        0     1654 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/shape_utils.py
--rw-r--r--   0        0        0    22858 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/sparsity.py
--rw-r--r--   0        0        0    23122 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/sparsity_test.py
--rw-r--r--   0        0        0     9798 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/stats.py
--rw-r--r--   0        0        0     6060 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/stats_tag.py
--rw-r--r--   0        0        0     9777 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/stats_tag_test.py
--rw-r--r--   0        0        0    10461 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/stats_test.py
--rw-r--r--   0        0        0     4637 2024-02-07 19:51:57.231827 aqtp-0.6.2/aqt/jax_legacy/jax/test_utils.py
--rw-r--r--   0        0        0     5435 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax_legacy/jax/train_utils.py
--rw-r--r--   0        0        0     6454 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax_legacy/jax/train_utils_test.py
--rw-r--r--   0        0        0      995 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/jax_legacy/jax/utils.py
--rw-r--r--   0        0        0     2888 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
--rw-r--r--   0        0        0     7056 2024-02-07 19:51:57.211826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
--rw-r--r--   0        0        0    15134 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/decode.py
--rw-r--r--   0        0        0    12107 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
--rw-r--r--   0        0        0    11082 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
--rw-r--r--   0        0        0    13257 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
--rw-r--r--   0        0        0     6573 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
--rw-r--r--   0        0        0     1069 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1069 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1056 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1041 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
--rw-r--r--   0        0        0     1006 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1193 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
--rw-r--r--   0        0        0      954 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1101 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
--rw-r--r--   0        0        0     1002 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1042 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
--rw-r--r--   0        0        0     1002 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
--rw-r--r--   0        0        0     1060 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1175 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
--rw-r--r--   0        0        0     1244 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
--rw-r--r--   0        0        0     1664 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
--rw-r--r--   0        0        0     1661 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
--rw-r--r--   0        0        0     1662 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
--rw-r--r--   0        0        0     1662 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
--rw-r--r--   0        0        0     2172 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
--rw-r--r--   0        0        0     1600 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1849 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1323 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1448 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1344 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
--rw-r--r--   0        0        0     1568 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1801 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1584 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
--rw-r--r--   0        0        0     1479 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
--rw-r--r--   0        0        0     1495 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
--rw-r--r--   0        0        0     1531 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
--rw-r--r--   0        0        0     1046 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
--rw-r--r--   0        0        0     1245 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
--rw-r--r--   0        0        0     1245 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
--rw-r--r--   0        0        0     1549 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1380 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1380 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2052 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
--rw-r--r--   0        0        0     1340 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
--rw-r--r--   0        0        0     1340 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     2032 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1757 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
--rw-r--r--   0        0        0     1729 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
--rw-r--r--   0        0        0     2133 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
--rw-r--r--   0        0        0     1238 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     1238 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
--rw-r--r--   0        0        0     1587 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1379 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1379 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2123 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
--rw-r--r--   0        0        0     1213 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
--rw-r--r--   0        0        0     1213 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
--rw-r--r--   0        0        0     1554 2024-02-07 19:51:57.215826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1375 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1375 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2063 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
--rw-r--r--   0        0        0     2523 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
--rw-r--r--   0        0        0      995 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
--rw-r--r--   0        0        0     1672 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
--rw-r--r--   0        0        0     2392 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
--rw-r--r--   0        0        0     1222 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
--rw-r--r--   0        0        0     2101 2024-03-11 23:38:05.878321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
--rw-r--r--   0        0        0     3356 2024-03-11 23:38:05.882321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
--rw-r--r--   0        0        0     1531 2024-03-11 23:38:05.882321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
--rw-r--r--   0        0        0     1965 2024-03-11 23:38:05.882321 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
--rw-r--r--   0        0        0      382 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
--rw-r--r--   0        0        0     1096 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1014 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1096 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1018 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
--rw-r--r--   0        0        0      995 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
--rw-r--r--   0        0        0     1925 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
--rw-r--r--   0        0        0    23300 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
--rw-r--r--   0        0        0    33382 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/models.py
--rw-r--r--   0        0        0    38051 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
--rw-r--r--   0        0        0     4055 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/predict.py
--rw-r--r--   0        0        0      160 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
--rw-r--r--   0        0        0    51615 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/train.py
--rw-r--r--   0        0        0     5666 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
--rw-r--r--   0        0        0    10503 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
--rw-r--r--   0        0        0     3939 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
--rw-r--r--   0        0        0    25395 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
--rw-r--r--   0        0        0     3284 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
--rw-r--r--   0        0        0      118 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/requirements.txt
--rw-r--r--   0        0        0    10519 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/README.md
--rw-r--r--   0        0        0      577 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/__init__.py
--rw-r--r--   0        0        0     4810 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/analysis_utils.py
--rw-r--r--   0        0        0     5109 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/analysis_utils_test.py
--rw-r--r--   0        0        0     1045 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/common.py
--rw-r--r--   0        0        0     8505 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/config_schema_utils.py
--rw-r--r--   0        0        0    11978 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/config_schema_utils_test.py
--rw-r--r--   0        0        0     6807 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/hparams_utils.py
--rw-r--r--   0        0        0    10185 2024-02-07 19:51:57.219826 aqtp-0.6.2/aqt/jax_legacy/utils/pandas_utils.py
--rw-r--r--   0        0        0    10192 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/pandas_utils_test.py
--rw-r--r--   0        0        0    20428 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/report_utils.py
--rw-r--r--   0        0        0    23689 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/report_utils_test.py
--rw-r--r--   0        0        0     2538 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/summary_utils.py
--rw-r--r--   0        0        0     3451 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/summary_utils_test.py
--rw-r--r--   0        0        0     6640 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/tfevent_utils.py
--rw-r--r--   0        0        0     4307 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/jax_legacy/utils/tfevent_utils_test.py
--rw-r--r--   0        0        0    15648 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/test/aqt_conv_test_base.py
--rw-r--r--   0        0        0    11192 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/test/aqt_matmul_test_base.py
--rw-r--r--   0        0        0    12101 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/test/aqt_stats_test_base.py
--rw-r--r--   0        0        0    23072 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/test/aqt_tensor_test_base.py
--rw-r--r--   0        0        0     4694 2024-02-07 19:51:57.223827 aqtp-0.6.2/aqt/test/aqt_test_shared_base.py
--rw-r--r--   0        0        0   129585 2024-02-07 19:51:57.223827 aqtp-0.6.2/papers/aqt/aqt.pdf
--rw-r--r--   0        0        0     1303 2024-02-07 19:51:57.223827 aqtp-0.6.2/papers/aqt/aqt.tex
--rw-r--r--   0        0        0     1468 2024-02-07 19:51:57.223827 aqtp-0.6.2/papers/pokebnn/README.md
--rw-r--r--   0        0        0     2862 2024-02-07 19:51:57.223827 aqtp-0.6.2/papers/pokebnn/cloudtpu_train_pokebnn.sh
--rw-r--r--   0        0        0   117523 2024-02-07 19:51:57.223827 aqtp-0.6.2/papers/pokebnn/tensorboard.ipynb
--rw-r--r--   0        0        0      727 2024-03-11 23:38:05.882321 aqtp-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1852 2024-02-07 19:51:57.227827 aqtp-0.6.2/setup.py
--rw-r--r--   0        0        0    16180 1970-01-01 00:00:00.000000 aqtp-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-09 23:55:52.438082 aqtp-0.7.0/.gitignore
+-rw-r--r--   0        0        0      107 2024-04-09 23:55:52.438082 aqtp-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2024-04-09 23:55:52.438082 aqtp-0.7.0/LICENSE
+-rw-r--r--   0        0        0    17310 2024-04-09 23:55:52.438082 aqtp-0.7.0/README.md
+-rw-r--r--   0        0        0      641 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/__init__.py
+-rw-r--r--   0        0        0      576 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/common/__init__.py
+-rw-r--r--   0        0        0     4354 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/common/aqt_common.py
+-rw-r--r--   0        0        0    16011 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/common/aqt_config.py
+-rw-r--r--   0        0        0    13928 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/common/aqt_config_schedule_test.py
+-rw-r--r--   0        0        0     5177 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/common/aqt_config_utils.py
+-rw-r--r--   0        0        0    15655 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/common/emulated_floating_points.py
+-rw-r--r--   0        0        0     5730 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/common/emulation_utils.py
+-rw-r--r--   0        0        0      576 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/__init__.py
+-rw-r--r--   0        0        0    13641 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_conv_general.py
+-rw-r--r--   0        0        0    12151 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_conv_general_test.py
+-rw-r--r--   0        0        0     8861 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_dot_general.py
+-rw-r--r--   0        0        0    14977 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     3693 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_matmul.py
+-rw-r--r--   0        0        0     3293 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_matmul_test.py
+-rw-r--r--   0        0        0     1083 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_ops.py
+-rw-r--r--   0        0        0    18180 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_tensor.py
+-rw-r--r--   0        0        0     4751 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2705 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/aqt_utils.py
+-rw-r--r--   0        0        0     4724 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax/v2/aqt_conv_general.py
+-rw-r--r--   0        0        0    28806 2024-04-10 00:32:01.566452 aqtp-0.7.0/aqt/jax/v2/aqt_dot_general.py
+-rw-r--r--   0        0        0    37788 2024-04-10 00:32:16.094696 aqtp-0.7.0/aqt/jax/v2/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     5240 2024-04-10 00:32:33.730992 aqtp-0.7.0/aqt/jax/v2/aqt_quantizer.py
+-rw-r--r--   0        0        0     9326 2024-04-10 00:32:46.899213 aqtp-0.7.0/aqt/jax/v2/aqt_tensor.py
+-rw-r--r--   0        0        0     2568 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2608 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/calibration.py
+-rw-r--r--   0        0        0    20547 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/config.py
+-rw-r--r--   0        0        0    37619 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/config_test.py
+-rw-r--r--   0        0        0     5550 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/examples/examples.ipynb
+-rw-r--r--   0        0        0    13343 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/examples/flax_e2e_model.py
+-rw-r--r--   0        0        0    14269 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/examples/flax_e2e_model_test.py
+-rw-r--r--   0        0        0    19139 2024-04-10 00:33:09.659596 aqtp-0.7.0/aqt/jax/v2/flax/aqt_flax.py
+-rw-r--r--   0        0        0     2380 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/aqt_flax_calibration.py
+-rw-r--r--   0        0        0     3835 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/aqt_flax_dg_core.py
+-rw-r--r--   0        0        0     7540 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/aqt_flax_test.py
+-rw-r--r--   0        0        0     3183 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/freezer.py
+-rw-r--r--   0        0        0     7422 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/freezer_test.py
+-rw-r--r--   0        0        0     1672 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/intercept/README.md
+-rw-r--r--   0        0        0     6896 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
+-rw-r--r--   0        0        0     3997 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
+-rw-r--r--   0        0        0     6087 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
+-rw-r--r--   0        0        0     8989 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
+-rw-r--r--   0        0        0     4731 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/numerics/fp8_numerics.py
+-rw-r--r--   0        0        0     8739 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax/v2/numerics/fp8_numerics_test.py
+-rw-r--r--   0        0        0     4451 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/numerics/int_numerics.py
+-rw-r--r--   0        0        0     1426 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/numerics/no_numerics.py
+-rw-r--r--   0        0        0     1338 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/numerics/numerics.py
+-rw-r--r--   0        0        0     2526 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/pax/pax_base_ops.py
+-rw-r--r--   0        0        0     2095 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/pax/pax_base_ops_test.py
+-rw-r--r--   0        0        0     1846 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/stochastic_rounding.py
+-rw-r--r--   0        0        0    15088 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/tiled_dot_general.py
+-rw-r--r--   0        0        0     6972 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/tiled_dot_general_test.py
+-rw-r--r--   0        0        0     4802 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/transpose.py
+-rw-r--r--   0        0        0     4187 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax/v2/transpose_test.py
+-rw-r--r--   0        0        0     4668 2024-04-10 00:32:58.511408 aqtp-0.7.0/aqt/jax/v2/utils.py
+-rw-r--r--   0        0        0     1590 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/__init__.py
+-rw-r--r--   0        0        0    14397 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
+-rw-r--r--   0        0        0     1921 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/__init__.py
+-rw-r--r--   0        0        0    17225 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/compute_cost_utils.py
+-rw-r--r--   0        0        0    24127 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/compute_cost_utils_test.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/flax/__init__.py
+-rw-r--r--   0        0        0     5671 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/flax/struct.py
+-rw-r--r--   0        0        0    35156 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/flax_attention.py
+-rw-r--r--   0        0        0    25400 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/flax_attention_test.py
+-rw-r--r--   0        0        0    43061 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/flax_layers.py
+-rw-r--r--   0        0        0    75454 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/flax_layers_test.py
+-rw-r--r--   0        0        0     6897 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/fp_cast.py
+-rw-r--r--   0        0        0     7682 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/fp_cast_test.py
+-rw-r--r--   0        0        0     9842 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/get_bounds.py
+-rw-r--r--   0        0        0    11477 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/get_bounds_test.py
+-rw-r--r--   0        0        0     3477 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/hlo_utils.py
+-rw-r--r--   0        0        0     2570 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/hlo_utils_test.py
+-rw-r--r--   0        0        0    10045 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/__init__.py
+-rw-r--r--   0        0        0     1963 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/check_config_util.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/__init__.py
+-rw-r--r--   0        0        0     7382 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/base_config.py
+-rw-r--r--   0        0        0     1207 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
+-rw-r--r--   0        0        0      853 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
+-rw-r--r--   0        0        0     1230 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
+-rw-r--r--   0        0        0     1439 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
+-rw-r--r--   0        0        0     1231 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
+-rw-r--r--   0        0        0     6443 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
+-rw-r--r--   0        0        0     1647 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
+-rw-r--r--   0        0        0     7476 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
+-rw-r--r--   0        0        0      855 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
+-rw-r--r--   0        0        0      855 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
+-rw-r--r--   0        0        0      925 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
+-rw-r--r--   0        0        0     1439 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
+-rw-r--r--   0        0        0     1440 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
+-rw-r--r--   0        0        0     1390 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
+-rw-r--r--   0        0        0     1514 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
+-rw-r--r--   0        0        0     1383 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
+-rw-r--r--   0        0        0     1025 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
+-rw-r--r--   0        0        0      925 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
+-rw-r--r--   0        0        0     1232 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
+-rw-r--r--   0        0        0     6856 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
+-rw-r--r--   0        0        0     9732 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
+-rw-r--r--   0        0        0     2423 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_test.py
+-rw-r--r--   0        0        0     2130 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/hparams_config.py
+-rw-r--r--   0        0        0   331485 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/imagenet.png
+-rw-r--r--   0        0        0     8129 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/input_pipeline.py
+-rw-r--r--   0        0        0     7345 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/models.py
+-rw-r--r--   0        0        0     9773 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/models_test.py
+-rw-r--r--   0        0        0    15474 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/pokebnn.py
+-rw-r--r--   0        0        0     3119 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
+-rw-r--r--   0        0        0       62 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/requirements.txt
+-rw-r--r--   0        0        0     5749 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
+-rw-r--r--   0        0        0    19735 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train.py
+-rw-r--r--   0        0        0     2611 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train_benchmark.py
+-rw-r--r--   0        0        0     2547 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train_test.py
+-rw-r--r--   0        0        0     7991 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train_utils.py
+-rw-r--r--   0        0        0     5854 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/primitives.py
+-rw-r--r--   0        0        0     6508 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/primitives_test.py
+-rw-r--r--   0        0        0     3927 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/quant_config.py
+-rw-r--r--   0        0        0    63283 2024-04-09 23:55:52.458082 aqtp-0.7.0/aqt/jax_legacy/jax/quantization.py
+-rw-r--r--   0        0        0    45534 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/quantization_test.py
+-rw-r--r--   0        0        0     1654 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/shape_utils.py
+-rw-r--r--   0        0        0    22231 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
+-rw-r--r--   0        0        0    23430 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
+-rw-r--r--   0        0        0     9798 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/stats.py
+-rw-r--r--   0        0        0     6060 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/stats_tag.py
+-rw-r--r--   0        0        0     9777 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/stats_tag_test.py
+-rw-r--r--   0        0        0    10461 2024-04-09 23:55:52.462082 aqtp-0.7.0/aqt/jax_legacy/jax/stats_test.py
+-rw-r--r--   0        0        0     4637 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/test_utils.py
+-rw-r--r--   0        0        0     5435 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/train_utils.py
+-rw-r--r--   0        0        0     6454 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/train_utils_test.py
+-rw-r--r--   0        0        0      995 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/utils.py
+-rw-r--r--   0        0        0     2888 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
+-rw-r--r--   0        0        0     7056 2024-04-09 23:55:52.438082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
+-rw-r--r--   0        0        0    15134 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/decode.py
+-rw-r--r--   0        0        0    12107 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
+-rw-r--r--   0        0        0    11082 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
+-rw-r--r--   0        0        0    13257 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
+-rw-r--r--   0        0        0     6573 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1069 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1056 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1041 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
+-rw-r--r--   0        0        0     1006 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1193 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
+-rw-r--r--   0        0        0      954 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1101 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
+-rw-r--r--   0        0        0     1002 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1042 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
+-rw-r--r--   0        0        0     1002 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
+-rw-r--r--   0        0        0     1060 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1175 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
+-rw-r--r--   0        0        0     1244 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
+-rw-r--r--   0        0        0     1664 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
+-rw-r--r--   0        0        0     1661 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
+-rw-r--r--   0        0        0     1662 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
+-rw-r--r--   0        0        0     1662 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
+-rw-r--r--   0        0        0     2172 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
+-rw-r--r--   0        0        0     1600 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1849 2024-04-09 23:55:52.442082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1323 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1448 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1344 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
+-rw-r--r--   0        0        0     1568 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1801 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1584 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
+-rw-r--r--   0        0        0     1479 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
+-rw-r--r--   0        0        0     1495 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
+-rw-r--r--   0        0        0     1531 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
+-rw-r--r--   0        0        0     1046 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
+-rw-r--r--   0        0        0     1245 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
+-rw-r--r--   0        0        0     1245 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
+-rw-r--r--   0        0        0     1549 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1380 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1380 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2052 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
+-rw-r--r--   0        0        0     1340 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
+-rw-r--r--   0        0        0     1340 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     2032 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1757 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
+-rw-r--r--   0        0        0     1729 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
+-rw-r--r--   0        0        0     2133 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1238 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1238 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1587 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1379 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1379 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2123 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1213 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1213 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1554 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1375 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1375 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2063 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
+-rw-r--r--   0        0        0     2523 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
+-rw-r--r--   0        0        0      995 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1672 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
+-rw-r--r--   0        0        0     2392 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
+-rw-r--r--   0        0        0     1222 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
+-rw-r--r--   0        0        0     2101 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
+-rw-r--r--   0        0        0     3356 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
+-rw-r--r--   0        0        0     1531 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
+-rw-r--r--   0        0        0     1965 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
+-rw-r--r--   0        0        0      382 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
+-rw-r--r--   0        0        0     1096 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1014 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1096 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1018 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
+-rw-r--r--   0        0        0      995 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1925 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
+-rw-r--r--   0        0        0    23300 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
+-rw-r--r--   0        0        0    33382 2024-04-09 23:55:52.446082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/models.py
+-rw-r--r--   0        0        0    38051 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
+-rw-r--r--   0        0        0     4055 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/predict.py
+-rw-r--r--   0        0        0      160 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
+-rw-r--r--   0        0        0    51590 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/train.py
+-rw-r--r--   0        0        0     5666 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
+-rw-r--r--   0        0        0    10503 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
+-rw-r--r--   0        0        0     3939 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
+-rw-r--r--   0        0        0    25395 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
+-rw-r--r--   0        0        0     3284 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
+-rw-r--r--   0        0        0      118 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/requirements.txt
+-rw-r--r--   0        0        0    10519 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/README.md
+-rw-r--r--   0        0        0      577 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/__init__.py
+-rw-r--r--   0        0        0     4810 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/analysis_utils.py
+-rw-r--r--   0        0        0     5109 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/analysis_utils_test.py
+-rw-r--r--   0        0        0     1045 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/common.py
+-rw-r--r--   0        0        0     8505 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/config_schema_utils.py
+-rw-r--r--   0        0        0    11978 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/config_schema_utils_test.py
+-rw-r--r--   0        0        0     6844 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/hparams_utils.py
+-rw-r--r--   0        0        0    10185 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/pandas_utils.py
+-rw-r--r--   0        0        0    10192 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/pandas_utils_test.py
+-rw-r--r--   0        0        0    20428 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/report_utils.py
+-rw-r--r--   0        0        0    23689 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/report_utils_test.py
+-rw-r--r--   0        0        0     2538 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/summary_utils.py
+-rw-r--r--   0        0        0     3451 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/summary_utils_test.py
+-rw-r--r--   0        0        0     6640 2024-04-09 23:55:52.450082 aqtp-0.7.0/aqt/jax_legacy/utils/tfevent_utils.py
+-rw-r--r--   0        0        0     4307 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/jax_legacy/utils/tfevent_utils_test.py
+-rw-r--r--   0        0        0    15648 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/test/aqt_conv_test_base.py
+-rw-r--r--   0        0        0    11192 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/test/aqt_matmul_test_base.py
+-rw-r--r--   0        0        0    12101 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/test/aqt_stats_test_base.py
+-rw-r--r--   0        0        0    23072 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/test/aqt_tensor_test_base.py
+-rw-r--r--   0        0        0     4694 2024-04-09 23:55:52.454082 aqtp-0.7.0/aqt/test/aqt_test_shared_base.py
+-rw-r--r--   0        0        0   129585 2024-04-09 23:55:52.454082 aqtp-0.7.0/papers/aqt/aqt.pdf
+-rw-r--r--   0        0        0     1303 2024-04-09 23:55:52.454082 aqtp-0.7.0/papers/aqt/aqt.tex
+-rw-r--r--   0        0        0     1468 2024-04-09 23:55:52.454082 aqtp-0.7.0/papers/pokebnn/README.md
+-rw-r--r--   0        0        0     2862 2024-04-09 23:55:52.454082 aqtp-0.7.0/papers/pokebnn/cloudtpu_train_pokebnn.sh
+-rw-r--r--   0        0        0   117523 2024-04-09 23:55:52.454082 aqtp-0.7.0/papers/pokebnn/tensorboard.ipynb
+-rw-r--r--   0        0        0      727 2024-04-09 23:55:52.454082 aqtp-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1852 2024-04-09 23:55:52.454082 aqtp-0.7.0/setup.py
+-rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.0/PKG-INFO
```

### Comparing `aqtp-0.6.2/LICENSE` & `aqtp-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/README.md` & `aqtp-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -154,14 +154,77 @@
   scale_stop_grad: bool
   calibration: calibration.Calibration  # calibration algorithm
   po2_scale: bool  # round calibration to power of 2
   use_fake_quant: bool
   use_fwd_quant: Optional[bool]  # use quantized fwd in the bwd pass
 ```
 
+## How to make and use a simple AQT quantizer
+
+This example demonstrates how to make a simple linear AQT quantizer.
+
+```python
+from aqt.jax.v2 import aqt_quantizer
+from aqt.jax.v2 import calibration
+from aqt.jax.v2 import utils as aqt_utils
+from aqt.jax.v2.numerics import int_numerics
+
+q = aqt_quantizer.Quantizer(
+    numerics=int_numerics.IntNumerics(
+        bits=4,
+        preserve_zero=True,
+        preserve_max_val=True,
+        clip=True,
+        clip_gradient=True,
+        round=True,
+        noise_fn=None,
+    ),
+    calib_shared_axes=-1,
+    scale_stop_grad=True,
+    calibration=calibration.AbsMaxCalibration(),
+    po2_scale=False,
+    context=aqt_utils.Context(key=jax.random.PRNGKey(0), train_step=0))
+```
+
+To view the quantized weights created by the quantizer, try quantizing a simple vector like so. Remember that these are the quantized values that are stored in memory for weight quantization.
+
+```python
+x = jnp.linspace(-10, 10, 10)
+x_q, _ = q.quant(x, calibration_axes=-1)
+print(x_q.qvalue)
+```
+
+To view the dequantized values that are used after multiplying the quantized values by the scale, use this code
+
+```python
+print(x_q.dequant())
+```
+
+To view the scales, simply call the scale attribute
+
+```python
+print(x_q.scale)
+```
+
+For a sanity check, we can assert that the scale in this example is simply equal to the dequantized values divided by the quantized values. (Hint: if you get an error check for nan values)
+
+```python
+assert jnp.all(x_q.dequant() / x_q.qvalue == x_q.scale[0])
+```
+
+Finally, we can plot the quantized values like so
+
+```python
+import matplotlib.pyplot as plt
+plt.plot(x, x_q.qvalue)
+```
+
+The specific quantizer parameters here are implemented in this tutorial are just for demonstration purposes and can be easily changed. Try altering the number of bits and see how the number of quantization steps changes accordingly.
+
+
 ## AQT Versions
 
 As of today there are several independent AQT implementations in this package:
 
 - [JAX Legacy AQT](https://github.com/google/aqt/blob/main/aqt/jax_legacy)
   Obsolete version of AQT still used by some customers.
 - [JAX AQTv1](https://github.com/google/aqt/blob/main/aqt/jax)
```

### Comparing `aqtp-0.6.2/aqt/__init__.py` & `aqtp-0.7.0/aqt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Accurate Quantized Training library."""
 
-__version__ = "0.6.2"
+__version__ = "0.7.0"
```

### Comparing `aqtp-0.6.2/aqt/common/__init__.py` & `aqtp-0.7.0/aqt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/common/aqt_common.py` & `aqtp-0.7.0/aqt/common/aqt_common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/common/aqt_config.py` & `aqtp-0.7.0/aqt/common/aqt_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/common/aqt_config_schedule_test.py` & `aqtp-0.7.0/aqt/common/aqt_config_schedule_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/common/aqt_config_utils.py` & `aqtp-0.7.0/aqt/common/aqt_config_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/common/emulated_floating_points.py` & `aqtp-0.7.0/aqt/common/emulated_floating_points.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/common/emulation_utils.py` & `aqtp-0.7.0/aqt/common/emulation_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/__init__.py` & `aqtp-0.7.0/aqt/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_conv_general.py` & `aqtp-0.7.0/aqt/jax/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_conv_general_test.py` & `aqtp-0.7.0/aqt/jax/aqt_conv_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_dot_general.py` & `aqtp-0.7.0/aqt/jax/aqt_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_dot_general_test.py` & `aqtp-0.7.0/aqt/jax/aqt_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_matmul.py` & `aqtp-0.7.0/aqt/jax/aqt_matmul.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 """Quantized matmul."""
 
 import builtins
 
 import jax
-from jax import core
 from jax import lax
 import jax.numpy as jnp
 import numpy as np
 
 
 shape = np.shape
 ndim = np.ndim
@@ -80,21 +79,21 @@
   idx_a_other = []  # other = non-batch, non-contracting.
   idx_b_other = []
   for i, (ba, bb) in enumerate(zip(a_batch_dims, b_batch_dims)):
     if ba is None:
       idx_b_other.append(i)
     elif bb is None:
       idx_a_other.append(i)
-    elif core.symbolic_equal_dim(ba, 1):
+    elif ba == 1:
       idx_b_other.append(i)
       a_squeeze.append(len(idx_batch) + len(idx_a_other) + len(a_squeeze))
-    elif core.symbolic_equal_dim(bb, 1):
+    elif bb == 1:
       idx_a_other.append(i)
       b_squeeze.append(len(idx_batch) + len(idx_b_other) + len(b_squeeze))
-    elif core.symbolic_equal_dim(ba, bb):
+    elif ba == bb:
       a_batch.append(len(idx_batch) + len(idx_a_other))
       b_batch.append(len(idx_batch) + len(idx_b_other))
       idx_batch.append(i)
     else:
       raise ValueError("Incompatible shapes for matmul arguments: {} and {}"
                        .format(shape(a), shape(b)))
```

### Comparing `aqtp-0.6.2/aqt/jax/aqt_matmul_test.py` & `aqtp-0.7.0/aqt/jax/aqt_matmul_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_ops.py` & `aqtp-0.7.0/aqt/jax/aqt_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_tensor.py` & `aqtp-0.7.0/aqt/jax/aqt_tensor.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_tensor_test.py` & `aqtp-0.7.0/aqt/jax/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/aqt_utils.py` & `aqtp-0.7.0/aqt/jax/aqt_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/aqt_conv_general.py` & `aqtp-0.7.0/aqt/jax/v2/aqt_conv_general.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 from jax import lax
 import jax.numpy as jnp
 
 
 def make_conv_general_dilated(cfg: config.DotGeneralRaw):
   """Makes quantized lax.make_conv_general_dilated replacement."""
   # TODO(lew): Either rename DotGeneralConfig or make a conv-specific cfg.
-  if cfg is None:
-    cfg = config.DotGeneralRaw.make()
+  assert cfg is not None, "Missing config for make_conv_general_dilated"
 
   def my_conv_general_dilated(
       lhs,
       rhs,
       window_strides,
       padding,
       lhs_dilation=None,
@@ -63,21 +62,21 @@
     # rhs layout is: spatials..., Ci, Co
     # out layous it: B, spatials..., Co
     #
     # we need to share these axes: lhs[1:] , rhs[:-1]
     # we have a scale/invscale per: lhs[0] / out[0] and rhs[-1] / out[-1]
 
     # Flax assumptions.
-    assert cfg.lhs.quantizer.calib_shared_axes == list(range(1, rank))
-    assert cfg.rhs.quantizer.calib_shared_axes == list(range(0, rank - 1))
-
-    lhs_qt, _ = cfg.lhs.quantizer.quant(lhs, calibration_axes=None)
-    rhs_qt, _ = cfg.rhs.quantizer.quant(rhs, calibration_axes=None)
-
-    # lax.conv_general_dilated does not support int8 * float.
+    msg = "Convolution formula does not follow flax assumption."
+    # TODO(lew): Perhaps we should rely only on passing  passing calib shared
+    # axes value instead of setting it in config. (we pass None below)
+    cfg.dg_quantizer.assert_calib_shared_axes_value(
+        list(range(1, rank)), list(range(0, rank - 1)), msg
+    )
+    (lhs_qt, _), (rhs_qt, _) = cfg.dg_quantizer((lhs, None), (rhs, None))
     # Therefore, cast qvalue back to its original data dtype.
     # Delete the following two lines when the constraint is lifted.
     lhs_qt = lhs_qt.qvalue_astype(lhs.dtype)
     rhs_qt = rhs_qt.qvalue_astype(rhs.dtype)
 
     out = lax.conv_general_dilated(
         lhs=lhs_qt.qvalue,
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/aqt_dot_general.py` & `aqtp-0.7.0/aqt/jax/v2/aqt_dot_general.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 # - ca - contraction axes
 # - ba - batch axes
 # - ra - remaining axes
 
 # pylint: disable=g-explicit-bool-comparison
 # pylint: disable=g-explicit-length-test
 
+import abc
 import enum
-import functools
 from typing import Any, Optional, Sequence, Union
+
 from aqt.jax.v2 import aqt_quantizer
 from aqt.jax.v2 import aqt_tensor
-from aqt.jax.v2 import calibration
+from aqt.jax.v2 import transpose
 from aqt.jax.v2 import utils
-from aqt.jax.v2.numerics import int_numerics
-from aqt.jax.v2.numerics import no_numerics
 import jax
 from jax import lax
 from jax._src.numpy import lax_numpy
 import jax.numpy as jnp
 import numpy as onp
 from typing_extensions import Self  # for python version < 3.11
 
+
 dtypes_allowed_for_int32_accum = [jnp.int4, jnp.int8]
 
 
 class CalibrationMode(enum.Enum):
   """Calibration axis modes."""
 
   CONTRACTING_AXIS = 1
@@ -64,15 +64,14 @@
   OTHER_INPUT = 3
 
 
 @utils.flax_slots_dataclass
 class Tensor:
   """Configuration of quantization of one tensor or one side of tensor op."""
 
-  quantizer: aqt_quantizer.Quantizer
   # Controls at what value of input tensor should be used.
   # Setting it to True, but not quantizing fwd pass will assert-fail.
   use_fwd_quant: Optional[bool] = utils.static_field()
   # Dequantization mode.
   dequant_mode: DequantMode = utils.static_field()
   # Calibration axis mode.
   calibration_mode: CalibrationMode = utils.static_field()
@@ -83,106 +82,77 @@
 
 
 @utils.flax_slots_dataclass
 class LocalAqt:
   contraction_axis_shard_count: int = utils.static_field()
 
 
-def tensor_make(
-    bits: Optional[int], preserve_max_val: bool = False
-) -> 'Tensor':
+def tensor_make() -> 'Tensor':
   """Makes config.Tensor."""
-  if bits is None:
-    effective_numerics = no_numerics.NoNumerics()
-  else:
-
-    def _dtype_from_bits(bits, pz):
-      if 2 <= bits <= 8 and pz:
-        if bits == 4:
-          return jnp.int4
-        else:
-          return jnp.int8
-      else:
-        return None
-
-    pz = False if bits == 1 else True
-    dtype = _dtype_from_bits(bits, pz)
-    effective_numerics = int_numerics.IntNumerics(
-        bits=bits,
-        preserve_zero=pz,
-        preserve_max_val=preserve_max_val,
-        clip=True,
-        round=True,
-        noise_fn=None,
-        clip_gradient=False,  # This can be disabled when using abs-max scaling.
-        dtype=dtype,
-    )
-  quantizer = aqt_quantizer.Quantizer(
-      numerics=effective_numerics,
-      calib_shared_axes=None,
-      scale_stop_grad=True,
-      calibration=calibration.AbsMaxCalibration(),
-      po2_scale=False,
-      context=aqt_quantizer.Context(key=None, train_step=None),
-  )
   return Tensor(
-      quantizer=quantizer,
-      # dtype_x=dtype,
       use_fwd_quant=None,
       dequant_mode=DequantMode.OUTPUT,
       calibration_mode=CalibrationMode.CONTRACTING_AXIS,
   )
 
 
 def dot_general_raw_make(
     lhs_bits=None,
     rhs_bits=None,
     local_aqt=None,
     jax_scope_name='aqt',
 ) -> 'DotGeneralRaw':
   """Create quantization configs for input matrices to a matmul."""
-  lhs_cfg = tensor_make(lhs_bits)
-  rhs_cfg = tensor_make(rhs_bits)
+  lhs_cfg = tensor_make()
+  rhs_cfg = tensor_make()
 
   # Binary uses 0.5 right now.
   if (
       lhs_bits is not None
       and rhs_bits is not None
       and 2 <= lhs_bits <= 8
       and 2 <= rhs_bits <= 8
   ):
     dg_accumulator_dtype = jnp.int32
   else:
     dg_accumulator_dtype = None
 
+  lhs = aqt_quantizer.quantizer_make(lhs_bits)
+  rhs = aqt_quantizer.quantizer_make(rhs_bits)
+  dg_quantizer = DefaultDotGeneralQuantizer(lhs=lhs, rhs=rhs)
+
   return DotGeneralRaw(
       lhs=lhs_cfg,
       rhs=rhs_cfg,
+      dg_quantizer=dg_quantizer,
       dg_accumulator_dtype=dg_accumulator_dtype,
       local_aqt=local_aqt,
       jax_scope_name=jax_scope_name,
   )
 
 
 def conv_general_dilated_make(
     spatial_dimensions=2,
     lhs_bits: Optional[int] = None,
     rhs_bits: Optional[int] = None,
 ) -> 'DotGeneralRaw':
   """Create quantization config conv_general_dilated."""
   config = dot_general_raw_make(lhs_bits, rhs_bits)
   # Hardcoding flax assumptions.
-  if config.lhs:
-    config.lhs.quantizer.calib_shared_axes = list(
-        range(1, spatial_dimensions + 2)
-    )
-  if config.rhs:
-    config.rhs.quantizer.calib_shared_axes = list(
-        range(0, spatial_dimensions + 2 - 1)
-    )
+  lhs_calib_shared_axes = (
+      list(range(1, spatial_dimensions + 2)) if config.lhs else None
+  )
+  rhs_calib_shared_axes = (
+      list(range(0, spatial_dimensions + 2 - 1)) if config.rhs else None
+  )
+
+  assert isinstance(config.dg_quantizer, DefaultDotGeneralQuantizer)
+  config.dg_quantizer.lhs.calib_shared_axes = lhs_calib_shared_axes
+  config.dg_quantizer.rhs.calib_shared_axes = rhs_calib_shared_axes
+
   return config
 
 
 def dot_general_make(
     lhs_bits: Optional[int] = None,
     rhs_bits: Optional[int] = None,
     bwd_bits: Optional[int] = None,
@@ -244,173 +214,129 @@
       contractions,
       precision=None,
       preferred_element_type=None,
       _dot_general=dg,
   )
 
 
-def _scale_trans(x, ca, ba):
-  """Transposes x to output dimension order."""
-  ca = list(ca)
-  ba = list(ba)
-  for i in ca:
-    assert x.shape[i] == 1
-  ra = list(i for i in range(len(x.shape)) if i not in ba + ca)
-  x = jnp.transpose(x, ba + ra + ca)
-  # TODO(lew): x = jnp.squeeze(x, axis=range(len(ba+ra): len(x.shape))
-  shape_ba = x.shape[: len(ba)]
-  shape_ra = x.shape[len(ba) : len(x.shape) - len(ca)]
-  # Will need to add additional axes (size 1) for the other shape_ra
-  x = x.reshape(shape_ba + shape_ra)
-  return x
-
-
-def _lhs_scale_transpose_to_output(
-    lhs_scale, dimension_numbers, lhs_shape, rhs_shape
-):
-  """Transposes lhs_scale to output dimension order."""
-  if lhs_scale is None:
-    return None
-  # The axis order in out is as follows: batch, lhs_ra, rhs_ra
-  # - batch axes order is uniquely determined by either lhs_ba or rhs_ba
-  # - contraction axes ca disappear from the output
-  # - order of the remaining axes (ra) is preserved.
-  (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
-  qlhs_scale_t = _scale_trans(lhs_scale, lhs_ca, lhs_ba)
-  # inserting dummy axes for rhs_ra
-  assert len(qlhs_scale_t.shape) == len(lhs_shape) - len(lhs_ca)
-  start = len(qlhs_scale_t.shape)
-  end = len(rhs_shape) - len(rhs_ca) - len(rhs_ba) + start
-  lhs_dummy_axes = range(start, end)
-  qlhs_scale_t = jnp.expand_dims(qlhs_scale_t, axis=lhs_dummy_axes)
-  return qlhs_scale_t
-
-
-def _rhs_scale_transpose_to_output(
-    rhs_scale, dimension_numbers, lhs_shape, rhs_shape
-):
-  """Transposes rhs_scale to output dimension order."""
-  if rhs_scale is None:
-    return None
-  del rhs_shape
-  (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
-  qrhs_scale_t = _scale_trans(rhs_scale, rhs_ca, rhs_ba)
-  start = len(rhs_ba)
-  end = len(lhs_shape) - len(lhs_ca) - len(lhs_ba) + start
-  rhs_dummy_axes = range(start, end)
-  qrhs_scale_t = jnp.expand_dims(qrhs_scale_t, axis=rhs_dummy_axes)
-  return qrhs_scale_t
-
-
-def _get_ra(rank: int, ca: Sequence[int], ba: Sequence[int]):
-  """Returns the remaining axes."""
-  ret = []
-  for i in range(rank):
-    if i not in list(ca) + list(ba):
-      ret.append(i)
-  return ret
-
-
-def _scale_trans_for_other_input(
-    x: jax.Array,
-    my_ca: Sequence[int],
-    my_ba: Sequence[int],
-    other_ca: Sequence[int],
-    other_ba: Sequence[int],
-    other_rank: int,
-):
-  """Transposes x to other inputs' dimension order."""
-  my_ca = list(my_ca)
-  my_ba = list(my_ba)
-  other_ca = list(other_ca)
-  other_ba = list(other_ba)
-
-  # Match the rank.
-  if len(x.shape) < other_rank:
-    x = x.reshape(list(x.shape) + [1] * (other_rank - len(x.shape)))
-
-  transpose_dim = [-1] * len(x.shape)
-  my_axis_mapped = my_ca + my_ba
-  other_axis_mapped = other_ca + other_ba
-  my_ra = _get_ra(x.ndim, my_ca, my_ba)
-  for axis in my_ra:
-    assert x.shape[axis] == 1
-  for my_axis, other_axis in zip(my_axis_mapped, other_axis_mapped):
-    transpose_dim[other_axis] = my_axis
-
-  # Fill unrelated axis with remaining axis.
-  ra_idx = 0
-  for transpose_dim_idx, transpose_dim_value in enumerate(transpose_dim):
-    if transpose_dim_value == -1:
-      transpose_dim[transpose_dim_idx] = my_ra[ra_idx]
-      ra_idx += 1
-  assert ra_idx == len(my_ra)
-
-  # Transpose.
-  x = jnp.transpose(x, transpose_dim)
-
-  # Remove redundant axis.
-  if len(x.shape) > other_rank:
-    for idx in range(len(x.shape), other_rank):
-      assert x.shape[idx] == 1
-    x = x.reshape(x.shape[:other_rank])
-
-  return x
-
-
-def _lhs_scale_transpose_for_rhs_input(lhs_scale, dimension_numbers, rhs_shape):
-  """Transposes lhs_scale to rhs input dimension order."""
-  if lhs_scale is None:
-    return None
-
-  (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
-  return _scale_trans_for_other_input(
-      lhs_scale, lhs_ca, lhs_ba, rhs_ca, rhs_ba, len(rhs_shape)
-  )
-
-
-def _rhs_scale_transpose_for_lhs_input(rhs_scale, dimension_numbers, lhs_shape):
-  """Transposes lhs_scale to rhs input dimension order."""
-  if rhs_scale is None:
-    return None
-
-  (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
-  return _scale_trans_for_other_input(
-      rhs_scale, rhs_ca, rhs_ba, lhs_ca, lhs_ba, len(lhs_shape)
-  )
-
-
 def _get_scale_t(
     qt: aqt_tensor.QTensor,
     transpose_fn: Any,
     dimension_numbers: lax.DotDimensionNumbers,
     lhs_shape: Sequence[int],
     rhs_shape: Sequence[int],
-) -> aqt_tensor.QTensor:
+) -> Sequence[jnp.ndarray]:
   list_scale_t = []
   for scale in qt.scale:
     scale_t = transpose_fn(scale, dimension_numbers, lhs_shape, rhs_shape)
     list_scale_t.append(scale_t)
-  return qt.replace(scale_t=list_scale_t)
+  return list_scale_t
+
+
+@utils.flax_slots_dataclass
+class DotGeneralQuantizer(abc.ABC):
+  """Abstract class for dot_general quantizer."""
+
+  @abc.abstractmethod
+  def __call__(
+      self,
+      lhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
+      rhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
+  ) -> tuple[
+      tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
+      tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
+  ]:
+    pass
+
+  @abc.abstractmethod
+  def swap_lhs_and_rhs(self) -> None:
+    """Swaps lhs and rhs configuration."""
+    pass
+
+  @abc.abstractmethod
+  def assert_calib_shared_axes_value(
+      self,
+      lhs_val: Sequence[utils.AxisIdx] | None,
+      rhs_val: Sequence[utils.AxisIdx] | None,
+      msg: str,
+  ) -> None:
+    """Asserts if calib_shared_axes have certain values."""
+    pass
+
+  @abc.abstractmethod
+  def set_context(
+      self,
+      lhs_context: utils.Context,
+      rhs_context: utils.Context,
+  ) -> None:
+    """Sets context for lhs and rhs."""
+    pass
+
+
+@utils.flax_slots_dataclass
+class DefaultDotGeneralQuantizer(DotGeneralQuantizer):
+  """Default dot_general quantizer."""
+
+  lhs: aqt_quantizer.Quantizer
+  rhs: aqt_quantizer.Quantizer
+
+  def __call__(
+      self,
+      lhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
+      rhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
+  ) -> tuple[
+      tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
+      tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
+  ]:
+    lhs_input, lhs_ca = lhs_quantization_info
+    rhs_input, rhs_ca = rhs_quantization_info
+    lhs_qt, lhs_quant_grad = self.lhs.quant(lhs_input, calibration_axes=lhs_ca)
+    rhs_qt, rhs_quant_grad = self.rhs.quant(rhs_input, calibration_axes=rhs_ca)
+
+    return (lhs_qt, lhs_quant_grad), (rhs_qt, rhs_quant_grad)
+
+  def swap_lhs_and_rhs(self) -> None:
+    self.lhs, self.rhs = self.rhs, self.lhs
+
+  def assert_calib_shared_axes_value(
+      self,
+      lhs_val: Sequence[utils.AxisIdx] | None,
+      rhs_val: Sequence[utils.AxisIdx] | None,
+      msg: str,
+  ) -> None:
+    assert self.lhs.calib_shared_axes == lhs_val, msg
+    assert self.rhs.calib_shared_axes == rhs_val, msg
+
+  def set_context(
+      self,
+      lhs_context: utils.Context,
+      rhs_context: utils.Context,
+  ) -> None:
+    self.lhs.context = lhs_context
+    self.rhs.context = rhs_context
 
 
 @utils.flax_slots_dataclass
 class DotGeneralRaw:
   """Configuration of quantization of one dot_general without gradient."""
 
   lhs: Tensor
   rhs: Tensor
+  dg_quantizer: DotGeneralQuantizer
   dg_accumulator_dtype: Optional[jnp.dtype] = utils.static_field()
   local_aqt: Optional[LocalAqt] = utils.static_field()
   jax_scope_name: str = utils.static_field()
 
   # Set it to true in order to train with non-None lhs_qt or rhs_qt.
   # Gradient will still flow into lhs_qt and/or rhs_qt, but it may be incorrect.
   # It is a caller responsibility to NOT update these QTensors
   allow_dummy_gradient_into_qtensor: bool = utils.static_field(default=False)
+  dot_general: utils.DotGeneralT = utils.static_field(
+      default=jax.lax.dot_general
+  )
 
   @classmethod
   def make(cls, *args, **kwargs) -> Self:
     return dot_general_raw_make(*args, **kwargs)
 
   @classmethod
   def make_conv_general_dilated(cls, *args, **kwargs) -> Self:
@@ -429,45 +355,64 @@
     with jax.named_scope(self.jax_scope_name):
       (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
       # TODO(lew):
       #  - Use qx.value with the int type.
       #  - Handle qx.value with the int type in an optimized way.
       #  - Add a "FQ" case we multiply qx.value*qx.value_scale (not transposed).
       #  - Can we carry untransposed scale and transpose here?
+      if utils.CALCULATE_SCALE_T_ONLINE:
+        if lhs_qt:
+          assert lhs_qt.scale_t is None
+        if rhs_qt:
+          assert rhs_qt.scale_t is None
+        if isinstance(rhs, MultiTensor):
+          assert rhs.qx.scale_t is None  # pytype: disable=attribute-error
+
       if isinstance(rhs, MultiTensor):
         # We are in gradient code.
         fwd_quantized = rhs.qx.scale_t is not None and len(rhs.qx.scale_t) == 1  # pytype: disable=attribute-error
+        if utils.CALCULATE_SCALE_T_ONLINE:
+          fwd_quantized = rhs.qx.scale is not None and len(rhs.qx.scale) == 1  # pytype: disable=attribute-error
+
         expect_fwd_quantized = self.rhs.use_fwd_quant is not None
         msg = (
             'If fwd is quantized, use_fwd_quant should be either True/False;'
             ' otherwise, use_fwd_quant should be None. Misconfiguration: found'
             f' use_fwd_quant is {self.rhs.use_fwd_quant} in bwd, but fwd'
             f' quantization is {fwd_quantized}.'
         )
         assert fwd_quantized == expect_fwd_quantized, msg
         if self.rhs.use_fwd_quant:
           assert fwd_quantized, msg
+          if utils.CALCULATE_SCALE_T_ONLINE:
+            scale_t = transpose.rhs_scale_transpose_for_lhs_input(
+                rhs.qx.scale[0], dimension_numbers, lhs.shape  # pytype: disable=attribute-error
+            )
+          else:
+            scale_t = rhs.qx.scale_t[0]  # pytype: disable=attribute-error
+
           # Cast rhs scales to lhs dtype when multiplying with lhs. This is to
           # avoid an unexpected upcast when rhs is float32 but lhs is float16.
-          lhs = lhs * rhs.qx.scale_t[0].astype(lhs.dtype)  # pytype: disable=attribute-error
+          lhs = lhs * scale_t.astype(lhs.dtype)  # pytype: disable=attribute-error
+
           # rhs qvalue may be integer. It will be quantized again later, so cast
           # its dtype back to dequant dtype.
           # TODO(yichizh): avoid double quantization and evaluate model quality.
           rhs = rhs.qx.qvalue.astype(rhs.qx.dequant_dtype)  # pytype: disable=attribute-error
         else:
           rhs = rhs.x  # pytype: disable=attribute-error
       else:
         assert self.rhs.use_fwd_quant is None, 'cannot set use_fwd_quant in fwd'
 
       if self.local_aqt is not None:
         local_aqt = self.local_aqt
         factor = local_aqt.contraction_axis_shard_count  # pytype: disable=attribute-error
         msg = 'Custom calib_shared_axes not implemented for local AQT.'
-        assert self.lhs.quantizer.calib_shared_axes is None, msg
-        assert self.rhs.quantizer.calib_shared_axes is None, msg
+        if isinstance(self.dg_quantizer, DefaultDotGeneralQuantizer):
+          self.dg_quantizer.assert_calib_shared_axes_value(None, None, msg)
 
         def factor_reshape(x, ca, ba):
           assert factor is not None
           if len(ca) == 0:
             return x, ca, ba
           shape = list(x.shape)
           ax = ca[0]
@@ -483,88 +428,95 @@
         lhs, lhs_ca, lhs_ba = factor_reshape(lhs, lhs_ca, lhs_ba)
         rhs, rhs_ca, rhs_ba = factor_reshape(rhs, rhs_ca, rhs_ba)
 
         dimension_numbers = (lhs_ca, rhs_ca), (lhs_ba, rhs_ba)
 
       assert isinstance(rhs, jnp.ndarray)
 
-      def _compute_qtensor(
-          inputs: jnp.ndarray,
-          input_qtensor: aqt_tensor.QTensor,
+      def _get_calibration_axes(
           tensor_cfg: Tensor,
           ndim: int,
-          ca: Sequence[int],
-          ba: Sequence[int],
-          transpose_fn: Any,
-      ) -> tuple[aqt_tensor.QTensor, str | aqt_tensor.GradientFn]:
-        """Compute qtensor from input or input_qtensor."""
+          ca: Sequence[utils.AxisIdx],
+          ba: Sequence[utils.AxisIdx],
+      ) -> Sequence[utils.AxisIdx]:
+        """Computes calibration axes for the given Tensor."""
         match tensor_cfg.calibration_mode:
           case CalibrationMode.REMAINING_AXIS:
-            calibration_axes = _get_ra(ndim, ca, ba)
+            calibration_axes = utils.get_remaining_axes(ndim, ca, ba)
           case CalibrationMode.CONTRACTING_AXIS:
             calibration_axes = ca
           case _:
             raise ValueError(
                 f'Unknown calibration mode: {tensor_cfg.calibration_mode}'
             )
+        return calibration_axes
 
+      def _postprocess_qtensor(
+          input_qtensor: Optional[aqt_tensor.QTensor],
+          calculated_qtensor: aqt_tensor.QTensor,
+          quant_grad: aqt_tensor.GradientFn,
+          tensor_cfg: Tensor,
+          transpose_fn: Any,
+      ) -> tuple[aqt_tensor.QTensor, str | aqt_tensor.GradientFn]:
+        """Compute qtensor from input or input_qtensor."""
         if input_qtensor is not None:
-          if self.allow_dummy_gradient_into_qtensor:
-            # quant_grad might be incorrect here, and should not be used.
-            _, quant_grad = tensor_cfg.quantizer.quant(
-                inputs, calibration_axes=calibration_axes
-            )
-          else:
+          if not self.allow_dummy_gradient_into_qtensor:
             quant_grad = (
                 'Poison. '
                 + 'Gradients are not generally expected in serving. '
                 + 'Please set allow_dummy_gradient_into_qtensor to True '
                 + 'if this is the intended behavior.'
             )
           output_qtensor = input_qtensor
         else:
-          output_qtensor, quant_grad = tensor_cfg.quantizer.quant(
-              inputs, calibration_axes=calibration_axes
-          )
+          output_qtensor = calculated_qtensor
         mode = tensor_cfg.calibration_mode
         if (
             output_qtensor.scale_t is None
             and mode == CalibrationMode.CONTRACTING_AXIS
+            and not utils.CALCULATE_SCALE_T_ONLINE
         ):
           msg = 'scale, scale_t cannot be both unknown'
           assert output_qtensor.scale is not None, msg
-          output_qtensor = _get_scale_t(
-              qt=output_qtensor,
-              transpose_fn=transpose_fn,
-              dimension_numbers=dimension_numbers,
-              lhs_shape=lhs.shape,
-              rhs_shape=rhs.shape,
+          output_qtensor = output_qtensor.replace(
+              scale_t=_get_scale_t(
+                  qt=output_qtensor,
+                  transpose_fn=transpose_fn,
+                  dimension_numbers=dimension_numbers,
+                  lhs_shape=lhs.shape,
+                  rhs_shape=rhs.shape,
+              )
           )
         return output_qtensor, quant_grad
 
-      lhs_qt, lhs_quant_grad = _compute_qtensor(
-          lhs,
+      lhs_calib_axes = _get_calibration_axes(self.lhs, lhs.ndim, lhs_ca, lhs_ba)
+      rhs_calib_axes = _get_calibration_axes(self.rhs, rhs.ndim, rhs_ca, rhs_ba)
+
+      lhs_quantized, rhs_quantized = (
+          self.dg_quantizer((lhs, lhs_calib_axes), (rhs, rhs_calib_axes))
+      )
+      lhs_qt_calculated, lhs_quant_grad = lhs_quantized
+      rhs_qt_calculated, rhs_quant_grad = rhs_quantized
+
+      lhs_qt, lhs_quant_grad = _postprocess_qtensor(
           lhs_qt,
+          lhs_qt_calculated,
+          lhs_quant_grad,
           self.lhs,
-          lhs.ndim,
-          lhs_ca,
-          lhs_ba,
-          _lhs_scale_transpose_to_output,
+          transpose.lhs_scale_transpose_to_output,
       )
       lhs_mt = MultiTensor(x=lhs, qx=lhs_qt)
       lhs_res = TensorRes(mt=lhs_mt, quant_grad=lhs_quant_grad)
 
-      rhs_qt, rhs_quant_grad = _compute_qtensor(
-          rhs,
+      rhs_qt, rhs_quant_grad = _postprocess_qtensor(
           rhs_qt,
+          rhs_qt_calculated,
+          rhs_quant_grad,
           self.rhs,
-          rhs.ndim,
-          rhs_ca,
-          rhs_ba,
-          _rhs_scale_transpose_to_output,
+          transpose.rhs_scale_transpose_to_output,
       )
       rhs_mt = MultiTensor(x=rhs, qx=rhs_qt)
       rhs_res = TensorRes(mt=rhs_mt, quant_grad=rhs_quant_grad)
 
       # TODO(lew): mt.x above should be clipped for clipping calibrations
 
       out = _qtensor_dot_general(
@@ -621,29 +573,29 @@
         and rhs_qin.dtype in dtypes_allowed_for_int32_accum
     ), dtype_ms
 
   dtypes_can_be_scaled = [jnp.bfloat16, jnp.float32, jnp.float64]
   if cfg.lhs.dequant_mode == DequantMode.OTHER_INPUT:
     assert rhs_qin.dtype in dtypes_can_be_scaled
     for scale in lhs_qt.scale:
-      transposed_scale = _lhs_scale_transpose_for_rhs_input(
+      transposed_scale = transpose.lhs_scale_transpose_for_rhs_input(
           scale, dimension_numbers, rhs_qt.shape
       )
       assert isinstance(transposed_scale, jnp.ndarray)  # make pytype quiet
       rhs_qin = rhs_qin * transposed_scale.astype(rhs_qin.dtype)
   if cfg.rhs.dequant_mode == DequantMode.OTHER_INPUT:
     assert lhs_qin.dtype in dtypes_can_be_scaled
     for scale in rhs_qt.scale:
-      transposed_scale = _rhs_scale_transpose_for_lhs_input(
+      transposed_scale = transpose.rhs_scale_transpose_for_lhs_input(
           scale, dimension_numbers, lhs_qt.shape
       )
       assert isinstance(transposed_scale, jnp.ndarray)  # make pytype quiet
       lhs_qin = lhs_qin * transposed_scale.astype(lhs_qin.dtype)
 
-  out = lax.dot_general(
+  out = cfg.dot_general(
       lhs_qin,
       rhs_qin,
       dimension_numbers=dimension_numbers,
       preferred_element_type=cfg.dg_accumulator_dtype,
       precision=lax.Precision.DEFAULT,
   )
   # TODO(lew): Do we have a correct precision above?
@@ -653,28 +605,51 @@
       scale=[],
       scale_t=None,
       dequant_dtype=dequant_dtype,
   )
   assert out.scale is not None  # pytype help
 
   if cfg.lhs.dequant_mode == DequantMode.OUTPUT:
-    out.scale.extend(lhs_qt.scale_t)
+    if utils.CALCULATE_SCALE_T_ONLINE:
+      extend_scale = _get_scale_t(
+          qt=lhs_qt,
+          transpose_fn=transpose.lhs_scale_transpose_to_output,
+          dimension_numbers=dimension_numbers,
+          lhs_shape=lhs_qin.shape,
+          rhs_shape=rhs_qin.shape,
+      )
+    else:
+      extend_scale = lhs_qt.scale_t
+
+    out.scale.extend(extend_scale)
   if cfg.rhs.dequant_mode == DequantMode.OUTPUT:
-    out.scale.extend(rhs_qt.scale_t)
+    if utils.CALCULATE_SCALE_T_ONLINE:
+      extend_scale = _get_scale_t(
+          qt=rhs_qt,
+          transpose_fn=transpose.rhs_scale_transpose_to_output,
+          dimension_numbers=dimension_numbers,
+          lhs_shape=lhs_qin.shape,
+          rhs_shape=rhs_qin.shape,
+      )
+    else:
+      extend_scale = rhs_qt.scale_t
+    out.scale.extend(extend_scale)
   return out
 
 
 @utils.flax_slots_dataclass
 class DotGeneral:
   """Configuration of quantization of dot_general and its gradients."""
 
   fwd: DotGeneralRaw
   dlhs: DotGeneralRaw
   drhs: DotGeneralRaw
 
+  apply_custom_vjp_on_jax: bool = utils.static_field(default=True)
+
   @classmethod
   def make(cls, *args, **kwargs) -> Self:
     return dot_general_make(*args, **kwargs)
 
   def dg_core(
       self,
       lhs: jnp.ndarray,
@@ -686,15 +661,24 @@
     """dot_general function with expanded API."""
     msg = 'AQT is not yet optimized to accept quantized types directly. '
     msg += f'lhs.dtype: {lhs.dtype}, rhs.dtype: {rhs.dtype}'
     assert lhs.dtype in [jnp.bfloat16, jnp.float32, jnp.float16], msg
     assert rhs.dtype in [jnp.bfloat16, jnp.float32, jnp.float16], msg
 
     self.assert_config_validity()
-    out, res = _dg_core(lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, self)
+    # TODO(dhchoi): Refactor this to make both branches to have the similar
+    # functionality of applying custom_vjp.
+    if self.apply_custom_vjp_on_jax:
+      dg_core_with_custom_grad = jax.custom_vjp(_dg_core, nondiff_argnums=(4,))
+      dg_core_with_custom_grad.defvjp(dg_core_vjp_fwd, dg_core_vjp_bwd)
+      out, res = dg_core_with_custom_grad(
+          lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, self
+      )
+    else:
+      out, res = _dg_core(lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, self)  # pytype: disable=wrong-arg-types
     return out, res
 
   def __call__(
       self,
       lhs,
       rhs,
       dimension_numbers,
@@ -715,32 +699,33 @@
     )
     return out
 
   def assert_config_validity(self: Self):
     """Asserts if configuration is valid."""
 
     # use_fwd_quant is not enabled when calibration_axis = remaining_axis.
+    expected_fwd_quant = False if utils.CALCULATE_SCALE_T_ONLINE else None
     msg_fwd_quant = (
-        'use_fwd_quant should be set to None when remaining axis are used for'
-        ' calibration axis.'
+        f'use_fwd_quant should be set to {expected_fwd_quant} when remaining'
+        ' axis are used for calibration axis.'
     )
 
     if self.fwd.rhs.calibration_mode == CalibrationMode.REMAINING_AXIS:
       msg_fwd_quant += (
           f'rhs.calibration_mode: {self.fwd.rhs.calibration_mode},'
           f' dlhs use_fwd_quant: {self.dlhs.rhs.use_fwd_quant}'
       )
-      assert self.dlhs.rhs.use_fwd_quant is None, msg_fwd_quant
+      assert self.dlhs.rhs.use_fwd_quant is expected_fwd_quant, msg_fwd_quant
 
     if self.fwd.lhs.calibration_mode == CalibrationMode.REMAINING_AXIS:
       msg_fwd_quant += (
           f'lhs.calibration_mode: {self.fwd.lhs.calibration_mode},'
           f' drhs use_fwd_quant: {self.drhs.rhs.use_fwd_quant}'
       )
-      assert self.drhs.rhs.use_fwd_quant is None, msg_fwd_quant
+      assert self.drhs.rhs.use_fwd_quant is expected_fwd_quant, msg_fwd_quant
 
     # Check valid combination between calibration_mode and dequant_mode
     unsupported_calibration_dequant_pairs = [
         (DequantMode.OUTPUT, CalibrationMode.REMAINING_AXIS),
         (DequantMode.OTHER_INPUT, CalibrationMode.CONTRACTING_AXIS),
     ]
     msg_mode_mismatch = (
@@ -766,33 +751,32 @@
           msg_mode_mismatch
           + ' for rhs. calibration_mode:'
           f' {self.fwd.rhs.calibration_mode}, dequant_mode:'
           f' {self.fwd.rhs.dequant_mode}'
       )
 
 
-@functools.partial(jax.custom_vjp, nondiff_argnums=(4,))
 def _dg_core(
     lhs: jnp.ndarray,
     rhs: jnp.ndarray,
     lhs_qt: Optional[aqt_tensor.QTensor],
     rhs_qt: Optional[aqt_tensor.QTensor],
     dimension_numbers: lax.DotDimensionNumbers,
     cfg: DotGeneral,
 ):
-  out, _ = _dg_core_vjp_fwd(lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, cfg)
+  out, _ = dg_core_vjp_fwd(lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, cfg)
   return out
 
 
 # When defining a vjp, all traceable variables must be input arguments of
 # both the fwd and bwd function.
 # The cfg (DotGeneral) contains the key used for stochastic rounding,
 # which are traceable dynamic variables. It needs to be an input argument
 # to prevent the jax side effect.
-def _dg_core_vjp_fwd(
+def dg_core_vjp_fwd(
     lhs: jnp.ndarray,
     rhs: jnp.ndarray,
     lhs_qt: Optional[aqt_tensor.QTensor],
     rhs_qt: Optional[aqt_tensor.QTensor],
     dimension_numbers: lax.DotDimensionNumbers,
     cfg: DotGeneral,
 ):
@@ -810,15 +794,15 @@
   ret = ret.astype(lhs.dtype)
   # We return these values to allow for materialization.
   assert res is not None, 'res cannot be None in fwd pass.'
   qret = (res.lhs.mt.qx, res.rhs.mt.qx)
   return ((ret, qret), (res, cfg))
 
 
-def _dg_core_vjp_bwd(
+def dg_core_vjp_bwd(
     fwd_dimension_numbers: lax.DotDimensionNumbers,
     res: tuple[Optional[DotGeneralRes], DotGeneral],
     g,
 ):
   """custom_vjp bwd pass."""
   dg_res, cfg = res
   msg = 'dg_res can only be None in 2nd derivative. It is not yet supported.'
@@ -840,16 +824,16 @@
     y_ndim = y_res.mt.x.ndim
 
     (x_ca, y_ca), (x_ba, y_ba) = fwd_dimension_numbers
     if y_is_lhs:
       (y_ca, x_ca) = (x_ca, y_ca)
       (y_ba, x_ba) = (x_ba, y_ba)
     g_ndim = g.ndim - y_ndim + len(x_ba) + 2 * len(x_ca)
-    x_ra = tuple(_get_ra(g_ndim, x_ca, x_ba))
-    y_ra = tuple(_get_ra(y_ndim, y_ca, y_ba))
+    x_ra = tuple(utils.get_remaining_axes(g_ndim, x_ca, x_ba))
+    y_ra = tuple(utils.get_remaining_axes(y_ndim, y_ca, y_ba))
     if y_is_lhs:
       g_ba, g_ca, _ = ranges_like(x_ba, y_ra, x_ra)
     else:
       g_ba, _, g_ca = ranges_like(x_ba, x_ra, y_ra)
     dims = ((g_ca, y_ra), (g_ba, y_ba))
 
     out, _ = dg_raw(g, y_res.mt, None, None, dims)
@@ -875,21 +859,13 @@
   )
   # fwd_dimension_numbers are marked as nondiff_argnums instead of returning
   # None as grad to it. This is because it is a tuple of Python integers
   # that cannot be traced by Jax.
   return (dlhs, drhs, None, None, None)
 
 
-_dg_core.defvjp(_dg_core_vjp_fwd, _dg_core_vjp_bwd)
-
-
 def make_dot_general(dg: Optional[DotGeneral]):
   # TODO(lew): call warnings.warn("Deprecated")
   if dg is None:
     return jax.lax.dot_general
   else:
     return dg
-
-
-def assert_config_validity(cfg):
-  # TODO(lew): call warnings.warn("Deprecated")
-  cfg.assert_config_validity()
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/aqt_dot_general_test.py` & `aqtp-0.7.0/aqt/jax/v2/aqt_dot_general_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 import copy
 import functools
 from typing import Callable
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.jax.v2 import aqt_quantizer
+from aqt.jax.v2 import calibration
 from aqt.jax.v2 import config
 from aqt.jax.v2 import stochastic_rounding
+from aqt.jax.v2 import utils
 import aqt.jax.v2.aqt_conv_general as aqt_conv
 import aqt.jax.v2.aqt_dot_general as aqt
 from aqt.jax.v2.numerics import int_numerics
 from aqt.jax.v2.numerics import no_numerics
 from aqt.jax.v2.numerics import numerics
 import flax.linen.linear as fl
 import flax.struct
@@ -55,20 +57,20 @@
   trityps = [trityp for trityp in jaxpr_to_trityp(f_jaxpr)]
   assert len(trityps) == len(cfgs)
   for (lhs_sa, rhs_sa, out_sa), cfg in zip(trityps, cfgs):
     # If cfg has None, the type is inherited from the arguments' type.
     def assert_dtype_eq(dtype1, dtype2):
       assert dtype1 == dtype2, f"dtype1 != dtype2: {dtype1=} != {dtype2=}"
 
-    assert_dtype_eq(
-        lhs_sa.dtype, cfg.lhs.quantizer.numerics.get_dtype() or float_dtype
-    )
-    assert_dtype_eq(
-        rhs_sa.dtype, cfg.rhs.quantizer.numerics.get_dtype() or float_dtype
-    )
+    assert isinstance(cfg.dg_quantizer, aqt.DefaultDotGeneralQuantizer)
+
+    lhs_dtype = cfg.dg_quantizer.lhs.numerics.get_dtype()
+    rhs_dtype = cfg.dg_quantizer.rhs.numerics.get_dtype()
+    assert_dtype_eq(lhs_sa.dtype, lhs_dtype or float_dtype)
+    assert_dtype_eq(rhs_sa.dtype, rhs_dtype or float_dtype)
     assert_dtype_eq(out_sa.dtype, cfg.dg_accumulator_dtype or float_dtype)
 
 
 def rand_unif(shape, maxval, seed, dtype=jnp.float32):
   key = jax.random.PRNGKey(seed)
   return jax.random.uniform(
       key=key, shape=shape, minval=-maxval, maxval=maxval, dtype=dtype
@@ -184,40 +186,42 @@
     fwd_lhs_tricky_clip_and_round: bool = False,
     local_aqt: aqt.LocalAqt | None = None,
     clip_gradient: bool = False,
 ) -> aqt.DotGeneral:
   cfg = copy.deepcopy(readonly_cfg)
   if fwd_lhs_tricky_clip_and_round:
     # Tricky means that we have zero gradient on x < 0
-    cfg.fwd.lhs.quantizer.numerics = _TrickyNumerics()
+    cfg.fwd.dg_quantizer.lhs.numerics = _TrickyNumerics()
     cfg.fwd.dg_accumulator_dtype = None
 
   # Setting po2_scale is ensuring that fake_quant and full dot_general
   # have the same numerics when scales are power of two (po2).
   # We are passing dims to config so that we can reuse it in fake_quant.
   # Power-of-2 scales allow FQ and AQT to be exactly the same.
   def _apply_po2_scale(c):
-    c.lhs.quantizer.po2_scale = True
-    c.rhs.quantizer.po2_scale = True
+    c.dg_quantizer.lhs.po2_scale = True
+    c.dg_quantizer.rhs.po2_scale = True
 
   def _apply_dequant_mode(c, lhs_dequant_mode, rhs_dequant_mode):
     c.lhs.dequant_mode = lhs_dequant_mode
     c.rhs.dequant_mode = rhs_dequant_mode
 
-  def _apply_calibration_mode(
-      c, lhs_calibration_mode, rhs_calibration_mode
-  ):
+  def _apply_calibration_mode(c, lhs_calibration_mode, rhs_calibration_mode):
     c.lhs.calibration_mode = lhs_calibration_mode
     c.rhs.calibration_mode = rhs_calibration_mode
 
   def _disable_quant_types(c, on_lhs=True, on_rhs=True):
     if on_lhs:
-      c.lhs.quantizer.numerics = c.lhs.quantizer.numerics.replace(dtype=None)
+      c.dg_quantizer.lhs.numerics = (
+          c.dg_quantizer.lhs.numerics.replace(dtype=None)
+      )
     if on_rhs:
-      c.rhs.quantizer.numerics = c.rhs.quantizer.numerics.replace(dtype=None)
+      c.dg_quantizer.rhs.numerics = (
+          c.dg_quantizer.rhs.numerics.replace(dtype=None)
+      )
     if on_lhs or on_rhs:
       c.dg_accumulator_dtype = None
 
   disable_lhs_quant = lhs_dequant_mode == aqt.DequantMode.THIS_INPUT
   disable_rhs_quant = rhs_dequant_mode == aqt.DequantMode.THIS_INPUT
   for c in [cfg.fwd, cfg.dlhs, cfg.drhs]:
     _apply_po2_scale(c)
@@ -229,48 +233,50 @@
 
   if use_fwd_quant is not None:
     # If we disable all rounding, we are just testing whether the scales are
     # correct. We don't even need to disable clipping and we are testing
     # that the scales are not too large.
     def disable_quant(c):
       _disable_quant_types(c)
-      if isinstance(c.lhs.quantizer.numerics, int_numerics.IntNumerics):
-        c.lhs.quantizer.numerics = c.lhs.quantizer.numerics.replace(round=False)
-      if isinstance(c.rhs.quantizer.numerics, int_numerics.IntNumerics):
-        c.rhs.quantizer.numerics = c.rhs.quantizer.numerics.replace(round=False)
-      # c.lhs.quantizer.numerics.clip = False
-      # c.rhs.quantizer.numerics.clip = False
+      if isinstance(c.dg_quantizer.lhs.numerics, int_numerics.IntNumerics):
+        c.dg_quantizer.lhs.numerics = (
+            c.dg_quantizer.lhs.numerics.replace(round=False)
+        )
+      if isinstance(c.dg_quantizer.rhs.numerics, int_numerics.IntNumerics):
+        c.dg_quantizer.rhs.numerics = (
+            c.dg_quantizer.rhs.numerics.replace(round=False)
+        )
 
     disable_quant(cfg.fwd)
     disable_quant(cfg.dlhs)
     disable_quant(cfg.drhs)
     lhs_quant = not isinstance(
-        cfg.fwd.lhs.quantizer.numerics, no_numerics.NoNumerics
+        cfg.fwd.dg_quantizer.lhs.numerics, no_numerics.NoNumerics
     )
     rhs_quant = not isinstance(
-        cfg.fwd.rhs.quantizer.numerics, no_numerics.NoNumerics
+        cfg.fwd.dg_quantizer.rhs.numerics, no_numerics.NoNumerics
     )
     if lhs_quant:
       cfg.drhs.rhs.use_fwd_quant = use_fwd_quant
     if rhs_quant:
       cfg.dlhs.rhs.use_fwd_quant = use_fwd_quant
   if local_aqt is not None:
     # Currently we are not supporting local_aqt in fwd pass
     # cfg.fwd.local_aqt = local_aqt
     cfg.dlhs.local_aqt = local_aqt
     cfg.drhs.local_aqt = local_aqt
 
     # When using abs-max scaling, this should be a no-op.
-  if isinstance(cfg.fwd.lhs.quantizer.numerics, int_numerics.IntNumerics):
-    cfg.fwd.lhs.quantizer.numerics = cfg.fwd.lhs.quantizer.numerics.replace(
-        clip_gradient=clip_gradient
-    )
-  if isinstance(cfg.fwd.rhs.quantizer.numerics, int_numerics.IntNumerics):
-    cfg.fwd.rhs.quantizer.numerics = cfg.fwd.rhs.quantizer.numerics.replace(
-        clip_gradient=clip_gradient
+  if isinstance(cfg.fwd.dg_quantizer.lhs.numerics, int_numerics.IntNumerics):
+    cfg.fwd.dg_quantizer.lhs.numerics = (
+        cfg.fwd.dg_quantizer.lhs.numerics.replace(clip_gradient=clip_gradient)
+    )
+  if isinstance(cfg.fwd.dg_quantizer.rhs.numerics, int_numerics.IntNumerics):
+    cfg.fwd.dg_quantizer.rhs.numerics = (
+        cfg.fwd.dg_quantizer.rhs.numerics.replace(clip_gradient=clip_gradient)
     )
 
   return cfg
 
 
 def _aqt_dg_full_lr_diff(
     lhs_dequant_mode: aqt.DequantMode,
@@ -373,24 +379,24 @@
       preserve_zero=[True, False],
       prec=[1, 2, 4, 8],
       v=[0.1, 1000.0],
       seed=list(range(10)),
   )
   def test_fq_noise(self, preserve_zero, prec, v, seed):
     key = jax.random.PRNGKey(seed)
-    cfg = config.tensor_make(prec)
-    if isinstance(cfg.quantizer.numerics, int_numerics.IntNumerics):
-      cfg.quantizer.numerics.preserve_zero = preserve_zero
+    quantizer = config.quantizer_make(prec)
+    if isinstance(quantizer.numerics, int_numerics.IntNumerics):
+      quantizer.numerics.preserve_zero = preserve_zero
       if not preserve_zero:
-        cfg.quantizer.numerics.dtype = None
-    cfg.quantizer.calib_shared_axes = (0,)
+        quantizer.numerics.dtype = None
+    quantizer.calib_shared_axes = (0,)
     sample_size = 10000
     shape = (sample_size,)
     a = jax.random.uniform(key, shape, minval=-v, maxval=v)
-    a_fq = aqt_quantizer.make_fake_quant(cfg)(a)
+    a_fq = aqt_quantizer.make_fake_quant(quantizer)(a)
     bucket_noise = a_fq - a  #  ~ U(-bucket_size/2, bucket_size/2)
     bucket_count = (2**prec - 1) if preserve_zero else (2**prec)
     bucket_size = (v * 2) / bucket_count
     noise = bucket_noise / bucket_size + 0.5  # ~U(0, 1)
     pvalue = scipy.stats.kstest(noise, "uniform").pvalue
     assert pvalue > 0.01
 
@@ -421,20 +427,20 @@
   ])
   def test_fake_quant(
       self,
       bits=4,
       maxval=10.0,
       shape=(20, 1),
   ):
-    cfg = config.tensor_make(bits)
-    cfg.quantizer.po2_scale = True
-    cfg.quantizer.calib_shared_axes = (0,)
+    quantizer = config.quantizer_make(bits)
+    quantizer.po2_scale = True
+    quantizer.calib_shared_axes = (0,)
     x = jnp.linspace(-maxval, maxval, num=shape[0]).reshape(shape)
     grad = jnp.ones(shape) * 12345.0
-    x_fq, backprop = jax.vjp(aqt_quantizer.make_fake_quant(cfg), x)
+    x_fq, backprop = jax.vjp(aqt_quantizer.make_fake_quant(quantizer), x)
     gx_fq = backprop(grad)
     # print(f"x     =\n{x}")
     # print(f"x_fq  =\n{x_fq}")
     # print(f"grad  =\n{grad}")
     # print(f"gx_fq =\n{gx_fq}")
     del x
     del x_fq
@@ -465,14 +471,15 @@
       dict(cfg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
       # That test could fail numerically because bf16
       # can't keep in the product of int8*int8 accurately.
       # It just so happens that this test does not fail but others do.
       # We do this test anyway, to catch jax-compilation-time errors.
       dict(cfg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
       dict(cfg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
+      dict(cfg=config.dot_general_make(8, 8), calculate_scale_t_online=True),
       dict(cfg=config.dot_general_make(None, 8)),
       dict(cfg=config.dot_general_make(8, None)),
       dict(
           cfg=fqt_param_dict(s=10, use_fwd_quant=True)["cfg"],
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
@@ -517,18 +524,21 @@
       # gra_shape=(1, 3),  # has to be the shape of the output
       lhs_shape=(10, 20),
       rhs_shape=(20, 30),
       gra_shape=(10, 30),  # has to be the shape of the output
       seed=0,
       dtype=jnp.float32,
       clip_gradient=False,
+      calculate_scale_t_online=False,
   ):
     readonly_cfg = cfg
     del cfg
 
+    utils.CALCULATE_SCALE_T_ONLINE = calculate_scale_t_online
+
     lhs = rand_unif(lhs_shape, lhs_maxval, seed, dtype)
     rhs = rand_unif(rhs_shape, rhs_maxval, seed + 1, dtype)
     gra = rand_unif(gra_shape, gra_maxval, seed + 2, dtype)
 
     # Prepare utility functions for test.
     aqt_dg_full = functools.partial(
         _aqt_dg_full,
@@ -598,15 +608,16 @@
             "default    ",
             aqt_dg_full(aqt.DequantMode.THIS_INPUT, local_aqt=aqt.LocalAqt(2)),
             dict(),
         ),
     ])
 
     if isinstance(
-        readonly_cfg.fwd.lhs.quantizer.numerics, int_numerics.IntNumerics
+        readonly_cfg.fwd.dg_quantizer.lhs.numerics,
+        int_numerics.IntNumerics,
     ):
       check([
           (
               "check_fwd_lhs_tricky_clip_and_round",
               aqt_dg_full(
                   aqt.DequantMode.OUTPUT, fwd_lhs_tricky_clip_and_round=True
               ),
@@ -624,15 +635,15 @@
     check([
         ("unquantized default:", unquant_aqt_dg, dict()),
         ("lax.dot_general:", lax_dg, dict()),
     ])
 
   @parameterized.parameters([
       dict(
-          cfg=config.config_v3(
+          cfg=lambda: config.config_v3(
               fwd_bits=3,
               dlhs_bits=4,
               drhs_bits=5,
               drhs_accumulator_dtype=jnp.int32,  # overwriting the default None
           )
       ),
       dict(cfg=config.dot_general_make(None, None)),
@@ -646,43 +657,64 @@
       dict(cfg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
       # That test could fail numerically because bf16
       # can't keep in the product of int8*int8 accurately.
       # It just so happens that this test does not fail but others do.
       # We do this test anyway, to catch jax-compilation-time errors.
       dict(cfg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
       dict(cfg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
+      dict(cfg=config.dot_general_make(8, 8), calculate_scale_t_online=True),
       dict(cfg=config.dot_general_make(None, 8)),
       dict(cfg=config.dot_general_make(8, None)),
       dict(
           cfg=config.dot_general_make(2, 2),
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
       *[fqt_param_dict(s, use_fwd_quant=None) for s in range(10)],
   ])
   def test_dot_general_calibration_with_remaining_axis(
       self,
-      cfg: config.DotGeneral,
+      cfg: config.DotGeneral | Callable[[], config.DotGeneral],
       lhs_maxval=10.0,
       rhs_maxval=20.0,
       gra_maxval=30.0,
       dims=(((1,), (0,)), ((), ())),  # classical matmul
       lhs_shape=(10, 20),
       rhs_shape=(20, 30),
       gra_shape=(10, 30),  # has to be the shape of the output
       seed=0,
       dtype=jnp.float32,
       clip_gradient=False,
+      calculate_scale_t_online=False,
   ):
-    # Set use_fwd_quant to None.
-    cfg.drhs.rhs.use_fwd_quant = None
-    cfg.dlhs.rhs.use_fwd_quant = None
+    # Deferred evaluation of config function calls. 4-bit config initialization
+    # triggers jax.local_devices(), which shouldn't be called before
+    # absl.app.run() in some environments.
+    if not isinstance(cfg, config.DotGeneral):
+      cfg = cfg()
+    # use_fwd_quant is not supported yet for calibration_with_remaining_axis.
+    # We should set the flag values to None in case CALCULATE_SCALE_T_ONLINE is
+    # False; the MultiTensor won't have the scale_t values so the backward
+    # dot_general would consider it as not quantized.
+    # If CALCULATE_SCALE_T_ONLINE is True, the MultiTensor won't have the
+    # the scale_t value neither, but the assertion will check the existence of
+    # scale value to see if the tensor is quantized or not. So in this case the
+    # use_fwd_quant flag should set to False, since the input MultiTensor is
+    # quantized but we do not support use_fwd_quant.
+    # Set use_fwd_quant to None in case .
+    utils.CALCULATE_SCALE_T_ONLINE = calculate_scale_t_online
+    if utils.CALCULATE_SCALE_T_ONLINE:
+      cfg.drhs.rhs.use_fwd_quant = False
+      cfg.dlhs.rhs.use_fwd_quant = False
+    else:
+      cfg.drhs.rhs.use_fwd_quant = None
+      cfg.dlhs.rhs.use_fwd_quant = None
     readonly_cfg = cfg
     del cfg
 
     lhs = rand_unif(lhs_shape, lhs_maxval, seed, dtype)
     rhs = rand_unif(rhs_shape, rhs_maxval, seed + 1, dtype)
     gra = rand_unif(gra_shape, gra_maxval, seed + 2, dtype)
 
@@ -960,16 +992,16 @@
           (((1,), (0,)), ((), ())),
       )
       return ret
 
     lhs = rand_unif((10, 20), 1.0, seed)
     rhs = rand_unif((20, 30), 1.0, seed + 1)
     test_jaxpr_dtype(lambda: dg(lhs, rhs), [cfg], lhs.dtype)
-    assert cfg.lhs.quantizer.numerics.get_dtype() == jnp.int8
-    assert cfg.rhs.quantizer.numerics.get_dtype() == jnp.int8
+    assert cfg.dg_quantizer.lhs.numerics.get_dtype() == jnp.int8
+    assert cfg.dg_quantizer.rhs.numerics.get_dtype() == jnp.int8
 
   @parameterized.parameters([
       (1, 1),
       (1, 2),
       (2, 1),
       (2, 2),
       (8, 8),
@@ -985,33 +1017,33 @@
       rhs_maxval=20.0,
       seed=0,
   ):
     cfg = config.conv_general_dilated_make(2, lhs_bits, rhs_bits)
 
     if cfg.lhs:
       # Power-of-2 scales allow FQ and AQT to be exactly the same.
-      cfg.lhs.quantizer.po2_scale = True
+      cfg.dg_quantizer.lhs.po2_scale = True
     if cfg.rhs:
-      cfg.rhs.quantizer.po2_scale = True
+      cfg.dg_quantizer.rhs.po2_scale = True
 
     batch_n = 10
     contr_n = 20
     feature_n = 30
     lhs = rand_unif((batch_n, 4, 5, contr_n), lhs_maxval, seed)
     rhs = rand_unif((3, 3, contr_n, feature_n), rhs_maxval, seed + 1)
 
     lax_conv = jax.lax.conv_general_dilated
     aqt_conv_fn = aqt_conv.make_conv_general_dilated(cfg)
     kwargs = {
         "window_strides": (1, 1),
         "padding": "SAME",
         "dimension_numbers": fl._conv_dimension_numbers(lhs.shape),
     }
-    lhs_fq = aqt_quantizer.make_fake_quant(cfg.lhs)(lhs)
-    rhs_fq = aqt_quantizer.make_fake_quant(cfg.rhs)(rhs)
+    lhs_fq = aqt_quantizer.make_fake_quant(cfg.dg_quantizer.lhs)(lhs)
+    rhs_fq = aqt_quantizer.make_fake_quant(cfg.dg_quantizer.rhs)(rhs)
     prod_fq = lax_conv(lhs_fq, rhs_fq, **kwargs)
     prod_aqt = aqt_conv_fn(lhs, rhs, **kwargs)
     assert (prod_aqt == prod_fq).all()
 
   @parameterized.parameters([
       dict(
           shard_count=2,
@@ -1029,99 +1061,63 @@
     # set the number of shards (local aqt) to 2
     cfg = config.fully_quantized(
         fwd_bits=8,
         bwd_bits=8,
         use_stochastic_rounding=False,
         drhs_local_aqt=aqt.LocalAqt(shard_count),
     )
-    cfg.fwd.lhs.quantizer.numerics = cfg.fwd.lhs.quantizer.numerics.replace(
-        preserve_max_val=True
+    cfg.fwd.dg_quantizer.lhs.numerics = (
+        cfg.fwd.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
     )
-    cfg.fwd.rhs.quantizer.numerics = cfg.fwd.rhs.quantizer.numerics.replace(
-        preserve_max_val=True
+    cfg.fwd.dg_quantizer.rhs.numerics = (
+        cfg.fwd.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
     )
-    cfg.drhs.lhs.quantizer.numerics = cfg.drhs.lhs.quantizer.numerics.replace(
-        preserve_max_val=True
+    cfg.drhs.dg_quantizer.lhs.numerics = (
+        cfg.drhs.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
     )
-    cfg.drhs.rhs.quantizer.numerics = cfg.drhs.rhs.quantizer.numerics.replace(
-        preserve_max_val=True
+    cfg.drhs.dg_quantizer.rhs.numerics = (
+        cfg.drhs.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
     )
     dg = lambda lhs, rhs: aqt.make_dot_general(cfg)(
         lhs,
         rhs,
         dimension_numbers=(((), ()), ((), ())),
     )
     lhs = jnp.array(lhs)
     rhs = jnp.array([1.0])
     output, bprop = jax.vjp(dg, lhs, rhs)
     _, drhs = bprop(jnp.ones_like(output))
     assert drhs == expected_product
 
-  @parameterized.parameters(
-      # 'bmnts,bsnh->bmtnh'
-      (
-          (2, 3, 4, 5, 6),
-          (2, 6, 4, 1),
-          (((4,), (1,)), ((0, 2), (0, 2))),
-          (2, 1, 4, 1, 6),
-      ),
-      # 'bmkgts,bskh->bmtkgh'
-      (
-          (2, 3, 4, 5, 6, 7),
-          (2, 7, 4, 1),
-          (((5,), (1,)), ((0, 2), (0, 2))),
-          (2, 1, 4, 1, 1, 7),
-      ),
-  )
-  def test_rhs_scale_transpose_for_lhs_input(
-      self, lhs_shape, rhs_scale_shape, dimension_numbers, expected_shape
-  ):
-    lhs = jnp.zeros(lhs_shape)
-    rhs_scale = jnp.zeros(rhs_scale_shape)
-    result = aqt._rhs_scale_transpose_for_lhs_input(
-        rhs_scale, dimension_numbers, lhs.shape
+  def test_per_tensor(self):
+    # TODO(lew): bits=8 started failing in VLP colab due x/x != 1.0 sometimes
+    bits = 4
+    my_numerics = int_numerics.IntNumerics(
+        bits=bits,
+        preserve_zero=True,
+        preserve_max_val=False,
+        clip=True,
+        clip_gradient=False,
+        round=True,
+        noise_fn=None,
+        dtype=jnp.int8,
+    )
+    quantizer = aqt_quantizer.Quantizer(
+        numerics=my_numerics,
+        calib_shared_axes="per_tensor",
+        scale_stop_grad=True,
+        calibration=calibration.AbsMaxCalibration,
+        po2_scale=False,
+        context=utils.Context(key=None, train_step=None),
     )
 
-    self.assertEqual(result.shape, expected_shape)
-
-  @parameterized.parameters(
-      # 'bmnts,bsnh->bmtnh'
-      (
-          (2, 1, 4, 1, 3),
-          (2, 3, 4, 5),
-          (((4,), (1,)), ((0, 2), (0, 2))),
-          (2, 3, 4, 1),
-      ),
-      # 'bmkgts,bskh->bmtkgh'
-      (
-          (2, 1, 4, 1, 1, 3),
-          (2, 3, 4, 5),
-          (((5,), (1,)), ((0, 2), (0, 2))),
-          (2, 3, 4, 1),
-      ),
-  )
-  def test_lhs_scale_transpose_for_rhs_input(
-      self, lhs_scale_shape, rhs_shape, dimension_numbers, expected_shape
-  ):
-    lhs_scale = jnp.zeros(lhs_scale_shape)
-    rhs = jnp.zeros(rhs_shape)
-    result = aqt._lhs_scale_transpose_for_rhs_input(
-        lhs_scale, dimension_numbers, rhs.shape
-    )
-
-    self.assertEqual(result.shape, expected_shape)
-
-  def test_per_tensor_quant(self):
     x = jnp.array([
         [1, 2, 3, 4],
-        [5, 6, 7, 8],
-        [3, 5, 1, 127.5],
+        [5, 6, 7, 2 ** (bits - 1) - 0.5],
+        [3, 5, 1, -1],
     ])
-    cfg = config.dot_general_make(lhs_bits=8, rhs_bits=8)
-    cfg.fwd.lhs.quantizer.calib_shared_axes = "per_tensor"
-    # calibration_axes will not be used when cfg.calib_shared_axes is set
-    y, _ = cfg.fwd.lhs.quantizer.quant(x, calibration_axes=None)
-    self.assertEqual(y.scale[0], jnp.array([[1.0]]))
+    qx, _ = quantizer.quant(x, calibration_axes=None)
+    self.assertEqual(qx.scale, [jnp.array([[1.0]])])
 
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/aqt_quantizer.py` & `aqtp-0.7.0/aqt/jax/v2/aqt_quantizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,62 +9,60 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Configuration dataclasses."""
 
-from typing import Literal
+from typing import Literal, Sequence
 from aqt.jax.v2 import aqt_tensor
 from aqt.jax.v2 import calibration
 from aqt.jax.v2 import utils
+from aqt.jax.v2.numerics import int_numerics
 from aqt.jax.v2.numerics import no_numerics
 from aqt.jax.v2.numerics import numerics
 import jax
 import jax.numpy as jnp
 
 
 AbstractAqtNumerics = numerics.AqtNumerics
 AbstractAqtCalibration = calibration.Calibration
 
 
 @utils.flax_slots_dataclass
-class Context:
-  key: jax.Array | None = utils.dynamic_field()
-  train_step: int | None = utils.dynamic_field()
-
-
-@utils.flax_slots_dataclass
 class Quantizer:
   """Configuration of quantization of one tensor."""
 
   numerics: AbstractAqtNumerics = utils.static_field()
-  calib_shared_axes: list[int] | Literal["per_tensor"] | None = (
+  calib_shared_axes: Sequence[utils.AxisIdx] | Literal["per_tensor"] | None = (
       utils.static_field()
   )
   scale_stop_grad: bool = utils.static_field()
   # noise+clip+round
   # We apply gradient of clip_and_round in bwd pass.
-  calibration: AbstractAqtCalibration = utils.static_field()
+  calibration: type[AbstractAqtCalibration] = utils.static_field()
   # Round up the calibration to power of 2 (po2).
   po2_scale: bool = utils.static_field()
   # TODO(yichizh): Factor out auxilliary dataclasses into a separate file.
-  context: Context
+  context: utils.Context
 
   # TODO(yichizh): Need to add type annotation back to cfg.
   def quant(
       self,
       x,
       *,
       calibration_axes,
   ) -> tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn]:
     """The core quantizing function."""
     if isinstance(self.numerics, no_numerics.NoNumerics):
       qt = aqt_tensor.QTensor(
-          qvalue=x, scale=[], scale_t=[], dequant_dtype=x.dtype
+          qvalue=x,
+          scale=[],
+          scale_t=None if utils.CALCULATE_SCALE_T_ONLINE else [],
+          dequant_dtype=x.dtype
       )
       return qt, None
 
     qt = self.calculate_scale(x, calibration_axes=calibration_axes)
     qt, quant_grad = self.calculate_qvalue(x, qt)
     return qt, quant_grad
 
@@ -79,15 +77,17 @@
     # TODO(lew): We should cast earlier. xhs_q should be in cfg.xhs.dtype
     # TODO(lew): After we implement optimization to not double-quantize,
     #   what would happen if we pass fq value (xhs_q2) in residual?
     if self.calib_shared_axes == "per_tensor":
       shared_axes = list(range(x.ndim))
     else:
       shared_axes = self.calib_shared_axes or calibration_axes
-    bound = self.calibration.get_bound(x, shared_axes)
+
+    calibrator = self.calibration()
+    bound = calibrator.get_bound(x, shared_axes, self.context)
     abs_max_mapped_to = self.numerics.abs_val_mapped_to()
     scale = bound / abs_max_mapped_to
 
     if self.po2_scale:
       # With floor the biggest value (we are using jnp.max) is in the range of
       # clipping and therefore have a correct gradinet.
       scale = 2 ** jnp.floor(jnp.log2(jax.lax.reciprocal(scale)))
@@ -118,13 +118,42 @@
     x_q, res = self.numerics.vjp_fwd(qt.qvalue, self.context)
     quant_grad = jax.tree_util.Partial(self.numerics.vjp_bwd, res)
 
     qt = qt.replace(qvalue=x_q)
     return qt, quant_grad
 
 
-def make_fake_quant(cfg, calibration_axes=None):
+def quantizer_make(
+    n_bits: int | None, preserve_max_val: bool = False
+) -> Quantizer:
+  """Makes Quantizer."""
+  if n_bits is None:
+    effective_numerics = no_numerics.NoNumerics()
+  else:
+    pz = False if n_bits == 1 else True
+    dtype = utils.infer_dtype_from_bits(n_bits, upcast=False) if pz else None
+    effective_numerics = int_numerics.IntNumerics(
+        bits=n_bits,
+        preserve_zero=pz,
+        preserve_max_val=preserve_max_val,
+        clip=True,
+        round=True,
+        noise_fn=None,
+        clip_gradient=False,  # This can be disabled when using abs-max scaling.
+        dtype=dtype,
+    )
+  return Quantizer(
+      numerics=effective_numerics,
+      calib_shared_axes=None,
+      scale_stop_grad=True,
+      calibration=calibration.AbsMaxCalibration,
+      po2_scale=False,
+      context=utils.Context(key=None, train_step=None),
+  )
+
+
+def make_fake_quant(quantizer: Quantizer, calibration_axes=None):
   def fake_quant(x):
-    x_q, _ = cfg.quantizer.quant(x, calibration_axes=calibration_axes)
+    x_q, _ = quantizer.quant(x, calibration_axes=calibration_axes)
     return x_q.dequant()
 
   return fake_quant
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/aqt_tensor.py` & `aqtp-0.7.0/aqt/jax/v2/aqt_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,22 +130,22 @@
 
 def zeros(
     shape: Sequence[int], qdtype: jnp.dtype, dequant_dtype: jnp.dtype
 ) -> QTensor:
   return QTensor(
       qvalue=jnp.zeros(shape, dtype=qdtype),
       scale=[],
-      scale_t=[],
+      scale_t=None if utils.CALCULATE_SCALE_T_ONLINE else [],
       dequant_dtype=dequant_dtype,
   )
 
 
 def zeros_with_scale(
     shape: Sequence[int],
-    calibration_axis: Sequence[int],
+    calibration_axis: Sequence[utils.AxisIdx],
     qdtype: jnp.dtype,
     dequant_dtype: jnp.dtype,
 ) -> QTensor:
   """Initializes a QTensor with empty qvalue along with empty scale value."""
   scale_shape = list(shape)
   for axis in calibration_axis:
     scale_shape[axis] = 1
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/aqt_tensor_test.py` & `aqtp-0.7.0/aqt/jax/v2/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/calibration.py` & `aqtp-0.7.0/aqt/jax/v2/calibration.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,33 +10,47 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Quantization calibration methods."""
 
 import abc
-from typing import Union
+from typing import Union, Sequence
 from aqt.jax.v2 import utils
 import jax.numpy as jnp
 
 
+@utils.flax_slots_dataclass
 class Calibration(abc.ABC):
+  """Abstract class for calibration."""
 
   @abc.abstractmethod
-  def get_bound(self, x, shared_axes) -> jnp.ndarray:
+  def get_bound(
+      self,
+      x: jnp.ndarray,
+      shared_axes: Sequence[utils.AxisIdx] | None,
+      context: utils.Context | None = None
+  ) -> jnp.ndarray:
     pass
 
 
 @utils.flax_slots_dataclass
 class ConstantCalibration(Calibration):
+  """Calibration with a constant value."""
+
   bound: Union[jnp.ndarray, float]
 
-  def get_bound(self, x, shared_axes) -> jnp.ndarray:
+  def get_bound(
+      self,
+      x: jnp.ndarray,
+      shared_axes: Sequence[utils.AxisIdx] | None,
+      context: utils.Context | None = None,
+  ) -> jnp.ndarray:
     """Calibration."""
-    del shared_axes
+    del shared_axes, context
     assert self.bound > 0, 'Bound should be positive.'
     # TODO(yichizh): hardcode bf16 for the scales, subject to quality evaluation
     return jnp.asarray(self.bound).reshape((1,) * len(x.shape)).astype(x.dtype)
 
 
 @utils.flax_slots_dataclass
 class AbsMaxCalibration(Calibration):
@@ -45,16 +59,23 @@
   Attributes:
     scale: Set it to something like 0.3, 0.1, 0.03. If scale < 1.0, setting
       IntNumerics.clip_gradient=True is likely to be important.
   """
 
   scale: float | None = None
 
-  def get_bound(self, x, shared_axes) -> jnp.ndarray:
+  def get_bound(
+      self,
+      x: jnp.ndarray,
+      shared_axes: Sequence[utils.AxisIdx] | None,
+      context: utils.Context | None = None,
+  ) -> jnp.ndarray:
     """Calibration."""
+    del context
+
     msg = (
         'Perhaps you are using DequantMode.THIS_INPUT (fake_quant) and forgot'
         ' to set them.'
     )
     assert shared_axes is not None, msg
 
     # NOTE: If you want to clip, consider using clip and clip_gradient in
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/config.py` & `aqtp-0.7.0/aqt/jax/v2/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,35 +11,40 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Configuration dataclasses."""
 
 
 import copy
+import functools
 from typing import Literal, Optional, TypeAlias, Union
+from aqt.jax.v2 import aqt_dot_general
 from aqt.jax.v2 import aqt_quantizer
 from aqt.jax.v2 import calibration
 from aqt.jax.v2 import stochastic_rounding
+from aqt.jax.v2 import utils
 
 # Temporary re-export from aqt.jax.v2.aqt_dot_general
+# TODO(lew): Remove these imports, use setters instead
 # pylint: disable=g-importing-member
 # pylint: disable=unused-import
-from aqt.jax.v2.aqt_dot_general import assert_config_validity
 from aqt.jax.v2.aqt_dot_general import CalibrationMode
 from aqt.jax.v2.aqt_dot_general import conv_general_dilated_make
 from aqt.jax.v2.aqt_dot_general import DequantMode
 from aqt.jax.v2.aqt_dot_general import dot_general_make
 from aqt.jax.v2.aqt_dot_general import dot_general_raw_make
 from aqt.jax.v2.aqt_dot_general import DotGeneral
 from aqt.jax.v2.aqt_dot_general import DotGeneralRaw
 from aqt.jax.v2.aqt_dot_general import dtypes_allowed_for_int32_accum
 from aqt.jax.v2.aqt_dot_general import LocalAqt
 from aqt.jax.v2.aqt_dot_general import Tensor
 from aqt.jax.v2.aqt_dot_general import tensor_make
 
+from aqt.jax.v2.aqt_quantizer import quantizer_make
+
 from aqt.jax.v2.numerics import fp8_numerics
 from aqt.jax.v2.numerics import int_numerics
 from aqt.jax.v2.numerics import no_numerics
 from aqt.jax.v2.numerics import numerics
 import jax
 import jax.numpy as jnp
 
@@ -48,57 +53,37 @@
 
 # SKIP can be used as an argument to some set_xyz functions.
 # It signals that set_xyz should make no changes to that option.
 SKIP = 'skip'
 SkipT: TypeAlias = Literal[SKIP]
 
 
-def infer_dtype_from_bits(bits: int) -> jnp.dtype | None:
-  """Get the dtype for the number of bits provided.
-
-  Args:
-    bits: number of bits for the dtype.
-
-  Returns:
-    The corresponding container dtype for the number of bits provided.
-  """
-  if bits == 4:
-    # this branch should return jnp.int4 directly but
-    # lax.dot_general(int4, int4) is illegal on cpu.
-    # TODO(aqt): Remove this platform check once
-    # https://github.com/google/jax/issues/19682 is fixed.
-    if jax.local_devices()[0].platform != 'cpu':
-      return jnp.int4
-    else:
-      return jnp.int8
-  else:
-    if bits <= 8 and bits >= 2:
-      return jnp.int8
-    else:
-      return None
-
-
 def _split_key(key: Optional[jax.Array], num_splits: int):
   default = (None,) * num_splits
   return default if key is None else jax.random.split(key, num_splits)
 
 
 def set_context(
-    cfg: DotGeneral, key: Optional[jax.Array], train_step: Optional[int]
+    cfg: DotGeneral,
+    key: Optional[jax.Array],
+    train_step: Optional[int],
+    lhs_quant_mode: utils.QuantMode = utils.QuantMode.TRAIN,
+    rhs_quant_mode: utils.QuantMode = utils.QuantMode.TRAIN,
 ):
   """Set context with prng keys and train_steps for dot_general config."""
 
   def set_dg_raw_context(cfg_raw: DotGeneralRaw, key: Optional[jax.Array]):
     key1, key2 = _split_key(key, num_splits=2)
-    cfg_raw.lhs.quantizer.context = aqt_quantizer.Context(
-        key=key1, train_step=train_step
+    lhs_context = utils.Context(
+        key=key1, train_step=train_step, quant_mode=lhs_quant_mode
     )
-    cfg_raw.rhs.quantizer.context = aqt_quantizer.Context(
-        key=key2, train_step=train_step
+    rhs_context = utils.Context(
+        key=key2, train_step=train_step, quant_mode=rhs_quant_mode
     )
+    cfg_raw.dg_quantizer.set_context(lhs_context, rhs_context)
 
   key_fwd, key_dlhs, key_drhs = _split_key(key, num_splits=3)
   ret_cfg = copy.deepcopy(cfg)
   set_dg_raw_context(ret_cfg.fwd, key_fwd)
   set_dg_raw_context(ret_cfg.dlhs, key_dlhs)
   set_dg_raw_context(ret_cfg.drhs, key_drhs)
   return ret_cfg
@@ -130,16 +115,19 @@
 
 def set_numerics(
     cfg: DotGeneralRaw,
     lhs_numerics: numerics.AqtNumerics,
     rhs_numerics: numerics.AqtNumerics,
 ):
   """Set numerics for DotGeneralRaw config."""
-  cfg.lhs.quantizer.numerics = lhs_numerics
-  cfg.rhs.quantizer.numerics = rhs_numerics
+  assert isinstance(
+      cfg.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  cfg.dg_quantizer.lhs.numerics = lhs_numerics
+  cfg.dg_quantizer.rhs.numerics = rhs_numerics
   if (
       lhs_numerics.get_dtype() in dtypes_allowed_for_int32_accum
       and rhs_numerics.get_dtype() in dtypes_allowed_for_int32_accum
   ):
     cfg.dg_accumulator_dtype = jnp.int32
   elif (
       lhs_numerics.get_dtype() in fp8_numerics.fp8_map.values()
@@ -177,53 +165,68 @@
   noise_implementations = {
       'jax.uniform': stochastic_rounding.JaxUniform(),
       'custom-1': stochastic_rounding.RandomCenteredUniform(),
   }
   msg = f'{implementation} not supported.'
   assert implementation in noise_implementations.keys(), msg
   noise_fn = noise_implementations[implementation]
+  assert isinstance(
+      cfg.dlhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.drhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
 
-  if vjp_lhs_stochastic_rounding:
-    cfg.dlhs.lhs.quantizer.numerics = cfg.dlhs.lhs.quantizer.numerics.replace(
-        noise_fn=noise_fn
-    )
-    cfg.drhs.lhs.quantizer.numerics = cfg.drhs.lhs.quantizer.numerics.replace(
-        noise_fn=noise_fn
-    )
-  else:
-    cfg.dlhs.lhs.quantizer.numerics = cfg.dlhs.lhs.quantizer.numerics.replace(
-        noise_fn=None
-    )
-    cfg.drhs.lhs.quantizer.numerics = cfg.drhs.lhs.quantizer.numerics.replace(
-        noise_fn=None
-    )
-
-  if vjp_rhs_stochastic_rounding:
-    cfg.dlhs.rhs.quantizer.numerics = cfg.dlhs.rhs.quantizer.numerics.replace(
-        noise_fn=noise_fn
-    )
-    cfg.drhs.rhs.quantizer.numerics = cfg.drhs.rhs.quantizer.numerics.replace(
-        noise_fn=noise_fn
-    )
-  else:
-    cfg.dlhs.rhs.quantizer.numerics = cfg.dlhs.rhs.quantizer.numerics.replace(
-        noise_fn=None
-    )
-    cfg.drhs.rhs.quantizer.numerics = cfg.drhs.rhs.quantizer.numerics.replace(
-        noise_fn=None
-    )
+  def _set_numerics_noise_fn(
+      dg_quantizer: aqt_dot_general.DefaultDotGeneralQuantizer,
+      is_lhs_sr: bool,
+      is_rhs_sr: bool,
+  ) -> None:
+    # set stochastic noise for each dg_quantizer
+    def _set_noise_fn(
+        quantizer: aqt_quantizer.Quantizer,
+        is_sr: bool,
+    ) -> None:
+      # set stochastic noise for each side of a dg_quantizer
+      if isinstance(quantizer.numerics, fp8_numerics.Fp8Numerics):
+        quantizer.numerics.stochastic_rounding = is_sr
+      else:
+        quantizer.numerics.noise_fn = noise_fn if is_sr else None
+
+    _set_noise_fn(dg_quantizer.lhs, is_lhs_sr)
+    _set_noise_fn(dg_quantizer.rhs, is_rhs_sr)
+
+  is_lhs_sr = vjp_lhs_stochastic_rounding
+  is_rhs_sr = vjp_rhs_stochastic_rounding
+  _set_numerics_noise_fn(cfg.dlhs.dg_quantizer, is_lhs_sr, is_rhs_sr)
+  _set_numerics_noise_fn(cfg.drhs.dg_quantizer, is_lhs_sr, is_rhs_sr)
 
 
 def set_static_bound(cfg: DotGeneral, bound: float = 1.0):
-  cfg.fwd.lhs.quantizer.calibration = calibration.ConstantCalibration(bound)
-  cfg.fwd.rhs.quantizer.calibration = calibration.ConstantCalibration(bound)
-  cfg.drhs.lhs.quantizer.calibration = calibration.ConstantCalibration(bound)
-  cfg.drhs.rhs.quantizer.calibration = calibration.ConstantCalibration(bound)
-  cfg.dlhs.lhs.quantizer.calibration = calibration.ConstantCalibration(bound)
-  cfg.dlhs.rhs.quantizer.calibration = calibration.ConstantCalibration(bound)
+  """Sets the static bound for calibration."""
+  calibration_cls = functools.partial(
+      calibration.ConstantCalibration, bound=bound
+  )
+
+  assert isinstance(
+      cfg.fwd.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.dlhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.drhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+
+  cfg.fwd.dg_quantizer.lhs.calibration = calibration_cls
+  cfg.fwd.dg_quantizer.rhs.calibration = calibration_cls
+  cfg.dlhs.dg_quantizer.lhs.calibration = calibration_cls
+  cfg.dlhs.dg_quantizer.rhs.calibration = calibration_cls
+  cfg.drhs.dg_quantizer.lhs.calibration = calibration_cls
+  cfg.drhs.dg_quantizer.rhs.calibration = calibration_cls
 
 
 def set_local_aqt(
     cfg: DotGeneral,
     fwd_local_aqt: Union[SkipT, LocalAqt, None],
     dlhs_local_aqt: Union[SkipT, LocalAqt, None],
     drhs_local_aqt: Union[SkipT, LocalAqt, None],
@@ -244,41 +247,67 @@
   if dlhs_use_fwd_quant != SKIP:
     cfg.dlhs.rhs.use_fwd_quant = dlhs_use_fwd_quant
   if drhs_use_fwd_quant != SKIP:
     cfg.drhs.rhs.use_fwd_quant = drhs_use_fwd_quant
 
 
 def set_int_numerics_preserve_zero(cfg: DotGeneral, preserve_zero: bool):
+  """Set preserve_zero for int_numerics."""
+  assert isinstance(
+      cfg.fwd.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.dlhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.drhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+
   for dot_general_raw in [cfg.fwd, cfg.dlhs, cfg.drhs]:
-    for tensor in [dot_general_raw.lhs, dot_general_raw.rhs]:
-      if isinstance(tensor.quantizer.numerics, int_numerics.IntNumerics):
-        tensor.quantizer.numerics.preserve_zero = preserve_zero
+    dg_quantizer = dot_general_raw.dg_quantizer
+    for q_numerics in [dg_quantizer.lhs.numerics, dg_quantizer.rhs.numerics]:
+      if isinstance(q_numerics, int_numerics.IntNumerics):
+        q_numerics.preserve_zero = preserve_zero
         updated_dtype = (
-            infer_dtype_from_bits(tensor.quantizer.numerics.bits)
+            utils.infer_dtype_from_bits(q_numerics.bits)  # pytype: disable=attribute-error
             if preserve_zero
             else None
         )
-        tensor.quantizer.numerics.dtype = updated_dtype
+        q_numerics.dtype = updated_dtype
 
 
 def set_absmax_calib_scale(cfg: DotGeneral, scale: float):
   """Set AbsMaxCalibration scale and update clip_gradient accordingly."""
+  assert isinstance(
+      cfg.fwd.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.dlhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+  assert isinstance(
+      cfg.drhs.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+
   for dot_general_raw in [cfg.fwd, cfg.dlhs, cfg.drhs]:
-    for tensor in [dot_general_raw.lhs, dot_general_raw.rhs]:
-      assert isinstance(
-          tensor.quantizer.calibration, calibration.AbsMaxCalibration
-      ), (
+    dg_quantizer = dot_general_raw.dg_quantizer
+    for quantizer in [dg_quantizer.lhs, dg_quantizer.rhs]:
+      calibration_cls = quantizer.calibration
+      if isinstance(calibration_cls, functools.partial):
+        calibration_cls = calibration_cls.func
+      assert calibration_cls == calibration.AbsMaxCalibration, (
           'scale is only available in AbsMaxCalibration, while'
-          f'{tensor.quantizer.calibration} is used in current config.'
+          f' {quantizer.calibration} is used in current config.'
+      )
+      quantizer.calibration = functools.partial(
+          calibration.AbsMaxCalibration, scale=scale
       )
-      tensor.quantizer.calibration = calibration.AbsMaxCalibration(scale)
       if scale < 1.0 and isinstance(
-          tensor.quantizer.numerics, int_numerics.IntNumerics
+          quantizer.numerics, int_numerics.IntNumerics
       ):
-        tensor.quantizer.numerics.clip_gradient = True
+        quantizer.numerics.clip_gradient = True
 
 
 def set_bits(
     cfg: DotGeneral,
     fwd_lhs_bit: Union[int, None, fp8_numerics.FP8Dtype],
     fwd_rhs_bit: Union[int, None, fp8_numerics.FP8Dtype],
     dlhs_lhs_bit: Union[int, None, fp8_numerics.FP8Dtype],
@@ -293,19 +322,18 @@
       effective_numerics = no_numerics.NoNumerics()
     elif bits in fp8_numerics.fp8_map.keys():
       exponent_bits, mantissa_bits = int(bits[1]), int(bits[3])
       effective_numerics = fp8_numerics.Fp8Numerics(
           exponent_bits=exponent_bits,
           mantissa_bits=mantissa_bits,
           dtype=fp8_numerics.fp8_map[bits],
-          noise_fn=None,
       )
     else:
       pz = False if bits == 1 else True
-      dtype = infer_dtype_from_bits(bits) if pz else None
+      dtype = utils.infer_dtype_from_bits(bits) if pz else None
       effective_numerics = int_numerics.IntNumerics(
           bits=bits,
           preserve_zero=pz,
           preserve_max_val=False,
           clip=True,
           round=True,
           noise_fn=None,
@@ -331,34 +359,38 @@
 # Functions below are auxiliary config creators.
 
 
 def default_unquantized_config() -> DotGeneral:
   """Aqt config for floating-point dot general."""
 
   def tensor_cfg() -> Tensor:
-    quantizer = aqt_quantizer.Quantizer(
-        numerics=no_numerics.NoNumerics(),
-        calib_shared_axes=None,
-        scale_stop_grad=True,
-        calibration=calibration.AbsMaxCalibration(),
-        po2_scale=False,
-        context=aqt_quantizer.Context(key=None, train_step=None),
-    )
     cfg = Tensor(
-        quantizer=quantizer,
         use_fwd_quant=None,
         dequant_mode=DequantMode.OUTPUT,
         calibration_mode=CalibrationMode.CONTRACTING_AXIS,
     )
     return cfg
 
+  def quantizer() -> aqt_quantizer.Quantizer:
+    return aqt_quantizer.Quantizer(
+        numerics=no_numerics.NoNumerics(),
+        calib_shared_axes=None,
+        scale_stop_grad=True,
+        calibration=calibration.AbsMaxCalibration,
+        po2_scale=False,
+        context=utils.Context(key=None, train_step=None),
+    )
+
   def dg_raw_cfg(jax_scope_name: str) -> DotGeneralRaw:
     return DotGeneralRaw(
         lhs=tensor_cfg(),
         rhs=tensor_cfg(),
+        dg_quantizer=aqt_dot_general.DefaultDotGeneralQuantizer(
+            lhs=quantizer(), rhs=quantizer()
+        ),
         dg_accumulator_dtype=None,
         local_aqt=None,
         jax_scope_name=jax_scope_name,
     )
 
   dg_cfg = DotGeneral(
       fwd=dg_raw_cfg('aqt_fwd'),
@@ -485,17 +517,17 @@
   )
   assert cfg.fwd.local_aqt is None, 'local_aqt is not yet supported in fwd.'
   return cfg
 
 
 def config_v4(
     *,
-    fwd_bits: Optional[int] = 8,
-    dlhs_bits: Optional[int] = 8,
-    drhs_bits: Optional[int] = None,
+    fwd_bits: Union[int, None, fp8_numerics.FP8Dtype] = 8,
+    dlhs_bits: Union[int, None, fp8_numerics.FP8Dtype] = 8,
+    drhs_bits: Union[int, None, fp8_numerics.FP8Dtype] = None,
     # The dummy static bound flag is for performance benchmarking.
     use_dummy_static_bound: bool = False,
     rng_type: str = 'jax.uniform',  # 'custom-1'
     dlhs_local_aqt: Optional[LocalAqt] = None,
     drhs_local_aqt: Optional[LocalAqt] = None,
     # accumulator dtype by default is automatically set in set_bits,
     # but users can still configure a special dtype such as jnp.int16, etc.
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/config_test.py` & `aqtp-0.7.0/aqt/jax/v2/config_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,372 +18,400 @@
 from aqt.jax.v2 import config
 from aqt.jax.v2 import utils
 import jax.numpy as jnp
 
 
 class AqtConfigTest(parameterized.TestCase):
 
+  def _retrieve_quantizers(self, dot_general_raws):
+    ret = []
+    for dot_general_raw in dot_general_raws:
+      ret.extend(
+          [dot_general_raw.dg_quantizer.lhs, dot_general_raw.dg_quantizer.rhs]
+      )
+    return ret
+
   def test_config_v4(self):
     cfg = config.config_v4(
         fwd_bits=8,
         dlhs_bits=7,
         drhs_bits=6,
         rng_type='custom-1',
         dlhs_local_aqt=config.LocalAqt(2),
         drhs_local_aqt=config.LocalAqt(3),
         fwd_accumulator_dtype=jnp.int16,
         dlhs_accumulator_dtype=jnp.int8,
         drhs_accumulator_dtype=jnp.int4,
     )
-    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=8,
-                                                                                 preserve_zero=True,
-                                                                                 preserve_max_val=False,
-                                                                                 clip=True,
-                                                                                 clip_gradient=False,
-                                                                                 round=True,
-                                                                                 noise_fn=None,
-                                                                                 dtype=<class 'jax.numpy.int8'>),
-                                                            calib_shared_axes=None,
-                                                            scale_stop_grad=True,
-                                                            calibration=AbsMaxCalibration(scale=None),
-                                                            po2_scale=False,
-                                                            context=Context(key=None,
-                                                                            train_step=None)),
-                                        use_fwd_quant=None,
+    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                             rhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=8,
-                                                                                 preserve_zero=True,
-                                                                                 preserve_max_val=False,
-                                                                                 clip=True,
-                                                                                 clip_gradient=False,
-                                                                                 round=True,
-                                                                                 noise_fn=None,
-                                                                                 dtype=<class 'jax.numpy.int8'>),
-                                                            calib_shared_axes=None,
-                                                            scale_stop_grad=True,
-                                                            calibration=AbsMaxCalibration(scale=None),
-                                                            po2_scale=False,
-                                                            context=Context(key=None,
-                                                                            train_step=None)),
-                                        use_fwd_quant=None,
+                             rhs=Tensor(use_fwd_quant=None,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                             dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=8,
+                                                                                                        preserve_zero=True,
+                                                                                                        preserve_max_val=False,
+                                                                                                        clip=True,
+                                                                                                        clip_gradient=False,
+                                                                                                        round=True,
+                                                                                                        noise_fn=None,
+                                                                                                        dtype=<class 'jax.numpy.int8'>),
+                                                                                   calib_shared_axes=None,
+                                                                                   scale_stop_grad=True,
+                                                                                   calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                   po2_scale=False,
+                                                                                   context=Context(key=None,
+                                                                                                   train_step=None,
+                                                                                                   quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                     rhs=Quantizer(numerics=IntNumerics(bits=8,
+                                                                                                        preserve_zero=True,
+                                                                                                        preserve_max_val=False,
+                                                                                                        clip=True,
+                                                                                                        clip_gradient=False,
+                                                                                                        round=True,
+                                                                                                        noise_fn=None,
+                                                                                                        dtype=<class 'jax.numpy.int8'>),
+                                                                                   calib_shared_axes=None,
+                                                                                   scale_stop_grad=True,
+                                                                                   calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                   po2_scale=False,
+                                                                                   context=Context(key=None,
+                                                                                                   train_step=None,
+                                                                                                   quant_mode=<QuantMode.TRAIN: 1>))),
                              dg_accumulator_dtype=<class 'jax.numpy.int16'>,
                              local_aqt=None,
                              jax_scope_name='aqt_fwd',
-                             allow_dummy_gradient_into_qtensor=False),
-           dlhs=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=7,
-                                                                                  preserve_zero=True,
-                                                                                  preserve_max_val=False,
-                                                                                  clip=True,
-                                                                                  clip_gradient=False,
-                                                                                  round=True,
-                                                                                  noise_fn=RandomCenteredUniform(),
-                                                                                  dtype=<class 'jax.numpy.int8'>),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=None,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                              rhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=7,
-                                                                                  preserve_zero=True,
-                                                                                  preserve_max_val=False,
-                                                                                  clip=True,
-                                                                                  clip_gradient=False,
-                                                                                  round=True,
-                                                                                  noise_fn=None,
-                                                                                  dtype=<class 'jax.numpy.int8'>),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=False,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                             allow_dummy_gradient_into_qtensor=False,
+                             dot_general=<function dot_general>),
+           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              rhs=Tensor(use_fwd_quant=False,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=7,
+                                                                                                         preserve_zero=True,
+                                                                                                         preserve_max_val=False,
+                                                                                                         clip=True,
+                                                                                                         clip_gradient=False,
+                                                                                                         round=True,
+                                                                                                         noise_fn=RandomCenteredUniform(),
+                                                                                                         dtype=<class 'jax.numpy.int8'>),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                      rhs=Quantizer(numerics=IntNumerics(bits=7,
+                                                                                                         preserve_zero=True,
+                                                                                                         preserve_max_val=False,
+                                                                                                         clip=True,
+                                                                                                         clip_gradient=False,
+                                                                                                         round=True,
+                                                                                                         noise_fn=None,
+                                                                                                         dtype=<class 'jax.numpy.int8'>),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=<class 'jax.numpy.int8'>,
                               local_aqt=LocalAqt(contraction_axis_shard_count=2),
                               jax_scope_name='aqt_dlhs',
-                              allow_dummy_gradient_into_qtensor=False),
-           drhs=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=6,
-                                                                                  preserve_zero=True,
-                                                                                  preserve_max_val=False,
-                                                                                  clip=True,
-                                                                                  clip_gradient=False,
-                                                                                  round=True,
-                                                                                  noise_fn=RandomCenteredUniform(),
-                                                                                  dtype=<class 'jax.numpy.int8'>),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=None,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                              rhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=6,
-                                                                                  preserve_zero=True,
-                                                                                  preserve_max_val=False,
-                                                                                  clip=True,
-                                                                                  clip_gradient=False,
-                                                                                  round=True,
-                                                                                  noise_fn=None,
-                                                                                  dtype=<class 'jax.numpy.int8'>),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=False,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              allow_dummy_gradient_into_qtensor=False,
+                              dot_general=<function dot_general>),
+           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              rhs=Tensor(use_fwd_quant=False,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=6,
+                                                                                                         preserve_zero=True,
+                                                                                                         preserve_max_val=False,
+                                                                                                         clip=True,
+                                                                                                         clip_gradient=False,
+                                                                                                         round=True,
+                                                                                                         noise_fn=RandomCenteredUniform(),
+                                                                                                         dtype=<class 'jax.numpy.int8'>),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                      rhs=Quantizer(numerics=IntNumerics(bits=6,
+                                                                                                         preserve_zero=True,
+                                                                                                         preserve_max_val=False,
+                                                                                                         clip=True,
+                                                                                                         clip_gradient=False,
+                                                                                                         round=True,
+                                                                                                         noise_fn=None,
+                                                                                                         dtype=<class 'jax.numpy.int8'>),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=<class 'jax.numpy.int4'>,
                               local_aqt=LocalAqt(contraction_axis_shard_count=3),
                               jax_scope_name='aqt_drhs',
-                              allow_dummy_gradient_into_qtensor=False))"""
-    utils.test_pprint_eq(cfg, expected_cfg_str)
+                              allow_dummy_gradient_into_qtensor=False,
+                              dot_general=<function dot_general>),
+           apply_custom_vjp_on_jax=True)"""
+    utils.test_pprint_eq(cfg, expected_cfg_str, remove_memory_addresses=True)
 
   def test_configv4_original(self):
-    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=8,
-                                                                                 preserve_zero=True,
-                                                                                 preserve_max_val=False,
-                                                                                 clip=True,
-                                                                                 clip_gradient=False,
-                                                                                 round=True,
-                                                                                 noise_fn=None,
-                                                                                 dtype=<class 'jax.numpy.int8'>),
-                                                            calib_shared_axes=None,
-                                                            scale_stop_grad=True,
-                                                            calibration=AbsMaxCalibration(scale=None),
-                                                            po2_scale=False,
-                                                            context=Context(key=None,
-                                                                            train_step=None)),
-                                        use_fwd_quant=None,
+    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                             rhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=8,
-                                                                                 preserve_zero=True,
-                                                                                 preserve_max_val=False,
-                                                                                 clip=True,
-                                                                                 clip_gradient=False,
-                                                                                 round=True,
-                                                                                 noise_fn=None,
-                                                                                 dtype=<class 'jax.numpy.int8'>),
-                                                            calib_shared_axes=None,
-                                                            scale_stop_grad=True,
-                                                            calibration=AbsMaxCalibration(scale=None),
-                                                            po2_scale=False,
-                                                            context=Context(key=None,
-                                                                            train_step=None)),
-                                        use_fwd_quant=None,
+                             rhs=Tensor(use_fwd_quant=None,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                             dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=8,
+                                                                                                        preserve_zero=True,
+                                                                                                        preserve_max_val=False,
+                                                                                                        clip=True,
+                                                                                                        clip_gradient=False,
+                                                                                                        round=True,
+                                                                                                        noise_fn=None,
+                                                                                                        dtype=<class 'jax.numpy.int8'>),
+                                                                                   calib_shared_axes=None,
+                                                                                   scale_stop_grad=True,
+                                                                                   calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                   po2_scale=False,
+                                                                                   context=Context(key=None,
+                                                                                                   train_step=None,
+                                                                                                   quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                     rhs=Quantizer(numerics=IntNumerics(bits=8,
+                                                                                                        preserve_zero=True,
+                                                                                                        preserve_max_val=False,
+                                                                                                        clip=True,
+                                                                                                        clip_gradient=False,
+                                                                                                        round=True,
+                                                                                                        noise_fn=None,
+                                                                                                        dtype=<class 'jax.numpy.int8'>),
+                                                                                   calib_shared_axes=None,
+                                                                                   scale_stop_grad=True,
+                                                                                   calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                   po2_scale=False,
+                                                                                   context=Context(key=None,
+                                                                                                   train_step=None,
+                                                                                                   quant_mode=<QuantMode.TRAIN: 1>))),
                              dg_accumulator_dtype=<class 'jax.numpy.int32'>,
                              local_aqt=None,
                              jax_scope_name='aqt_fwd',
-                             allow_dummy_gradient_into_qtensor=False),
-           dlhs=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=8,
-                                                                                  preserve_zero=True,
-                                                                                  preserve_max_val=False,
-                                                                                  clip=True,
-                                                                                  clip_gradient=False,
-                                                                                  round=True,
-                                                                                  noise_fn=JaxUniform(),
-                                                                                  dtype=<class 'jax.numpy.int8'>),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=None,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                              rhs=Tensor(quantizer=Quantizer(numerics=IntNumerics(bits=8,
-                                                                                  preserve_zero=True,
-                                                                                  preserve_max_val=False,
-                                                                                  clip=True,
-                                                                                  clip_gradient=False,
-                                                                                  round=True,
-                                                                                  noise_fn=None,
-                                                                                  dtype=<class 'jax.numpy.int8'>),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=False,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                             allow_dummy_gradient_into_qtensor=False,
+                             dot_general=<function dot_general>),
+           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              rhs=Tensor(use_fwd_quant=False,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=8,
+                                                                                                         preserve_zero=True,
+                                                                                                         preserve_max_val=False,
+                                                                                                         clip=True,
+                                                                                                         clip_gradient=False,
+                                                                                                         round=True,
+                                                                                                         noise_fn=JaxUniform(),
+                                                                                                         dtype=<class 'jax.numpy.int8'>),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                      rhs=Quantizer(numerics=IntNumerics(bits=8,
+                                                                                                         preserve_zero=True,
+                                                                                                         preserve_max_val=False,
+                                                                                                         clip=True,
+                                                                                                         clip_gradient=False,
+                                                                                                         round=True,
+                                                                                                         noise_fn=None,
+                                                                                                         dtype=<class 'jax.numpy.int8'>),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=<class 'jax.numpy.int32'>,
                               local_aqt=None,
                               jax_scope_name='aqt_dlhs',
-                              allow_dummy_gradient_into_qtensor=False),
-           drhs=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=NoNumerics(noise_fn=JaxUniform(),
-                                                                                 dtype=None),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=None,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                              rhs=Tensor(quantizer=Quantizer(numerics=NoNumerics(noise_fn=None,
-                                                                                 dtype=None),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=False,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              allow_dummy_gradient_into_qtensor=False,
+                              dot_general=<function dot_general>),
+           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              rhs=Tensor(use_fwd_quant=False,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=NoNumerics(noise_fn=JaxUniform(),
+                                                                                                        dtype=None),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                      rhs=Quantizer(numerics=NoNumerics(noise_fn=None,
+                                                                                                        dtype=None),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=None,
                               local_aqt=None,
                               jax_scope_name='aqt_drhs',
-                              allow_dummy_gradient_into_qtensor=False))"""
-    utils.test_pprint_eq(config.config_v4(), expected_cfg_str)
+                              allow_dummy_gradient_into_qtensor=False,
+                              dot_general=<function dot_general>),
+           apply_custom_vjp_on_jax=True)"""
+    utils.test_pprint_eq(
+        config.config_v4(), expected_cfg_str, remove_memory_addresses=True
+    )
 
   def test_config_fwd_fp8(self):
-    expected_cfg = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=Fp8Numerics(dtype=<class 'jax.numpy.float8_e4m3fn'>,
-                                                                                 exponent_bits=4,
-                                                                                 mantissa_bits=3,
-                                                                                 noise_fn=None),
-                                                            calib_shared_axes=None,
-                                                            scale_stop_grad=True,
-                                                            calibration=AbsMaxCalibration(scale=None),
-                                                            po2_scale=False,
-                                                            context=Context(key=None,
-                                                                            train_step=None)),
-                                        use_fwd_quant=None,
+    expected_cfg = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                             rhs=Tensor(quantizer=Quantizer(numerics=Fp8Numerics(dtype=<class 'jax.numpy.float8_e4m3fn'>,
-                                                                                 exponent_bits=4,
-                                                                                 mantissa_bits=3,
-                                                                                 noise_fn=None),
-                                                            calib_shared_axes=None,
-                                                            scale_stop_grad=True,
-                                                            calibration=AbsMaxCalibration(scale=None),
-                                                            po2_scale=False,
-                                                            context=Context(key=None,
-                                                                            train_step=None)),
-                                        use_fwd_quant=None,
+                             rhs=Tensor(use_fwd_quant=None,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                             dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=Fp8Numerics(dtype=<class 'jax.numpy.float8_e4m3fn'>,
+                                                                                                        exponent_bits=4,
+                                                                                                        mantissa_bits=3,
+                                                                                                        stochastic_rounding=False),
+                                                                                   calib_shared_axes=None,
+                                                                                   scale_stop_grad=True,
+                                                                                   calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                   po2_scale=False,
+                                                                                   context=Context(key=None,
+                                                                                                   train_step=None,
+                                                                                                   quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                     rhs=Quantizer(numerics=Fp8Numerics(dtype=<class 'jax.numpy.float8_e4m3fn'>,
+                                                                                                        exponent_bits=4,
+                                                                                                        mantissa_bits=3,
+                                                                                                        stochastic_rounding=False),
+                                                                                   calib_shared_axes=None,
+                                                                                   scale_stop_grad=True,
+                                                                                   calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                   po2_scale=False,
+                                                                                   context=Context(key=None,
+                                                                                                   train_step=None,
+                                                                                                   quant_mode=<QuantMode.TRAIN: 1>))),
                              dg_accumulator_dtype=<class 'jax.numpy.float32'>,
                              local_aqt=None,
                              jax_scope_name='aqt_fwd',
-                             allow_dummy_gradient_into_qtensor=False),
-           dlhs=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=NoNumerics(noise_fn=None,
-                                                                                 dtype=None),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=None,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                              rhs=Tensor(quantizer=Quantizer(numerics=NoNumerics(noise_fn=None,
-                                                                                 dtype=None),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=False,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                             allow_dummy_gradient_into_qtensor=False,
+                             dot_general=<function dot_general>),
+           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              rhs=Tensor(use_fwd_quant=False,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=NoNumerics(noise_fn=None,
+                                                                                                        dtype=None),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                      rhs=Quantizer(numerics=NoNumerics(noise_fn=None,
+                                                                                                        dtype=None),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=None,
                               local_aqt=None,
                               jax_scope_name='aqt_dlhs',
-                              allow_dummy_gradient_into_qtensor=False),
-           drhs=DotGeneralRaw(lhs=Tensor(quantizer=Quantizer(numerics=NoNumerics(noise_fn=None,
-                                                                                 dtype=None),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=None,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                              rhs=Tensor(quantizer=Quantizer(numerics=NoNumerics(noise_fn=None,
-                                                                                 dtype=None),
-                                                             calib_shared_axes=None,
-                                                             scale_stop_grad=True,
-                                                             calibration=AbsMaxCalibration(scale=None),
-                                                             po2_scale=False,
-                                                             context=Context(key=None,
-                                                                             train_step=None)),
-                                         use_fwd_quant=False,
-                                         dequant_mode=<DequantMode.OUTPUT: 1>,
-                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              allow_dummy_gradient_into_qtensor=False,
+                              dot_general=<function dot_general>),
+           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              rhs=Tensor(use_fwd_quant=False,
+                                         dequant_mode=<DequantMode.OUTPUT: 1>,
+                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
+                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=NoNumerics(noise_fn=None,
+                                                                                                        dtype=None),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>)),
+                                                                      rhs=Quantizer(numerics=NoNumerics(noise_fn=None,
+                                                                                                        dtype=None),
+                                                                                    calib_shared_axes=None,
+                                                                                    scale_stop_grad=True,
+                                                                                    calibration=<class 'aqt.jax.v2.calibration.AbsMaxCalibration'>,
+                                                                                    po2_scale=False,
+                                                                                    context=Context(key=None,
+                                                                                                    train_step=None,
+                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=None,
                               local_aqt=None,
                               jax_scope_name='aqt_drhs',
-                              allow_dummy_gradient_into_qtensor=False))"""
-    utils.test_pprint_eq(config.config_fwd_fp8(), expected_cfg)
+                              allow_dummy_gradient_into_qtensor=False,
+                              dot_general=<function dot_general>),
+           apply_custom_vjp_on_jax=True)"""
+    utils.test_pprint_eq(
+        config.config_fwd_fp8(), expected_cfg, remove_memory_addresses=True
+    )
 
   def test_set_int_numerics_preserve_zero(self):
     cfg = config.config_v4()
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertTrue(tensor.quantizer.numerics.preserve_zero)
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertEqual(tensor.quantizer.numerics.dtype, jnp.int8)
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs]):
+      self.assertTrue(quantizer.numerics.preserve_zero)
+      self.assertEqual(quantizer.numerics.dtype, jnp.int8)
 
     config.set_int_numerics_preserve_zero(cfg, preserve_zero=False)
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertFalse(tensor.quantizer.numerics.preserve_zero)
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertIsNone(tensor.quantizer.numerics.dtype)
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs]):
+      self.assertFalse(quantizer.numerics.preserve_zero)
+      self.assertIsNone(quantizer.numerics.dtype)
 
   def test_set_absmax_calib_scale(self):
     cfg = config.config_v4()
-    for tensor in [
-        cfg.fwd.lhs,
-        cfg.fwd.rhs,
-        cfg.dlhs.lhs,
-        cfg.dlhs.rhs,
-        cfg.drhs.lhs,
-        cfg.drhs.rhs,
-    ]:
-      self.assertIsNone(tensor.quantizer.calibration.scale)
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertFalse(tensor.quantizer.numerics.clip_gradient)
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs, cfg.drhs]):
+      self.assertIsNone(quantizer.calibration().scale)
+
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs]):
+      self.assertFalse(quantizer.numerics.clip_gradient)
 
     config.set_absmax_calib_scale(cfg, scale=3)
-    for tensor in [
-        cfg.fwd.lhs,
-        cfg.fwd.rhs,
-        cfg.dlhs.lhs,
-        cfg.dlhs.rhs,
-        cfg.drhs.lhs,
-        cfg.drhs.rhs,
-    ]:
-      self.assertAlmostEqual(tensor.quantizer.calibration.scale, 3)
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertFalse(tensor.quantizer.numerics.clip_gradient)
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs, cfg.drhs]):
+      self.assertAlmostEqual(quantizer.calibration().scale, 3)
+
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs]):
+      self.assertFalse(quantizer.numerics.clip_gradient)
 
     config.set_absmax_calib_scale(cfg, scale=0.1)
-    for tensor in [cfg.fwd.lhs, cfg.fwd.rhs, cfg.dlhs.lhs, cfg.dlhs.rhs]:
-      self.assertTrue(tensor.quantizer.numerics.clip_gradient)
+    for quantizer in self._retrieve_quantizers([cfg.fwd, cfg.dlhs]):
+      self.assertTrue(quantizer.numerics.clip_gradient)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/examples/examples.ipynb` & `aqtp-0.7.0/aqt/jax/v2/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/examples/flax_e2e_model_test.py` & `aqtp-0.7.0/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 # limitations under the License.
 
 """Test for flax e2e model."""
 import copy
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.jax.v2 import config
+from aqt.jax.v2 import tiled_dot_general
 from aqt.jax.v2.examples import flax_e2e_model
+from aqt.jax.v2.flax.intercept import aqt_intercept_methods
+from aqt.jax.v2.flax.intercept.examples import flax_e2e_intercept_model
 import jax
 import jax.numpy as jnp
 
 
 class MnistTest(parameterized.TestCase):
 
   # Unable to use config_v4() in parameters since it needs jax.device info.
@@ -41,31 +44,38 @@
               "dlhs_accumulator_dtype": None,
           },
           4,
       ),
   ])
   def test_mnist_training(self, configs, bits):
     aqt_cfg = config.config_v4(**configs)
+    tiling_cfg = tiled_dot_general.Cfg(
+        lhs=tiled_dot_general.TensorTiling(
+            contraction_axes=[
+                tiled_dot_general.AxisTiling(
+                    axis=1, tile_count=2, tile_size=None
+                ),
+            ],
+            remaining_axes=[],
+        ),
+        rhs=tiled_dot_general.TensorTiling(
+            contraction_axes=[
+                tiled_dot_general.AxisTiling(
+                    axis=0, tile_count=2, tile_size=None
+                ),
+            ],
+            remaining_axes=[],
+        ),
+    )
     target_loss = {
         8: {
-            "cpu": [
-                3.128226041793823242187500000000,
-                3.128226757049560546875000000000,
-            ],
-            "TPU v2": [3.179433345794677734375000000000],
-            "TPU v3": [3.179433345794677734375000000000],
-            "TPU v4": [3.179425239562988281250000000000],
-            "TPU v5 lite": [3.179427385330200195312500000000],
+            "TPU v5 lite": [3.222228527069091796875000000000],
         },
         4: {
-            "cpu": [2.263035058975219726562500000000],
-            "TPU v2": [2.302649736404418945312500000000],
-            "TPU v3": [2.302649736404418945312500000000],
-            "TPU v4": [2.302649736404418945312500000000],
-            "TPU v5 lite": [2.302649736404418945312500000000],
+            "TPU v5 lite": [2.292296886444091796875000000000],
         },
     }
     # below 3 lines are differences between config_v4/v3 and fully_quantized
     config.set_stochastic_rounding(aqt_cfg, True, True, "jax.uniform")
     aqt_cfg.dlhs.rhs.use_fwd_quant = True
     aqt_cfg.drhs.rhs.use_fwd_quant = True
 
@@ -91,46 +101,43 @@
         "image": jax.random.uniform(key=image_rng, shape=(ds_size, 28, 28, 1)),
         "label": jax.random.randint(
             key=label_rng, shape=(ds_size,), minval=0, maxval=10
         ),
     }
 
     # Stage 1: regular training
-    state = flax_e2e_model.create_train_state(init_rng, aqt_cfg)
+    state = flax_e2e_intercept_model.create_train_state(init_rng)
 
-    state, train_loss, _ = flax_e2e_model.train_epoch(
-        state, ds, batch_size=ds_size // 2, rng=input_rng
-    )
+    with aqt_intercept_methods.intercept_methods(
+        aqt_cfg, tiling_cfg=tiling_cfg):
+      state, train_loss, _ = flax_e2e_model.train_epoch(
+          state, ds, batch_size=ds_size // 2, rng=input_rng
+      )
 
     device_kind = jax.devices()[0].device_kind
     expected_train_loss = target_loss[bits][device_kind]
     if train_loss not in expected_train_loss:
       msg = "train_loss changed. Consider updating with the following:\n"
       msg += f'        "{device_kind}": [{train_loss:.30f}]'
       self.fail(msg)
 
     # Run forward once more in the same mode to get logits for testing below.
-    logits_s1, _ = forward(state.model, state.cnn_eval.apply)
+    with aqt_intercept_methods.intercept_methods(
+        aqt_cfg, tiling_cfg=tiling_cfg):
+      logits_s1, _ = forward(state.model, state.cnn_eval.apply)
 
     # Stage 2: Model conversion (quantized weights freezing)
 
-    apply_serving, model_serving = flax_e2e_model.serving_conversion(state)
+    apply_serving, model_serving = flax_e2e_intercept_model.serving_conversion(
+        state, aqt_cfg, tiling_cfg)
 
     dtype = jnp.dtype
     expected_dtype = jnp.int8
     expected_aqt_pytree = {
         "aqt": {
-            "AqtEinsum_0": {
-                "AqtDotGeneral_0": {
-                    "qlhs": {
-                        "scale": (dtype("float32"), (1, 10)),
-                        "value": (expected_dtype, (10, 10)),
-                    }
-                }
-            },
             "Dense_0": {
                 "AqtDotGeneral_0": {
                     "qrhs": {
                         # The scale_t shape was (1, 256) before tiling.
                         # After tiling the scale shape is (1, 2, 1, 1, 256),
                         # then transposed to (2, 1, 1, 1, 256).
                         "scale": (dtype("float32"), (2, 1, 1, 1, 256)),
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/flax/aqt_flax.py` & `aqtp-0.7.0/aqt/jax/v2/flax/aqt_flax.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,26 +13,36 @@
 # limitations under the License.
 """Flax layer for AQT injection."""
 
 # pylint: disable=unnecessary-lambda
 # pylint: disable=g-importing-member
 import copy
 import functools
-from typing import Iterable
-from typing import Optional, Union
+from typing import Callable, Iterable, Optional, Sequence, Union
 from aqt.jax.v2 import aqt_dot_general
 from aqt.jax.v2 import aqt_tensor
 from aqt.jax.v2 import config
 from aqt.jax.v2 import tiled_dot_general
-from aqt.jax.v2.flax.utils import QuantMode
+from aqt.jax.v2 import transpose
+from aqt.jax.v2 import utils
+from aqt.jax.v2.flax import aqt_flax_dg_core
+from aqt.jax.v2.flax import freezer as general_freezer
+from aqt.jax.v2.utils import QuantMode
+import flax.core.meta as nn_meta
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
 
+NoShardingAxes = Sequence[utils.AxisIdx]
+AxisMetadataWrapper = Callable[
+    [jnp.ndarray, NoShardingAxes], nn_meta.AxisMetadata
+]
+
+
 class Freezer(nn.Module):
   """Identity function that can freeze its input.
 
   On default it is an identity function that saves the input in a variable.
   In 'quant_mode=QuantMode.Serve' mode, ignores the input and returns the frozen
   value. It is usefult to implement 'constant folding' and put quantized weights
   and scales in the checkpoint for serving. Specifically:
@@ -67,38 +77,45 @@
       # sharding axises, etc.
       self.qvalue = self.variable(collection, 'value', q_init, q_shape, q_dtype)
       self.scale_t = self.variable(collection, 'scale', s_init, s_shape)
 
   def get(self) -> Optional[aqt_tensor.QTensor]:
     if self.quant_mode == QuantMode.TRAIN:
       return None
+    elif self.quant_mode == QuantMode.CALIBRATE:
+      return None
     elif self.quant_mode == QuantMode.CONVERT:
       return None
     elif self.quant_mode == QuantMode.SERVE:
       qvalue = self.qvalue.value
       # TODO(b/325626080): Remove the optional logic.
       if self.q_dtype == jnp.int4:
         qvalue = qvalue.astype(jnp.int4)
       return aqt_tensor.QTensor(
           qvalue,
           scale=None,
           scale_t=[self.scale_t.value],
-          dequant_dtype=None,  # Rely on dg output dtype for dequant
+          # TODO(lew): Ideal solution: To find out this dequant_dtype one should
+          # use the dtype of inputs of the quant function. We should store it as
+          # a dtype of small-sized scale tensor.
+          dequant_dtype=self.scale_t.value.dtype,
       )
     else:
       assert False, 'Unknown quant mode.'
 
   def set(self, inputs: aqt_tensor.QTensor) -> None:
     # TODO(b/325626080): Uncomment the assert.
     # assert inputs.qvalue.dtype == self.q_dtype, (
     #     f'Freezer got a QTensor of type {inputs.qvalue.dtype} but expected'
     #     f' {self.q_dtype}.'
     # )
     if self.quant_mode == QuantMode.TRAIN:
       pass
+    elif self.quant_mode == QuantMode.CALIBRATE:
+      pass
     elif self.quant_mode == QuantMode.CONVERT:
       qvalue = inputs.qvalue
       # TODO(b/325626080): Remove the optional logic.
       if self.q_dtype == jnp.int4:
         assert qvalue.dtype == jnp.int4
         qvalue = qvalue.astype(jnp.int8)
       self.qvalue.value = qvalue
@@ -119,31 +136,42 @@
 
   # TODO(lew): split out separate class for each side.
   # Quant mode determines whether flax variables are created to store quantized
   # inputs. Refer to the Freezer doc str to see variable creation in each mode.
   lhs_quant_mode: QuantMode = QuantMode.TRAIN
   # apply_quant_mode determines if using Freezer in cfg.get/set_tensor
   lhs_apply_quant_mode: bool = True
-  lhs_init: nn.initializers.Initializer = jnp.zeros
-  lhs_scale_init: nn.initializers.Initializer = jnp.zeros
   lhs_var_name: str = 'qlhs'
   lhs_qtensor: Optional[aqt_tensor.QTensor] = None
 
   rhs_quant_mode: QuantMode = QuantMode.TRAIN
   rhs_apply_quant_mode: bool = True
-  rhs_init: nn.initializers.Initializer = jnp.zeros
-  rhs_scale_init: nn.initializers.Initializer = jnp.zeros
   rhs_var_name: str = 'qrhs'
   rhs_qtensor: Optional[aqt_tensor.QTensor] = None
 
+  # Variables only for the legacy Freezer.
+  lhs_init: nn.initializers.Initializer = jnp.zeros
+  lhs_scale_init: nn.initializers.Initializer = jnp.zeros
+
+  rhs_init: nn.initializers.Initializer = jnp.zeros
+  rhs_scale_init: nn.initializers.Initializer = jnp.zeros
+
+  # Variables only for the new Freezer.
+  lhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
+  rhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
+
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
   tiling_cfg: Optional[tiled_dot_general.Cfg] = None
 
+  # If set to True, use the current Freezer. Otherwise, use the new
+  # QuantFreezer.
+  use_legacy_freezer: bool = True
+
   def make_aqt_dg(
       self,
       lhs_shape,
       rhs_shape,
       dimension_numbers: tuple[Iterable[int], Iterable[int]],
   ):
     if self.cfg is None:
@@ -152,52 +180,116 @@
     cfg = copy.deepcopy(self.cfg)
     lhs_scale_shape = list(lhs_shape)
     rhs_scale_shape = list(rhs_shape)
     (contr, _) = dimension_numbers
     for li, ri in zip(*contr):
       lhs_scale_shape[li] = 1
       rhs_scale_shape[ri] = 1
-    lhs_scale = aqt_dot_general._lhs_scale_transpose_to_output(  # pylint: disable=protected-access
+    lhs_scale = transpose.lhs_scale_transpose_to_output(
         jnp.zeros(lhs_scale_shape), dimension_numbers, lhs_shape, rhs_shape
     )
     assert lhs_scale is not None
     lhs_scale_shape = lhs_scale.shape
-    rhs_scale = aqt_dot_general._rhs_scale_transpose_to_output(  # pylint: disable=protected-access
+    rhs_scale = transpose.rhs_scale_transpose_to_output(
         jnp.zeros(rhs_scale_shape), dimension_numbers, lhs_shape, rhs_shape
     )
     assert rhs_scale is not None
     rhs_scale_shape = rhs_scale.shape
     rhs_qm = self.rhs_quant_mode
     lhs_qm = self.lhs_quant_mode
 
-    lhs_freezer = Freezer(
-        name=self.lhs_var_name,
-        quant_mode=lhs_qm,
-        q_shape=lhs_shape,
-        q_dtype=cfg.fwd.lhs.quantizer.numerics.get_dtype(),
-        q_init=self.lhs_init,
-        s_shape=lhs_scale_shape,
-        s_init=self.lhs_scale_init,
-        quant_collection=self.quant_collection,
+    assert isinstance(
+        cfg.fwd.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
     )
+    lhs_q_dtype = cfg.fwd.dg_quantizer.lhs.numerics.get_dtype()
+    rhs_q_dtype = cfg.fwd.dg_quantizer.rhs.numerics.get_dtype()
 
-    rhs_freezer = Freezer(
-        name=self.rhs_var_name,
-        quant_mode=rhs_qm,
-        q_shape=rhs_shape,
-        q_dtype=cfg.fwd.rhs.quantizer.numerics.get_dtype(),
-        q_init=self.rhs_init,
-        s_shape=rhs_scale_shape,
-        s_init=self.rhs_scale_init,
-        quant_collection=self.quant_collection,
-    )
+    if self.use_legacy_freezer:
+      lhs_freezer = Freezer(
+          name=self.lhs_var_name,
+          quant_mode=lhs_qm,
+          q_shape=lhs_shape,
+          q_dtype=lhs_q_dtype,
+          q_init=self.lhs_init,
+          s_shape=lhs_scale_shape,
+          s_init=self.lhs_scale_init,
+          quant_collection=self.quant_collection,
+      )
+
+      rhs_freezer = Freezer(
+          name=self.rhs_var_name,
+          quant_mode=rhs_qm,
+          q_shape=rhs_shape,
+          q_dtype=rhs_q_dtype,
+          q_init=self.rhs_init,
+          s_shape=rhs_scale_shape,
+          s_init=self.rhs_scale_init,
+          quant_collection=self.quant_collection,
+      )
+    else:
+      quant_to_freezer_mode = {
+          QuantMode.TRAIN: general_freezer.FreezerMode.NONE,
+          QuantMode.CALIBRATE: general_freezer.FreezerMode.NONE,
+          QuantMode.CONVERT: general_freezer.FreezerMode.WRITE,
+          QuantMode.SERVE: general_freezer.FreezerMode.READ,
+      }
+
+      def init_wrapper(
+          qt: aqt_tensor.QTensor,
+          axis_metadata_wrapper: Optional[AxisMetadataWrapper],
+      ):
+        if axis_metadata_wrapper is None:
+          return qt
+
+        # We are not doing any sharding for scale and scale_t, for now.
+        scale_non_shard_axis = range(qt.ndim)
+
+        qt = qt.replace(
+            qvalue=axis_metadata_wrapper(qt.qvalue, []),
+            scale=jax.tree_map(
+                lambda x: axis_metadata_wrapper(x, scale_non_shard_axis),
+                qt.scale,
+            ),
+            scale_t=jax.tree_map(
+                lambda x: axis_metadata_wrapper(x, scale_non_shard_axis),
+                qt.scale_t,
+            ),
+        )
+        return qt
+
+      lhs_init_wrapper = functools.partial(
+          init_wrapper, axis_metadata_wrapper=self.lhs_axis_metadata_wrapper
+      )
+      rhs_init_wrapper = functools.partial(
+          init_wrapper, axis_metadata_wrapper=self.rhs_axis_metadata_wrapper
+      )
+
+      lhs_freezer = general_freezer.Freezer(
+          name=self.lhs_var_name,
+          mode=quant_to_freezer_mode[lhs_qm],
+          collection=self.quant_collection,
+          axis_metadata_wrapper=lhs_init_wrapper,
+      )
+
+      rhs_freezer = general_freezer.Freezer(
+          name=self.rhs_var_name,
+          mode=quant_to_freezer_mode[rhs_qm],
+          collection=self.quant_collection,
+          axis_metadata_wrapper=rhs_init_wrapper,
+      )
 
     prng_name = self.prng_name
     key = self.make_rng(prng_name) if prng_name is not None else None
-    cfg = config.set_context(cfg, key, train_step=None)
+    cfg = config.set_context(
+        cfg,
+        key,
+        train_step=None,
+        lhs_quant_mode=self.lhs_quant_mode,
+        rhs_quant_mode=self.rhs_quant_mode,
+    )
 
     def ret_dg(
         lhs,
         rhs,
         dimension_numbers,
         precision=None,
         preferred_element_type=None,
@@ -210,29 +302,32 @@
       # TODO(yichizh): asserting xhs dtype only when apply_quant_mode=False
       # and cfg.get_qtensor() is None
       msg = 'AQT is not yet optimized to accept quantized types directly. '
       msg += f'lhs.dtype: {lhs.dtype}, rhs.dtype: {rhs.dtype}'
       assert lhs.dtype in [jnp.bfloat16, jnp.float32, jnp.float16], msg
       assert rhs.dtype in [jnp.bfloat16, jnp.float32, jnp.float16], msg
 
-      config.assert_config_validity(cfg)
+      cfg.assert_config_validity()
 
       # Getter
       lhs_apply_quant_mode = self.lhs_apply_quant_mode
       rhs_apply_quant_mode = self.rhs_apply_quant_mode
       lhs_qt = lhs_freezer.get() if lhs_apply_quant_mode else self.lhs_qtensor
       rhs_qt = rhs_freezer.get() if rhs_apply_quant_mode else self.rhs_qtensor
-      out, (out_lhs_qt, out_rhs_qt) = cfg.dg_core(
-          lhs=lhs,
-          rhs=rhs,
-          lhs_qt=lhs_qt,
-          rhs_qt=rhs_qt,
-          dimension_numbers=dimension_numbers,
+
+      cfg.apply_custom_vjp_on_jax = False
+      out, (out_lhs_qt, out_rhs_qt) = aqt_flax_dg_core.dg_core_flax_lifted(
+          lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, self, cfg
       )
+
       # Setter
+      msg = 'Only the newer version of freezer allows not storing scale_t.'
+      assert not (
+          self.use_legacy_freezer and utils.CALCULATE_SCALE_T_ONLINE
+      ), msg
       if self.lhs_apply_quant_mode:
         lhs_freezer.set(out_lhs_qt)
       if self.rhs_apply_quant_mode:
         rhs_freezer.set(out_rhs_qt)
 
       return out
 
@@ -243,25 +338,43 @@
       self,
       lhs,
       rhs,
       dimension_numbers,
       precision,
       preferred_element_type=None,
   ):
-
-    aqt_dg = self.make_aqt_dg(lhs.shape, rhs.shape, dimension_numbers)
     if self.tiling_cfg is not None:
+      # Extract tiled input shapes and dimension numbers from jaxpr
+      def dummy_tiled_dg(lhs_in, rhs_in):
+        return tiled_dot_general.tiled_dot_general(
+            self.tiling_cfg, lhs_in, rhs_in, dimension_numbers
+        )
+
+      tiled_dg_jaxpr = jax.make_jaxpr(dummy_tiled_dg)(lhs, rhs)
+      dg_eqn = [eqn for eqn in tiled_dg_jaxpr.eqns if 'dot_general' in str(eqn)]
+      assert len(dg_eqn) == 1, 'Multiple dg calls are found in tiled dg jaxpr.'
+      lhs_invar, rhs_invar = dg_eqn[0].invars
+      tiled_lhs_shape = lhs_invar.aval.shape
+      tiled_rhs_shape = rhs_invar.aval.shape
+      tiled_dimension_numbers = dg_eqn[0].params['dimension_numbers']
+      # Use tiled input shapes and dimension numbers to create aqt_dg that
+      # will be injected to tiled_dot_general
+      aqt_dg = self.make_aqt_dg(
+          tiled_lhs_shape, tiled_rhs_shape, tiled_dimension_numbers
+      )
       # We integrate tiling here and not on Jax level, so that the Freezers
       # observe tiled shapes.
-      aqt_dg = functools.partial(
+      ret_dg = functools.partial(
           tiled_dot_general.tiled_dot_general,
           self.tiling_cfg,
           dot_general=aqt_dg,
       )
-    return aqt_dg(
+    else:
+      ret_dg = self.make_aqt_dg(lhs.shape, rhs.shape, dimension_numbers)
+    return ret_dg(
         lhs,
         rhs,
         dimension_numbers,
         precision,
         preferred_element_type,
     )
 
@@ -270,34 +383,57 @@
   """Quantized Einsum class for model injection."""
 
   cfg: Optional[config.DotGeneral] = None
   prng_name: Optional[str] = 'params'
 
   # TODO(lew): split out separate class for each side.
   lhs_quant_mode: QuantMode = QuantMode.TRAIN
-  lhs_init: nn.initializers.Initializer = jnp.zeros
-  lhs_scale_init: nn.initializers.Initializer = jnp.zeros
   lhs_var_name: str = 'qlhs'
 
   rhs_quant_mode: QuantMode = QuantMode.TRAIN
+  rhs_var_name: str = 'qrhs'
+
+  # Variables only for the legacy Freezer.
+  lhs_init: nn.initializers.Initializer = jnp.zeros
+  lhs_scale_init: nn.initializers.Initializer = jnp.zeros
+
   rhs_init: nn.initializers.Initializer = jnp.zeros
   rhs_scale_init: nn.initializers.Initializer = jnp.zeros
-  rhs_var_name: str = 'qrhs'
+
+  # Variables only for the new Freezer.
+  lhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
+  rhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
 
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
 
+  assert_eqn: Optional[str] = None
+  assert_lhs_shape: Optional[utils.ShapeTemplate] = None
+  assert_rhs_shape: Optional[utils.ShapeTemplate] = None
+  tile_sizes: Optional[tiled_dot_general.EinsumTileSizes] = None
+
+  # If set to True, use the current Freezer. Otherwise, use the new
+  # QTensorFreezer.
+  use_legacy_freezer: bool = True
+
   @nn.compact
   def __call__(
       self,
       eqn,
       lhs_g: Union[jnp.ndarray, aqt_tensor.QTensor],
       rhs_g: Union[jnp.ndarray, aqt_tensor.QTensor],
   ):
+    if self.assert_eqn is not None:
+      utils.assert_eq(eqn, self.assert_eqn, 'einsum_eqn')
+    if self.assert_lhs_shape is not None:
+      utils.assert_shape(lhs_g.shape, self.assert_lhs_shape, 'lhs.shape')
+    if self.assert_rhs_shape is not None:
+      utils.assert_shape(rhs_g.shape, self.assert_rhs_shape, 'rhs.shape')
+
     cfg = self.cfg
     lhs_is_qt = isinstance(lhs_g, aqt_tensor.QTensor)
     rhs_is_qt = isinstance(rhs_g, aqt_tensor.QTensor)
     msg = 'Aqt config is None but inputs to AqtEinsum are QTensor.'
     assert not ((lhs_is_qt or rhs_is_qt) and cfg is None), msg
     # when inputs are qtensor, xhs_in is a dummy input that will be consumed by
     # lax einsum API, but it is not used for computation in aqt_dg because it
@@ -322,52 +458,70 @@
     yes_swap = lhs_g_id == rhs_l_id and rhs_g_id == lhs_l_id
     assert not_swap != yes_swap
 
     prng_name = self.prng_name
 
     lhs_quant_mode = self.lhs_quant_mode
     lhs_init = self.lhs_init
+    lhs_axis_metadata_wrapper = self.lhs_axis_metadata_wrapper
     lhs_scale_init = self.lhs_scale_init
     lhs_var_name = self.lhs_var_name
     lhs_qtensor = lhs_g if lhs_is_qt else None
 
     rhs_quant_mode = self.rhs_quant_mode
     rhs_init = self.rhs_init
+    rhs_axis_metadata_wrapper = self.rhs_axis_metadata_wrapper
     rhs_scale_init = self.rhs_scale_init
     rhs_var_name = self.rhs_var_name
     rhs_qtensor = rhs_g if rhs_is_qt else None
 
     quant_collection = self.quant_collection
+    tiling_config = None
+    if self.tile_sizes is not None:
+      tiling_config = tiled_dot_general.Cfg.from_einsum(eqn, self.tile_sizes)
 
     if yes_swap:
       if cfg is not None:
         cfg = copy.deepcopy(cfg)
         cfg.fwd.lhs, cfg.fwd.rhs = cfg.fwd.rhs, cfg.fwd.lhs
+        cfg.fwd.dg_quantizer.swap_lhs_and_rhs()
         cfg.dlhs, cfg.drhs = cfg.drhs, cfg.dlhs
       lhs_quant_mode, rhs_quant_mode = rhs_quant_mode, lhs_quant_mode
       lhs_init, rhs_init = rhs_init, lhs_init
       lhs_scale_init, rhs_scale_init = rhs_scale_init, lhs_scale_init
       lhs_var_name, rhs_var_name = rhs_var_name, lhs_var_name
       lhs_is_qt, rhs_is_qt = rhs_is_qt, lhs_is_qt
       lhs_qtensor, rhs_qtensor = rhs_qtensor, lhs_qtensor
+      lhs_axis_metadata_wrapper, rhs_axis_metadata_wrapper = (
+          rhs_axis_metadata_wrapper,
+          lhs_axis_metadata_wrapper,
+      )
+      if tiling_config is not None:
+        tiling_config = tiled_dot_general.Cfg(
+            lhs=tiling_config.rhs, rhs=tiling_config.lhs
+        )
 
     aqt_dg = AqtDotGeneral(
         cfg=cfg,
         prng_name=prng_name,
         lhs_quant_mode=lhs_quant_mode,
         # when passing pre-computed qtensor as inputs, apply_quant_mode flag
         # should be set to False so that Freezer will not be set to overwrite
         # the qtensor passed to dg.
         lhs_apply_quant_mode=not lhs_is_qt,  # Freezer not used if lhs is qt
         lhs_init=lhs_init,
+        lhs_axis_metadata_wrapper=lhs_axis_metadata_wrapper,
         lhs_scale_init=lhs_scale_init,
         lhs_var_name=lhs_var_name,
         lhs_qtensor=lhs_qtensor,
         rhs_quant_mode=rhs_quant_mode,
         rhs_apply_quant_mode=not rhs_is_qt,  # Freezer not used if rhs is qt
         rhs_init=rhs_init,
+        rhs_axis_metadata_wrapper=rhs_axis_metadata_wrapper,
         rhs_scale_init=rhs_scale_init,
         rhs_var_name=rhs_var_name,
         rhs_qtensor=rhs_qtensor,
         quant_collection=quant_collection,
+        tiling_cfg=tiling_config,
+        use_legacy_freezer=self.use_legacy_freezer,
     )
     return einsum(lhs=lhs_in, rhs=rhs_in, dg=aqt_dg)
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/flax/aqt_flax_test.py` & `aqtp-0.7.0/aqt/jax/v2/numerics/int_numerics.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,114 +7,117 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Numerics for int8, int4, binary and other integer types."""
 
-"""Test for AQT flax."""
-import functools
-from absl.testing import absltest
-from absl.testing import parameterized
-from aqt.jax.v2 import config
-from aqt.jax.v2.flax import aqt_flax
-import flax.linen as nn
-import jax
+from typing import Any, Optional
+from aqt.jax.v2 import stochastic_rounding
+from aqt.jax.v2 import utils
+from aqt.jax.v2.numerics import numerics
+from jax import lax
 import jax.numpy as jnp
 
 
-class AqtFlaxTest(parameterized.TestCase):
-
-  def test_aqt_einsum(self):
-    class Model(nn.Module):
-      aqt_cfg: config.DotGeneral | None
-      lhs_qt_external: bool = False
-      rhs_qt_external: bool = False
-
-      @nn.compact
-      def __call__(self, lhs, rhs):
-        lhs_in = lhs
-        assert not (
-            (self.lhs_qt_external or self.rhs_qt_external)
-            and (self.aqt_cfg is None)
-        ), 'aqt_cfg cannot be None when providing qtensor as inputs to einsum'
-        if self.lhs_qt_external:
-          lhs_in, _ = self.aqt_cfg.fwd.lhs.quantizer.quant(
-              lhs, calibration_axes=(2, 3)
-          )
-          lhs_dtype = self.aqt_cfg.fwd.lhs.quantizer.numerics.get_dtype()
-          lhs_in = lhs_in.qvalue_astype(lhs_dtype)
-        rhs_in = rhs
-        if self.rhs_qt_external:
-          rhs_in, _ = self.aqt_cfg.fwd.rhs.quantizer.quant(
-              rhs, calibration_axes=(1, 2)
-          )
-          rhs_dtype = self.aqt_cfg.fwd.rhs.quantizer.numerics.get_dtype()
-          rhs_in = rhs_in.qvalue_astype(rhs_dtype)
-        einsum = aqt_flax.AqtEinsum(cfg=self.aqt_cfg)
-        # xhs_qt can be inputs to AqtEinsum
-        # xhs->xhs_qt can happen outside of AqtEinsum, e.g., k/v cache quant
-        # input xhs_qt will force get_tensor() to always return xhs_qt
-        out = einsum('ijkh,mkh->ijm', lhs_in, rhs_in)
-        return out
-
-    key = jax.random.PRNGKey(0)
-    subkey1, subkey2 = jax.random.split(key, num=2)
-    lhs = jax.random.uniform(subkey1, shape=(3, 4, 5, 6))
-    rhs = jax.random.uniform(subkey2, shape=(2, 5, 6))
-
-    def test(model_cls, cfg):
-      model = model_cls(cfg)
-      out = model.apply({}, lhs, rhs, rngs={'params': jax.random.PRNGKey(0)})
-      # print(f'{out.shape=}')
-      # print(f'{out=}')
-      return out
-
-    out_float = test(Model, None)
-    out_int8 = test(Model, config.config_v4())
-    out_int8_lqt = test(
-        functools.partial(Model, lhs_qt_external=True), config.config_v4()
-    )
-    out_int8_rqt = test(
-        functools.partial(Model, rhs_qt_external=True), config.config_v4()
-    )
-    out_int8_qt = test(
-        functools.partial(Model, lhs_qt_external=True, rhs_qt_external=True),
-        config.config_v4(),
-    )
-
-    assert (out_int8 == out_int8_lqt).all(), 'lhs external qt failed'
-    assert (out_int8 == out_int8_rqt).all(), 'rhs external qt failed'
-    assert (out_int8 == out_int8_qt).all(), 'both external qt failed'
-    mse = jnp.mean(jnp.square(out_int8_qt - out_float))
-    assert mse > 0, 'Mean square error is 0. Einsum is not quantized.'
-
-  def test_einsum_grad_leak(self):
-    class CNN(nn.Module):
-      aqt_cfg: config.DotGeneral
-
-      @nn.compact
-      def __call__(self, x):
-        einsum = aqt_flax.AqtEinsum(self.aqt_cfg)
-        x = einsum('bc,ab->ac', jnp.identity(10, dtype=x.dtype), x)
-        return x
-
-    model = CNN(aqt_cfg=config.fully_quantized())
-    var = model.init({'params': jax.random.PRNGKey(0)}, jnp.ones(shape=(1, 10)))
-
-    @jax.jit
-    def apply_fn(inputs):
-      return model.apply(
-          var, inputs, rngs={'params': jax.random.PRNGKey(0)}, mutable=True
+@utils.flax_slots_dataclass
+class IntNumerics(numerics.AqtNumerics):
+  """Numerics for int8, int4, binary, etc."""
+
+  bits: int
+  preserve_zero: bool
+  # false = map max val on the end of the last bucket
+  # true = map max val on the middle of the last
+  preserve_max_val: bool
+  clip: bool
+  clip_gradient: bool
+  round: bool
+  noise_fn: Optional[stochastic_rounding.NoiseFn]
+  dtype: Optional[Any] = None
+
+  # pylint: disable=line-too-long
+  # Verifying the correctness of these functions amounts to verifying this table:
+  # if preserve_zero == F, zero might be rounded either to [-1, 0] bucket or to [0, 1] bucket
+  # preserve_zero, preserve_max_val, 8b, 2b, 1b
+  # F, F, 128.0, 2.0, 1.0  # bucket count is even; map onto the far edge of the last bucket
+  # F, T, 127.5, 1.5, 0.5  # bucket count is even; map onto the center of the last bucket
+  # T, F, 127.5, 1.5, 0.5  # bucket count is odd;  map onto the far edge of the last bucket
+  # T, T, 127.0, 1.0, 0.0  # bucket count is odd;  map onto the center of the last bucket
+  # pylint: enable=line-too-long
+
+  def get_edge_of_last_int_bucket(self):
+    ret = 2.0 ** (self.bits - 1)
+    if self.preserve_zero:
+      # Lose one bucket.
+      ret -= 0.5
+    return ret
+
+  def get_center_of_last_int_bucket(self):
+    return self.get_edge_of_last_int_bucket() - 0.5
+
+  def abs_val_mapped_to(self):
+    if self.preserve_max_val:
+      return self.get_center_of_last_int_bucket()
+    else:
+      return self.get_edge_of_last_int_bucket()
+
+  def _get_fwd_clip_bound(self):
+    # If we are not rounding, we just clip to bucket edges.
+    fwd_clip_bound = self.get_edge_of_last_int_bucket()
+    # If, after clip, we are rounding, we need to make sure that
+    # we won't round values at the clip_bound away to the
+    # non-existing bucket.
+    if self.round:
+      # Reducing fwd_clip_bound by any value in (0.0, 1.0) is correct.
+      fwd_clip_bound -= 0.5
+    return fwd_clip_bound
+
+  def get_dtype(self):
+    return self.dtype
+
+  def vjp_fwd(self, x, context):
+    """Forward pass."""
+    res = (x,)
+    input_dtype = x.dtype
+    assert self.bits <= 22, 'Too many bits, float32 has less precision.'
+
+    # Maybe noise
+    if self.noise_fn:
+      assert context.key is not None, (
+          'noise_fn is set, requestic stochastic rounding, but RNG was not '
+          'passed in Context.key'
       )
+      x = (x + self.noise_fn(x.shape, context.key)).astype(input_dtype)
 
-    @jax.jit
-    @jax.value_and_grad
-    def train_step(inputs):
-      return jnp.sum(apply_fn(inputs)[0])
-
-    train_step(jnp.ones(shape=(1, 10)))
-
-
-if __name__ == '__main__':
-  absltest.main()
+    if self.clip:
+      fwd_clip_bound = self._get_fwd_clip_bound()
+      x = jnp.clip(x, -fwd_clip_bound, fwd_clip_bound)
+
+    # Maybe round
+    if self.round:
+      # TODO(lew): Have bucket centers at 2*k + 1, not at halves.
+      round_to_halves = not self.preserve_zero
+      if round_to_halves:
+        x = jnp.floor(x) + 0.5
+      else:
+        x = lax.round(x, lax.RoundingMethod.TO_NEAREST_EVEN)
+
+    # Maybe cast: return dtype is either int or the input dtype
+    dtype = self.get_dtype()
+    x = x.astype(dtype if dtype is not None else input_dtype)
+    return x, res
+
+  def vjp_bwd(self, res, grad):
+    # Gradient of the clip function.
+    # For boundary values we will have full gradient.
+    # When using abs(max(x)) scaling, x is always in the interior, and the
+    # gradient clip is always 1. So, we can always set clip_gradient to false.
+    # However, other types of scaling may result in x being outside (i.e., there
+    # is clipping). In that case it may be desirable to make the gradient zero.
+    ret = grad
+    if self.clip_gradient:
+      (x,) = res
+      clip_bound = self._get_fwd_clip_bound()
+      ret *= (-clip_bound <= x) * (x <= clip_bound)
+    return (ret, None)
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/numerics/no_numerics.py` & `aqtp-0.7.0/aqt/jax/v2/numerics/no_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/numerics/numerics.py` & `aqtp-0.7.0/aqt/jax/v2/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/pax/pax_base_ops.py` & `aqtp-0.7.0/aqt/jax/v2/pax/pax_base_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,24 +14,30 @@
 
 """Injectable AQT ops.
 
 Pax implements vanilla op wrappers in praxis/layers/base_ops.py
 This file contains AQT variants of these.
 """
 
+import functools
+from aqt.jax.v2 import tiled_dot_general
 import aqt.jax.v2.aqt_dot_general as aqt
 import aqt.jax.v2.config as aqt_config
 import jax.numpy as jnp
 from praxis import base_layer
 
 
 class AqtEinsum(base_layer.BaseLayer):
   """Quantized Einsum class for model injection."""
 
   cfg: aqt_config.DotGeneral | None = None
+  # Einsum can switch the argument order before they are passed to dot_general
+  # tiling_cfg is a config for the underlying dot_general, not for the einsum.
+  # TODO(lew): Port the switch logic from flax/ to pax/
+  tiling_cfg: tiled_dot_general.Cfg | None = None
   track_train_step: bool = False
 
   def setup(self) -> None:
     if self.track_train_step:
       self.create_variable(
           'train_step',
           base_layer.WeightHParams(
@@ -52,10 +58,16 @@
     else:
       train_step = None
     cfg = self.cfg
     if cfg is not None:
       key = self.next_prng_key()
       cfg = aqt_config.set_context(cfg, key, train_step)
     dg = aqt.make_dot_general(cfg)
+    if self.tiling_cfg is not None:
+      dg = functools.partial(
+          tiled_dot_general.tiled_dot_general,
+          self.tiling_cfg,
+          dot_general=dg,
+      )
     # jnp.einsum is by default jitted, which makes the key storing in cfg
     # cross the jit boundary. We need to call a non-jitted jnp.einsum below
     return aqt.einsum(eqn, lhs, rhs, dg)
```

### Comparing `aqtp-0.6.2/aqt/jax/v2/pax/pax_base_ops_test.py` & `aqtp-0.7.0/aqt/jax/v2/pax/pax_base_ops_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/stochastic_rounding.py` & `aqtp-0.7.0/aqt/jax/v2/stochastic_rounding.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax/v2/tiled_dot_general_test.py` & `aqtp-0.7.0/aqt/jax/v2/tiled_dot_general_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 
 """Test for AQT Tiled Dot General."""
 import itertools
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.jax.v2 import tiled_dot_general
+from aqt.jax.v2 import utils
 import jax
 import jax.numpy as jnp
 import numpy as np
 import sympy
 
 
-AxisIdx = tiled_dot_general.AxisIdx
+AxisIdx = utils.AxisIdx
 TensorTiling = tiled_dot_general.TensorTiling
 Cfg = tiled_dot_general.Cfg
 AxisTiling = tiled_dot_general.AxisTiling
 
 
-def get_shape_from_axes(
-    axes: list[tiled_dot_general.AxisIdx], shape
-) -> list[int]:
+def get_shape_from_axes(axes: list[AxisIdx], shape) -> list[int]:
   return [shape[i] for i in axes]
 
 
 def assign_input_shape(
     rng_key, ca_shape: list[int], ba_shape: list[int], ra_shape: list[int]
 ):
   """Randomly assign an axis to a shape."""
@@ -50,16 +49,16 @@
   ra = axes[num_ca + num_ba :]
   raw_input_shape = np.array(ca_shape + ba_shape + ra_shape)
   input_shape = raw_input_shape[np.argsort(axes)].tolist()
   return ca, ba, ra, input_shape
 
 
 def get_axis_tiles(
-    axes: list[tiled_dot_general.AxisIdx], shape: list[int]
-) -> list[list[tiled_dot_general.AxisTiling]]:
+    axes: list[AxisIdx], shape: list[int]
+) -> list[list[AxisTiling]]:
   # Assume tiling all axes
   ret = list(
       itertools.product(*[
           [
               tiled_dot_general.AxisTiling(axis, tc, shape[axis] // tc)
               for tc in sympy.divisors(shape[axis])
           ]
```

### Comparing `aqtp-0.6.2/aqt/jax_legacy/README.md` & `aqtp-0.7.0/aqt/jax_legacy/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb` & `aqtp-0.7.0/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/README.md` & `aqtp-0.7.0/aqt/jax_legacy/jax/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/compute_cost_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/compute_cost_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/compute_cost_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/compute_cost_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/flax/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/flax/struct.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/flax/struct.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/flax_attention.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/flax_attention.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/flax_attention_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/flax_attention_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/flax_layers.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/flax_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from aqt.jax_legacy.jax import quantization
 from aqt.jax_legacy.jax import shape_utils
 from aqt.jax_legacy.jax import stats_tag
 from aqt.jax_legacy.jax import utils
 from aqt.jax_legacy.jax.flax import struct as flax_struct
 from aqt.jax_legacy.jax.quantization import QuantOps
 from aqt.jax_legacy.jax.quantization import QuantType
-from aqt.jax_legacy.jax.sparsity import SparseHParams
-from aqt.jax_legacy.jax.sparsity import Sparsity
+from aqt.jax_legacy.jax.sparsity.sparsity_core_depr import SparseHParams
+from aqt.jax_legacy.jax.sparsity.sparsity_core_depr import Sparsity
 import flax
 from flax import linen as nn
 from flax.core import frozen_dict
 from flax.linen import partitioning
 import jax
 from jax import lax
 import jax.numpy as jnp
@@ -49,23 +49,30 @@
 # Alias for initializer function.
 # Should follow the template `def init(key, shape, dtype=dtype) -> ndarray:`.
 # See flax.linen.initializers and jax.nn.initializers for more details.
 InitializerType = Callable[[jnp.ndarray, Sequence[int], Type[Any]], jnp.ndarray]
 
 default_kernel_init = nn.initializers.lecun_normal()
 
-dataclass = flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
+dataclass = (
+    flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
+)
 
 Array = jnp.ndarray
 DType = jnp.dtype
 PRNGKey = jnp.ndarray
 Shape = Sequence[int]
 Initializer = Callable[[PRNGKey, Shape, DType], Array]
-PrecisionLike = Union[None, str, lax.Precision, Tuple[str, str],
-                      Tuple[lax.Precision, lax.Precision]]
+PrecisionLike = Union[
+    None,
+    str,
+    lax.Precision,
+    Tuple[str, str],
+    Tuple[lax.Precision, lax.Precision],
+]
 
 
 # Based on flax.linen.Dense
 class DenseAqt(nn.Module):
   """A linear transformation with optional per-feature weight quantization.
 
   Attributes:
@@ -148,23 +155,27 @@
     batch_size = inputs.shape[0]
     if padding_mask is not None:
       shape_utils.assert_shapes_equal(padding_mask.shape, (batch_size, 1))
     # TODO(wanglisa): Replace fake quant with AQT.
 
     if self.dynamic_context.collect_acts_stats:
       stats_tag.StatsTag(
-          channel_axis=-1, name='inputs', update_stats=self.train)(
-              inputs, mask=padding_mask)
+          channel_axis=-1, name='inputs', update_stats=self.train
+      )(inputs, mask=padding_mask)
     hparams = self.hparams
 
-    if (hparams.weight_prec is not None and
-        isinstance(hparams.weight_prec, int) and hparams.weight_prec > 8):
+    if (
+        hparams.weight_prec is not None
+        and isinstance(hparams.weight_prec, int)
+        and hparams.weight_prec > 8
+    ):
       raise NotImplementedError(
-          'If you want to use more than 8bits for quantization, please revisit '
-          'jax.lax.Precision.DEFAULT to determine whether it is still sufficient.'
+          'If you want to use more than 8bits for quantization, please revisit'
+          ' jax.lax.Precision.DEFAULT to determine whether it is still'
+          ' sufficient.'
       )
 
     if not isinstance(self.features, tuple):
       features = (self.features,)
     else:
       features = self.features
     kernel_shape = (inputs.shape[-1],) + features
@@ -399,26 +410,32 @@
     axis = _canonicalize_tuple(self.axis)
 
     inputs = jnp.asarray(inputs, self.dtype)
     axis = _normalize_axes(axis, inputs.ndim)
 
     hparams = self.hparams
 
-    if (hparams.weight_prec is not None and
-        isinstance(hparams.weight_prec, int) and hparams.weight_prec > 8):
+    if (
+        hparams.weight_prec is not None
+        and isinstance(hparams.weight_prec, int)
+        and hparams.weight_prec > 8
+    ):
       raise NotImplementedError(
-          'If you want to use more than 8bits for quantization, please revisit '
-          'jax.lax.Precision.DEFAULT to determine whether it is still sufficient.'
+          'If you want to use more than 8bits for quantization, please revisit'
+          ' jax.lax.Precision.DEFAULT to determine whether it is still'
+          ' sufficient.'
       )
 
     kernel_shape = tuple([inputs.shape[ax] for ax in axis]) + features
     scale_shape = (1,) * len(axis) + features
     if self.reshape_kernel:
-      kernel_param_shape = (np.prod([inputs.shape[ax] for ax in axis]),
-                            np.prod(features))
+      kernel_param_shape = (
+          np.prod([inputs.shape[ax] for ax in axis]),
+          np.prod(features),
+      )
       scale_param_shape = (1, np.prod(features))
     else:
       kernel_param_shape = kernel_shape
       scale_param_shape = scale_shape
 
     # Determine axes names metadata for partitioning/adafactor rules.
     if self.kernel_axis_names is None:
@@ -628,16 +645,17 @@
 
     Returns:
       The convolved data.
     """
     hparams = self.hparams
     if hparams.weight_prec is not None and hparams.weight_prec > 8:
       raise NotImplementedError(
-          'If you want to use more than 8bits for quantization, please revisit '
-          'jax.lax.Precision.DEFAULT to determine whether it is still sufficient.'
+          'If you want to use more than 8bits for quantization, please revisit'
+          ' jax.lax.Precision.DEFAULT to determine whether it is still'
+          ' sufficient.'
       )
     jax_precision = jax.lax.Precision.DEFAULT
 
     if self.strides is None:
       strides = (1,) * (inputs.ndim - 2)
     else:
       strides = self.strides
```

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/flax_layers_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/flax_layers_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/fp_cast.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/fp_cast.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/fp_cast_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/fp_cast_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/get_bounds.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/get_bounds.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/get_bounds_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/get_bounds_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/hlo_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/hlo_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/hlo_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/hlo_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/README.md` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/check_config_util.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/check_config_util.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/base_config.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/README.md` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/configs_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/configs_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/hparams_config.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/hparams_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/imagenet.png` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/imagenet.png`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/input_pipeline.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/models.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/models_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/pokebnn.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/pokebnn.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/pokebnn_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/pokebnn_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train_benchmark.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train_benchmark.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/imagenet/train_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/imagenet/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/primitives.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/primitives.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/primitives_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/primitives_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/quant_config.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/quant_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/quantization.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/quantization_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/quantization_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/shape_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/shape_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/sparsity.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
 )
 
 
 # TODO(ayazdan): Create abstract class for sparsity configurations.
 class SparseType(str, enum.Enum):
   """Pruning types dataclass."""
+
   STRUCTURED_NM = 'STRUCTURED_NM'
   UNSTRUCTURED = 'UNSTRUCTURED'
 
 
 @dataclass
 class SparseHParams:
   """Hyper parameters for sparsity.
@@ -49,22 +50,22 @@
     type: Input array for which pruning mask is computed.
     prune_rate: Pruning rate.
     order: Apply pruning using this index order. Supported values are `C`, `R`.
       `C` and `R` indicate column-wise and row-wise ordering, respectively.
     absolute: If True, the absolute value of the values are used for sorting.
     smallest: If True, the smallest values in inputs are masked.
     structure_decay: If True, a decaying mechanism is applied on the structure.
-    mask_decay_weight: If 0.0, no mask decay is applied. The mask value
-      start with 1.0 and each time `num_update_sparsity` * `mask_decay_weight`
-      is subtracted from 1.0. Due to overhead of jit, we limited the number of
+    mask_decay_weight: If 0.0, no mask decay is applied. The mask value start
+      with 1.0 and each time `num_update_sparsity` * `mask_decay_weight` is
+      subtracted from 1.0. Due to overhead of jit, we limited the number of
       updates to `num_update_sparsity` to 16. After 16 iterations, we forcefully
       set `mask_decay_value` to zero. Mask decaying works for both structured
       and unstructured sparsity.
-    sparse_ste: If True, a sparse-refined straight-through estimator (SR-STE)
-      is applied, following the algorithm described in:
+    sparse_ste: If True, a sparse-refined straight-through estimator (SR-STE) is
+      applied, following the algorithm described in:
         https://arxiv.org/abs/2102.04010
     sparse_ste_weight: Denotes the relative weight for the sparse-refined term.
       As mentioned in the paper (https://arxiv.org/abs/2102.04010), the best
       default value is 0.0002 (lambda_w in the paper).
   """
 
   type: SparseType
@@ -79,50 +80,56 @@
   mask_decay_weight: float = 0.0
   sparse_ste: bool = False
   sparse_ste_weight: float = 0.0002
 
   def __post_init__(self):
     if self.prune_rate is not None:
       if self.type == SparseType.STRUCTURED_NM:
-        assert isinstance(self.prune_rate,
-                          Tuple), ('prune rate should be either '
-                                   'None for no pruning or a '
-                                   'Tuple (N, M) for '
-                                   'STRUCTURED_NM sparsity')
+        assert isinstance(self.prune_rate, Tuple), (
+            'prune rate should be either '
+            'None for no pruning or a '
+            'Tuple (N, M) for '
+            'STRUCTURED_NM sparsity'
+        )
       elif self.type == SparseType.UNSTRUCTURED:
-        assert isinstance(self.prune_rate,
-                          float), ('prune rate should be either '
-                                   'None for no pruning or float for '
-                                   'UNSTRUCTURED sparsity')
+        assert isinstance(self.prune_rate, float), (
+            'prune rate should be either '
+            'None for no pruning or float for '
+            'UNSTRUCTURED sparsity'
+        )
       else:
         assert False, 'prune rate unknown!'
 
       assert self.mask_decay_weight >= 0.0, (
           'Invalid value for '
           f'{self.mask_decay_weight}. '
-          '`mask_decay_weight` must be positive.')
+          '`mask_decay_weight` must be positive.'
+      )
 
       if self.sparse_ste:
         if self.mask_decay_weight != 0.0:
           raise ValueError('SR-STE only works with non-decaying mask.')
         if self.structure_decay:
           raise ValueError(
-              'SR-STE only works with non-decaying sparse structure.')
+              'SR-STE only works with non-decaying sparse structure.'
+          )
         if self.type != SparseType.STRUCTURED_NM:
           raise ValueError('SR-STE only works with structured sparsity.')
 
 
 @functools.partial(jax.custom_vjp, nondiff_argnums=(4, 5, 6))
-def sr_ste(inputs: jnp.ndarray,
-           mask: jnp.ndarray,
-           update_mask: bool,
-           apply_mask: bool,
-           sparsity_hparams: SparseHParams,
-           n_sparsity: int = 0,
-           m_sparsity: int = 0):
+def sr_ste(
+    inputs: jnp.ndarray,
+    mask: jnp.ndarray,
+    update_mask: bool,
+    apply_mask: bool,
+    sparsity_hparams: SparseHParams,
+    n_sparsity: int = 0,
+    m_sparsity: int = 0,
+):
   """Wrapper function for custom derivative rule for structured sparsity.
 
   Algorithm description: https://arxiv.org/abs/2102.04010
 
   The last three arguments are forced to be static to simplify
     the implementation.
 
@@ -142,37 +149,46 @@
   return sr_ste_fwd(
       inputs=inputs,
       mask=mask,
       update_mask=update_mask,
       apply_mask=apply_mask,
       sparsity_hparams=sparsity_hparams,
       n_sparsity=n_sparsity,
-      m_sparsity=m_sparsity)[0]
+      m_sparsity=m_sparsity,
+  )[0]
 
 
 @functools.partial(jax.jit, static_argnums=(4, 5, 6))
-def sr_ste_fwd(inputs: jnp.ndarray,
-               mask: jnp.ndarray,
-               update_mask: bool,
-               apply_mask: bool,
-               sparsity_hparams: SparseHParams,
-               n_sparsity: int = 0,
-               m_sparsity: int = 0) -> jnp.ndarray:
+def sr_ste_fwd(
+    inputs: jnp.ndarray,
+    mask: jnp.ndarray,
+    update_mask: bool,
+    apply_mask: bool,
+    sparsity_hparams: SparseHParams,
+    n_sparsity: int = 0,
+    m_sparsity: int = 0,
+) -> jnp.ndarray:
   """Custom forward pass for structured sparsity."""
   # pylint:disable=g-long-lambda
   updated_mask = jax.lax.cond(
-      update_mask, lambda: get_sparsity_mask(
-          inputs, sparsity_hparams, n_sparsity, m_sparsity), lambda: mask)
-  updated_inputs = jax.lax.cond(apply_mask,
-                                lambda: jnp.multiply(updated_mask, inputs),
-                                lambda: inputs)
+      update_mask,
+      lambda: get_sparsity_mask(
+          inputs, sparsity_hparams, n_sparsity, m_sparsity
+      ),
+      lambda: mask,
+  )
+  updated_inputs = jax.lax.cond(
+      apply_mask, lambda: jnp.multiply(updated_mask, inputs), lambda: inputs
+  )
   # pylint:enable=g-long-lambda
-  return (updated_inputs, updated_mask,  # pytype: disable=bad-return-type  # jax-ndarray
-          jnp.array(SparseHParams.sparse_ste_weight)), (
-              inputs, updated_mask, jnp.array(SparseHParams.sparse_ste_weight))
+  return (
+      updated_inputs,
+      updated_mask,  # pytype: disable=bad-return-type  # jax-ndarray
+      jnp.array(SparseHParams.sparse_ste_weight),
+  ), (inputs, updated_mask, jnp.array(SparseHParams.sparse_ste_weight))
 
 
 def sr_ste_bwd(sparsity_hparams, n_sparsity, m_sparsity, res, g):
   """Implements custom gradient for backward pass.
 
   Args:
     sparsity_hparams: Non-diff arguments as defined in `sr_ste`.
@@ -202,80 +218,90 @@
 
 class Sparsity(nn.Module):
   """Abstract class sparsity for applying sparsity."""
 
   sparsity_hparams: SparseHParams
 
   @nn.compact
-  def __call__(self,
-               inputs: jnp.ndarray,
-               *,
-               update_mask: bool,
-               apply_mask: bool,
-               num_update_sparsity: int = 0) -> jnp.ndarray:
+  def __call__(
+      self,
+      inputs: jnp.ndarray,
+      *,
+      update_mask: bool,
+      apply_mask: bool,
+      num_update_sparsity: int = 0,
+  ) -> jnp.ndarray:
 
     # TODO(shivaniagrawal): make a decision on creating/not creating mask for
     # when sparsity hparams is None itself.
-    if (self.sparsity_hparams is None or
-        self.sparsity_hparams.prune_rate is None):
+    if (
+        self.sparsity_hparams is None
+        or self.sparsity_hparams.prune_rate is None
+    ):
       return inputs
 
     if self.sparsity_hparams.type == 'STRUCTURED_NM':
       n_sparsity = self.sparsity_hparams.prune_rate[0]
       m_sparsity = self.sparsity_hparams.prune_rate[1]
       if self.sparsity_hparams.structure_decay:
         if num_update_sparsity == 1:
           n_sparsity = n_sparsity - 1
         else:
           n_sparsity = int(
-              math.ceil(n_sparsity / math.pow(2, num_update_sparsity)))
+              math.ceil(n_sparsity / math.pow(2, num_update_sparsity))
+          )
     else:
       logging.info('Unstructured sparsity does not support structure decaying.')
       n_sparsity = 0
       m_sparsity = 0
 
     # Due to overhead of jit, we limited the number of updates to
     # `num_update_sparsity` to 16. Once we reach to 16, we forcefully set
     # `mask_decay_value` to zero.
     # TODO(ayazdan): Support more than 16 decay.
     mask_decay_value = 1.0
     if self.sparsity_hparams.mask_decay_weight != 0.0:
       if num_update_sparsity < 16:
         mask_decay_value = max(
-            mask_decay_value -
-            (num_update_sparsity * self.sparsity_hparams.mask_decay_weight),
-            0.0)
+            mask_decay_value
+            - (num_update_sparsity * self.sparsity_hparams.mask_decay_weight),
+            0.0,
+        )
       else:
         mask_decay_value = 0.0
     mask = self.variable('sparsity', 'mask', jnp.ones, inputs.shape, jnp.bool_)
 
     if self.sparsity_hparams.sparse_ste:
       updated_inputs, updated_mask, _ = sr_ste(
           inputs=inputs,
           mask=mask.value,
           update_mask=update_mask,
           apply_mask=apply_mask,
           sparsity_hparams=self.sparsity_hparams,
           n_sparsity=n_sparsity,
-          m_sparsity=m_sparsity)
+          m_sparsity=m_sparsity,
+      )
       if update_mask and self.has_variable('sparsity', 'mask'):
         mask.value = updated_mask
       return updated_inputs
     else:
       if update_mask and self.has_variable('sparsity', 'mask'):
-        mask.value = get_sparsity_mask(inputs, self.sparsity_hparams,
-                                       n_sparsity, m_sparsity)
+        mask.value = get_sparsity_mask(
+            inputs, self.sparsity_hparams, n_sparsity, m_sparsity
+        )
 
       if apply_mask and self.has_variable('sparsity', 'mask'):
         if self.sparsity_hparams.mask_decay_weight != 0.0:
-          return jnp.multiply(~mask.value * mask_decay_value + mask.value,
-                              inputs)
+          return jnp.multiply(
+              ~mask.value * mask_decay_value + mask.value, inputs
+          )
         else:
-          return jnp.where(mask.value, inputs,
-                           jnp.zeros(inputs.shape, inputs.dtype))
+          return jnp.where(
+              mask.value, inputs, jnp.zeros(inputs.shape, inputs.dtype)
+          )
       return inputs
 
 
 def apply_sparsity(
     inputs: jnp.ndarray,
     sparsity_hparams: SparseHParams,
     n_sparsity: int,
@@ -294,79 +320,83 @@
 ) -> jnp.ndarray:
   """Returns sparsified inputs based on sparsity hparams."""
   if sparsity_hparams is None or sparsity_hparams.prune_rate is None:
     return jnp.ones(inputs.shape, dtype=bool)
   prune_rate = sparsity_hparams.prune_rate
   if sparsity_hparams.type == 'STRUCTURED_NM':
     assert isinstance(
-        prune_rate, Tuple), 'prune rate must be tuple for structured sparsity.'
+        prune_rate, Tuple
+    ), 'prune rate must be tuple for structured sparsity.'
     assert prune_rate[0] <= prune_rate[1], (
         'prune_rate[0] must be lower than prune_rate[1] for N:M'
         f' ({prune_rate[0]}:{prune_rate[1]}) sparsity.'
     )
     return get_pruning_n_m_mask(
         inputs,
         n=n_sparsity,
         m=m_sparsity,
         order=sparsity_hparams.order,
         absolute=sparsity_hparams.absolute,
-        smallest=sparsity_hparams.smallest)
+        smallest=sparsity_hparams.smallest,
+    )
   elif sparsity_hparams.type == 'UNSTRUCTURED':
     assert (
         isinstance(prune_rate, float) and prune_rate < 1
     ), f'sparsity ratio can not be > 1, provided prune_rate {prune_rate}.'
     return get_pruning_unstruct_mask(
-        inputs, prune_rate=prune_rate, smallest=sparsity_hparams.smallest)
+        inputs, prune_rate=prune_rate, smallest=sparsity_hparams.smallest
+    )
   else:
     raise ValueError(f'invalid sparsity type {sparsity_hparams.type}!')
 
 
 # TODO(ayazdan): Support arrays with length not divisible by `m`.
-def prune_inputs_n_m(inputs: jnp.ndarray,
-                     *,
-                     n: int,
-                     m: int,
-                     order: str = 'R',
-                     offset: int = 0,
-                     absolute: bool = True,
-                     smallest: bool = True) -> jnp.ndarray:
+def prune_inputs_n_m(
+    inputs: jnp.ndarray,
+    *,
+    n: int,
+    m: int,
+    order: str = 'R',
+    offset: int = 0,
+    absolute: bool = True,
+    smallest: bool = True,
+) -> jnp.ndarray:
   """Returns pruned array with N:M (structured) pruning.
 
   N:M pruning makes at most N values non-zero in each block of M consecutive
   values.
 
   Args:
     inputs: Input array for which N:M pruning mask is computed.
     n: Maximum number of non-zero values in each block.
     m: Number of values in each block.
     order: Apply pruning using this index order. Supported values are `C`, `R`.
-    `C` -> Column-wise pruning.
-    `R` -> Row-wise pruning.
+      `C` -> Column-wise pruning. `R` -> Row-wise pruning.
     offset: Indicates the offset between the group of M elements on which
       N:M sparsity is applied. The default is `0` (narrowly-separate),
-      indicating that `M` elements are selected from adjacent values in
-      the input matrix. Generally, because of the XLA layout
-      (lanes 128/sublanes 8), another value for offset would be 128
-      (widely-separated).
-      If offset > 0, we only support scenarios where the input array size is
-      equal to (offset * m).
+        indicating that `M` elements are selected from adjacent values in the
+        input matrix. Generally, because of the XLA layout (lanes 128/sublanes
+        8), another value for offset would be 128 (widely-separated). If offset
+        > 0, we only support scenarios where the input array size is equal to
+        (offset * m).
     absolute: If True, the absolute value of the values are used for sorting.
     smallest: If True, the smallest values in inputs are masked.
 
   Returns:
     An array with the same shape as inputs pruned with N:M strategy.
   """
   mask = get_pruning_n_m_mask(
       inputs,
       n,
       m,
       order=order,
       offset=offset,
       absolute=absolute,
-      smallest=smallest)
+      smallest=smallest,
+  )
   return jnp.where(mask, inputs, jnp.zeros(inputs.shape, inputs.dtype))
 
 
 # TODO(ayazdan): Add supports for magnitude pruning.
 # TODO(ayazdan): Add supports for column-wise pruning.
 # TODO(ayazdan): Add for other form of N:M pruning.
 # TODO(ayazdan): Add parameter `r` for decaying weights.
@@ -375,14 +405,15 @@
 
   Args:
     inputs: Input array for which N:M pruning mask is computed.
 
   Returns:
     An array with the same shape as inputs pruned with 2:4 strategy.
   """
+
   def _cswap(a, b, cond):
     """Conditional swap of two vector."""
     return jnp.where(cond, a, b), jnp.where(cond, b, a)
 
   def _prune(a, n, r):
     """Prunes the first n elements with a decaying factor of (1-r).
 
@@ -425,15 +456,16 @@
     end = list(jnp.shape(xin))
     strides = [1] * (len(jnp.shape(xin)) - 1) + [m]
     xs = []
     for i in range(m):
       start_i = start
       start_i[-1] = i
       xs.append(
-          jnp.reshape(lax.slice(xin, start_i, end, strides), [-1, red_dim]))
+          jnp.reshape(lax.slice(xin, start_i, end, strides), [-1, red_dim])
+      )
     return xs, start, end, red_dim
 
   def _postprocessing(xin, start, end, red_dim, shape_in):
     """Reorganizes the input vector back to its original shape.
 
     Example:
       Input:
@@ -444,16 +476,16 @@
       Output:
         (0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (0, 5), (0, 6), (0, 7)
 
     Args:
       xin: Input array on which the reorganizatin occurs.
       start: The starting indices of each dimension.
       end: The ending indices of each dimension.
-      red_dim: Indicates the last dimension of input array divided
-        by group size (m).
+      red_dim: Indicates the last dimension of input array divided by group size
+        (m).
       shape_in: The original shape of the input array.
 
     Returns:
       A reorganized array back to its original shape after sparsification.
     """
 
     filtered = jax.numpy.reshape(xin, shape_in)
@@ -481,103 +513,109 @@
     x, y = xy
     pruned[x], pruned[y] = _cswap(pruned[x], pruned[y], cond)
   xs_final = jnp.array(jnp.concatenate(pruned, axis=1), dtype=xs[0].dtype)
   # post-processing: reshape the array to its original form.
   return _postprocessing(xs_final, start, end, red_dim, jax.numpy.shape(inputs))
 
 
-def get_pruning_n_m_mask(inputs: jnp.ndarray,
-                         n: int,
-                         m: int,
-                         *,
-                         order: str = 'R',
-                         offset: int = 0,
-                         absolute: bool = True,
-                         smallest: bool = True) -> jnp.ndarray:
+def get_pruning_n_m_mask(
+    inputs: jnp.ndarray,
+    n: int,
+    m: int,
+    *,
+    order: str = 'R',
+    offset: int = 0,
+    absolute: bool = True,
+    smallest: bool = True,
+) -> jnp.ndarray:
   """Returns a mask for N:M (structured) pruning.
 
   N:M pruning makes at most N values non-zero in each block of M consecutive
   values.
 
   Args:
     inputs: Input array for which N:M pruning mask is computed.
     n: Maximum number of non-zero values in each block.
     m: Number of values in each block.
     order: Apply pruning using this index order. Supported values are `C`, `R`.
       `C` and `R` indicate column-wise and row-wise masking, respectively.
-      Default is `R` indicating to applying N:M sparsity across rows of
-      the input matrix.
+      Default is `R` indicating to applying N:M sparsity across rows of the
+      input matrix.
     offset: Indicates the offset between the group of M elements on which
       N:M sparsity is applied. The default is `0` (narrowly-separate),
-      indicating that `M` elements are selected from adjacent values in
-      the input matrix. Generally, because of the XLA layout
-      (lanes 128/sublanes 8), another value for offset would be 128
-      (widely-separated).
-      If offset > 0, we only support scenarios where the input array size is
-      equal to (offset * m).
+        indicating that `M` elements are selected from adjacent values in the
+        input matrix. Generally, because of the XLA layout (lanes 128/sublanes
+        8), another value for offset would be 128 (widely-separated). If offset
+        > 0, we only support scenarios where the input array size is equal to
+        (offset * m).
     absolute: If True, the absolute value of the values are used for sorting.
     smallest: If True, the smallest values in inputs are masked.
 
   Returns:
     A mask that indicates the pruning locations (`0`: no pruning, `1`: pruned).
   """
   if n > m:
     raise ValueError(f'N must be lower than M for N:M ({n}:{m}) sparsity.')
   if order not in ['C', 'R']:
     raise ValueError(f'Index order {order} not supported.')
   if offset < 0:
-    raise ValueError('Offset value must be positive. '
-                     f'You provided {offset}.')
+    raise ValueError(f'Offset value must be positive. You provided {offset}.')
   if offset != 0 and offset != 128:
     logging.warning(
         'Value %d may not be best optimized for the memory layout. '
-        'We suggest a value of `0` or `128` for offset.', offset
+        'We suggest a value of `0` or `128` for offset.',
+        offset,
     )
   length = jnp.size(inputs)
   # TODO(b/228458062): support m which is not a factor of inputs size.
   if length % m != 0:
     raise ValueError(
-        f'inputs size must be divisible by m, provided {length} and {m}')
+        f'inputs size must be divisible by m, provided {length} and {m}'
+    )
   group = int(length / m)
   inputs = jnp.abs(inputs) if absolute else inputs
   if order == 'R':
     if offset == 0:
       inputs_temp = inputs.reshape(group, m, order='C')
     else:
       if offset * m != length:
-        raise ValueError('When offset > 0, we only support an array size '
-                         '(length) equal to (offset * m). '
-                         f'Provided offset = {offset}, m = {m}, '
-                         f'length = {length}.')
+        raise ValueError(
+            'When offset > 0, we only support an array size '
+            '(length) equal to (offset * m). '
+            f'Provided offset = {offset}, m = {m}, '
+            f'length = {length}.'
+        )
       inputs_temp = jnp.transpose(inputs.reshape(m, offset, order='C'))
   else:
     inputs_temp = jnp.einsum('...ij->...ji', inputs).reshape(
-        group, m, order='C')
+        group, m, order='C'
+    )
   mask = jnp.ones(inputs_temp.shape, dtype=bool)
   # Extract the smallest elements and forcefully make them zero.
-  _, top_k_indices = jax.lax.top_k(
-      -inputs_temp, k=m - n) if smallest else jax.lax.top_k(
-          inputs_temp, k=m - n)
+  _, top_k_indices = (
+      jax.lax.top_k(-inputs_temp, k=m - n)
+      if smallest
+      else jax.lax.top_k(inputs_temp, k=m - n)
+  )
   mask = jax.vmap(lambda x, i: x.at[i].set(False))(mask, top_k_indices)
   if order == 'R':
     if offset == 0:
       return mask.reshape(inputs.shape, order='C')
     else:
       return jnp.transpose(mask).reshape(inputs.shape, order='C')
   else:
     if len(inputs.shape) > 2:
       return jnp.einsum('...ij->...ji', mask.reshape(inputs.shape, order='F'))
     else:
       return jnp.einsum('ij->ji', mask).reshape(inputs.shape, order='F')
 
 
-def get_pruning_unstruct_mask(inputs: jnp.ndarray,
-                              *,
-                              prune_rate: float = 0.1,
-                              smallest: bool = True) -> jnp.ndarray:
+def get_pruning_unstruct_mask(
+    inputs: jnp.ndarray, *, prune_rate: float = 0.1, smallest: bool = True
+) -> jnp.ndarray:
   """Returns a mask for pruning according to the prune rate.
 
   Args:
     inputs: Input array for which pruning mask is computed.
     prune_rate: Pruning rate. The ratio of the elements that are pruned. 0
       meaning no pruning. Defaults to 0.1.
     smallest: If True, the smallest values in inputs are masked.
@@ -588,25 +626,25 @@
   inputs = -jnp.abs(inputs) if smallest else jnp.abs(inputs)
   mask = jnp.ones(inputs.shape, dtype=bool)
   k = int(inputs.size * prune_rate)
   _, idxs = jax.lax.top_k(inputs.reshape(-1), k)
   return mask.reshape(-1).at[idxs].set(False).reshape(inputs.shape)
 
 
-def prune_inputs_unstruct(inputs: jnp.ndarray,
-                          *,
-                          prune_rate: float = 0.1,
-                          smallest: bool = True) -> jnp.ndarray:
+def prune_inputs_unstruct(
+    inputs: jnp.ndarray, *, prune_rate: float = 0.1, smallest: bool = True
+) -> jnp.ndarray:
   """Returns unstructured pruning for inputs according to the prune rate.
 
   Args:
     inputs: Input array which is being pruned.
     prune_rate: Pruning rate. The ratio of the elements that are pruned. 0
       meaning no pruning. Defaults to 0.1.
     smallest: If True, the smallest values in inputs are masked.
 
   Returns:
     Pruned input.
   """
   mask = get_pruning_unstruct_mask(
-      inputs, prune_rate=prune_rate, smallest=smallest)
+      inputs, prune_rate=prune_rate, smallest=smallest
+  )
   return jnp.where(mask, inputs, jnp.zeros(inputs.shape, inputs.dtype))
```

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/sparsity_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for sparsity."""
+"""Tests for sparsity_core_depr."""
 
 import dataclasses
 import typing
 
 from absl.testing import absltest
 from absl.testing import parameterized
-from aqt.jax_legacy.jax import sparsity
 from aqt.jax_legacy.jax.flax import struct as flax_struct
-from aqt.jax_legacy.jax.sparsity import SparseHParams
-from aqt.jax_legacy.jax.sparsity import Sparsity
+from aqt.jax_legacy.jax.sparsity import sparsity_core_depr
+from aqt.jax_legacy.jax.sparsity.sparsity_core_depr import SparseHParams
+from aqt.jax_legacy.jax.sparsity.sparsity_core_depr import Sparsity
 import flax
 from flax import linen as nn
 import jax
 from jax import numpy as jnp
 from jax import random
 import numpy as np
 
@@ -201,15 +201,15 @@
                        jnp.shape(xs)[-1]), axis=len(jnp.shape(inputs)))
     topk_filter = jnp.where(
         jnp.equal(mask, 0.), jnp.full(list(jnp.shape(mask)), alpha - 1), mask)
     filtered = jnp.multiply(xs, topk_filter)
     ys = jnp.concatenate(
         jnp.moveaxis(filtered, 0, 0), axis=len(jnp.shape(inputs)) - 1)
     print(ys)
-    ys_hat = sparsity.prune_2_4(inputs)
+    ys_hat = sparsity_core_depr.prune_2_4(inputs)
     print(ys_hat)
     np.testing.assert_array_equal(ys, ys_hat)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='row_wise_pruning',
           order='R',
@@ -222,15 +222,15 @@
           order='C',
           exp_output=[[0, 0, 0, 0, 0, 0, 0, 0],
                       [0, 0, 0, 0, 0, 0, 0, 0],
                       [17, 18, 19, 20, 21, 22, 23, 24],
                       [25, 26, 27, 28, 29, 30, 31, 32]]))
   def test_column_row_pruning(self, order, exp_output):
     inputs = jnp.reshape(jnp.arange(1, 33), (4, 8))
-    output = sparsity.prune_inputs_n_m(inputs, n=2, m=4, order=order)
+    output = sparsity_core_depr.prune_inputs_n_m(inputs, n=2, m=4, order=order)
     np.testing.assert_array_equal(output, exp_output)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='column_wise_pruning',
           order='C',
           exp_output=[[[0, 0, 0, 0],
@@ -247,15 +247,15 @@
                        [45, 46, 47, 48]],
                       [[0, 0, 0, 0],
                        [0, 0, 0, 0],
                        [57, 58, 59, 60],
                        [61, 62, 63, 64]]]))
   def test_3d_column_pruning(self, order, exp_output):
     inputs = jnp.reshape(jnp.arange(1, 65), (4, 4, 4))
-    output = sparsity.prune_inputs_n_m(inputs, n=2, m=4, order=order)
+    output = sparsity_core_depr.prune_inputs_n_m(inputs, n=2, m=4, order=order)
     np.testing.assert_array_equal(output, exp_output)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='offset_zero',
           offset=0,
           exp_output=[[0, 0, 3, 14, 0, 16, 0, 18, 0, 20],
@@ -265,15 +265,17 @@
           offset=5,
           exp_output=[[0, 0, 0, 14, 0, 16, 0, 18, 0, 20],
                       [11, 12, 13, 0, 15, 0, 17, 0, 19, 0]]))
   def test_n_m_row_wise_sparsity_with_offset(self, offset, exp_output):
     inputs = jnp.array([[1, 2, 3, 14, 5, 16, 7, 18, 9, 20],
                         [11, 12, 13, 4, 15, 6, 17, 8, 19, 10]])
 
-    output = sparsity.prune_inputs_n_m(inputs, n=2, m=4, offset=offset)
+    output = sparsity_core_depr.prune_inputs_n_m(
+        inputs, n=2, m=4, offset=offset
+    )
     np.testing.assert_array_equal(output, exp_output)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='update_mask_apply_mask',
           update_mask=True,
           apply_mask=True),
@@ -416,16 +418,15 @@
       (_, state), grads = jax.value_and_grad(
           loss_fn, has_aux=True, allow_int=True)(params, state)
       np.testing.assert_allclose(
           grads['kernel'], inputs + 0.0002 * jnp.multiply(
               ~state['sparsity']['weight_sparsity']['mask'], params['kernel']))
       params = update_params(params, grads)
 
-
-# TODO(shivaniagrawal): Add tests for struct sparsity as well.
+  # TODO(shivaniagrawal): Add tests for struct sparsity as well.
 
   @parameterized.named_parameters(
       dict(
           testcase_name='update_mask_apply_mask',
           update_mask=True,
           apply_mask=True,
       ),
@@ -488,30 +489,31 @@
 
   @parameterized.parameters(
       dict(sparse_type='STRUCTURED_NM', prune_rate=0.1),
       dict(sparse_type='UNSTRUCTURED', prune_rate=(4, 1)))
   def test_invalid_params(self, sparse_type, prune_rate):
     with self.assertRaisesRegex(
         AssertionError, 'prune rate should be either None for no pruning'):
-      sparsity.SparseHParams(type=sparse_type, prune_rate=prune_rate)
+      sparsity_core_depr.SparseHParams(type=sparse_type, prune_rate=prune_rate)
 
   @parameterized.parameters(
       dict(
           sparse_type='STRUCTURED_NM',
           prune_rate=(4, 1),
           mask_decay_weight=-0.1),
       dict(sparse_type='UNSTRUCTURED', prune_rate=0.2, mask_decay_weight=-0.1))
   def test_invalid_mask_decay_weight(self, sparse_type, prune_rate,
                                      mask_decay_weight):
     with self.assertRaisesRegex(AssertionError,
                                 '.* `mask_decay_weight` must be positive.'):
-      sparsity.SparseHParams(
+      sparsity_core_depr.SparseHParams(
           type=sparse_type,
           prune_rate=prune_rate,
-          mask_decay_weight=mask_decay_weight)
+          mask_decay_weight=mask_decay_weight,
+      )
 
   @parameterized.parameters(
       dict(
           sparse_type='STRUCTURED_NM',
           prune_rate=(4, 1),
           sparse_ste=True,
           mask_decay_weight=0.1),
@@ -520,19 +522,20 @@
           prune_rate=0.2,
           sparse_ste=True,
           mask_decay_weight=0.1))
   def test_invalid_sparse_ste_with_non_zero_mask_decay_weight(
       self, sparse_type, prune_rate, sparse_ste, mask_decay_weight):
     with self.assertRaisesRegex(ValueError,
                                 'SR-STE only works with non-decaying mask.'):
-      sparsity.SparseHParams(
+      sparsity_core_depr.SparseHParams(
           type=sparse_type,
           prune_rate=prune_rate,
           sparse_ste=sparse_ste,
-          mask_decay_weight=mask_decay_weight)
+          mask_decay_weight=mask_decay_weight,
+      )
 
   @parameterized.parameters(
       dict(
           sparse_type='STRUCTURED_NM',
           prune_rate=(4, 1),
           sparse_ste=True,
           structure_decay=True),
@@ -543,108 +546,115 @@
           structure_decay=True))
   def test_invalid_sparse_ste_with_structure_decay(self, sparse_type,
                                                    prune_rate, sparse_ste,
                                                    structure_decay):
     with self.assertRaisesRegex(
         ValueError,
         'SR-STE only works with non-decaying sparse structure.'):
-      sparsity.SparseHParams(
+      sparsity_core_depr.SparseHParams(
           type=sparse_type,
           prune_rate=prune_rate,
           sparse_ste=sparse_ste,
-          structure_decay=structure_decay)
+          structure_decay=structure_decay,
+      )
 
   @parameterized.parameters(
       dict(sparse_type='UNSTRUCTURED', prune_rate=0.2, sparse_ste=True))
   def test_invalid_sparse_ste_with_unstructured_sparsity(
       self, sparse_type, prune_rate, sparse_ste):
-    with self.assertRaisesRegex(ValueError,
-                                'SR-STE only works with structured sparsity.'):
-      sparsity.SparseHParams(
-          type=sparse_type,
-          prune_rate=prune_rate,
-          sparse_ste=sparse_ste)
+    with self.assertRaisesRegex(
+        ValueError, 'SR-STE only works with structured sparsity'
+    ):
+      sparsity_core_depr.SparseHParams(
+          type=sparse_type, prune_rate=prune_rate, sparse_ste=sparse_ste
+      )
 
   @parameterized.parameters(
       dict(
           sparse_type='STRUCTURED_NM',
           prune_rate=(4, 1),
           error_msg='must be lower than prune_rate'),
       dict(
           sparse_type='UNSTRUCTURED',
           prune_rate=2.5,
           error_msg='sparsity ratio can not be > 1, provided prune_rate'))
   def test_invalid_prune_rate(self, sparse_type, prune_rate, error_msg):
-    sparsity_hparams = sparsity.SparseHParams(
-        type=sparse_type, prune_rate=prune_rate)
+    sparsity_hparams = sparsity_core_depr.SparseHParams(
+        type=sparse_type, prune_rate=prune_rate
+    )
 
     inputs = jnp.arange(12)
     with self.assertRaisesRegex(AssertionError, error_msg):
-      sparsity.get_sparsity_mask(inputs, sparsity_hparams)
+      sparsity_core_depr.get_sparsity_mask(inputs, sparsity_hparams)
 
 
 class PruningFunctionalityTest(parameterized.TestCase):
 
   def test_pruning_mask(self):
     # Total number of parameters = 20
     inputs = jnp.array(np.random.rand(10, 2))
-    mask = sparsity.get_pruning_unstruct_mask(inputs, prune_rate=0.1)
+    mask = sparsity_core_depr.get_pruning_unstruct_mask(inputs, prune_rate=0.1)
     self.assertEqual(jnp.sum(mask), 18)
 
   def test_smallest_largest_magnitude_mask(self):
     # Total number of parameters = 20
     inputs = jnp.array(np.arange(20))
-    mask = sparsity.get_pruning_unstruct_mask(
-        inputs, smallest=True, prune_rate=0.1)
+    mask = sparsity_core_depr.get_pruning_unstruct_mask(
+        inputs, smallest=True, prune_rate=0.1
+    )
     self.assertFalse(mask[0])
     self.assertFalse(mask[1])
 
-    mask = sparsity.get_pruning_unstruct_mask(
-        inputs, smallest=False, prune_rate=0.1)
+    mask = sparsity_core_depr.get_pruning_unstruct_mask(
+        inputs, smallest=False, prune_rate=0.1
+    )
     self.assertFalse(mask[-1])
     self.assertFalse(mask[-2], 0)
 
   def test_prune_inputs_unstruct(self):
     # Total number of parameters = 20
     inputs = jnp.array(np.random.rand(10, 2))
-    prune_input = sparsity.prune_inputs_unstruct(inputs)
+    prune_input = sparsity_core_depr.prune_inputs_unstruct(inputs)
     self.assertEqual(jnp.sum(prune_input == 0), 2)
 
   def test_smallest_largest_magnitude_prune_unstruct(self):
     # Total number of parameters = 20
     inputs = jnp.array(np.arange(20))
-    prune_input = sparsity.prune_inputs_unstruct(inputs, prune_rate=0.1)
+    prune_input = sparsity_core_depr.prune_inputs_unstruct(
+        inputs, prune_rate=0.1
+    )
     self.assertEqual(prune_input[0], 0)
     self.assertEqual(prune_input[1], 0)
 
-    prune_input = sparsity.prune_inputs_unstruct(
-        inputs, prune_rate=0.1, smallest=False)
+    prune_input = sparsity_core_depr.prune_inputs_unstruct(
+        inputs, prune_rate=0.1, smallest=False
+    )
     self.assertEqual(prune_input[-1], 0)
     self.assertEqual(prune_input[-2], 0)
 
   def test_prune_inputs_n_m(self):
     inputs = jnp.array(np.random.rand(10, 2, 4))
-    out = sparsity.prune_inputs_n_m(inputs, n=1, m=4)
+    out = sparsity_core_depr.prune_inputs_n_m(inputs, n=1, m=4)
     self.assertEqual(out.shape[0], inputs.shape[0])
     self.assertEqual(out.shape[1], inputs.shape[1])
     self.assertEqual(out.shape[2], inputs.shape[2])
     # Only 20 non-zero elements must exist after pruning.
     self.assertEqual(out[out != 0].shape[0], 20)
     self.assertEqual(
         list(np.argmax(inputs, axis=2).flatten()),
         list(np.argmax(out != 0, axis=2).flatten()))
 
   def test_order_not_valid(self):
     inputs = jnp.array(np.random.rand(10, 2, 4))
     with self.assertRaises(ValueError):
-      _ = sparsity.prune_inputs_n_m(inputs, n=1, m=4, order='X')
+      _ = sparsity_core_depr.prune_inputs_n_m(inputs, n=1, m=4, order='X')
 
   def test_n_m_pruning_mask(self):
     inputs = jnp.array(np.random.rand(10, 2, 4))
-    mask = sparsity.get_pruning_n_m_mask(inputs, n=1, m=4)
+    mask = sparsity_core_depr.get_pruning_n_m_mask(inputs, n=1, m=4)
     self.assertEqual(
         list(np.argmax(inputs, axis=2).flatten()),
         list(np.argmax(mask == 1, axis=2).flatten()))
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/stats.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/stats_tag.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/stats_tag.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/stats_tag_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/stats_tag_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/stats_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/stats_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/test_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/test_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/train_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/train_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/utils.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/README.md` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/bleu.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/bleu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/decode.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/decode.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/models.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/models_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/predict.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/predict.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/train.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,18 +204,18 @@
   Returns:
     Tuple of scalar loss and custom gradient function.
   """
   shifted = logits - logits.max(axis=-1, keepdims=True)
   exp_shifted = jnp.exp(shifted)
   sum_exp = jnp.sum(exp_shifted, axis=-1, keepdims=True)
   log_softmax = shifted - jnp.log(sum_exp)
-  loss = -jnp.sum(targets * log_softmax, axis=-1)
+  loss = - targets * log_softmax
 
   def grad_fn(g):
-    return jnp.expand_dims(g, axis=-1) * (exp_shifted / sum_exp - targets), g
+    return g * (exp_shifted / sum_exp - targets), g
 
   return loss, grad_fn
 
 
 def compute_weighted_cross_entropy(logits,
                                    targets,
                                    weights=None,
@@ -242,15 +242,15 @@
   low_confidence = (1.0 - confidence) / (vocab_size - 1)
   normalizing_constant = -(
       confidence * jnp.log(confidence) +
       (vocab_size - 1) * low_confidence * jnp.log(low_confidence + 1e-20))
   soft_targets = common_utils.onehot(
       targets, vocab_size, on_value=confidence, off_value=low_confidence)
 
-  loss = cross_entropy_with_logits(logits, soft_targets)
+  loss = jnp.sum(cross_entropy_with_logits(logits, soft_targets), axis=-1)
 
   loss = loss - normalizing_constant
 
   normalizing_factor = np.prod(targets.shape)
   if weights is not None:
     loss = loss * weights
     normalizing_factor = weights.sum()
```

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/train_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py` & `aqtp-0.7.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/README.md` & `aqtp-0.7.0/aqt/jax_legacy/utils/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/__init__.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/analysis_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/analysis_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/analysis_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/common.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/config_schema_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/config_schema_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/config_schema_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/config_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/hparams_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/hparams_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 import json
 import os
 import typing
 from typing import Any, Dict, Optional, Type, TypeVar
 
 from aqt.jax_legacy.jax import quant_config
 from aqt.jax_legacy.jax import quantization
-from aqt.jax_legacy.jax import sparsity
 from aqt.jax_legacy.jax.flax import struct as flax_struct
+from aqt.jax_legacy.jax.sparsity import sparsity_core_depr
 import dacite
 import jax
 import ml_collections
 
 
 T = TypeVar('T')
 
-dataclass = flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
+dataclass = (
+    flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
+)
 
 
 @dataclass
 class HParamsMetadata:
   """Metadata associated with an experiment configuration."""
 
   # Human-readable description of this hparams configuration. Mainly
@@ -103,15 +105,15 @@
   # to convert from a string into an enum. The classes of all enum values which
   # are stored in a TrainingHParams instance (directly or indirectly) should be
   # listed here. See https://github.com/konradhalas/dacite#casting.
   enum_classes = [
       quantization.QuantOps.ActHParams.InputDistribution,
       quantization.QuantType,
       quant_config.QuantGranularity,
-      sparsity.SparseType,
+      sparsity_core_depr.SparseType,
   ]
   data_dict = _convert_lists_to_tuples(data_dict)
   return dacite.from_dict(
       data_class=dataclass_name,
       data=data_dict,
       config=dacite.Config(cast=enum_classes))
```

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/pandas_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/pandas_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/pandas_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/report_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/report_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/report_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/summary_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/summary_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/tfevent_utils.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/tfevent_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/jax_legacy/utils/tfevent_utils_test.py` & `aqtp-0.7.0/aqt/jax_legacy/utils/tfevent_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/test/aqt_conv_test_base.py` & `aqtp-0.7.0/aqt/test/aqt_conv_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/test/aqt_matmul_test_base.py` & `aqtp-0.7.0/aqt/test/aqt_matmul_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/test/aqt_stats_test_base.py` & `aqtp-0.7.0/aqt/test/aqt_stats_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/test/aqt_tensor_test_base.py` & `aqtp-0.7.0/aqt/test/aqt_tensor_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/aqt/test/aqt_test_shared_base.py` & `aqtp-0.7.0/aqt/test/aqt_test_shared_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/papers/aqt/aqt.pdf` & `aqtp-0.7.0/papers/aqt/aqt.pdf`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/papers/aqt/aqt.tex` & `aqtp-0.7.0/papers/aqt/aqt.tex`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/papers/pokebnn/README.md` & `aqtp-0.7.0/papers/pokebnn/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/papers/pokebnn/cloudtpu_train_pokebnn.sh` & `aqtp-0.7.0/papers/pokebnn/cloudtpu_train_pokebnn.sh`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/papers/pokebnn/tensorboard.ipynb` & `aqtp-0.7.0/papers/pokebnn/tensorboard.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/pyproject.toml` & `aqtp-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/setup.py` & `aqtp-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.6.2/PKG-INFO` & `aqtp-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtp
-Version: 0.6.2
+Version: 0.7.0
 Summary: Accurate Quantized Training library.
 Author-email: Lukasz Lew <lew@google.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -175,14 +175,77 @@
   scale_stop_grad: bool
   calibration: calibration.Calibration  # calibration algorithm
   po2_scale: bool  # round calibration to power of 2
   use_fake_quant: bool
   use_fwd_quant: Optional[bool]  # use quantized fwd in the bwd pass
 ```
 
+## How to make and use a simple AQT quantizer
+
+This example demonstrates how to make a simple linear AQT quantizer.
+
+```python
+from aqt.jax.v2 import aqt_quantizer
+from aqt.jax.v2 import calibration
+from aqt.jax.v2 import utils as aqt_utils
+from aqt.jax.v2.numerics import int_numerics
+
+q = aqt_quantizer.Quantizer(
+    numerics=int_numerics.IntNumerics(
+        bits=4,
+        preserve_zero=True,
+        preserve_max_val=True,
+        clip=True,
+        clip_gradient=True,
+        round=True,
+        noise_fn=None,
+    ),
+    calib_shared_axes=-1,
+    scale_stop_grad=True,
+    calibration=calibration.AbsMaxCalibration(),
+    po2_scale=False,
+    context=aqt_utils.Context(key=jax.random.PRNGKey(0), train_step=0))
+```
+
+To view the quantized weights created by the quantizer, try quantizing a simple vector like so. Remember that these are the quantized values that are stored in memory for weight quantization.
+
+```python
+x = jnp.linspace(-10, 10, 10)
+x_q, _ = q.quant(x, calibration_axes=-1)
+print(x_q.qvalue)
+```
+
+To view the dequantized values that are used after multiplying the quantized values by the scale, use this code
+
+```python
+print(x_q.dequant())
+```
+
+To view the scales, simply call the scale attribute
+
+```python
+print(x_q.scale)
+```
+
+For a sanity check, we can assert that the scale in this example is simply equal to the dequantized values divided by the quantized values. (Hint: if you get an error check for nan values)
+
+```python
+assert jnp.all(x_q.dequant() / x_q.qvalue == x_q.scale[0])
+```
+
+Finally, we can plot the quantized values like so
+
+```python
+import matplotlib.pyplot as plt
+plt.plot(x, x_q.qvalue)
+```
+
+The specific quantizer parameters here are implemented in this tutorial are just for demonstration purposes and can be easily changed. Try altering the number of bits and see how the number of quantization steps changes accordingly.
+
+
 ## AQT Versions
 
 As of today there are several independent AQT implementations in this package:
 
 - [JAX Legacy AQT](https://github.com/google/aqt/blob/main/aqt/jax_legacy)
   Obsolete version of AQT still used by some customers.
 - [JAX AQTv1](https://github.com/google/aqt/blob/main/aqt/jax)
```

