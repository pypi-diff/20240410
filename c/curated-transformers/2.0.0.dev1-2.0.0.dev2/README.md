# Comparing `tmp/curated-transformers-2.0.0.dev1.tar.gz` & `tmp/curated-transformers-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-2.0.0.dev1.tar", last modified: Mon Apr  8 11:39:52 2024, max compression
+gzip compressed data, was "curated-transformers-2.0.0.dev2.tar", last modified: Wed Apr 10 07:03:40 2024, max compression
```

## Comparing `curated-transformers-2.0.0.dev1.tar` & `curated-transformers-2.0.0.dev2.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.358737 curated-transformers-2.0.0.dev1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-08 11:39:52.358737 curated-transformers-2.0.0.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4606 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.286736 curated-transformers-2.0.0.dev1/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.294736 curated-transformers-2.0.0.dev1/curated_transformers/generation/
--rw-r--r--   0 vsts      (1001) docker     (127)     1346 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3787 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/default_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1962 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4303 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/generator_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1756 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/llama.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6591 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/logits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      631 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/mpt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/state.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2794 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/stop_conditions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/string_generator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.298736 curated-transformers-2.0.0.dev1/curated_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4055 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/activations.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35234 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10495 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/feedforward.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16063 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.298736 curated-transformers-2.0.0.dev1/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (127)     1921 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.302736 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4065 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4484 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4481 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3650 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7766 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/auto_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.302736 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3528 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3473 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5325 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.302736 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1159 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3729 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/config.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.306736 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/
--rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3881 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1369 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.306736 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3988 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5677 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.310736 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3763 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2737 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3796 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5763 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.310736 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11545 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8623 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.310736 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4236 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2819 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3637 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6035 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5468 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/module.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.314736 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/
--rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4259 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3444 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5505 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2629 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.314736 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3718 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1995 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5330 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4187 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.318736 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      646 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.318736 curated-transformers-2.0.0.dev1/curated_transformers/quantization/
--rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.318736 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5987 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/impl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      676 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/quantizable.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.322736 curated-transformers-2.0.0.dev1/curated_transformers/repository/
--rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4362 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/fsspec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11957 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9625 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/repository.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1490 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/transaction.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/semver.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.322736 curated-transformers-2.0.0.dev1/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      588 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.326737 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      933 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5058 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4514 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5152 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_generic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5066 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_logits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2954 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_stop.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.326737 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9040 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7236 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_embeddings.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1821 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      722 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5424 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1961 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2300 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2267 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2229 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3081 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_auto_models.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14286 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.338737 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1639 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.338737 curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3736 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/test_generation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.338737 curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2648 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/test_hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.342737 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.346737 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10775 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10748 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10809 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10557 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.model
--rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3856 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.346737 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30593 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.346737 curated-transformers-2.0.0.dev1/curated_transformers/tests/util/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.350737 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2924 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/_hf_compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4904 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/chunks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)      812 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2325 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/_fairseq.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4508 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7320 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3011 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4255 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2287 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3230 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4017 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13473 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers/util/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/profile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1208 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/pytorch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/checkpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7302 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/load.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7231 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/string.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     9297 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1986 2024-04-08 11:39:52.358737 curated-transformers-2.0.0.dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4606 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.793956 curated-transformers-2.0.0.dev2/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.797956 curated-transformers-2.0.0.dev2/curated_transformers/generation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1346 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3787 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/default_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1962 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4303 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/generator_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1756 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/llama.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6591 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/logits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      631 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/mpt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2794 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/stop_conditions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/string_generator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.797956 curated-transformers-2.0.0.dev2/curated_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4055 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/activations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35234 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10495 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/feedforward.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16063 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.797956 curated-transformers-2.0.0.dev2/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1921 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4593 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4481 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3650 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7766 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/auto_model.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3599 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3582 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5325 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1159 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3729 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/config.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3881 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1369 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9443 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4097 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5677 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/layer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2737 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5763 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12330 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10952 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2819 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3746 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6035 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5468 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/module.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/
+-rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4331 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3553 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5505 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2629 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3789 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2104 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5330 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4187 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      646 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5987 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/impl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      676 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/quantizable.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4362 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/fsspec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11957 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9625 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/repository.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1490 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/transaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/semver.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      588 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      933 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5058 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4514 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5152 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_generic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5066 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_logits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2954 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_stop.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9040 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7236 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_embeddings.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1821 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      722 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5424 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1961 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2300 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2267 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2229 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3081 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_auto_models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14286 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1639 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3736 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/test_generation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2648 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/test_hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10775 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10748 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10809 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10557 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3856 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30593 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2924 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/_hf_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4904 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)      812 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2325 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/_fairseq.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4508 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7320 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3011 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4255 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2287 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3230 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4017 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13473 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/profile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1208 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/pytorch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/checkpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7302 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/load.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7231 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/string.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     9297 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1986 2024-04-10 07:03:40.821957 curated-transformers-2.0.0.dev2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/setup.py
```

### Comparing `curated-transformers-2.0.0.dev1/LICENSE` & `curated-transformers-2.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/PKG-INFO` & `curated-transformers-2.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `curated-transformers-2.0.0.dev1/README.md` & `curated-transformers-2.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/__init__.py` & `curated-transformers-2.0.0.dev2/curated_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/_compat.py` & `curated-transformers-2.0.0.dev2/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/__init__.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/auto_generator.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/default_generator.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/default_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/dolly_v2.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/falcon.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/generator.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/generator_wrapper.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/generator_wrapper.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/hf_hub.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/llama.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/llama.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/logits.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/mpt.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/mpt.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/state.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/state.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/stop_conditions.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/generation/string_generator.py` & `curated-transformers-2.0.0.dev2/curated_transformers/generation/string_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/__init__.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/activations.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/attention.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/cache.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/cache.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/embeddings.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/feedforward.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/normalization.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/layers/transformer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/__init__.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
     config_from_hf,
@@ -78,14 +80,15 @@
         "n_hidden_groups",
         lambda c: HFConfigKeys.conv_n_hidden_groups(c),
     )
 
 
 HF_CONFIG_KEYS: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
     (CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB, None),
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("float32")),
     (CommonHFKeys.EMBEDDING_SIZE, None),
     (CommonHFKeys.HIDDEN_DROPOUT_PROB, None),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (CommonHFKeys.HIDDEN_ACT, None),
     (CommonHFKeys.INTERMEDIATE_SIZE, None),
     (CommonHFKeys.LAYER_NORM_EPS, None),
     (CommonHFKeys.NUM_ATTENTION_HEADS_UNIFORM, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     """
 
     layer: ALBERTLayerConfig
 
     def __init__(
         self,
         *,
+        dtype: torch.dtype = torch.float32,
         embedding_width: int = 128,
         hidden_width: int = 768,
         n_layers_per_group: int = 1,
         intermediate_width: int = 3072,
         n_attention_heads: int = 12,
         n_hidden_layers: int = 12,
         n_hidden_groups: int = 1,
@@ -63,14 +64,16 @@
         n_pieces: int = 30000,
         n_types: int = 2,
         n_positions: int = 512,
         model_max_length: int = 512,
         layer_norm_eps: float = 1e-12,
     ):
         """
+        :param dtype:
+            Data type to use for model parameters.
         :param embedding_width:
             Width of the embedding representations.
         :param hidden_width:
             Width of the transformer hidden layers.
         :param n_layers_per_group:
             Number of layers per layer group.
         :param intermediate_width:
@@ -128,9 +131,9 @@
             ),
             n_hidden_layers=n_hidden_layers,
             layer_norm_eps=layer_norm_eps,
             dropout_prob=hidden_dropout_prob,
             n_layers_per_group=n_layers_per_group,
             n_hidden_groups=n_hidden_groups,
         )
-        self.dtype = torch.float32
+        self.dtype = dtype
         self.model_max_length = model_max_length
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/layer_group.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/auto_model.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/bert/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/bert/_hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
     config_from_hf,
@@ -59,14 +61,15 @@
     StringTransformations.replace(
         "embeddings.LayerNorm.bias", "embeddings.embed_output_layer_norm.bias"
     ),
 ]
 
 HF_CONFIG_KEYS: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
     (CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB, None),
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("float32")),
     (CommonHFKeys.HIDDEN_DROPOUT_PROB, None),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (CommonHFKeys.HIDDEN_ACT, None),
     (CommonHFKeys.INTERMEDIATE_SIZE, None),
     (CommonHFKeys.LAYER_NORM_EPS, None),
     (CommonHFKeys.NUM_ATTENTION_HEADS_UNIFORM, None),
     (CommonHFKeys.NUM_HIDDEN_LAYERS, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/bert/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/bert/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """
 
     model_max_length: int
 
     def __init__(
         self,
         *,
+        dtype: torch.dtype = torch.float32,
         embedding_width: int = 768,
         hidden_width: int = 768,
         intermediate_width: int = 3072,
         n_attention_heads: int = 12,
         n_hidden_layers: int = 12,
         attention_probs_dropout_prob: float = 0.1,
         hidden_dropout_prob: float = 0.1,
@@ -36,14 +37,16 @@
         n_pieces: int = 30000,
         n_types: int = 2,
         n_positions: int = 512,
         model_max_length: int = 512,
         layer_norm_eps: float = 1e-12,
     ):
         """
+        :param dtype:
+            Data type to use for model parameters.
         :param embedding_width:
             Width of the embedding representations.
         :param hidden_width:
             Width of the transformer hidden layers.
         :param intermediate_width:
             Width of the intermediate projection layer in the
             point-wise feed-forward layer.
@@ -95,9 +98,9 @@
                 use_bias=True,
                 use_gate=False,
             ),
             n_hidden_layers=n_hidden_layers,
             layer_norm_eps=layer_norm_eps,
             dropout_prob=hidden_dropout_prob,
         )
-        self.dtype = torch.float32
+        self.dtype = dtype
         self.model_max_length = model_max_length
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/bert/encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/bert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/electra/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/electra/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/electra/encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/electra/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/_hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonCuratedToHFConverters,
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
@@ -144,14 +146,15 @@
 
 
 # Corresponds to the implementation that the Falcon models
 # originally shipped with.
 HF_CONFIG_KEYS_REFINED_WEB_MODEL: List[
     Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]
 ] = [
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("bfloat16")),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (HFConfigKeys.N_HEAD, None),
     (HFConfigKeys.N_HEAD_KV, HFConfigKeyDefault(-1)),
     (HFConfigKeys.MULTI_QUERY, HFConfigKeyDefault(False)),
     (HFConfigKeys.N_LAYER, None),
     (HFConfigKeys.PARALLEL_ATTN, None),
     (HFConfigKeys.BIAS, None),
@@ -161,14 +164,15 @@
     (CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB, HFConfigKeyDefault(0.0)),
     (CommonHFKeys.HIDDEN_DROPOUT_PROB, HFConfigKeyDefault(0.0)),
 ]
 
 # Corresponds to the mainline implementation for Falcon models
 # in the `transformers` library.
 HF_CONFIG_KEYS_FALCON: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("bfloat16")),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (HFConfigKeys.NUM_ATTENTION_HEADS, None),
     (HFConfigKeys.NUM_HEAD_KV, HFConfigKeyDefault(-1)),
     (HFConfigKeys.MULTI_QUERY, HFConfigKeyDefault(False)),
     (CommonHFKeys.NUM_HIDDEN_LAYERS, None),
     (HFConfigKeys.PARALLEL_ATTN, None),
     (HFConfigKeys.BIAS, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     new_decoder_architecture: bool
 
     def __init__(
         self,
         *,
         attention_probs_dropout_prob: float = 0.0,
+        dtype: torch.dtype = torch.bfloat16,
         hidden_dropout_prob: float = 0.0,
         hidden_width: int = 2560,
         layer_norm_eps: float = 1e-5,
         new_decoder_architecture: bool = False,
         n_query_heads: int = 71,
         n_key_value_heads: int = 1,
         n_hidden_layers: int = 32,
@@ -40,14 +41,16 @@
         use_bias: bool = False,
         use_parallel_attention: bool = True,
         n_pieces: int = 50280,
     ):
         """
         :param attention_probs_dropout_prob:
             Dropout to apply after attention.
+        :param dtype:
+            Data type to use for model parameters.
         :param hidden_dropout_prob:
             Dropout to apply to the hidden and embedding layers.
         :param hidden_width:
             Hidden width of the transformer.
         :param layer_norm_eps:
             Epsilon for layer normalization.
         :param n_query_heads:
@@ -105,9 +108,9 @@
                 use_bias=use_bias,
                 use_gate=False,
             ),
             dropout_prob=hidden_dropout_prob,
             layer_norm_eps=layer_norm_eps,
             n_hidden_layers=n_hidden_layers,
         )
-        self.dtype = torch.bfloat16
+        self.dtype = dtype
         self.new_decoder_architecture = new_decoder_architecture
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/layer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/_hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
     config_from_hf,
@@ -58,14 +60,15 @@
         "rotary_pct",
         "rotary_embedding_fraction",
         lambda c: HFConfigKeys.conv_rotary_embedding_fraction(c),
     )
 
 
 HF_CONFIG_KEYS: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("float16")),
     (CommonHFKeys.HIDDEN_ACT, None),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (CommonHFKeys.INTERMEDIATE_SIZE, None),
     (CommonHFKeys.LAYER_NORM_EPS, None),
     (CommonHFKeys.VOCAB_SIZE, None),
     (CommonHFKeys.MAX_POSITION_EMBEDDINGS, None),
     (CommonHFKeys.NUM_HIDDEN_LAYERS, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     """
 
     def __init__(
         self,
         *,
         attention_probs_dropout_prob: float = 0.0,
         activation: Activation = Activation.GELU,
+        dtype: torch.dtype = torch.float16,
         hidden_dropout_prob: float = 0.0,
         hidden_width: int = 2560,
         intermediate_width: int = 10240,
         layer_norm_eps: float = 1e-5,
         n_positions: int = 2048,
         model_max_length: int = 2048,
         n_attention_heads: int = 32,
@@ -39,14 +40,16 @@
         n_pieces: int = 50280,
     ):
         """
         :param attention_probs_dropout_prob:
             Dropout to apply after attention.
         :param activation:
             Activation used by the pointwise feed-forward layers.
+        :param dtype:
+            Data type to use for model parameters.
         :param hidden_dropout_prob:
             Dropout to apply to the hidden and embedding layers.
         :param hidden_width:
             Hidden width of the transformer.
         :param intermediate_width:
             Intermediate width in the feed-forward layer. The non-linearity
             is applied in this intermediate width.
@@ -99,8 +102,8 @@
                 use_bias=True,
                 use_gate=False,
             ),
             dropout_prob=hidden_dropout_prob,
             layer_norm_eps=layer_norm_eps,
             n_hidden_layers=n_hidden_layers,
         )
-        self.dtype = torch.float16
+        self.dtype = dtype
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/conversion.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Union
 
+import torch
 from torch import Tensor
 
 from ...layers import Activation
 from ...util.string import StringTransform
 from ..config import TransformerConfig
 
 
@@ -160,14 +161,18 @@
         return config.layer.attention.dropout_prob
 
     @staticmethod
     def activation(config: TransformerConfig) -> str:
         return config.layer.feedforward.activation.value
 
     @staticmethod
+    def dtype(config: TransformerConfig) -> str:
+        return str(torch.float32).split(".")[1]
+
+    @staticmethod
     def embedding_width(config: TransformerConfig) -> int:
         return config.embedding.embedding_width
 
     @staticmethod
     def hidden_width(config: TransformerConfig) -> int:
         return config.layer.feedforward.hidden_width
 
@@ -196,26 +201,45 @@
         return config.layer.n_hidden_layers
 
     @staticmethod
     def n_positions(config: TransformerConfig) -> Optional[int]:
         return config.embedding.n_positions
 
 
+class CommonHFToCuratedConverters:
+    """
+    Common functions to convert Hugging Face config
+    values to a compatible Curated config format.
+    """
+
+    @staticmethod
+    def dtype(serialized_dtype_str: str) -> Optional[torch.dtype]:
+        serialized_dtype = getattr(torch, serialized_dtype_str, None)
+        if not isinstance(serialized_dtype, torch.dtype):
+            raise ValueError(f"Invalid torch dtype `{serialized_dtype_str}`")
+        return serialized_dtype
+
+
 class CommonHFKeys:
     """
     Common Hugging Face config keys.
     """
 
     ATTENTION_PROBS_DROPOUT_PROB = HFConfigKey(
         "attention_probs_dropout_prob",
         "attention_probs_dropout_prob",
         # Workaround for Python 3.8 limitation that doesn't allow
         # passing/calling static methods as without a class bound.
         lambda c: CommonCuratedToHFConverters.attention_dropout(c),
     )
+    DTYPE = HFConfigKey(
+        "torch_dtype",
+        ("dtype", lambda h: CommonHFToCuratedConverters.dtype(h)),
+        lambda c: CommonCuratedToHFConverters.dtype(c),
+    )
     EMBEDDING_SIZE = HFConfigKey(
         "embedding_size",
         "embedding_width",
         lambda c: CommonCuratedToHFConverters.embedding_width(c),
     )
     HIDDEN_ACT = HFConfigKey(
         "hidden_act",
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/mixin.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -165,14 +165,46 @@
         """
         return cls.from_repo(
             repo=FsspecRepository(fs, model_path, fsspec_args),
             device=device,
             quantization_config=quantization_config,
         )
 
+    def from_fsspec_(
+        self: Self,
+        *,
+        fs: AbstractFileSystem,
+        model_path: str,
+        fsspec_args: Optional[FsspecArgs] = None,
+        device: Optional[torch.device] = None,
+        quantization_config: Optional[BitsAndBytesConfig] = None,
+    ) -> Self:
+        """
+        Load parameters from a fsspec filestytem in-place into the model.
+
+        :param fs:
+            The filesystem to load the model from.
+        :param model_path:
+            The path of the model on the filesystem.
+        :param fsspec_args:
+            Implementation-specific keyword arguments to pass to fsspec
+            filesystem operations.
+        :param device:
+            Device on which the model is initialized.
+        :param quantization_config:
+            Configuration for loading quantized weights.
+        :returns:
+            Module with the parameters loaded.
+        """
+        return self.from_repo_(
+            repo=FsspecRepository(fs, model_path, fsspec_args),
+            device=device,
+            quantization_config=quantization_config,
+        )
+
     @classmethod
     def from_hf_hub(
         cls: Type[Self],
         *,
         name: str,
         revision: str = "main",
         device: Optional[torch.device] = None,
@@ -194,14 +226,42 @@
         """
         return cls.from_repo(
             repo=HfHubRepository(name=name, revision=revision),
             device=device,
             quantization_config=quantization_config,
         )
 
+    def from_hf_hub_(
+        self: Self,
+        *,
+        name: str,
+        revision: str = "main",
+        device: Optional[torch.device] = None,
+        quantization_config: Optional[BitsAndBytesConfig] = None,
+    ) -> Self:
+        """
+        Load parameters from Hugging Face Hub in-place into the model.
+
+        :param name:
+            Model name.
+        :param revision:
+            Model revision.
+        :param device:
+            Device on which the model is initialized.
+        :param quantization_config:
+            Configuration for loading quantized weights.
+        :returns:
+            Module with the parameters loaded.
+        """
+        return self.from_repo_(
+            repo=HfHubRepository(name=name, revision=revision),
+            device=device,
+            quantization_config=quantization_config,
+        )
+
     @classmethod
     @abstractmethod
     def is_supported(cls: Type[Self], config: Dict[str, Any]) -> bool:
         """
         Check if the model with the given configuration is supported by this
         class.
 
@@ -233,41 +293,60 @@
             Loaded model.
         """
         model_repo = ModelRepository(repo)
         config = model_repo.model_config()
         model = cls.from_hf_config(hf_config=config, device=torch.device("meta"))
         assert isinstance(model, Module)
 
+        return model.from_repo_(
+            repo=repo, device=device, quantization_config=quantization_config
+        )
+
+    def from_repo_(
+        self: Self,
+        *,
+        repo: Repository,
+        device: Optional[torch.device] = None,
+        quantization_config: Optional[BitsAndBytesConfig] = None,
+    ) -> Self:
+        """
+        Load parameters from a repository in-place into the model.
+
+        :param repository:
+            The repository to load from.
+        :param device:
+            Device on which to initialize the model.
+        :param quantization_config:
+            Configuration for loading quantized weights.
+        :returns:
+            Loaded model.
+        """
+        model_repo = ModelRepository(repo)
+
         # Convert the model to the expected dtype.
-        assert isinstance(model, TransformerModule)
-        dtype: torch.dtype = model.config.dtype
-        serialized_dtype_str = config.get("torch_dtype")
-        if serialized_dtype_str is not None:
-            serialized_dtype = getattr(torch, serialized_dtype_str, None)
-            if not isinstance(serialized_dtype, torch.dtype):
-                raise ValueError(f"Invalid torch dtype `{serialized_dtype_str}`")
-            dtype = serialized_dtype
-        model.to(dtype=dtype)
+        assert isinstance(self, TransformerModule)
+        dtype: torch.dtype = self.config.dtype
+        self.to(dtype=dtype)
 
         # Prepare for quantization.
         if quantization_config is not None:
-            tensor2param = prepare_module_for_quantization(model, quantization_config)  # type: ignore
+            tensor2param = prepare_module_for_quantization(self, quantization_config)  # type: ignore
         else:
             tensor2param = None
 
         # Download model and convert HF parameter names to ours.
         checkpoint_filenames, checkpoint_type = model_repo.model_checkpoints()
         load_model_from_checkpoints(
-            model,  # type:ignore
+            self,  # type:ignore
             filepaths=checkpoint_filenames,
             checkpoint_type=checkpoint_type,
-            state_dict_converter=cls.convert_hf_state_dict,
+            state_dict_converter=type(self).convert_hf_state_dict,
             tensor_to_param_converter=tensor2param,
             device=device,
         )
 
         # Ensure that any non-persistent buffers are also moved to
         # the correct device.
         if device is not None:
-            model.to(device)
+            self.to(device)
 
-        return model
+        return self
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonCuratedToHFConverters,
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
@@ -73,14 +75,15 @@
         "num_key_value_heads",
         "n_key_value_heads",
         lambda c: HFConfigKeys.conv_n_attention_keyvalue_heads(c),
     )
 
 
 HF_CONFIG_KEYS: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("float16")),
     (CommonHFKeys.HIDDEN_ACT, None),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (CommonHFKeys.INTERMEDIATE_SIZE, None),
     (CommonHFKeys.VOCAB_SIZE, None),
     (CommonHFKeys.NUM_HIDDEN_LAYERS, None),
     (HFConfigKeys.NUM_ATTENTION_HEADS, None),
     (HFConfigKeys.RMS_NORM_EPS, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     """
 
     def __init__(
         self,
         *,
         attention_probs_dropout_prob: float = 0.0,
         activation: Activation = Activation.GELU,
+        dtype: torch.dtype = torch.float16,
         hidden_dropout_prob: float = 0.0,
         hidden_width: int = 2560,
         intermediate_width: int = 10240,
         rms_norm_eps: float = 1e-5,
         n_query_heads: int = 32,
         n_hidden_layers: int = 32,
         n_key_value_heads: int = 32,
@@ -39,14 +40,16 @@
         n_pieces: int = 50280,
     ):
         """
         :param attention_probs_dropout_prob:
             Dropout to apply after attention.
         :param activation:
             Activation used by the pointwise feed-forward layers.
+        :param dtype:
+            Data type to use for model parameters.
         :param hidden_dropout_prob:
             Dropout to apply to the hidden and embedding layers.
         :param hidden_width:
             Hidden width of the transformer.
         :param intermediate_width:
             Intermediate width in the feed-forward layer.
             The non-linearity is applied in this intermediate width.
@@ -96,8 +99,8 @@
                 use_bias=False,
                 use_gate=True,
             ),
             dropout_prob=hidden_dropout_prob,
             layer_norm_eps=rms_norm_eps,
             n_hidden_layers=n_hidden_layers,
         )
-        self.dtype = torch.float16
+        self.dtype = dtype
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/module.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/module.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonCuratedToHFConverters,
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
@@ -90,14 +92,15 @@
         "layer_norm_epsilon",
         "layer_norm_eps",
         lambda c: CommonCuratedToHFConverters.layer_norm_eps(c),
     )
 
 
 HF_CONFIG_KEYS: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("bfloat16")),
     (HFConfigKeys.D_MODEL, None),
     (HFConfigKeys.EXPANSION_RATIO, None),
     (HFConfigKeys.MAX_SEQ_LEN, None),
     (HFConfigKeys.N_LAYERS, None),
     (HFConfigKeys.N_HEADS, None),
     (HFConfigKeys.NO_BIAS, None),
     (CommonHFKeys.VOCAB_SIZE, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """
 
     def __init__(
         self,
         *,
         attention_probs_dropout_prob: float = 0.0,
         activation: Activation = Activation.GELU,
+        dtype: torch.dtype = torch.bfloat16,
         hidden_dropout_prob: float = 0.0,
         hidden_width: int = 4096,
         intermediate_width_multiplier: int = 4,
         layer_norm_eps: float = 1e-5,
         model_max_length: int = 2048,
         n_attention_heads: int = 32,
         n_hidden_layers: int = 32,
@@ -36,14 +37,16 @@
         use_bias=False
     ):
         """
         :param attention_probs_dropout_prob:
             Dropout to apply after attention.
         :param activation:
             Activation used by the pointwise feed-forward layers.
+        :param dtype:
+            Data type to use for model parameters.
         :param hidden_dropout_prob:
             Dropout to apply to the hidden and embedding layers.
         :param hidden_width:
             Hidden width of the transformer.
         :param intermediate_width_multiplier:
             Multiplier for the intermediate width. The hidden width is
             multiplied by this value to get the intermediate width.
@@ -90,9 +93,9 @@
                 use_bias=use_bias,
                 use_gate=False,
             ),
             dropout_prob=hidden_dropout_prob,
             layer_norm_eps=layer_norm_eps,
             n_hidden_layers=n_hidden_layers,
         )
-        self.dtype = torch.bfloat16
+        self.dtype = dtype
         self.model_max_length = model_max_length
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/output.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/_hf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
+import torch
+
 from ...util.string import StringTransform, StringTransformations
 from ..hf_hub.conversion import (
     CommonHFKeys,
     HFConfigKey,
     HFConfigKeyDefault,
     HFSpecificConfig,
     config_from_hf,
@@ -69,14 +71,15 @@
         "padding_id",
         lambda c: HFConfigKeys.conv_padding_id(c),
     )
 
 
 HF_CONFIG_KEYS: List[Tuple[HFConfigKey, Optional[HFConfigKeyDefault]]] = [
     (CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB, None),
+    (CommonHFKeys.DTYPE, HFConfigKeyDefault("float32")),
     (CommonHFKeys.HIDDEN_DROPOUT_PROB, None),
     (CommonHFKeys.HIDDEN_SIZE, None),
     (CommonHFKeys.HIDDEN_ACT, None),
     (CommonHFKeys.INTERMEDIATE_SIZE, None),
     (CommonHFKeys.LAYER_NORM_EPS, None),
     (CommonHFKeys.NUM_ATTENTION_HEADS_UNIFORM, None),
     (CommonHFKeys.NUM_HIDDEN_LAYERS, None),
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 
     .. _Liu et al., 2019: https://arxiv.org/abs/1907.11692
     """
 
     def __init__(
         self,
         *args,
+        dtype: torch.dtype = torch.float32,
         layer_norm_eps=1e-05,
         n_positions=514,
         padding_id=1,
         n_types=1,
         n_pieces=50265,
         **kwargs
     ):
         """
+        :param dtype:
+            Data type to use for model parameters.
         :param embedding_width:
             Width of the embedding representations.
         :param hidden_width:
             Width of the transformer hidden layers.
         :param intermediate_width:
             Width of the intermediate projection layer in the
             point-wise feed-forward layer.
@@ -59,9 +62,9 @@
             *args,
             layer_norm_eps=layer_norm_eps,
             n_positions=n_positions,
             n_types=n_types,
             n_pieces=n_pieces,
             **kwargs
         )
-        self.dtype = torch.float32
+        self.dtype = dtype
         self.padding_id = padding_id
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/embeddings.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/transformer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/config.py` & `curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/impl.py` & `curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/impl.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/quantization/helpers.py` & `curated-transformers-2.0.0.dev2/curated_transformers/quantization/helpers.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/quantization/quantizable.py` & `curated-transformers-2.0.0.dev2/curated_transformers/quantization/quantizable.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/__init__.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/_hf.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/file.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/file.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/fsspec.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/fsspec.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/hf_hub.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/repository.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/repository.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/repository/transaction.py` & `curated-transformers-2.0.0.dev2/curated_transformers/repository/transaction.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/semver.py` & `curated-transformers-2.0.0.dev2/curated_transformers/semver.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/compat.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/conftest.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_auto_generator.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_dolly_v2.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_falcon.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_generic.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_generic.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_logits.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_stop.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_stop.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_attention.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_embeddings.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/test_encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/test_encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/test_encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/test_encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/test_decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_causal_lm.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_decoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/test_encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_auto_models.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_auto_models.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_hf_hub.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/util.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/test_encoder.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/test_generation.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/test_generation.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/test_hf_hub.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-merges.txt` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-vocab.json` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.model` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.wordpieces` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_auto_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_chunks.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_hf_hub.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/util.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/_hf_compat.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/_hf_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/auto_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/chunks.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/hf_hub.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/__init__.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/_fairseq.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/_fairseq.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bert_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/camembert_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/legacy_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/legacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/llama_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/roberta_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/tokenizer.py` & `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/util/profile.py` & `curated-transformers-2.0.0.dev2/curated_transformers/util/profile.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/util/pytorch.py` & `curated-transformers-2.0.0.dev2/curated_transformers/util/pytorch.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/util/serde/checkpoint.py` & `curated-transformers-2.0.0.dev2/curated_transformers/util/serde/checkpoint.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/util/serde/load.py` & `curated-transformers-2.0.0.dev2/curated_transformers/util/serde/load.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers/util/string.py` & `curated-transformers-2.0.0.dev2/curated_transformers/util/string.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-2.0.0.dev2/curated_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-2.0.0.dev2/curated_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/curated_transformers.egg-info/entry_points.txt` & `curated-transformers-2.0.0.dev2/curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev1/setup.cfg` & `curated-transformers-2.0.0.dev2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.0.0.dev1
+version = 2.0.0.dev2
 description = A PyTorch library of transformer models and components
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
```

