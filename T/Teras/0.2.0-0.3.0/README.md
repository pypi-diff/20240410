# Comparing `tmp/Teras-0.2.0.tar.gz` & `tmp/Teras-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Teras-0.2.0.tar", last modified: Tue Aug  1 18:09:08 2023, max compression
+gzip compressed data, was "Teras-0.3.0.tar", last modified: Wed Apr 10 14:42:57 2024, max compression
```

## Comparing `Teras-0.2.0.tar` & `Teras-0.3.0.tar`

### file list

```diff
@@ -1,229 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.103215 Teras-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-01 18:07:59.000000 Teras-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-08-01 18:09:08.103215 Teras-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-08-01 18:07:59.000000 Teras-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.075214 Teras-0.2.0/Teras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-01 18:07:59.000000 Teras-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:09:08.103215 Teras-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 18:07:59.000000 Teras-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.075214 Teras-0.2.0/teras/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/activations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/config/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/tabtransformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/ensemble/bagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/ensemble/stacking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/generative/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/generative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/impute/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/impute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/layers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/common/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/layers/saint/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_projection_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_reconstruction_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layerflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/dnfnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/ft_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/rtdl_resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/saint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabtransformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layers/activation/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/activation/gumbel_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/activation/gumbel_softmax_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/categorical_feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/categorical_feature_embedding_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/ctgan/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_discriminator_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_discriminator_block_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_generator_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_generator_block_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/dnfnet/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_feature_selection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_localization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnnf.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnnf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/ft_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_cls_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_cls_token_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_numerical_feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_numerical_feature_embedding_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/gain/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_discriminator_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_discriminator_block_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_generator_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_generator_block_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/node/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/node_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/node_feature_selector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/odst.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/odst_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_feature_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_feature_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_features_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_features_extractor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/label_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/label_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/periodic_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/periodic_embedding_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/cutmix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/mixup_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/rtdl_resnet/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/rtdl_resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/rtdl_resnet/rtd_resnet_block_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/rtdl_resnet/rtdl_resnet_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/saint/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/multi_head_inter_sample_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/multi_head_inter_sample_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_numerical_feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_numerical_feature_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_projection_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_projection_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_reconstruction_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_reconstruction_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/tabnet/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_attentive_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_attentive_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer_block_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.095215 Teras-0.2.0/teras/layers/tabtransformer/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabtransformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabtransformer/tabtransformer_column_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabtransformer/tabtransformer_column_embedding_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.095215 Teras-0.2.0/teras/layers/vime/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_feature_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_feature_estimator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_estimator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_generation_and_corruption.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_generation_and_corruption_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_predictor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.095215 Teras-0.2.0/teras/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.099215 Teras-0.2.0/teras/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ctgan_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/dnfnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ft_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/gain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/pcgain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/rtdl_resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/saint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32249 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24544 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabtransformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.099215 Teras-0.2.0/teras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.099215 Teras-0.2.0/teras/preprocessing/base/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/base/base_data_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/oenf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.103215 Teras-0.2.0/teras/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-10 14:42:46.000000 Teras-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-10 14:42:57.921204 Teras-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-10 14:42:46.000000 Teras-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/Teras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 14:42:46.000000 Teras-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-10 14:42:57.921204 Teras-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 14:42:46.000000 Teras-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/pcgain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/gain_fit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/jaxgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/pcgain_fit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/gain_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/pcgain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/data_samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/data_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/pcgain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/activation/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_extraction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token_extraction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/continuous_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/continuous_extraction_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/generator_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/generator_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cutmix_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/ft_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ft_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ft_transformer/feature_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ft_transformer/feature_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/layer_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/mixup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/saint/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/encoder_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/multi_head_inter_sample_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/multi_head_inter_sample_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/projection_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/projection_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/reconstruction_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/reconstruction_head_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tab_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tab_transformer/column_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tab_transformer/column_embedding_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/attentive_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/attentive_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/encoder_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/feedforward_layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/tabnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/tvae_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/ft_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/backbones/saint/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/saint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/saint/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/saint/saint_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/tab_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/backbones/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/backbones/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/transformer/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/transformer/encoder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/ctgan_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/discriminator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/gans/gain/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/discriminator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/gain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/gans/pcgain/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/pcgain_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/pretrainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/saint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tab_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/tabnet_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/ops/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/preprocessing/data_samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_samplers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_samplers/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/preprocessing/data_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/data_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/tasks/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/tasks/imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/testing/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/api_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/version.py
```

### Comparing `Teras-0.2.0/LICENSE` & `Teras-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Teras-0.2.0/PKG-INFO` & `Teras-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1
-Name: Teras
-Version: 0.2.0
-Summary: A Unified Deep Learning Library for Tabular Data
-Author: Khawaja Abaid
-Author-email: Khawaja Abaid <khawaja.abaid@gmail.com>
-Project-URL: Homepage, https://github.com/KhawajaAbaid/teras
-Project-URL: Bug Tracker, https://github.com/KhawajaAbaid/teras/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Teras — A Unified Deep Learning Library for Tabular Data
 
 ![Teras logo banner](./data/imgs/Teras_logo_github_banner.jpg)
 
+## STATUS UPDATE as of January 19, 2024:
+
+The current repository is in a highly unstable state as I'm starting to rewrite this whole library from scratch. All the previous code uptil Teras v0.2.0 has been moved to the new `teras.legacy` module.
+
+
+#### Status update as of January 12, 2024:
+I'm actively working on the Teras v0.3 update but I've discovered some critical flaws in the design as well as code, and many inefficiencies and hacks that shouldn't be part of a good stable project, especially not that offers the state of the art research models. Because I'm a self taught ML and Software Engineer, there's so many things for me to learn and the more I learn the more flaws I keep finding in my code. Also, this library was my first attempt at translating research to usable code, and not just usable code but also one that is modular and intuitive, which is an inspiration from the Keras design. I made lots of mistakes in my first attempt, I redesigned the whole library in Teras v0.2 release and thought that'll now be a solid foundation, and i'd like to think it kind of was, but now with the release of Keras 3, there's lot to change, way more than I anticipated, mainly because of how some of the models require bunch of low level code.
+I'll try my best to release this update within this month!
+Peace!
+
+---
+
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
 It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
 While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
@@ -75,15 +73,15 @@
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
 9. `teras.losses`: It contains custom losses for various architectures.
 
 ## Motivation
 The main purposes of Teras are to:
-1. Provide a uniform interface for all the different proposed architectures.
+1. Provide a uniform interface for all the different proposed architectures to abstract away the complexities to make them accessible to everyone!
 2. Further bridge the gap between research and application.
 3. Be a one-stop for everything concerning deep learning for tabular data.
 4. Accelerate research in tabular domain of deep learning by making it easier for researchers to access, use and experiment with exisiting architectures — saving them lots of valuable time.
 
 
 ## Support
 If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my current laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
```

### Comparing `Teras-0.2.0/pyproject.toml` & `Teras-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
-requires = ["setuptools>=61.0", "tensorflow", "tensorflow-probability",
-            "tensorflow-addons", "pandas", "numpy", "tqdm"]
+requires = ["setuptools>=61.0", "keras>=3.1.1", "pandas", "numpy",
+    "scikit-learn"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Teras"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Khawaja Abaid", email="khawaja.abaid@gmail.com" },
 ]
 description = "A Unified Deep Learning Library for Tabular Data"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/KhawajaAbaid/teras"
-"Bug Tracker" = "https://github.com/KhawajaAbaid/teras/issues"
+"Bug Tracker" = "https://github.com/KhawajaAbaid/teras/issues"
+"Docs" = "https://teras.readthedocs.io/"
```

### Comparing `Teras-0.2.0/teras/__init__.py` & `Teras-0.3.0/teras/_src/layers/ctgan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.5
+# limitations under the License.
```

### Comparing `Teras-0.2.0/teras/activations_test.py` & `Teras-0.3.0/teras/_src/activations_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from teras.activations import (glu,
+from keras import ops
+from teras._src.activations import (glu,
                                geglu,
                                gumbel_softmax,
                                sparsemax)
-import tensorflow as tf
 
 
 # ================== glu tests ====================
 def test_glu_valid_call():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = glu(inputs)
 
 
 def test_glu_output_shape():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = glu(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 8
-    assert tf.shape(outputs)[1] == 2    # glu halves the dimensions
+    assert len(ops.shape(outputs)) == 2
+    assert ops.shape(outputs)[0] == 8
+    assert ops.shape(outputs)[1] == 2    # glu halves the dimensions
 
 
 # ================== geglu tests ====================
 def test_geglu_valid_call():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = geglu(inputs)
 
 
 def test_geglu_output_shape():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = geglu(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 8
-    assert tf.shape(outputs)[1] == 2    # geglu halves the dimensions
+    assert len(ops.shape(outputs)) == 2
+    assert ops.shape(outputs)[0] == 8
+    assert ops.shape(outputs)[1] == 2    # geglu halves the dimensions
 
 
 # ================== gumbel_softmax tests ====================
 def test_gumbel_softmax_valid_call():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = gumbel_softmax(inputs)
 
 
 def test_gumbel_softmax_output_shape():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = gumbel_softmax(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 8
-    assert tf.shape(outputs)[1] == 4
+    assert len(ops.shape(outputs)) == 2
+    assert ops.shape(outputs)[0] == 8
+    assert ops.shape(outputs)[1] == 4
 
 
 # ================== sparsemax tests ====================
 def test_sparsemax_valid_call():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = gumbel_softmax(inputs)
 
 
 def test_sparsemax_output_shape():
-    inputs = tf.ones((8, 4), dtype=tf.float32)
+    inputs = ops.ones((8, 4), dtype="float32")
     outputs = gumbel_softmax(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 8
-    assert tf.shape(outputs)[1] == 4
+    assert len(ops.shape(outputs)) == 2
+    assert ops.shape(outputs)[0] == 8
+    assert ops.shape(outputs)[1] == 4
```

### Comparing `Teras-0.2.0/teras/config/__init__.py` & `Teras-0.3.0/teras/api_export.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-
-# This module contains default parameter values config classes for all Model and Layer classes.
+from teras._src.api_export import teras_export
```

### Comparing `Teras-0.2.0/teras/ensemble/__init__.py` & `Teras-0.3.0/teras/data_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.5
+# limitations under the License.
 
 
-from teras.ensemble.bagging import Bagging
-from teras.ensemble.stacking import Stacking
+from teras._src.data_utils import (
+    create_gain_dataset as create_gain_dataset
+)
```

### Comparing `Teras-0.2.0/teras/generative/__init__.py` & `Teras-0.3.0/teras/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 The KerasCV Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.5
+# limitations under the License.
 
 
-# CTGAN models
-from teras.models.ctgan import CTGAN
+# Unique source of truth for the version number.
+__version__ = "0.3.0"
 
 
-# TVAE models
-from teras.models.tvae import TVAE
-
+def version():
+    return __version__
```

### Comparing `Teras-0.2.0/teras/impute/__init__.py` & `Teras-0.3.0/teras/_src/ops/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.5
+# limitations under the License.
 
 
-# GAIN
-from teras.models.gain import GAIN
```

### Comparing `Teras-0.2.0/teras/layerflow/__init__.py` & `Teras-0.3.0/teras/_src/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-from teras.layerflow import layers
-from teras.layerflow import models
+# Jaxifying!
```

### Comparing `Teras-0.2.0/teras/layerflow/layers/common/__init__.py` & `Teras-0.3.0/teras/_src/models/tasks/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-# General purpose common layers
-from teras.layerflow.layers.common.common import HiLOL
-
-
-# Transformer layers
-from teras.layerflow.layers.common.transformer import (FeedForward,
-                                                       Transformer,
-                                                       Encoder)
-
+from teras._src.models.tasks.classification import Classifier
+from teras._src.models.tasks.regression import Regressor
```

### Comparing `Teras-0.2.0/teras/layerflow/layers/saint/saint_transformer.py` & `Teras-0.3.0/teras/_src/layers/transformer/encoder_layer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,129 @@
-from tensorflow import keras
+import keras
+from teras._src.layers.transformer.feedforward import TransformerFeedForward
+from teras._src.api_export import teras_export
 
 
-@keras.saving.register_keras_serializable(package="teras.layerflow.layers.saint")
-class SAINTTransformer(keras.layers.Layer):
+@teras_export("teras.layers.TransformerEncoderLayer")
+class TransformerEncoderLayer(keras.layers.Layer):
     """
-    SAINT Transformer layer with LayerFlow design.
-    It is part of the SAINT architecture,
-    which is proposed by Gowthami Somepalli et al.
-    in the paper SAINT: Improved Neural Networks for Tabular Data
-    via Row Attention and Contrastive Pre-Training.
-    It differs from the usual Transformer (L) block in that it contains additional
-    ``MultiHeadInterSampleAttention`` layer in addition to the usual
-    ``MultiHeadAttention`` layer.
+    Transformer Encoder Layer as proposed in the original Transformer
+    architecture in the "Attention is all you need" paper.
+
+    This is the layer that makes up the encoder in the architecture.
+    This is made up of `MultiHeadAttention` and `TransformerFeedForward`
+    layers.
 
     Reference(s):
-        https://arxiv.org/abs/2106.01342
+        https://arxiv.org/abs/1706.03762
 
     Args:
-        multi_head_inter_sample_attention: ``keras.layers.Layer``,
-            An instance of ``MultiHeadInterSampleAttention`` layer or any other custom
-            layer that can work in its place.
-            You can import this layer as follows,
-                >>> from teras.layers import MultiHeadInterSampleAttention
-
-        feed_forward: ``keras.layers.Layer``,
-            An instance of ``FeedForward`` layer or any custom layer that can work
-            in its place.
-            You can import this layer as follows,
-                >>> from teras.layerflow.layers import FeedForward
-
-        transformer: ``keras.layers.Layer``,
-            An instance of the regular ``Transformer`` layer, or any custom layer
-            that can work in its place.
-            You can import this layer as follows,
-                >>> from teras.layerflow.layers import Transformer
+        embedding_dim: int, dimensionality of the embeddings used
+            by the model. It is also referred to as the `d_model` or
+            model dimensionality.
+        num_heads: int, number of attention heads to use in the
+            `MultiHeadAttention` layer.
+        feedforward_dim: int, hidden dimensionality to use in the
+            `TransformerFeedForward` layer.
+        attention_dropout: float, dropout value to use in the
+        `MultiHeadAttention` layer. Defaults to 0.
+        feedforward_dropout: float, dropout value to use in the
+            `TransformerFeedForward` layer. Defaults to 0.
+        layer_norm_epsilon: float, epsilon value to use in the
+            `LayerNormalization` layer. Defaults to 1e-5.
+        use_normalization: bool, whether to use `LayerNormalization`.
+            In some architecture, normalization isn't applied to the
+            very first layer, so to accomodate such architectures,
+            we introduced this parameter.
+            Defaults to `True`.
+        pre_normalization: bool, whether to use Pre-Normalization technique
+            whereby `LayerNormalization` is applied to inputs of the
+            `MultiHeadAttention` or `FeedForward` and then outputs of
+            those layers are elementwise added to the original inputs.
+            Defaults to `False`, as the original Transformers architecture
+            doesn't use pre-normalization.
+
+    Shapes:
+        Input Shape: `(batch_size, num_features, embedding_dim)`
+        Output Shape: `(batch_size, num_features, embedding_dim)`
     """
     def __init__(self,
-                 multi_head_inter_sample_attention: keras.layers.Layer,
-                 feed_forward: keras.layers.Layer,
-                 transformer: keras.layers.Layer,
+                 embedding_dim: int,
+                 num_heads: int = 8,
+                 feedforward_dim: int = None,
+                 attention_dropout: float = 0.,
+                 feedforward_dropout: float = 0.,
+                 layer_norm_epsilon: float = 1e-5,
+                 use_normalization: bool = True,
+                 pre_normalization: bool = False,
                  **kwargs):
         super().__init__(**kwargs)
-        self.multi_head_inter_sample_attention = multi_head_inter_sample_attention
-        self.feed_forward = feed_forward
-        self.transformer = transformer
+        self.embedding_dim = embedding_dim
+        self.num_heads = num_heads
+        self.feedforward_dim = feedforward_dim
+        self.attention_dropout = attention_dropout
+        self.feedforward_dropout = feedforward_dropout
+        self.layer_norm_epsilon = layer_norm_epsilon
+        self.use_normalization = use_normalization
+        self.pre_normalization = pre_normalization
+
+        self.attention = keras.layers.MultiHeadAttention(
+            num_heads=self.num_heads,
+            key_dim=self.embedding_dim,
+            dropout=attention_dropout
+        )
+        self.feedforward = TransformerFeedForward(
+            embedding_dim=self.embedding_dim,
+            hidden_dim=self.feedforward_dim,
+            dropout=self.feedforward_dropout
+        )
+        self.add_1 = keras.layers.Add()
+        self.add_2 = keras.layers.Add()
+        if self.use_normalization:
+            self.layer_norm_1 = keras.layers.LayerNormalization(
+                epsilon=self.layer_norm_epsilon
+            )
+            self.layer_norm_2 = keras.layers.LayerNormalization(
+                epsilon=self.layer_norm_epsilon
+            )
 
     def build(self, input_shape):
-        # We build the inner SAINT Transformer block using keras Functional API
-        # and since we need the input dimensions that's why we're building it in the build method.
-
-        # Inter Sample Attention Block: this attention is applied to rows.
-        inputs = keras.layers.Input(shape=tuple(input_shape[1:]))
-        intermediate_outputs = inputs
-        if self.apply_attention_to_rows:
-            residual = inputs
-            x = self.multi_head_inter_sample_attention(inputs)
-            x = keras.layers.Add()([x, residual])
-            x = keras.layers.LayerNormalization()(x)
-            residual = x
-            x = self.feed_forward(x)
-            x = keras.layers.Add()([x, residual])
-            intermediate_outputs = keras.layers.LayerNormalization()(x)
-            final_outputs = intermediate_outputs
-
-        # MultiHeadAttention block: this attention is applied to columns
-        if self.apply_attention_to_features:
-            # If `apply_attention_to_features` is set to True,
-            # then attention will be applied to columns/features
-            # The MultiHeadInterSampleAttention appollection)lies attention over rows,
-            # but the regular MultiHeadAttention layer is used to apply attention over features.
-            # Since the common Transformer layer applies MutliHeadAttention over features
-            # as well as takes care of applying all the preceding and following layers,
-            # so we'll just use that here.
-            final_outputs = self.transformer(intermediate_outputs)
-
-        self.transformer_block = keras.Model(inputs=inputs,
-                                             outputs=final_outputs,
-                                             name="saint_inner_transformer_block")
+        self.feedforward.build(input_shape)
+        if self.use_normalization:
+            self.layer_norm_1.build(input_shape)
+            self.layer_norm_2.build(input_shape)
 
     def call(self, inputs):
-        outputs = self.transformer_block(inputs)
-        return outputs
+        residue = inputs
+        if self.use_normalization and self.pre_normalization:
+            x = self.layer_norm_1(inputs)
+            x = self.attention(x, x)
+            x = self.add_1([x, residue])
+            residue = x
+            x = self.layer_norm_2(x)
+            x = self.feedforward(x)
+            x = self.add_2([x, residue])
+        else:
+            x = self.attention(inputs, inputs)
+            x = self.add_1([x, residue])
+            if self.use_normalization:
+                x = self.layer_norm_1(x)
+            residue = x
+            x = self.feedforward(x)
+            x = self.add_2([x, residue])
+            if self.use_normalization:
+                x = self.layer_norm_2(x)
+        return x
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'multi_head_inter_sample_attention': keras.layers.serialize(self.multi_head_inter_sample_attention),
-                      'feed_forward': keras.layers.serialize(self.feed_forward),
-                      'transformer': keras.layers.serialize(self.transformer),
-                      }
-        config.update(new_config)
+        config.update({
+            "embedding_dim": self.embedding_dim,
+            "num_heads": self.num_heads,
+            "feedforward_dim": self.feedforward_dim,
+            "attention_dropout": self.attention_dropout,
+            "feedforward_dropout": self.feedforward_dropout,
+            "layer_norm_epsilon": self.layer_norm_epsilon,
+            "use_normalization": self.use_normalization,
+            "pre_normalization": self.pre_normalization
+        })
         return config
-
-    @classmethod
-    def from_config(cls, config):
-        multi_head_inter_sample_attention = keras.layers.deserialize(config.pop("multi_head_inter_sample_attention"))
-        feed_forward = keras.layers.deserialize(config.pop("feed_forward"))
-        transformer = keras.layers.deserialize(config.pop("transformer"))
-        return cls(multi_head_inter_sample_attention=multi_head_inter_sample_attention,
-                   feed_forward=feed_forward,
-                   transformer=transformer,
-                   **config)
```

### Comparing `Teras-0.2.0/teras/layers/activation/__init__.py` & `Teras-0.3.0/teras/activations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from teras.layers.activation.gumbel_softmax import GumbelSoftmax
+from teras._src.activations import (
+    glu as glu,
+    geglu as geglu,
+    sparsemax as sparsemax,
+    gumbel_softmax as gumbel_softmax
+)
```

### Comparing `Teras-0.2.0/teras/layers/activation/gumbel_softmax.py` & `Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-import tensorflow as tf
-from tensorflow import keras
-from teras.activations import gumbel_softmax
+import keras
+from teras._src.activations import gumbel_softmax
+from teras._src.api_export import teras_export
 
 
-@keras.saving.register_keras_serializable(package="teras.layers.activation")
+@teras_export("teras.layers.GumbelSoftmax")
 class GumbelSoftmax(keras.layers.Layer):
     """
     Implementation of the Gumbel Softmax activation
-    proposed by Eric Jang et al. in the paper
-    Categorical Reparameterization with Gumbel-Softmax
+    proposed by Eric Jang et al. in the paper,
+    "Categorical Reparameterization with Gumbel-Softmax"
 
     Reference(s):
         https://arxiv.org/abs/1611.01144
 
     Args:
-        temperature: ``float``, default 0.2,
-            Controls the sharpness or smoothness of the resulting probability distribution.
-            A higher temperature value leads to a smoother and more uniform probability distribution.
-            Conversely, a lower temperature value makes the distribution concentrated around
-            the category with the highest probability.
-
-        hard: ``bool``, default False,
-            Whether to return soft probabilities or hard one hot vectors.
+        temperature: float, Controls the sharpness or smoothness of the
+            resulting probability distribution. A higher temperature value
+            leads to a smoother and more uniform probability distribution.
+            Conversely, a lower temperature value makes the distribution
+            concentrated around the category with the highest probability.
+        hard: bool, Whether to return soft probabilities or hard one hot
+        vectors. Defaults to False.
+        seed: int, Seed for random sampling.
     """
     def __init__(self,
                  temperature: float = 0.2,
                  hard: bool = False,
+                 seed: int = 1337,
                  **kwargs):
         super().__init__(**kwargs)
         self.temperature = temperature
         self.hard = hard
+        self.seed = seed
+
+    def build(self, input_shape):
+        # nothing to build
+        self.built = True
 
-    def call(self, logits: tf.Tensor):
+    def call(self, logits):
         return gumbel_softmax(logits,
                               temperature=self.temperature,
-                              hard=self.hard)
+                              hard=self.hard,
+                              seed=self.seed)
 
     def get_config(self):
         config = super().get_config()
         new_config = {'temperature': self.temperature,
                       'hard': self.hard}
         config.update(new_config)
         return config
```

### Comparing `Teras-0.2.0/teras/layers/activation/gumbel_softmax_test.py` & `Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from teras.layers.activation import GumbelSoftmax
+from teras._src.layers.activation import GumbelSoftmax
 import tensorflow as tf
 
 
 def test_gumble_softmax_valid_call():
     gumble_softmax = GumbelSoftmax()
     inputs = tf.ones((8, 4), dtype=tf.float32)
     outputs = gumble_softmax(inputs)
```

### Comparing `Teras-0.2.0/teras/layers/common/__init__.py` & `Teras-0.3.0/teras/_src/trainers/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitatiFions under the License.
 
+from keras.backend import backend
 
-# Head layers
-from teras.layers.common.head import (ClassificationHead,
-                                      RegressionHead)
-
-
-# Transformer layers
-from teras.layers.common.transformer import (FeedForward,
-                                             Transformer,
-                                             Encoder)
+if backend() == "jax":
+    from teras._src.backend.jax.trainers import *
+else:
+    # raise ImportError(
+    #     "`teras.trainers` module is only available for `jax` backend. "
+    #     "Please set your `KERAS_BACKEND` environment variable to `jax` before "
+    #     "importing `teras.trainers`.")
+    pass
```

### Comparing `Teras-0.2.0/teras/layers/ctgan/__init__.py` & `Teras-0.3.0/teras/_src/backend/jax/trainers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-from teras.layers.ctgan.ctgan_generator_block import CTGANGeneratorBlock
-from teras.layers.ctgan.ctgan_discriminator_block import CTGANDiscriminatorBlock
+# Good code? Bad code?
+from teras._src.backend.jax.trainers import gain as GAINTrainer
+from teras._src.backend.jax.trainers import ctgan as CTGANTrainer
```

### Comparing `Teras-0.2.0/teras/layers/ctgan/ctgan_discriminator_block.py` & `Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,62 @@
-from tensorflow import keras
+import keras
+from teras._src.api_export import teras_export
 
 
-@keras.saving.register_keras_serializable(package="teras.layers.ctgan")
-class CTGANDiscriminatorBlock(keras.layers.Layer):
+@teras_export("teras.layers.CTGANDiscriminatorLayer")
+class CTGANDiscriminatorLayer(keras.layers.Layer):
     """
-    Discriminator Block based on the architecture proposed by
+    Discriminator Layer based on the architecture proposed by
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     outputs = Dropout(LeakyReLU(Dense(inputs)))
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        units: ``int``, default 256,
-            Dimensionality of the hidden layer
-
-        leaky_relu_alpha: ``float``, default 0.2,
-            Alpha value to use for leaky relu activation
-
-        dropout_rate: ``float``, default 0.,
-            Dropout rate to use in the ``Dropout`` layer,
-            which is applied after hidden layer.
+        dim: int, Dimensionality of the hidden layer. Default to 256.
+        leaky_relu_alpha: float, Alpha value to use for leaky relu activation.
+            Defaults to 0.2
+        dropout_rate: float, Dropout rate to use in the `Dropout` layer,
+            which is applied after hidden layer. Defaults to 0.
     """
     def __init__(self,
-                 units: int = 256,
+                 dim: int = 256,
                  leaky_relu_alpha: float = 0.2,
                  dropout_rate: float = 0.,
                  **kwargs):
         super().__init__(**kwargs)
-        self.units = units
+        self.dim = dim
         self.leaky_relu_alpha = leaky_relu_alpha
         self.dropout_rate = dropout_rate
 
-        self.dense = keras.layers.Dense(units)
-        self.leaky_relu = keras.layers.LeakyReLU(alpha=self.leaky_relu_alpha)
+        self.dense = keras.layers.Dense(dim)
+        self.leaky_relu = keras.layers.LeakyReLU(
+            negative_slope=self.leaky_relu_alpha)
         self.dropout = keras.layers.Dropout(rate=self.dropout_rate)
 
+    def build(self, input_shape):
+        self.dense.build(input_shape)
+        input_shape = self.dense.compute_output_shape(input_shape)
+        self.leaky_relu.build(input_shape)
+        self.dropout.build(input_shape)
+
     def call(self, inputs):
         out = self.dense(inputs)
         out = self.leaky_relu(out)
         out = self.dropout(out)
         return out
 
+    def compute_output_shape(self, input_shape):
+        return input_shape[:-1] + (self.dim,)
+
     def get_config(self):
         config = super().get_config()
-        config.update({'units': self.units,
-                       'leaky_relu_alpha': self.leaky_relu_alpha,
-                       'dropout_rate': self.dropout_rate}
-                      )
+        config.update({
+            'dim': self.dim,
+            'leaky_relu_alpha': self.leaky_relu_alpha,
+            'dropout_rate': self.dropout_rate}
+        )
         return config
```

### Comparing `Teras-0.2.0/teras/layers/ctgan/ctgan_generator_block.py` & `Teras-0.3.0/teras/_src/layers/ctgan/generator_layer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-from tensorflow import keras
+import keras
+from keras import ops
+from teras._src.api_export import teras_export
 
 
-@keras.saving.register_keras_serializable(package="teras.layers.ctgan")
-class CTGANGeneratorBlock(keras.layers.Layer):
+@teras_export("teras.layers.CTGANGeneratorLayer")
+class CTGANGeneratorLayer(keras.layers.Layer):
     """
     Residual Block for Generator as used by the authors of CTGAN
     proposed in the paper Modeling Tabular data using Conditional GAN.
 
-    ``outputs = Concat([ReLU(BatchNorm(Dense(inputs))), inputs])``
+    `outputs = Concat([ReLU(BatchNorm(Dense(inputs))), inputs])`
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        units: ``int``, default 256,
-            Dimensionality of the hidden layer
+        dim: int, Dimensionality of the hidden layer.
+            Defaults to 256.
     """
     def __init__(self,
-                 units: int = 256,
+                 dim: int = 256,
                  **kwargs):
         super().__init__(**kwargs)
-        self.units = units
-        self.dense = keras.layers.Dense(self.units)
+        self.dim = dim
+        self.dense = keras.layers.Dense(self.dim)
         self.batch_norm = keras.layers.BatchNormalization()
         self.relu = keras.layers.ReLU()
-        self.concat = keras.layers.Concatenate(axis=1)
+
+    def build(self, input_shape):
+        self.dense.build(input_shape)
+        input_shape = self.dense.compute_output_shape(input_shape)
+        self.batch_norm.build(input_shape)
+        self.relu.build(input_shape)
 
     def call(self, inputs):
         x = self.dense(inputs)
         x = self.batch_norm(x)
         x = self.relu(x)
-        out = self.concat([x, inputs])
+        out = ops.concatenate([x, inputs], axis=1)
         return out
 
+    def compute_output_shape(self, input_shape):
+        return input_shape[:-1] + (input_shape[-1] + self.dim,)
+
     def get_config(self):
         config = super().get_config()
-        config.update({"units": self.units})
+        config.update({"dim": self.dim})
         return config
```

### Comparing `Teras-0.2.0/teras/layers/dnfnet/__init__.py` & `Teras-0.3.0/teras/_src/layers/ft_transformer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,12 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
-from teras.layers.dnfnet.dnfnet_feature_selection import DNFNetFeatureSelection
-from teras.layers.dnfnet.dnfnet_localization import DNFNetLocalization
-from teras.layers.dnfnet.dnnf import DNNF
```

### Comparing `Teras-0.2.0/teras/layers/gain/__init__.py` & `Teras-0.3.0/teras/_src/layers/activation/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from teras.layers.gain.gain_generator_block import GAINGeneratorBlock
-from teras.layers.gain.gain_discriminator_block import GAINDiscriminatorBlock
+from teras._src.layers.activation.gumbel_softmax import GumbelSoftmax
```

### Comparing `Teras-0.2.0/teras/layers/node/__init__.py` & `Teras-0.3.0/teras/ops/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from teras.layers.node.odst import ObliviousDecisionTree
-from teras.layers.node.node_feature_selector import NodeFeatureSelector
+from teras._src.ops.ops import norm
```

### Comparing `Teras-0.2.0/teras/layers/numerical_features_extractor.py` & `Teras-0.3.0/teras/_src/layers/categorical_embedding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,61 @@
-import tensorflow as tf
-from tensorflow import keras
+import keras
+from keras import ops
+from teras._src.api_export import teras_export
 
 
-@keras.saving.register_keras_serializable(package="teras.layers")
-class NumericalFeaturesExtractor(keras.layers.Layer):
+@teras_export("teras.layers.CategoricalEmbedding")
+class CategoricalEmbedding(keras.layers.Layer):
     """
-    NumericalFeaturesExtractor layer extracts numerical features as is.
-    It helps us build functional model, in case we don't want to apply
-    any special layer to numerical features but still want to extract
-    numerical features to concatenate them with the categorical features.
+    Categorical Embedding layer that create trainable embeddings for
+    categorical features values.
 
     Args:
-        features_metadata: ``dict``,
-            A nested dictionary of metadata for features where
-            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
-            feature indices and the lists of unique values (vocabulary) in them,
-            while numerical dictionary is a mapping of numerical feature names to their indices.
-            ``{feature_name: (feature_idx, vocabulary)}`` for feature in categorical features.
-            ``{feature_name: feature_idx}`` for feature in numerical features.
-            You can get this dictionary from
-                >>> from teras.utils import get_features_metadata_for_embedding
-                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                ..                                                      categorical_features,
-                ..                                                      numerical_features)
-
-    Raises:
-        If no numerical features exist, this layer raises a ``ValueError``.
+        embedding_dim: int, dimensionality of the embeddings
+        cardinalities: list or ndarray, a list or 1d-array of
+            cardinalities of all the features in the dataset in the
+            same order as the features' occurrence.
+            For numerical features, use 0 as indicator at
+            the corresponding index of the array.
+            You can use the `compute_cardinalities` function from
+            `teras.utils` package for this purpose.
     """
     def __init__(self,
-                 features_metadata: dict,
+                 embedding_dim: int,
+                 cardinalities: list,
                  **kwargs):
         super().__init__(**kwargs)
-        self.features_metadata = features_metadata
-        if not len(self.features_metadata["numerical"]) > 0:
-            raise ValueError("`features_metadata` contains no numerical features. "
-                             "Either you forgot to pass numerical features names list to the "
-                             "`get_features_metadata_for_embedding` or the dataset does not contain "
-                             "any numerical features to begin with. \n"
-                             "In either case, "
-                             "`NumericalFeaturesExtractor` cannot be called on inputs with no numerical features. ")
-        self._numerical_features_idx = list(self.features_metadata["numerical"].values())
+        self.embedding_dim = embedding_dim
+        self.cardinalities = cardinalities
+        self.embedding_layers = []
+        self._categorical_idx = []
+        for idx, card in enumerate(self.cardinalities):
+            if card > 0:
+                embedding = keras.layers.Embedding(
+                    input_dim=card + 1,
+                    output_dim=self.embedding_dim)
+                self.embedding_layers.append(embedding)
+                self._categorical_idx.append(idx)
 
     def call(self, inputs):
-        numerical_features = tf.gather(inputs,
-                                       indices=self._numerical_features_idx,
-                                       axis=1)
-        return numerical_features
+        idx = self._categorical_idx[0]
+        feature = ops.expand_dims(inputs[:, idx], axis=1)
+        categorical_embeddings = self.embedding_layers[0](feature)
+        for feature_idx, embedding_layer in zip(self._categorical_idx[1:],
+                                                self.embedding_layers[1:]):
+            feature = ops.expand_dims(inputs[:, feature_idx], axis=1)
+            f_e = embedding_layer(feature)
+            # Concatenate feature embeddings along the feature axis
+            categorical_embeddings = ops.concatenate(
+                xs=[categorical_embeddings, f_e], axis=1)
+        return categorical_embeddings
+
+    def compute_output_shape(self, input_shape):
+        return input_shape[:-1] + (len(self._categorical_idx),
+                                   self.embedding_dim,)
+
+    def get_config(self):
+        config = super().get_config()
+        config.update({
+            "embedding_dim": self.embedding_dim,
+            "cardinalities": self.cardinalities
+        })
```

### Comparing `Teras-0.2.0/teras/layers/preprocessing/__init__.py` & `Teras-0.3.0/teras/tasks/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from teras.layers.preprocessing.periodic_embedding import PeriodicEmbedding
+from teras._src.tasks.imputation import Imputer
+from teras._src.tasks.generation import Generator
```

### Comparing `Teras-0.2.0/teras/layers/regularization/__init__.py` & `Teras-0.3.0/teras/_src/models/backbones/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-from teras.layers.regularization.mixup import MixUp
-from teras.layers.regularization.cutmix import CutMix
+# The concept of this module is copied from Keras-CV - some things may vary.
```

### Comparing `Teras-0.2.0/teras/layers/rtdl_resnet/__init__.py` & `Teras-0.3.0/teras/_src/layers/tab_transformer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,10 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
-from teras.layers.rtdl_resnet.rtdl_resnet_block import RTDLResNetBlock
```

### Comparing `Teras-0.2.0/teras/layers/saint/__init__.py` & `Teras-0.3.0/teras/_src/backend/tensorflow/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,31 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from teras.layers.saint.multi_head_inter_sample_attention import MultiHeadInterSampleAttention
-from teras.layers.saint.saint_numerical_feature_embedding import SAINTNumericalFeatureEmbedding
-from teras.layers.saint.saint_transformer import SAINTTransformer
-from teras.layers.saint.saint_encoder import SAINTEncoder
-from teras.layers.saint.saint_reconstruction_head import (SAINTReconstructionHeadBlock,
-                                                          SAINTReconstructionHead)
-from teras.layers.saint.saint_projection_head import SAINTProjectionHead
+
+from teras._src.backend.tensorflow.models.pretrainers.tabnet import TabNetPretrainer
+from teras._src.backend.tensorflow.models.pretrainers.tab_transformer import (
+    TabTransformerMLMPretrainer,
+    TabTransformerRTDPretrainer
+)
+from teras._src.backend.tensorflow.models.pretrainers.saint import SAINTPretrainer
+
+# GANs
+from teras._src.backend.tensorflow.models.gans.gain import GAIN
+from teras._src.backend.tensorflow.models.gans.pcgain import PCGAIN
+from teras._src.backend.tensorflow.models.gans.ctgan.discriminator import CTGANDiscriminator
+from teras._src.backend.tensorflow.models.gans.ctgan.generator import CTGANGenerator
+from teras._src.backend.tensorflow.models.gans.ctgan.ctgan import CTGAN
+
+# Autoencoders
+from teras._src.backend.tensorflow.models.autoencoders.tvae.tvae import TVAE
```

### Comparing `Teras-0.2.0/teras/layers/saint/saint_transformer.py` & `Teras-0.3.0/teras/_src/models/backbones/saint/saint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,127 @@
-from tensorflow import keras
-from teras.layerflow.layers.saint.saint_transformer import SAINTTransformer as _SAINTTransformerLF
-from teras.layers.saint.multi_head_inter_sample_attention import MultiHeadInterSampleAttention
-from teras.layers.common.transformer import Transformer, FeedForward
+import keras
 
+from teras._src.layers.cls_token import CLSToken
+from teras._src.layers.cls_token_extraction import CLSTokenExtraction
+from teras._src.layers.saint.embedding import SAINTEmbedding
+from teras._src.layers.saint.encoder_layer import SAINTEncoderLayer
+from teras._src.models.backbones.backbone import Backbone
+from teras._src.api_export import teras_export
 
-@keras.saving.register_keras_serializable(package="teras.layers.saint")
-class SAINTTransformer(_SAINTTransformerLF):
+
+@teras_export("teras.model.SAINTBackbone")
+class SAINTBackbone(Backbone):
     """
-    SAINT Transformer layer as proposed by Gowthami Somepalli et al.
-    in the paper SAINT: Improved Neural Networks for Tabular Data
-    via Row Attention and Contrastive Pre-Training.
-    It differs from the usual Transformer (L) block in that it contains additional
-    multihead intersample attention layer in addition to the usual multihead attention layer
+    SAINT Backbone based on the SAINT architecture proposed in the paper,
+    "SAINT: Improved Neural Networks for Tabular Data".
 
     Reference(s):
         https://arxiv.org/abs/2106.01342
 
     Args:
-        data_dim: ``int``,
-            Dimensionality of the input dataset,
-            or the total number of features in the dataset.
-
-        embedding_dim: ``int``, default 32,
-            Embedding dimensions used to embedd numerical and
-            categorical features. These server as the key dimensions
-            in the MultiHeadAttention layer.
-
-        num_attention_heads: ``int``, default 8,
-            Number of heads to use in the typical ``MultiHeadAttention``
-            layer that will be applied over features.
-
-        num_inter_sample_attention_heads: ``int``, default 8,
-            Number of heads to use in the ``MultiHeadInterSampleAttention``
-            that will be applied over rows
-
-        embedding_dim: ``int``, default 32,
-            Embedding dimensions. These will also serve as key dimensions
-             for the attention layers
-
-        attention_dropout: ``float``, default 0.1,
-            Dropout rate for ``MultiHeadAttention`` which is applied over
-             features.
-
-        inter_sample_attention_dropout: ``float``, default 0.1,
-            Dropout rate for ``MultiHeadInterSampleAttention`` which is
-            applied over rows.
-
-        feedforward_dropout: ``float``, default 0.1,
-            Dropout rate for the ``Dropout`` layer that is part of the
-            ``FeedForward`` layer.
-
-        feedforward_multiplier: ``int``, default 4.
-            Multiplier that is multiplied with the ``embedding_dim``
-            and the resultant value is used as hidden dimensions value for the
-            hidden layer in the ``FeedForward`` layer.
-
-        apply_attention_to_features: ``bool``, default True,
-            Whether to apply attention over features.
-            If True, the regular ``MultiHeadAttention`` layer will be applied
-            over features.
-
-        apply_attention_to_rows: ``bool``, default True,
-            Whether to apply attention over rows.
-            If True, the ``MultiHeadInterSampleAttention`` will apply attention
-            over rows.
-            NOTE: It is strongly recommended to keep both as True, but you
-            can turn one off for experiment's sake.
-            Also, note that, both CANNOT be False at the same time!
+        input_dim: int, dimensionality of the input dataset. i.e. the
+            number of features in the dataset.
+        cardinalities: list, a list cardinalities of all the features
+            in the dataset in the same order as the features' occurrence.
+            For numerical features, use any value <=0 as indicator at
+            the corresponding index.
+            You can use the `compute_cardinalities` function from
+            `teras.utils` package for this purpose.
+        embedding_dim: int, dimensionality of the embeddings used
+            by the model. It is also referred to as the `d_model` or
+            model dimensionality.
+        num_layers: int, number of `TransformerEncoderLayer`s to use in
+            the encoder.
+        num_heads: int, number of attention heads to use in the
+            `MultiHeadAttention` layer.
+        feedforward_dim: int, hidden dimensionality to use in the
+            `TransformerFeedForward` layer.
+        attention_dropout: float, dropout value to use in the
+            `MultiHeadAttention` layer. Defaults to 0.
+        feedforward_dropout: float, dropout value to use in the
+            `TransformerFeedForward` layer. Defaults to 0.
+        layer_norm_epsilon: float, epsilon value to use in the
+            `LayerNormalization` layer. Defaults to 1e-5.
+        embedd_inputs: bool, whether to use `SAINTEmbedding` layer to
+            create emebddings of inputs. Defaults to `True` as this is
+            what we want. but when pretraining we want to use the
+            `SAINTBackbone` as encoder only which expects embeddings as
+            inputs, so that's when we set this parameter to `False`.
+        return_cls_token_only: bool, whether to return only embeddings
+            for the `CLS` token. Defaults to `True`.
     """
     def __init__(self,
-                 data_dim: int,
-                 embedding_dim: int = 32,
-                 num_attention_heads: int = 8,
-                 num_inter_sample_attention_heads: int = 8,
-                 attention_dropout: float = 0.1,
-                 inter_sample_attention_dropout: float = 0.1,
-                 feedforward_dropout: float = 0.1,
-                 feedforward_multiplier: int = 4,
-                 norm_epsilon: float = 1e-6,
-                 apply_attention_to_features: bool = True,
-                 apply_attention_to_rows: bool = True,
+                 input_dim: int,
+                 cardinalities: list,
+                 embedding_dim: int,
+                 num_layers: int = 6,
+                 num_heads: int = 8,
+                 feedforward_dim: int = None,
+                 attention_dropout: float = 0.,
+                 feedforward_dropout: float = 0.,
+                 layer_norm_epsilon: float = 1e-5,
+                 embedd_inputs: bool = True,
+                 return_cls_token_only: bool = True,
                  **kwargs):
-        multihead_inter_sample_attention = MultiHeadInterSampleAttention(
-            num_heads=num_inter_sample_attention_heads,
-            key_dim=embedding_dim * data_dim,
-            dropout=inter_sample_attention_dropout,
-            name="inter_sample_multihead_attention"
-        )
-        feed_forward = FeedForward(embedding_dim=embedding_dim,
-                                   multiplier=feedforward_multiplier,
-                                   dropout=feedforward_dropout)
-        transformer = Transformer(embedding_dim=embedding_dim,
-                                  num_attention_heads=num_attention_heads,
-                                  attention_dropout=attention_dropout,
-                                  feedforward_dropout=feedforward_dropout,
-                                  feedforward_multiplier=feedforward_multiplier,
-                                  norm_epsilon=norm_epsilon,
-                                  name="inner_trasnformer_block_for_features")
-
-        super().__init__(multi_head_inter_sample_attention=multihead_inter_sample_attention,
-                         feed_forward=feed_forward,
-                         transformer=transformer,
-                         **kwargs)
-
-        self.data_dim = data_dim
+        if embedd_inputs:
+            inputs = keras.layers.Input((input_dim,), name="inputs")
+        else:
+            # Embeddings will be computed by an external embedding layer,
+            # so in that case, the model should expect inputs with dims
+            # (input_dim, embedding_dim)
+            inputs = keras.layers.Input((input_dim, embedding_dim),
+                                        name="inputs")
+        x = inputs
+        if embedd_inputs:
+            x = SAINTEmbedding(
+                embedding_dim=embedding_dim,
+                cardinalities=cardinalities)(x)
+        x = CLSToken(embedding_dim=embedding_dim)(x)
+        for i in range(num_layers):
+            x = SAINTEncoderLayer(
+                embedding_dim=embedding_dim,
+                num_heads=num_heads,
+                feedforward_dim=feedforward_dim,
+                attention_dropout=attention_dropout,
+                feedforward_dropout=feedforward_dropout,
+                layer_norm_epsilon=layer_norm_epsilon,
+                name=f"saint_encoder_layer_{i}")(x)
+        if return_cls_token_only:
+            outputs = CLSTokenExtraction()(x)
+        else:
+            outputs = x
+        super().__init__(inputs=inputs, outputs=outputs, **kwargs)
+
+        self.input_dim = input_dim
+        self.cardinalities = cardinalities
+        self.num_layers = num_layers
         self.embedding_dim = embedding_dim
-        self.num_attention_heads = num_attention_heads
-        self.num_inter_sample_attention_heads = num_inter_sample_attention_heads
+        self.num_heads = num_heads
+        self.feedforward_dim = feedforward_dim
         self.attention_dropout = attention_dropout
-        self.inter_sample_attention_dropout = inter_sample_attention_dropout
         self.feedforward_dropout = feedforward_dropout
-        self.feedforward_multiplier = feedforward_multiplier
-        self.norm_epsilon = norm_epsilon
-        self.apply_attention_to_features = apply_attention_to_features
-        self.apply_attention_to_rows = apply_attention_to_rows
+        self.layer_norm_epsilon = layer_norm_epsilon
+        self.embedd_inputs = embedd_inputs
+        self.return_cls_token_only = return_cls_token_only
+
+    def compute_output_shape(self, input_shape):
+        if self.return_cls_token_only:
+            return input_shape[:1] + (1, self.embedding_dim)
+        else:
+            return input_shape + (self.embedding_dim,)
 
     def get_config(self):
-        config = {'name': self.name,
-                  'trainable': self.trainable,
-                  'data_dim': self.data_dim,
-                  'embedding_dim': self.embedding_dim,
-                  'num_attention_heads': self.num_attention_heads,
-                  'num_inter_sample_attention_heads': self.num_inter_sample_attention_heads,
-                  'attention_dropout': self.attention_dropout,
-                  'inter_sample_attention_dropout': self.inter_sample_attention_dropout,
-                  'feedforward_dropout': self.feedforward_dropout,
-                  'feedforward_multiplier': self.feedforward_multiplier,
-                  'norm_epsilon': self.norm_epsilon,
-                  'apply_attention_to_features': self.apply_attention_to_features,
-                  'apply_attention_to_rows': self.apply_attention_to_rows,
-                  'num_embedded_features': self.num_embedded_features,
-                  }
+        config = super().get_config()
+        config.update({
+            "input_dim": self.input_dim,
+            "cardinalities": self.cardinalities,
+            "embedding_dim": self.embedding_dim,
+            "num_layers": self.num_layers,
+            "num_heads": self.num_heads,
+            "feedforward_dim": self.feedforward_dim,
+            "attention_dropout": self.attention_dropout,
+            "feedforward_dropout": self.feedforward_dropout,
+            "layer_norm_epsilon": self.layer_norm_epsilon,
+            "embedd_inputs": self.embedd_inputs,
+            "return_cls_token_only": self.return_cls_token_only,
+        })
         return config
-
-    @classmethod
-    def from_config(cls, config):
-        # data_dim is the only positional argument
-        data_dim = config.pop("data_dim")
-        return cls(data_dim=data_dim, **config)
```

### Comparing `Teras-0.2.0/teras/layers/tabnet/tabnet_decoder.py` & `Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,219 @@
-import tensorflow as tf
-from tensorflow import keras
-from teras.layers.tabnet import TabNetFeatureTransformer
+import keras
+from keras import ops
 
+from teras._src.layers.layer_list import LayerList
+from teras._src.layers.tabnet.attentive_transformer import \
+    TabNetAttentiveTransformer
+from teras._src.layers.tabnet.feature_transformer import \
+    TabNetFeatureTransformer
+from teras._src.api_export import teras_export
 
-@keras.saving.register_keras_serializable("teras.layers.tabnet")
-class TabNetDecoder(keras.layers.Layer):
+
+@teras_export("teras.models.TabNetEncoderBackbone")
+class TabNetEncoderBackbone(keras.Model):
     """
-    TabNetDecoder as proposed by Sercan et al. in TabNet paper.
+    TabNetEncoder proposed by Arik et al. in the
+    "TabNet: Attentive Interpretable Tabular Learning" paper.
 
     Reference(s):
         https://arxiv.org/abs/1908.07442
 
     Args:
-        data_dim: ``int``,
-            The dimensionality of the original input dataset,
-            or the number of features in the original input dataset.
-
-        feature_transformer_dim: ``int``, default 32,
-            The dimensionality of the hidden representation in feature transformation block.
-            Each layer first maps the representation to a `2 * feature_transformer_dim`
-            output and half of it is used to determine the
-            non-linearity of the GLU activation where the other half is used as an
-            input to GLU, and eventually `feature_transformer_dim` output is
-            transferred to the next layer.
-
-        decision_step_output_dim: ``int``, default 32,
-            The dimensionality of output at each decision step, which is later mapped to the
-            final classification or regression output.
-            It is recommended to keep ``decision_step_output_dim`` and ``feature_transformer_dim``
-            equal to each other.
-            Adjusting these two parameters values is a good way of obtaining a tradeoff between
-            performance and complexity.
-
-        num_decision_steps: ``int``, default 5,
-            The number of sequential decision steps.
+        input_dim: int, The dimensionality of the input dataset.
+        feature_transformer_dim: int, the dimensionality of the hidden
+            representation in feature transformation block.
+            The dense layer inside the `TabNetFeatureTransformer` first
+            maps  the inputs to `feature_transformer_dim` * 2 dimension
+            hidden representations and later the glu activation
+            maps the hidden representations to
+            `feature_transformer_dim` dimensions.
+        decision_step_dim: int, the dimensionality of output at each
+            decision step, which is later mapped to the final
+            classification or regression output.
+            It is recommended to keep `decision_step_dim` and
+            `feature_transformer_dim` equal to each other.
+            Adjusting these two parameters values is a good way of
+            obtaining a tradeoff between performance and complexity.
+        num_decision_steps: int, the number of sequential decision steps.
             For most datasets a value in the range [3, 10] is optimal.
-            If there are more informative features in the dataset, the value tends to
-            be higher. That said, a very high value of `num_decision_steps` may suffer
-            from overfitting.
-
-        num_shared_layers: ``int``, default 2,
-            Number of shared layers to use in the ``TabNetFeatureTransformer``.
-            These shared layers are *shared* across decision steps.
-
-        num_decision_dependent_layers: ``int``, default 2,
-            Number of decision dependent layers to use in the ``TabNetFeatureTransformer``.
-            In simple words, ``num_decision_dependent_layers`` are created
-            for each decision step in the ``num_decision_steps``.
-            For instance, if ``num_decision_steps = `5` and  ``num_decision_dependent_layers = 2``
+            If there are more informative features in the dataset,
+            the value tends to be higher. That said, a very high value
+            of `num_decision_steps` may suffer from overfitting.
+            Defaults to 5.
+        num_shared_layers: int, Number of shared layers to use in the
+            ``TabNetFeatureTransformer``.
+            These shared layers are shared across decision steps.
+            Defaults to 2.
+        num_decision_dependent_layers: int, number of decision dependent
+            layers to use in the `TabNetFeatureTransformer`.
+            In simple words, `num_decision_dependent_layers` are created
+            for each decision step in the `num_decision_steps`.
+            For instance, if `num_decision_steps = 5` and
+            `num_decision_dependent_layers = 2`
             then 10 layers will be created, 2 for each decision step.
-
-        relaxation_factor: ``float``, default 1.5,
-            Relaxation factor that promotes the reuse of each
-            feature at different decision steps. When it is 1, a feature is enforced
-            to be used only at one decision step and as it increases, more
-            flexibility is provided to use a feature at multiple decision steps.
-            An optimal value of relaxation_factor can have a major role on the performance.
-            Typically, a larger value for `num_decision_steps` favors for a larger ``relaxation_factor``.
-
-        batch_momentum: ``float``, default 0.9,
-            Momentum value to use for ``BatchNormalization`` layer.
-
-        virtual_batch_size: `int`, default 64,
-            Batch size to use for ``virtual_batch_size`` parameter in ``BatchNormalization`` layer.
-            This is typically much smaller than the ``batch_size`` used for training.
-
-        residual_normalization_factor: ``float``, default 0.5,
-            In the feature transformer, except for the first layer, every other layer utilizes
-            normalized residuals, where ``residual_normalization_factor``
-            determines the scale of normalization.
+        relaxation_factor: float, relaxation factor that promotes the
+            reuse of each feature at different decision steps. When it
+            is 1, a feature is enforced to be used only at one decision
+            step and as it increases, more flexibility is provided to
+            use a feature at multiple decision steps.
+            An optimal value of relaxation_factor can have a major role on
+            the performance. Typically, a larger value for
+            `num_decision_steps` favors for a larger `relaxation_factor`.
+        batch_momentum: float, momentum value to use for
+            `BatchNormalization` layer.
+            Defaults to 0.9
+        epsilon: float, epsilon is a small number for numerical stability
+            during the computation of entropy loss.
+            Defaults to 0.00001
+        reuse_shared_layers: bool, whether to reset shared layers of the
+            `TabNetFeatureTransformer` layer.
+            Although we want to use the same shared layers across
+            multiple instances of `TabNetFeatureTransformer` but we may
+            not want to use the same shared layers across different
+            `TabNetEncoder` instances.
+            Defaults to `True`.
     """
     def __init__(self,
-                 data_dim: int,
-                 feature_transformer_dim: int = 32,
-                 decision_step_output_dim: int = 32,
+                 input_dim: int,
+                 feature_transformer_dim: int,
+                 decision_step_dim: int,
                  num_decision_steps: int = 5,
                  num_shared_layers: int = 2,
-                 num_decision_dependent_layers: int = 2,
+                 num_decision_dependent_layers: int = 5,
+                 relaxation_factor: float = 1.5,
                  batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 residual_normalization_factor: float = 0.5,
+                 epsilon: float = 1e-5,
+                 reset_shared_layers: bool = True,
                  **kwargs):
         super().__init__(**kwargs)
-        self.data_dim = data_dim
+        self.input_dim = input_dim
         self.feature_transformer_dim = feature_transformer_dim
-        self.decision_step_output_dim = decision_step_output_dim
+        self.decision_step_dim = decision_step_dim
+        self.num_decision_steps = num_decision_steps
         self.num_shared_layers = num_shared_layers
         self.num_decision_dependent_layers = num_decision_dependent_layers
-        self.num_decision_steps = num_decision_steps
+        self.relaxation_factor = relaxation_factor
         self.batch_momentum = batch_momentum
-        self.virtual_batch_size = virtual_batch_size
-        self.residual_normalization_factor = residual_normalization_factor
+        self.epsilon = epsilon
+        self.reset_shared_layers = reset_shared_layers
 
-        self.features_transformers_per_step = []
-        self.projection_layers_per_step = []
+        if self.reset_shared_layers:
+            TabNetFeatureTransformer.reset_shared_layers()
 
-        # To be able to share the `shared_layers` across instances, we introduced
-        # a class attribute called `shared_layers` in the FeatureTransformer class
-        # BUT here's the problem,
-        # even though we now want to create new shared layers separately for our Decoder, it won't ... unless...
-        # we do this
-        TabNetFeatureTransformer.reset_shared_layers()
-        # Why? Because each time we create `TabNetFeatureTransformer` instance, it first checks if `shared_layers`
-        # attribute is None or not, if it's None it will create new shared layers, otherwise it won't.
-
-        for i in range(self.num_decision_steps):
-            self.features_transformers_per_step.append(TabNetFeatureTransformer(
-                                                        units=self.feature_transformer_dim,
-                                                        num_shared_layers=self.num_shared_layers,
-                                                        num_decision_dependent_layers=self.num_decision_dependent_layers,
-                                                        batch_momentum=self.batch_momentum,
-                                                        virtual_batch_size=self.virtual_batch_size,
-                                                        residual_normalization_factor=self.residual_normalization_factor,
-                                                        name=f"step_{i}_feature_transformer"
-                                                        ))
-            self.projection_layers_per_step.append(keras.layers.Dense(self.data_dim))
+        self.feature_transformers = LayerList([
+            TabNetFeatureTransformer(
+                hidden_dim=self.feature_transformer_dim,
+                num_shared_layers=self.num_decision_steps,
+                num_decision_dependent_layers=self.num_decision_dependent_layers,
+                batch_momentum=self.batch_momentum,
+                name=f"encoder_feature_transformer_{i}"
+            )
+            for i in range(self.num_decision_steps)
+        ],
+            sequential=False,
+            name="encoder_feature_transformers"
+        )
+        self.attentive_transformers = LayerList([
+            TabNetAttentiveTransformer(
+                data_dim=input_dim,
+                batch_momentum=self.batch_momentum,
+                name=f"encoder_attentive_transformer_{i}"
+            )
+            for i in range(self.num_decision_steps - 1)
+        ],
+            sequential=False,
+            name="encoder_attentive_transformers"
+        )
+        self.batch_norm = keras.layers.BatchNormalization(
+            momentum=self.batch_momentum
+        )
+
+    def build(self, input_shape):
+        input_shape = tuple(input_shape)
+        self._input_shape = input_shape
+        self.batch_norm.build(input_shape)
+        self.feature_transformers.build(input_shape)
+        input_shape = input_shape[:-1] + (
+            self.feature_transformer_dim - self.decision_step_dim,)
+        self.attentive_transformers.build(input_shape)
 
     def call(self, inputs, mask=None):
-        """
-        Args:
-            inputs: Encoded representations.
-
-        Returns:
-
-        """
-        batch_size = tf.shape(inputs)[0]
-        reconstructed_features = tf.zeros(shape=(batch_size, self.data_dim))
-
-        for i in range(self.num_decision_steps):
-            feat_output = self.features_transformers_per_step[i](inputs)
-            reconstructed_features += self.projection_layers_per_step[i](feat_output)
-
-        # The paper says,
-        # the decoder’s last FC (dense) layer is multiplied with S (binary mask indicating which features are missing)
-        # to output the unknown features.
+        normalized_inputs = self.batch_norm(inputs)
+        batch_size = ops.shape(inputs)[0]
+        decision_out_aggregated = ops.zeros(
+            (batch_size, self.decision_step_dim))
+        # During pretraining, we pass mask alongside inputs to the encoder
+        masked_features = normalized_inputs
         if mask is not None:
-            reconstructed_features *= mask
+            mask_values = mask
+        else:
+            mask_values = ops.zeros_like(inputs)
+        aggregated_mask_values = ops.zeros_like(inputs)
+        # Prior scales denote how much a feature has been used previously
+        prior_scales = ops.ones_like(inputs)
+        total_entropy = 0.
+
+        for d_step in range(self.num_decision_steps):
+            feat_transformer_out = self.feature_transformers[d_step](
+                masked_features)
+            if d_step > 0 or self.num_decision_steps == 1:
+                decision_out = ops.relu(
+                    feat_transformer_out[:, :self.decision_step_dim])
+                decision_out_aggregated += decision_out
+
+                # Aggregated masks are used for the visualization of the
+                # feature importance attributes.
+                scale = ops.sum(
+                    decision_out, axis=-1, keepdims=True) / (
+                                self.num_decision_steps - 1)
+                aggregated_mask_values += mask_values / scale
+
+            the_other_output_half = feat_transformer_out[:, self.decision_step_dim:]
+
+            if d_step < self.num_decision_steps - 1:
+                mask = self.attentive_transformers[d_step](
+                    the_other_output_half,
+                    prior_scales)
+                # Relaxation factor controls the amount of reuse of
+                # features between different decision blocks and updated
+                # with the values of coefficients.
+                prior_scales = prior_scales * (self.relaxation_factor -
+                                               mask)
+
+                # Entropy is used to penalize the amount of sparsity in
+                # feature selection.
+                total_entropy = total_entropy + ops.mean(
+                    ops.sum(-mask * ops.log(mask + self.epsilon), axis=-1)
+                ) / self.num_decision_steps - 1
 
-        return reconstructed_features
+                masked_features = mask * normalized_inputs
+
+        self.add_loss(total_entropy)
+
+        return decision_out_aggregated
+
+    def compute_output_shape(self, input_shape):
+        return input_shape[:-1] + (self.decision_step_dim,)
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'data_dim': self.data_dim,
-                      'feature_transformer_dim': self.feature_transformer_dim,
-                      'decision_step_output_dim': self.decision_step_output_dim,
-                      'num_decision_steps': self.num_decision_steps,
-                      'num_shared_layers': self.num_shared_layers,
-                      'num_decision_dependent_layers': self.num_decision_dependent_layers,
-                      'batch_momentum': self.batch_momentum,
-                      'virtual_batch_size': self.virtual_batch_size,
-                      'residual_normalization_factor': self.residual_normalization_factor,
-                      }
-        config.update(new_config)
+        config.update({
+            'input_dim': self.input_dim,
+            'feature_transformer_dim': self.feature_transformer_dim,
+            'decision_step_dim': self.decision_step_dim,
+            'num_decision_steps': self.num_decision_steps,
+            'num_shared_layers': self.num_shared_layers,
+            'num_decision_dependent_layers': self.num_decision_dependent_layers,
+            'relaxation_factor': self.relaxation_factor,
+            'batch_momentum': self.batch_momentum,
+            'epsilon': self.epsilon,
+            'reset_shared_layers': self.reset_shared_layers,
+        })
         return config
+
+    def get_build_config(self):
+        build_config = dict(input_shape=self._input_shape)
+        return build_config
+
+    def build_from_config(self, build_config):
+        self.build(build_config["input_shape"])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer.py` & `Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,148 +1,192 @@
-from tensorflow import keras
-from teras.layers.tabnet.tabnet_feature_transformer_block import TabNetFeatureTransformerBlock
+import keras
+from keras import ops
 
+from teras._src.layers.layer_list import LayerList
+from teras._src.layers.tabnet.feature_transformer_layer import \
+    TabNetFeatureTransformerLayer
+from teras._src.api_export import teras_export
 
-@keras.saving.register_keras_serializable("teras.layers.tabnet")
-class TabNetFeatureTransformer(keras.layers.Layer):
+
+@teras_export("teras.models.TabNetDecoder")
+class TabNetDecoder(keras.Model):
     """
-    Feature Transformer as proposed by Sercan et al. in TabNet paper.
-    It is made up of ``FeatureTransformerBlock`` building blocks.
+    TabNetDecoder model for self-supervised learning,
+    proposed by Arik et al. in the
+    "TabNet: Attentive Interpretable Tabular Learning" paper.
 
     Reference(s):
         https://arxiv.org/abs/1908.07442
 
     Args:
-        units: ``int``, default 32,
-            the dimensionality of the hidden representation in feature transformation block.
-            Each layer first maps the representation to a ``2 * feature_transformer_dim``
-            output and half of it is used to determine the
-            non-linearity of the GLU activation where the other half is used as an
-            input to GLU, and eventually ``feature_transformer_dim`` output is
-            transferred to the next layer.
-
-        num_shared_layers: ``int``, default 2.
-            Number of shared layers to use in the Feature Transformer.
-            These shared layers are `shared` across decision steps.
-
-        num_decision_dependent_layers: ``int``, default 2.
-            Number of decision dependent layers to use.
-            In simple words, ``num_decision_dependent_layers`` are created for each
-            decision step in the ``num_decision_steps``.
-            For instance, if ``num_decision_steps = 5`` and  ``num_decision_dependent_layers = `2`
+        data_dim: int, The dimensionality of the input dataset.
+        feature_transformer_dim: int, the dimensionality of the hidden
+            representation in feature transformation block.
+            The dense layer inside the `TabNetFeatureTransformer` first
+            maps  the inputs to `feature_transformer_dim` * 2 dimension
+            hidden representations and later the glu activation
+            maps the hidden representations to
+            `feature_transformer_dim` dimensions.
+        decision_step_dim: int, the dimensionality of output at each
+            decision step, which is later mapped to the final
+            classification or regression output.
+            It is recommended to keep `decision_step_dim` and
+            `feature_transformer_dim` equal to each other.
+            Adjusting these two parameters values is a good way of
+            obtaining a tradeoff between performance and complexity.
+        num_decision_steps: int, the number of sequential decision steps.
+            For most datasets a value in the range [3, 10] is optimal.
+            If there are more informative features in the dataset,
+            the value tends to be higher. That said, a very high value
+            of `num_decision_steps` may suffer from overfitting.
+            Defaults to 5.
+        num_shared_layers: int, Number of shared layers to use in the
+            ``TabNetFeatureTransformer``.
+            These shared layers are shared across decision steps.
+            Defaults to 2.
+        num_decision_dependent_layers: int, number of decision dependent
+            layers to use in the `TabNetFeatureTransformer`.
+            In simple words, `num_decision_dependent_layers` are created
+            for each decision step in the `num_decision_steps`.
+            For instance, if `num_decision_steps = 5` and
+            `num_decision_dependent_layers = 2`
             then 10 layers will be created, 2 for each decision step.
-
-        batch_momentum: ``float``, default 0.9,
-            Momentum value to use for ``BatchNormalization`` layer.
-
-        virtual_batch_size: ``int``, default 64,
-            Batch size to use for ``virtual_batch_size`` parameter in ``BatchNormalization`` layer.
-            This is typically much smaller than the `batch_size` used for training.
-            And most importantly, the ``batch_size`` must always be divisible by the ``virtual_batch_size``.
-
-        residual_normalization_factor: ``float``, default 0.5,
-            In the feature transformer, except for the layer, every other layer utilizes
-            normalized residuals, where ``residual_normalization_factor`` determines the scale of normalization.
+        relaxation_factor: float, relaxation factor that promotes the
+            reuse of each feature at different decision steps. When it
+            is 1, a feature is enforced to be used only at one decision
+            step and as it increases, more flexibility is provided to
+            use a feature at multiple decision steps.
+            An optimal value of relaxation_factor can have a major role on
+            the performance. Typically, a larger value for
+            `num_decision_steps` favors for a larger `relaxation_factor`.
+        batch_momentum: float, momentum value to use for
+            `BatchNormalization` layer.
+            Defaults to 0.9
+        epsilon: float, epsilon is a small number for numerical stability
+            during the computation of entropy loss.
+            Defaults to 0.00001
     """
-    shared_layers = None
-
     def __init__(self,
-                 units: int = 32,
+                 data_dim: int,
+                 feature_transformer_dim: int,
+                 decision_step_dim: int,
+                 num_decision_steps: int = 5,
                  num_shared_layers: int = 2,
-                 num_decision_dependent_layers: int = 2,
+                 num_decision_dependent_layers: int = 5,
+                 relaxation_factor: float = 1.5,
                  batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 residual_normalization_factor: float = 0.5,
+                 epsilon: float = 1e-5,
                  **kwargs):
-
-        if num_shared_layers == 0 and num_decision_dependent_layers == 0:
-            raise ValueError("Feature Transformer requires at least one of either shared or decision depenedent layers."
-                             " But both `num_shared_layers` and `num_decision_dependent_layers` were passed a 0 value.")
-
         super().__init__(**kwargs)
-        self.units = units
+        self.data_dim = data_dim
+        self.feature_transformer_dim = feature_transformer_dim
+        self.decision_step_dim = decision_step_dim
+        self.num_decision_steps = num_decision_steps
         self.num_shared_layers = num_shared_layers
         self.num_decision_dependent_layers = num_decision_dependent_layers
+        self.relaxation_factor = relaxation_factor
         self.batch_momentum = batch_momentum
-        self.virtual_batch_size = virtual_batch_size
-        self.residual_normalization_factor = residual_normalization_factor
+        self.epsilon = epsilon
+
+        # self.feature_transformers = [
+        #     TabNetFeatureTransformer(
+        #         hidden_dim=self.feature_transformer_dim,
+        #         num_shared_layers=self.num_decision_steps,
+        #         num_decision_dependent_layers=self.num_decision_dependent_layers,
+        #         batch_momentum=self.batch_momentum,
+        #         name=f"decoder_feature_transformer_{i}"
+        #     )
+        #     for i in range(self.num_decision_steps)
+        # ]
+        self.shared_layers = LayerList([
+            TabNetFeatureTransformerLayer(
+                dim=feature_transformer_dim,
+                batch_momentum=batch_momentum,
+                name=f"decoder_shared_layer_{i}")
+            for i in range(self.num_shared_layers)
+        ],
+            name="shared_layers")
+        self.decision_dependent_layers = LayerList([
+            TabNetFeatureTransformerLayer(
+                dim=feature_transformer_dim,
+                batch_momentum=batch_momentum,
+                name=f"decoder_decision_dependent_layer_{i}")
+            for i in range(self.num_decision_steps * self.num_decision_dependent_layers)
+        ],
+            name="decision_dependent_layers"
+        )
+        self.projection_layers = LayerList([
+            keras.layers.Dense(units=self.data_dim,
+                               name=f"projection_layer_{i}")
+            for i in range(self.num_decision_steps)
+        ],
+            sequential=False,
+            name="projection_layers"
+        )
+
+    def build(self, input_shape):
+        input_shape = tuple(input_shape)
+        self._input_shape = input_shape
+        if not self.shared_layers.built:
+            self.shared_layers.build(input_shape)
+        input_shape = self.shared_layers.compute_output_shape(input_shape)
+        self.decision_dependent_layers.build(input_shape)
+        input_shape = self.decision_dependent_layers.compute_output_shape(
+            input_shape
+        )
+        self.projection_layers.build(input_shape)
+
+    def call(self, inputs, mask=None):
+        batch_size = ops.shape(inputs)[0]
+        reconstructed_features = ops.zeros(
+            shape=(batch_size, self.data_dim)
+        )
+
+        for i in range(self.num_decision_steps):
+            # feature_out = self.feature_transformers[i](inputs)
+            # reconstructed_features += self.projection_layers[i](feature_out)
+            x = inputs
+            residue = None
+            for layer in self.shared_layers:
+                x = layer(x)
+                if residue is not None:
+                    x += ops.sqrt(0.5) * residue
+                residue = x
+
+            start_idx = i * self.num_decision_steps
+            end_idx = start_idx + self.num_decision_steps
+            for layer in self.decision_dependent_layers[start_idx: end_idx]:
+                x = layer(x)
+                if residue is not None:
+                    x += ops.sqrt(0.5) * residue
+                residue = x
+            reconstructed_features += self.projection_layers[i](x)
+
+        # According to the paper, the decoder’s last FC (dense) layer is
+        # multiplied with S (binary mask indicating which features are
+        # missing) to output the unknown features.
+        if mask is not None:
+            reconstructed_features *= mask
 
-        # Since shared layers should be accessible across instances so we make them as class attributes
-        # and use class method to instantiate them, the first time an instance of this FeatureTransformer
-        # class is made.
-        if self.shared_layers is None and num_shared_layers > 0:
-            self._create_shared_layers(num_shared_layers,
-                                       units,
-                                       batch_momentum=batch_momentum,
-                                       virtual_batch_size=virtual_batch_size,
-                                       residual_normalization_factor=residual_normalization_factor)
-
-        self.inner_block = keras.models.Sequential(name="inner_block")
-
-        self.inner_block.add(self.shared_layers)
-
-        if self.num_decision_dependent_layers > 0:
-            decision_dependent_layers = keras.models.Sequential(name=f"decision_dependent_layers")
-            for j in range(self.num_decision_dependent_layers):
-                if j == 0 and self.num_shared_layers == 0:
-                    # then it means that this is the very first layer in the Feature Transformer
-                    # because no shard layers exist.
-                    # hence we shouldn't use residual normalization
-                    use_residual_normalization = False
-                else:
-                    use_residual_normalization = True
-                decision_dependent_layers.add(TabNetFeatureTransformerBlock(
-                    units=self.units,
-                    batch_momentum=self.batch_momentum,
-                    virtual_batch_size=self.virtual_batch_size,
-                    use_residual_normalization=use_residual_normalization,
-                    name=f"decision_dependent_layer_{j}")
-                )
-
-            self.inner_block.add(decision_dependent_layers)
-
-    @classmethod
-    def _create_shared_layers(cls, num_shared_layers, units, **kwargs):
-        # The outputs of first layer in feature transformer isn't residual normalized
-        # so we use a pointer to know which layer is first.
-        # Important to keep in mind that shared layers ALWAYS precede the decision dependent layers
-        # BUT we want to allow user to be able to use NO shared layers at all, i.e. 0.
-        # Hence, only if the `num_shared_layers` is 0, should the first dependent layer for each step
-        # be treated differently.
-        # Initialize the block of shared layers
-        cls.shared_layers = keras.models.Sequential(name="shared_layers")
-        for i in range(num_shared_layers):
-            if i == 0:
-                # First layer should not use residual normalization
-                use_residual_normalization = False
-            else:
-                use_residual_normalization = True
-            cls.shared_layers.add(TabNetFeatureTransformerBlock(units=units,
-                                                                use_residual_normalization=use_residual_normalization,
-                                                                name=f"shared_layer_{i}",
-                                                                **kwargs))
-
-    @classmethod
-    def reset_shared_layers(cls):
-        """
-        Resets the shared layers.
-
-        You must reset shared layers, when you want to create
-        new instances of ``TabNetFeatureTransformer`` for ``TabNetDecoder``
-        after you have created those for the ``TabNetEncoder``.
-        """
-        cls.shared_layers = None
-
-    def call(self, inputs):
-        outputs = self.inner_block(inputs)
-        return outputs
+        return reconstructed_features
 
     def get_config(self):
         config = super().get_config()
-        config.update({'units': self.units,
-                       'num_shared_layers': self.num_shared_layers,
-                       'num_decision_dependent_layers': self.num_decision_dependent_layers,
-                       'batch_momentum': self.batch_momentum,
-                       'virtual_batch_size': self.virtual_batch_size,
-                       'residual_normalization_factor': self.residual_normalization_factor,
-                       })
+        config.update({
+            'data_dim': self.data_dim,
+            'feature_transformer_dim': self.feature_transformer_dim,
+            'decision_step_dim': self.decision_step_dim,
+            'num_decision_steps': self.num_decision_steps,
+            'num_shared_layers': self.num_shared_layers,
+            'num_decision_dependent_layers': self.num_decision_dependent_layers,
+            'relaxation_factor': self.relaxation_factor,
+            'batch_momentum': self.batch_momentum,
+            'epsilon': self.epsilon,
+        })
         return config
+
+    def get_build_config(self):
+        build_config = dict(input_shape=self._input_shape)
+        return build_config
+
+    def build_from_config(self, build_config):
+        self.build(build_config["input_shape"])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Teras-0.2.0/teras/layers/tabtransformer/__init__.py` & `Teras-0.3.0/teras/_src/losses/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,10 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
-from teras.layers.tabtransformer.tabtransformer_column_embedding import TabTransformerColumnEmbedding
```

### Comparing `Teras-0.2.0/teras/losses/ctgan.py` & `Teras-0.3.0/teras/_src/losses/ctgan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,76 @@
-import tensorflow as tf
-from tensorflow import keras
+import keras
+from keras import ops
+from teras._src.api_export import teras_export
 
 
-def generator_loss(generated_samples,
-                   y_generated,
-                   cond_vectors=None,
-                   mask=None,
-                   metadata=None):
+@teras_export("teras.losses.ctgan_generator_loss")
+def ctgan_generator_loss(x_generated,
+                         y_pred_generated,
+                         cond_vectors,
+                         mask,
+                         metadata):
     """
     Loss for the Generator model in the CTGAN architecture.
 
     CTGAN is a state-of-the-art tabular data generation architecture
     proposed by Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        generated_samples: Samples drawn from the input dataset
-        y_generated: Discriminator's output for the generated samples
+        x_generated: Samples drawn from the input dataset
+        y_pred_generated: Discriminator's output for the generated samples
         cond_vectors: Conditional vectors that are used for and with
             generated samples
         mask: Mask created during the conditional vectors generation step
-        metadata: Namedtuple meta deta of features.
-            That meta data contains miscellaneous information about features,
-            which is calculated during data transformation step.
+        metadata: dict, metadata computed during the data transformation step.
 
     Returns:
         Generator's loss.
     """
     loss = []
-    cross_entropy_loss = keras.losses.SparseCategoricalCrossentropy(from_logits=True,
-                                                                    reduction=keras.losses.Reduction.NONE)
+    cross_entropy_loss = keras.losses.SparseCategoricalCrossentropy(
+        from_logits=True, reduction=None)
     numerical_features_relative_indices = metadata["numerical"]["relative_indices_all"]
     features_relative_indices_all = metadata["relative_indices_all"]
     num_categories_all = metadata["categorical"]["num_categories_all"]
-    # the first k features in the data are numerical which we'll ignore as we're only
-    # concerned with the categorical features here
+    # the first k features in the data are numerical which we'll ignore as
+    # we're only concerned with the categorical features here
     offset = len(numerical_features_relative_indices)
     for i, index in enumerate(features_relative_indices_all[offset:]):
-        logits = generated_samples[:, index: index + num_categories_all[i]]
+        logits = x_generated[:, index: index + num_categories_all[i]]
         temp_cond_vector = cond_vectors[:, i: i + num_categories_all[i]]
-        labels = tf.argmax(temp_cond_vector, axis=1)
+        labels = ops.argmax(temp_cond_vector, axis=1)
         ce_loss = cross_entropy_loss(y_pred=logits,
                                      y_true=labels
                                      )
         loss.append(ce_loss)
-    loss = tf.stack(loss, axis=1)
-    loss = tf.reduce_sum(loss * tf.cast(mask, dtype=tf.float32)) / tf.cast(tf.shape(y_generated)[0], dtype=tf.float32)
-    loss = -tf.reduce_mean(y_generated) * loss
+    loss = ops.stack(loss, axis=1)
+    loss = ops.sum(loss * ops.cast(mask, dtype="float32")
+                   ) / ops.cast(ops.shape(y_pred_generated)[0], dtype="float32")
+    loss = -ops.mean(y_pred_generated) * loss
     return loss
 
 
-def discriminator_loss(y_real, y_generated):
+@teras_export("teras.losses.ctgan_discriminator_loss")
+def ctgan_discriminator_loss(y_pred_real, y_pred_generated):
     """
     Loss for the Discriminator model in the CTGAN architecture.
 
     CTGAN is a state-of-the-art tabular data generation architecture
     proposed by Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        y_real: Discriminator's output for real samples
-        y_generated: Discriminator's output for generated samples
+        y_pred_real: Discriminator's output for real samples
+        y_pred_generated: Discriminator's output for generated samples
 
     Returns:
         Discriminator's loss.
     """
-    return -(tf.reduce_mean(y_real) - tf.reduce_mean(y_generated))
-
-
-def generator_dummy_loss(y_dummy, y_pred):
-    """
-    For the generator model to track the loss function, and show it in outputs
-    we create a dummy loss function which receives the loss function
-    and returns it as is. It is passed to the model during compilation step.
-
-    Reference(s):
-        Idea taken from:
-        https://towardsdatascience.com/solving-the-tensorflow-keras-model-loss-problem-fd8281aeeb11
-
-    Args:
-        y_dummy: An array of length batch_size, filled with dummy values.
-        y_pred: The loss value computed using a custom loss function.
-
-    Returns:
-        Returns y_pred (i.e. loss) as is.
-    """
-    return tf.squeeze(y_pred)
+    return -(ops.mean(y_pred_real) - ops.mean(y_pred_generated))
```

### Comparing `Teras-0.2.0/teras/preprocessing/__init__.py` & `Teras-0.3.0/teras/preprocessing/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,28 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from teras.preprocessing.oenf import PiecewiseLinearEncoding
-
-# CTGAN preprocessing classes
-from teras.preprocessing.ctgan import ModeSpecificNormalization
-from teras.preprocessing.ctgan import (CTGANDataTransformer,
-                                       CTGANDataSampler)
-
-# TVAE preprocessing classes
-from teras.preprocessing.tvae import (TVAEDataTransformer,
-                                      TVAEDataSampler)
-
-
-# GAIN preprocessing classes
-from teras.preprocessing.gain import (GAINDataTransformer,
-                                      GAINDataSampler)
-
-
-# PCGAIN preprocessing classes
-from teras.preprocessing.pcgain import (PCGAINDataTransformer,
-                                        PCGAINDataSampler)
-
-# Vime preprocessing classes
-from teras.preprocessing.vime import (VimeDataTransformer,
-                                      VimeDataSampler)
+# Data Samplers
+from teras._src.preprocessing.data_samplers.ctgan import (
+    CTGANDataSampler as CTGANDataSampler)
+from teras._src.preprocessing.data_samplers.tvae import (
+    TVAEDataSampler as TVAEDataSampler)
+
+# Data Transformers
+from teras._src.preprocessing.data_transformers.gain import (
+    GAINDataTransformer as GAINDataTransformer)
+from teras._src.preprocessing.data_transformers.ctgan import (
+    CTGANDataTransformer as CTGANDataTransformer)
+from teras._src.preprocessing.data_transformers.tvae import (
+    TVAEDataTransformer as TVAEDataTransformer)
```

### Comparing `Teras-0.2.0/teras/preprocessing/base/__init__.py` & `Teras-0.3.0/teras/_src/backend/common/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# Copyright 2023 Khawaja Abaid Ullah
+# Copyright 2024 Khawaja Abaid Ullah
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .base_data_transformer import BaseDataTransformer
```

### Comparing `Teras-0.2.0/teras/preprocessing/base/base_data_transformer.py` & `Teras-0.3.0/teras/_src/preprocessing/data_transformers/data_transformer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 from abc import abstractmethod
 import pandas as pd
 
 
-class BaseDataTransformer:
+class DataTransformer:
     """
-    Base class for ``DataTransformer`` classes.
+    Base `DataTransformer` class.
     It provides the common methods and attributes.
     """
     def __init__(self):
-        self.metadata = dict()
-        self.metadata["numerical"] = dict()
-        self.metadata["categorical"] = dict()
-        self.fitted = False
+        self._metadata = dict()
+        self._metadata["continuous"] = dict()
+        self._metadata["categorical"] = dict()
+        self._fitted = False
 
     @abstractmethod
-    def fit(self, x, **kwargs):
-        pass
+    def fit(self, x):
+        raise NotImplementedError
 
     @abstractmethod
-    def transform(self, x, **kwargs):
-        pass
+    def transform(self, x):
+        raise NotImplementedError
 
     def get_metadata(self):
         """
         Returns:
-            named tuple of features metadata.
+            dictionary of features metadata.
         """
-        return self.metadata
+        if not self._fitted:
+            raise AssertionError(
+                "The `fit` method has not yet been called. Please fit the "
+                "`DataTransformer` before accessing the `get_metadata` method."
+            )
+        return self._metadata
+
+    @property
+    def metadata(self):
+        return self.get_metadata()
 
     def fit_transform(self,
-                      x: pd.DataFrame,
-                      return_dataframe: bool = True):
+                      x: pd.DataFrame):
         self.fit(x)
-        return self.transform(x, return_dataframe=return_dataframe)
+        self._fitted = True
+        return self.transform(x)
+
+    @abstractmethod
+    def save(self, filename):
+        raise NotImplementedError
+
+    @classmethod
+    @abstractmethod
+    def load(cls, filename):
+        raise NotImplementedError
```

### Comparing `Teras-0.2.0/teras/utils/types.py` & `Teras-0.3.0/teras/_src/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import tensorflow as tf
-from tensorflow import keras
+import keras
 from typing import Union, List, Callable, Tuple
 import numpy as np
+import pandas as pd
 
 
-# Taken from TensorFlow Addons
+# Taken from TensorFlow Addons - Sorry!
 
 Number = Union[
                 float,
                 int,
                 np.float16,
                 np.float32,
                 np.float64,
@@ -19,31 +19,21 @@
                 np.uint8,
                 np.uint16,
                 np.uint32,
                 np.uint64,
             ]
 
 
-TensorLike = Union[
-                List[Union[Number, list]],
-                tuple,
-                Number,
-                np.ndarray,
-                tf.Tensor,
-                tf.SparseTensor,
-                tf.Variable,
-            ]
-
 ActivationType = Union[str,
                        Callable,
                        keras.layers.Layer,
                 ]
 
 
-UnitsValuesType = Union[List[int], Tuple[int]]
+IntegerSequence = Union[List[int], Tuple[int]]
 
 LayersList = List[keras.layers.Layer]
 
 LayersCollection = Union[keras.layers.Layer,
                          List[keras.layers.Layer],
                          keras.Model]
 
@@ -58,7 +48,12 @@
 InitializerType = Union[str, keras.initializers.Initializer]
 
 
 LayerOrModelType = Union[keras.layers.Layer, keras.Model]
 
 FeaturesNamesType = Union[List[str], Tuple[str]]
 
+OptionalIntOrStr = Union[int, str, None]
+
+ListOrArray = Union[list, np.array]
+
+DataFrameOrNdArray = Union[pd.DataFrame, np.ndarray]
```

### Comparing `Teras-0.2.0/teras/utils/utils_test.py` & `Teras-0.3.0/teras/_src/backend/tensorflow/utils_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from teras.utils.utils import dataframe_to_tf_dataset
+from .utils import dataframe_to_tf_dataset
 import pandas as pd
 import numpy as np
 
 
 def test_dataframe_to_tf_dataset_without_label():
     df = pd.DataFrame(data={"length": np.ones(10),
                             "area": np.ones(10) * 2})
```

