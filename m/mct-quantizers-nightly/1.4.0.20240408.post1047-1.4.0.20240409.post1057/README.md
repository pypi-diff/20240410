# Comparing `tmp/mct-quantizers-nightly-1.4.0.20240408.post1047.tar.gz` & `tmp/mct-quantizers-nightly-1.4.0.20240409.post1057.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.4.0.20240408.post1047.tar", last modified: Mon Apr  8 00:10:47 2024, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.4.0.20240409.post1057.tar", last modified: Tue Apr  9 00:10:58 2024, max compression
```

## Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047.tar` & `mct-quantizers-nightly-1.4.0.20240409.post1057.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.507244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.507244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.511244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.511244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.511244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.511244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.511244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/onnxruntime_session_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/onnxruntime_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-08 00:10:34.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-08 00:10:47.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-08 00:10:47.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:10:47.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 00:10:47.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 00:10:47.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 00:10:47.515244 mct-quantizers-nightly-1.4.0.20240408.post1047/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-08 00:10:47.000000 mct-quantizers-nightly-1.4.0.20240408.post1047/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.887954 mct-quantizers-nightly-1.4.0.20240409.post1057/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-09 00:10:58.887954 mct-quantizers-nightly-1.4.0.20240409.post1057/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.875954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.879954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.879954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.879954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.879954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.879954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.883954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/onnxruntime_session_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/onnxruntime_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14196 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.883954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.883954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.887954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-09 00:10:35.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:10:58.887954 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-09 00:10:58.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-09 00:10:58.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:10:58.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 00:10:58.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 00:10:58.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 00:10:58.887954 mct-quantizers-nightly-1.4.0.20240409.post1057/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-09 00:10:57.000000 mct-quantizers-nightly-1.4.0.20240409.post1057/setup.py
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/LICENSE.md` & `mct-quantizers-nightly-1.4.0.20240409.post1057/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/PKG-INFO` & `mct-quantizers-nightly-1.4.0.20240409.post1057/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.4.0.20240408.post1047
+Version: 1.4.0.20240409.post1057
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/README.md` & `mct-quantizers-nightly-1.4.0.20240409.post1057/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 ## Constant values
 
 LAYER = "layer"
 STEPS = "optimizer_step"
 TRAINING = "training"
 EPS = 1e-8
 LUT_VALUES_BITWIDTH = 8
-MCTQ_VERSION = "mctq_version"
 
 POSITIONAL_WEIGHT = 'positional_weight'
 QUANTIZED_POSITIONAL_WEIGHT = f'quantized_{POSITIONAL_WEIGHT}'
 
 # ONNX ops domain
 ONNX_CUSTOM_OP_DOMAIN = f"mct_quantizers"
+
+
+## Metadata common fields
+FRAMEWORK_VERSION = 'framework_version'
+PYTHON_VERSION = 'python_version'
+MCTQ_VERSION = "mctq_version"
+ONNX_VERSION = 'onnx_version'
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/load_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from mct_quantizers.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.saved_model.load_options import LoadOptions
     from mct_quantizers.keras.activation_quantization_holder import KerasActivationQuantizationHolder
     from mct_quantizers.keras.quantize_wrapper import KerasQuantizationWrapper
+    from mct_quantizers.keras.metadata import MetadataLayer
     from mct_quantizers.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
     keras = tf.keras
 
     def keras_load_quantized_model(filepath: str, custom_objects: Any = None, compile: bool = True,
                                    options: LoadOptions = None):
         """
         This function wraps the keras load model and MCT quantization custom class to it.
@@ -55,15 +56,26 @@
 
         if custom_objects is not None:
             qi_custom_objects.update(custom_objects)
         # in keras format (v3) passing option is an error
         kwargs = {}
         if options is not None:
             kwargs['options'] = options
-        return tf.keras.models.load_model(filepath, custom_objects=qi_custom_objects, compile=compile, **kwargs)
+
+        # Load model
+        loaded_model = tf.keras.models.load_model(filepath, custom_objects=qi_custom_objects, compile=compile, **kwargs)
+
+        # Extract metadata if exists
+        metadata_layers = [l for l in loaded_model.layers if isinstance(l, MetadataLayer)]
+        if len(metadata_layers) > 0:
+            if len(metadata_layers) > 1:
+                Logger.warning('Found more than 1 MetadataLayer layers in model. Loading the metadata from the first layer only.')
+            loaded_model.metadata_layer = metadata_layers[0]
+            loaded_model.metadata = metadata_layers[0].metadata
+        return loaded_model
 else:
     def keras_load_quantized_model(filepath, custom_objects=None, compile=True, options=None):
         """
         This function wraps the keras load model and MCT quantization custom class to it.
 
         Args:
             filepath: the model file path.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/onnxruntime_session_options.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/onnxruntime_session_options.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/onnxruntime_validations.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/onnxruntime_validations.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================f
+# ==============================================================================
 from typing import List, Union, Any, Dict, Tuple, Callable
 
 import inspect
 
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
 from mct_quantizers.common.constants import FOUND_TORCH, LAYER, TRAINING, POSITIONAL_WEIGHT, \
     QUANTIZED_POSITIONAL_WEIGHT
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.4.0.20240408.post1047
+Version: 1.4.0.20240409.post1057
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.4.0.20240409.post1057/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 mct_quantizers/__init__.py
 mct_quantizers/logger.py
 mct_quantizers/common/__init__.py
 mct_quantizers/common/base_inferable_quantizer.py
 mct_quantizers/common/constants.py
 mct_quantizers/common/get_all_subclasses.py
 mct_quantizers/common/get_quantizers.py
+mct_quantizers/common/metadata.py
 mct_quantizers/common/quant_info.py
 mct_quantizers/common/quant_utils.py
 mct_quantizers/keras/__init__.py
 mct_quantizers/keras/activation_quantization_holder.py
 mct_quantizers/keras/load_model.py
+mct_quantizers/keras/metadata.py
 mct_quantizers/keras/quantize_wrapper.py
 mct_quantizers/keras/quantizer_utils.py
 mct_quantizers/keras/validation_functions.py
 mct_quantizers/keras/quantizers/__init__.py
 mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
 mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
 mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
@@ -29,14 +31,15 @@
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
 mct_quantizers/pytorch/__init__.py
 mct_quantizers/pytorch/activation_quantization_holder.py
 mct_quantizers/pytorch/load_model.py
+mct_quantizers/pytorch/metadata.py
 mct_quantizers/pytorch/onnxruntime_session_options.py
 mct_quantizers/pytorch/onnxruntime_validations.py
 mct_quantizers/pytorch/quantize_wrapper.py
 mct_quantizers/pytorch/quantizer_utils.py
 mct_quantizers/pytorch/quantizers/__init__.py
 mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
 mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
```

### Comparing `mct-quantizers-nightly-1.4.0.20240408.post1047/setup.py` & `mct-quantizers-nightly-1.4.0.20240409.post1057/setup.py`

 * *Files identical despite different names*

