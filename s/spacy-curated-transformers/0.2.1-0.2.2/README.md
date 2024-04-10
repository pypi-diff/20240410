# Comparing `tmp/spacy-curated-transformers-0.2.1.tar.gz` & `tmp/spacy-curated-transformers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-curated-transformers-0.2.1.tar", last modified: Tue Nov 28 12:23:22 2023, max compression
+gzip compressed data, was "spacy-curated-transformers-0.2.2.tar", last modified: Fri Jan 26 08:49:22 2024, max compression
```

## Comparing `spacy-curated-transformers-0.2.1.tar` & `spacy-curated-transformers-0.2.2.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.771933 spacy-curated-transformers-0.2.1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2728 2023-11-28 12:23:22.771933 spacy-curated-transformers-0.2.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     4318 2023-11-28 12:23:22.771933 spacy-curated-transformers-0.2.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      210 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.763933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      570 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.763933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4113 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17845 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/cli/fill_config_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3188 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.763933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27328 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1226 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24366 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2704 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4016 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/pooling.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2193 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4670 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2665 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7876 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10280 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.767933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17737 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.767933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2341 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)       45 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.767933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3394 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2653 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4556 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1425 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6177 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3195 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4326 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.767933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23987 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2703 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (127)     9822 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2514 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)      794 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.771933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3411 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4116 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2716 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7953 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4908 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      138 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     4690 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    14493 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (127)   253270 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (127)     4968 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (127)      906 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.771933 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (127)      568 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3602 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3714 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5380 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2483 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3813 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5880 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2742 2023-11-28 12:23:11.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-28 12:23:22.771933 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2728 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3509 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     3518 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-28 12:23:22.000000 spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.655189 spacy-curated-transformers-0.2.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2728 2024-01-26 08:49:22.655189 spacy-curated-transformers-0.2.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     4318 2024-01-26 08:49:22.655189 spacy-curated-transformers-0.2.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.643188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      570 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.647188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4113 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17845 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/cli/fill_config_transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.647188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27430 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1233 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25092 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4016 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2384 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4845 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7876 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10513 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.647188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17826 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/pipeline/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.651188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2341 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       45 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.651188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3394 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2653 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4556 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6177 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3195 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4326 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.651188 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26066 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2703 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (127)     9822 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2514 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      794 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.655189 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3411 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4116 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2716 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7953 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4908 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      138 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.655189 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (127)      568 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3736 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6020 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3813 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5880 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3036 2024-01-26 08:49:07.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-26 08:49:22.655189 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2728 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3472 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     3518 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-26 08:49:22.000000 spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/zip-safe
```

### Comparing `spacy-curated-transformers-0.2.1/LICENSE` & `spacy-curated-transformers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/PKG-INFO` & `spacy-curated-transformers-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Curated transformer models for spaCy pipelines
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curated-transformers<0.2.0,>=0.1.0
-Requires-Dist: curated-tokenizers<0.1.0,>=0.0.7
+Requires-Dist: curated-tokenizers<0.1.0,>=0.0.9
 Requires-Dist: spacy<4.0.0,>=3.7.0.dev0
 Requires-Dist: torch>=1.12.0
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # 💫 🤖 spaCy Curated Transformers
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 0.2.2 Summary:
 Curated transformer models for spaCy pipelines Home-page: https://github.com/
 explosion/spacy-curated-transformers Author: Explosion Author-email:
 contact@explosion.ai License: MIT Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: curated-
-transformers<0.2.0,>=0.1.0 Requires-Dist: curated-tokenizers<0.1.0,>=0.0.7
+transformers<0.2.0,>=0.1.0 Requires-Dist: curated-tokenizers<0.1.0,>=0.0.9
 Requires-Dist: spacy<4.0.0,>=3.7.0.dev0 Requires-Dist: torch>=1.12.0 _[_h_t_t_p_s_:_/_/
 _e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# ð« ð¤ spaCy Curated Transformers This
 package provides [spaCy](https://github.com/explosion/spaCy) components and
 architectures to use a curated set of transformer models via [`curated-
 transformers`](https://github.com/explosion/curated-transformers) in spaCy. [!
 [PyPi](https://img.shields.io/pypi/v/spacy-curated-transformers.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-curated-
```

### Comparing `spacy-curated-transformers-0.2.1/README.md` & `spacy-curated-transformers-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/setup.cfg` & `spacy-curated-transformers-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.2.1
+version = 0.2.2
 description = Curated transformer models for spaCy pipelines
 url = https://github.com/explosion/spacy-curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
@@ -11,15 +11,15 @@
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	curated-transformers>=0.1.0,<0.2.0
-	curated-tokenizers>=0.0.7,<0.1.0
+	curated-tokenizers>=0.0.9,<0.1.0
 	spacy>=3.7.0.dev0,<4.0.0
 	torch>=1.12.0
 
 [options.entry_points]
 spacy_factories = 
 	curated_transformer = spacy_curated_transformers.pipeline.transformer:make_transformer
 spacy_architectures =
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/_compat.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/cli/debug_pieces.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/cli/debug_pieces.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/cli/fill_config_transformer.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/cli/fill_config_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/architectures.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/architectures.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     xp2torch,
 )
 from thinc.layers import chain
 from thinc.model import Model
 from thinc.shims.pytorch_grad_scaler import PyTorchGradScaler
 from thinc.types import ArgsKwargs, Floats2d, Ints1d
 
-from ..errors import Errors
 from ..tokenization.types import Tok2PiecesModelT
 from .listeners import (
     WrappedTransformerAndListener,
     replace_listener_callback,
     replace_listener_cfg_callback,
 )
 from .output import TransformerModelOutput
@@ -720,15 +719,17 @@
     max_model_seq_len: int,
     padding_idx: int,
 ) -> Tuple[ArgsKwargs, Callable[[Any], List[Ints1d]]]:
     ops = model.ops
     max_seq_len = max(x.size for x in X)
     if max_seq_len > max_model_seq_len:
         raise ValueError(
-            Errors.E009.format(seq_len=max_seq_len, max_seq_len=max_model_seq_len)
+            "At least one sequence in the transformer's input has a length "
+            f"of {max_seq_len}, which is larger than the model's maximum sequence "
+            f"length of {max_model_seq_len} tokens"
         )
 
     # Transform the list of strided spans to a padded array.
     Xt = ops.xp.full((len(X), max_seq_len), padding_idx)
     for i in range(len(X)):
         span = X[i]
         span_len = span.shape[0]
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/hf_loader.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/hf_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Callable, List, Optional
 
 from curated_transformers.models.hf_util import convert_hf_pretrained_model_parameters
 from spacy.tokens import Doc
 
 from .._compat import has_hf_transformers, transformers
-from ..errors import Errors
 from .types import TorchTransformerModelT
 
 
 def build_hf_transformer_encoder_loader_v1(
     *,
     name: str,
     revision: str = "main",
@@ -24,15 +23,15 @@
     revision (str):
         Name of the model revision/branch.
     """
 
     def load(model, X=None, Y=None):
         if not has_hf_transformers:
             raise ValueError(
-                Errors.E011.format(loader_name="HFTransformerEncoderLoader")
+                "`HFTransformerEncoderLoader` requires the Hugging Face `transformers` package to be installed"
             )
 
         encoder = model.shims[0]._model
 
         hf_model = transformers.AutoModel.from_pretrained(name, revision=revision)
         params = convert_hf_pretrained_model_parameters(hf_model)
         encoder.load_state_dict(params)
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/listeners.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/listeners.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Callable, Iterable, List, Optional, Tuple
 
 from spacy import Errors as SpacyErrors
 from spacy.tokens import Doc
 from thinc.api import Model, deserialize_attr, serialize_attr
 from thinc.types import Floats2d, Ragged
 
-from ..errors import Errors
 from .output import TransformerModelOutput
 from .pooling import with_ragged_last_layer, with_ragged_layers
 from .types import (
     PoolingModelT,
     ScalarWeightModelT,
     ScalarWeightOutT,
     TransformerListenerModelT,
@@ -318,17 +317,20 @@
 
     _outputs = ListenerStateUtils.get_output(model)
     _backprop = ListenerStateUtils.get_backprop(model)
 
     if is_train:
         assert _outputs is not None
         if _outputs.last_layer_only:
-            raise ValueError(
-                Errors.E012.format(listener_name="TransformerLayersListener")
-            )
+            raise ValueError
+        (
+            "`TransformerLayersListener` requires the upstream transformer pipe to output "
+            "all hidden layer outputs. This can be enabled by setting the pipe's "
+            "`all_layer_outputs` parameter to `True` in the pipeline config"
+        )
 
         ListenerStateUtils.verify_inputs(model, docs)
 
         Y, backprop_pooling = pooling(_outputs.all_outputs, is_train)
 
         def backprop(dY):
             dX = backprop_pooling(dY)
@@ -356,15 +358,17 @@
                 return [
                     [model.ops.alloc2f(len(doc), width) for _ in range(n_layers)]
                     for doc in docs
                 ], lambda dY: []
 
             if any(doc._.trf_data.last_layer_only for doc in docs):
                 raise ValueError(
-                    Errors.E012.format(listener_name="TransformerLayersListener")
+                    "`TransformerLayersListener` requires the upstream transformer pipe to output "
+                    "all hidden layer outputs. This can be enabled by setting the pipe's "
+                    "`all_layer_outputs` parameter to `True` in the pipeline config"
                 )
 
             return pooling.predict(docs), lambda dY: []
         else:
             assert _outputs is not None
             ListenerStateUtils.verify_inputs(model, docs)
             outputs: Tuple[List[List[Floats2d]], Callable[[Any], Any]] = (
@@ -434,16 +438,19 @@
     _outputs = ListenerStateUtils.get_output(model)
     _backprop = ListenerStateUtils.get_backprop(model)
 
     if is_train:
         assert _outputs is not None
         if _outputs.last_layer_only:
             raise ValueError(
-                Errors.E012.format(listener_name="ScalarWeightingListener")
+                "`ScalarWeightingListener` requires the upstream transformer pipe to output "
+                "all hidden layer outputs. This can be enabled by setting the pipe's "
+                "`all_layer_outputs` parameter to `True` in the pipeline config"
             )
+
         ListenerStateUtils.verify_inputs(model, docs)
 
         Y_weighting: ScalarWeightOutT = []
         weighting_inputs = _outputs.all_outputs
         outputs_to_backprop = tuple(i for i in range(_outputs.num_outputs))
 
         Y_weighting, backprop_weighting = weighting(weighting_inputs, is_train)
@@ -472,15 +479,17 @@
                 assert all(no_trf_data)
                 return [
                     model.ops.alloc2f(len(doc), width) for doc in docs
                 ], lambda dY: []
 
             if any(doc._.trf_data.last_layer_only for doc in docs):
                 raise ValueError(
-                    Errors.E012.format(listener_name="ScalarWeightingListener")
+                    "`ScalarWeightingListener` requires the upstream transformer pipe to output "
+                    "all hidden layer outputs. This can be enabled by setting the pipe's "
+                    "`all_layer_outputs` parameter to `True` in the pipeline config"
                 )
 
             Y_weighting = weighting.predict(
                 [doc._.trf_data.all_outputs for doc in docs]
             )
             Y = pooling.predict(Y_weighting)
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/output.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/output.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from dataclasses import dataclass
-from typing import Generic, List, Optional, TypeVar
+from typing import Any, Dict, Generic, List, Optional, TypeVar
 
-import torch
+import srsly
 from thinc.types import Floats2d, Ragged
-from torch import Tensor
-
-from ..errors import Errors
 
 TrfOutputT = TypeVar("TrfOutputT", Floats2d, Ragged)
 
 
 @dataclass
 class TransformerModelOutput(Generic[TrfOutputT]):
     """Wrapper for PyTorchTransformerOutput consumed by downstream non-PyTorch components.
@@ -82,7 +79,38 @@
     @property
     def all_hidden_layer_states(self) -> List[Ragged]:
         return self.all_outputs[1:]
 
     @property
     def num_outputs(self) -> int:
         return len(self.all_outputs)
+
+    def from_dict(self, msg: Dict[str, Any]) -> "DocTransformerOutput":
+        self.all_outputs = [
+            Ragged(dataXd, lengths) for (dataXd, lengths) in msg["all_outputs"]
+        ]
+        self.last_layer_only = msg["last_layer_only"]
+        return self
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            "all_outputs": [
+                (layer.dataXd, layer.lengths) for layer in self.all_outputs
+            ],
+            "last_layer_only": self.last_layer_only,
+        }
+
+
+@srsly.msgpack_encoders("doc_transformer_output")
+def serialize_transformer_data(obj: DocTransformerOutput, chain=None):
+    if isinstance(obj, DocTransformerOutput):
+        return {"__doc_transformer_output__": obj.to_dict()}
+    return obj if chain is None else chain(obj)
+
+
+@srsly.msgpack_decoders("doc_transformer_output")
+def deserialize_transformer_data(obj, chain=None):
+    if "__doc_transformer_output__" in obj:
+        return DocTransformerOutput(all_outputs=[], last_layer_only=False).from_dict(
+            obj["__doc_transformer_output__"]
+        )
+    return obj if chain is None else chain(obj)
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/pooling.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/remove_eos_bos.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/remove_eos_bos.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Tuple, cast
 
 from thinc.api import Model, Ragged
 
-from ..errors import Errors
 from .output import TransformerModelOutput
 from .types import (
     RaggedInOutT,
     SentMarkerRemoverBackpropT,
     SentMarkerRemoverInOutT,
     SentMarkerRemoverModelT,
 )
@@ -17,15 +16,19 @@
     return Model("remove_bos_eos", remove_bos_eos_forward)
 
 
 def remove_bos_eos_forward(
     model: Model, X: SentMarkerRemoverInOutT, is_train: bool
 ) -> Tuple[SentMarkerRemoverInOutT, SentMarkerRemoverBackpropT]:
     if not isinstance(X, TransformerModelOutput):
-        raise ValueError(Errors.E014.format(model_name=model.name, input_type=type(X)))
+        raise ValueError(
+            f"Model '{model.name}' received an unexpected input of type '{type(X)}'. "
+            "It can only wrap/be chained with models whose outputs are of type  "
+            "`TransformerModelOutput` (in almost all cases, models of type `TorchTransformerModelT`)"
+        )
 
     X.all_outputs = [[Xr[1:-1] for Xr in inner] for inner in X.all_outputs]
 
     def backprop(dY: RaggedInOutT) -> RaggedInOutT:
         # Pass-through dY, but add zero gradient for the special bos/eos
         # tokens.
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/scalar_weight.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/scalar_weight.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from thinc.layers.pytorchwrapper import PyTorchWrapper_v2
 from thinc.model import Model
 from thinc.shims.pytorch_grad_scaler import PyTorchGradScaler
 from thinc.types import ArgsKwargs, Ragged
 from thinc.util import torch2xp, xp2torch
 from torch import Tensor
 
-from ..errors import Errors
 from ..util import all_equal
 from .types import ScalarWeightInT, ScalarWeightModelT, ScalarWeightOutT
 
 
 def build_scalar_weight_v1(
     *,
     num_layers: int,
@@ -62,18 +61,24 @@
     ops = model.ops
 
     batch_size = len(X)
     seq_lens = [x[0].data.shape[0] for x in X]
     max_seq_len = max(seq_lens)
     num_layers = [len(x) for x in X]
     if not all_equal(num_layers):
-        raise ValueError(Errors.E015.format(layer_counts=set(num_layers)))
+        raise ValueError(
+            "Input passed to the `ScalarWeight` model do not have the same number "
+            f"layers. Distinct layer counts: {set(num_layers)}"
+        )
     layer_widths = [layer.data.shape[1] for x in X for layer in x]
     if not all_equal(layer_widths):
-        raise ValueError(Errors.E016.format(hidden_widths=set(layer_widths)))
+        raise ValueError(
+            "Input passed to the `ScalarWeight` model do not have the same width. "
+            f"Distinct widths: {set(layer_widths)}"
+        )
 
     # [batch_size, max_seq_len, num_layers, layer_width]
     Xops = ops.alloc4f(batch_size, max_seq_len, num_layers[0], layer_widths[0])
     for doc_idx, layers in enumerate(X):
         seq_len = seq_lens[doc_idx]
         for layer_idx, data in enumerate(layers):
             Xops[doc_idx, :seq_len, layer_idx, :] = data.dataXd  # type: ignore
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/types.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/with_non_ws_tokens.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/models/with_strided_spans.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/models/with_strided_spans.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial
 from typing import Any, Callable, Iterable, List, Optional, Tuple, Union, cast
 
 from thinc.model import Model
 from thinc.types import Floats2d, Ints1d, Ragged
 
-from ..errors import Errors
 from .output import TransformerModelOutput
 from .types import (
     Floats2dInOutT,
     RaggedInOutT,
     SpanExtractorBackpropT,
     SpanExtractorInT,
     SpanExtractorModelT,
@@ -43,20 +42,20 @@
     *,
     stride: int = 96,
     window: int = 128,
     batch_size: int = 384,
 ) -> Model[List[Ragged], TransformerModelOutput]:
     if not (window // 2 <= stride <= window):
         raise ValueError(
-            Errors.E017.format(
-                stride=stride, half_window_size=window // 2, window_size=window
-            )
+            f"Span extractor stride ({stride}) must be within [window_size / 2, "
+            f"window_size] ([{window // 2}, {window}])"
         )
+
     if batch_size <= 0:
-        raise ValueError(Errors.E018)
+        raise ValueError("Span extractor batch size must be greater than zero")
 
     attrs = {
         "stride": stride,
         "window": window,
         "batch_size": batch_size,
     }
     return Model(
@@ -105,16 +104,19 @@
 
     backprops = []
     outputs = []
     for batch in _split_spans(spans, batch_size):
         output, bp = transformer(cast(TorchTransformerInT, batch), is_train=is_train)
         if not isinstance(output, TransformerModelOutput):
             raise ValueError(
-                Errors.E014.format(model_name=model.name, input_type=type(output))
+                f"Model '{model.name}' received an unexpected input of type '{type(output)}'. "
+                "It can only wrap/be chained with models whose outputs are of type  "
+                "`TransformerModelOutput` (in almost all cases, models of type `TorchTransformerModelT`)"
             )
+
         outputs.append(output)
         backprops.append(bp)
 
     trf_output = _unsplit_outputs(outputs)
 
     # Suppose we have:
     #
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/pipeline/transformer.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/pipeline/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from spacy.tokens import Doc
 from spacy.training import Example, validate_examples, validate_get_examples
 from spacy.util import minibatch
 from thinc.api import Config, Optimizer, set_dropout_rate
 from thinc.model import Model
 from thinc.types import Ragged
 
-from ..errors import Errors
 from ..models.listeners import ListenerStateUtils
 from ..models.output import DocTransformerOutput, TransformerModelOutput
 from ..models.types import TransformerListenerModelT
 
 DEFAULT_CONFIG_STR = """
     [transformer]
 
@@ -146,15 +145,18 @@
         return list(self.listener_map.keys())
 
     def add_listener(
         self, listener: TransformerListenerModelT, component_name: str
     ) -> None:
         """Add a listener for a downstream component. Usually internals."""
         if not ListenerStateUtils.is_listener(listener):
-            raise ValueError(Errors.E026.format(model_name=listener.name))
+            raise ValueError(
+                f"Attempting to register a model ('{listener.name}') with the transformer pipe"
+                "that isn't a transformer listener"
+            )
 
         self.listener_map.setdefault(component_name, [])
         if listener not in self.listener_map[component_name]:
             self.listener_map[component_name].append(listener)
 
     def remove_listener(
         self, listener: TransformerListenerModelT, component_name: str
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/conftest.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_hf_model.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_listeners.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_pooling.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_scalar_weight.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_transformer_model.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/models/test_with_strided_spans.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/pipeline/test_transformer.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/pipeline/test_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import multiprocessing
 from functools import partial
 from typing import Any, Dict
 
 import numpy
 import pytest
 import spacy
 import torch
 from spacy import Config, util
 from spacy.language import Language
+from spacy.tokens import Doc
 from spacy.training import Example
 from spacy.training.initialize import init_nlp
 from spacy.training.loop import train
 from spacy.util import registry as spacy_registry
+from thinc.api import CupyOps, get_current_ops
+from thinc.backends import get_array_ops
 from thinc.model import Model
 
 from spacy_curated_transformers._compat import has_hf_transformers, transformers
 from spacy_curated_transformers.models.architectures import (
     build_bert_transformer_model_v1,
     build_camembert_transformer_model_v1,
     build_roberta_transformer_model_v1,
@@ -45,14 +49,18 @@
 from spacy_curated_transformers.tokenization.sentencepiece_encoder import (
     build_sentencepiece_encoder_loader_v1,
 )
 from spacy_curated_transformers.util import create_gradual_transformer_unfreezing
 
 from ..util import make_tempdir, torch_assertclose, xp_assert_array_equal
 
+# Torch currently interacts badly with the fork method:
+# https://github.com/pytorch/pytorch/issues/17199
+multiprocessing.set_start_method("spawn")
+
 cfg_string_last_layer_listener = """
     # LastTransformerLayerListener
 
     [nlp]
     lang = "en"
     pipeline = ["transformer","tagger"]
 
@@ -149,26 +157,39 @@
     (
         "Eat blue ham",
         {"tags": ["V", "J", "N"], "cats": {"preference": 0.0, "imperative": 1.0}},
     ),
 ]
 
 
-def create_and_train_tagger(cfg_string):
+def create_tagger(cfg_string):
     config = Config().from_str(cfg_string)
     nlp = util.load_model_from_config(config, auto_fill=True, validate=True)
+
     tagger = nlp.get_pipe("tagger")
 
     train_examples = []
     for t in TRAIN_DATA:
         train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
         for tag in t[1]["tags"]:
             tagger.add_label(tag)
 
-    optimizer = nlp.initialize(lambda: train_examples)
+    nlp.initialize(lambda: train_examples)
+
+    return nlp
+
+
+def create_and_train_tagger(cfg_string):
+    nlp = create_tagger(cfg_string)
+
+    train_examples = []
+    for t in TRAIN_DATA:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    optimizer = nlp.create_optimizer()
 
     for _ in range(10):
         losses = {}
         nlp.update(train_examples, sgd=optimizer, losses=losses)
 
     return nlp
 
@@ -191,14 +212,30 @@
     [cfg_string_last_layer_listener, cfg_string_scalar_weighting_layer_listener],
 )
 def test_tagger(cfg_string):
     model = create_and_train_tagger(cfg_string)
     evaluate_tagger_on_train_data(model)
 
 
+@pytest.mark.slow
+@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
+@pytest.mark.parametrize(
+    "cfg_string",
+    [cfg_string_last_layer_listener, cfg_string_scalar_weighting_layer_listener],
+)
+@pytest.mark.skipif(
+    isinstance(get_current_ops(), CupyOps),
+    reason="multiprocessing and GPU support are incompatible",
+)
+def test_tagger_multiprocessing(cfg_string):
+    model = create_tagger(cfg_string)
+    for _ in model.pipe(["This is a test..."] * 100, n_process=2):
+        pass
+
+
 def _hf_tokenize_per_token(tokenizer, docs, *, roberta=False):
     if roberta:
         hf_encoding = [
             tokenizer(
                 [
                     doc[idx - 1].whitespace_ + token.text if idx > 0 else token.text
                     for idx, token in enumerate(doc)
@@ -474,19 +511,29 @@
         nlp.make_doc("I saw a girl with a telescope."),
         nlp.make_doc("Today we will eat poké bowl."),
     ]
     docs = list(pipe.pipe(docs))
     assert all([doc._.trf_data.last_layer_only for doc in docs]) == True
     assert all([len(doc._.trf_data.all_outputs) == 1 for doc in docs]) == True
 
+    serialized = [doc.to_bytes() for doc in docs]
+    deserialized = [Doc(nlp.vocab).from_bytes(doc_bytes) for doc_bytes in serialized]
+    for doc, doc_deserialized in zip(docs, deserialized):
+        _assert_doc_model_output_equal(doc, doc_deserialized)
+
     pipe = make_transformer(nlp, "transformer", model, all_layer_outputs=True)
     docs = list(pipe.pipe(docs))
     assert all([not doc._.trf_data.last_layer_only for doc in docs]) == True
     assert all([len(doc._.trf_data.all_outputs) == 12 + 1 for doc in docs]) == True
 
+    serialized = [doc.to_bytes() for doc in docs]
+    deserialized = [Doc(nlp.vocab).from_bytes(doc_bytes) for doc_bytes in serialized]
+    for doc, doc_deserialized in zip(docs, deserialized):
+        _assert_doc_model_output_equal(doc, doc_deserialized)
+
 
 cfg_string_gradual_unfreezing = (
     cfg_string_last_layer_listener
     + """
     [corpora]
 
     [corpora.train]
@@ -713,7 +760,20 @@
     )
     assert (
         nlp.config["components"]["curated_transformer"]["model"]["with_spans"][
             "@architectures"
         ]
         == DEFAULT_CONFIG["transformer"]["model"]["with_spans"]["@architectures"]
     )
+
+
+def _assert_doc_model_output_equal(doc1: Doc, doc2: Doc):
+    output1 = doc1._.trf_data
+    output2 = doc2._.trf_data
+
+    assert output1.last_layer_only == output2.last_layer_only
+    assert len(output1.all_outputs) == len(output2.all_outputs)
+
+    for layer1, layer2 in zip(output1.all_outputs, output2.all_outputs):
+        ops = get_array_ops(layer1.dataXd)
+        ops.xp.testing.assert_allclose(layer1.dataXd, layer2.dataXd)
+        ops.xp.testing.assert_array_equal(layer1.lengths, layer2.lengths)
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/test_cli_app.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/test_cli_app.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/test_registry.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/test_torchscript_wrapper.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy-merges.txt` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy-vocab.json` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy.model` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy.model`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/tokenization/toy.wordpieces` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/tokenization/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tests/util.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tests/util.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/__init__.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/bbpe_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/bbpe_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pathlib import Path
 from typing import Callable, Optional, Tuple
 
 import srsly
 from curated_tokenizers import ByteBPEProcessor
 from thinc.api import Model, Ragged, deserialize_attr, serialize_attr
 
-from ..errors import Errors
 from .types import Tok2PiecesBackpropT, Tok2PiecesInT, Tok2PiecesModelT, Tok2PiecesOutT
 
 
 @serialize_attr.register(ByteBPEProcessor)
 def serialize_byte_bpe_processor(_, value: ByteBPEProcessor, name: str, model) -> bytes:
     data = {"merges": value.merges, "vocab": value.vocab}
     return srsly.msgpack_dumps(data)
@@ -48,21 +47,27 @@
 ) -> Tuple[Tok2PiecesOutT, Tok2PiecesBackpropT]:
     bbp: ByteBPEProcessor = model.attrs["byte_bpe_processor"]
     bos_piece: str = model.attrs["bos_piece"]
     eos_piece: str = model.attrs["eos_piece"]
     unk_piece: str = model.attrs["unk_piece"]
     bos_id = bbp.piece_id(bos_piece)
     if bos_id is None:
-        raise ValueError(Errors.E019.format(piece="BOS"))
+        raise ValueError(
+            "Byte-BPE piece encoder vocabulary doesn't contain 'BOS' piece"
+        )
     eos_id = bbp.piece_id(eos_piece)
     if eos_id is None:
-        raise ValueError(Errors.E019.format(piece="EOS"))
+        raise ValueError(
+            "Byte-BPE piece encoder vocabulary doesn't contain 'EOS' piece"
+        )
     unk_id = bbp.piece_id(unk_piece)
     if unk_id is None:
-        raise ValueError(Errors.E019.format(piece="UNK"))
+        raise ValueError(
+            "Byte-BPE piece encoder vocabulary doesn't contain 'UNK' piece"
+        )
 
     pieces = []
     for doc in X:
         # TODO: check whether as single bos/eos per doc is what we want.
         #   The issue is that we probably do not have sentence
         #   boundaries yet, since they are predicted by a pipe.
         doc_pieces = [bos_id]
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/char_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/char_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unicodedata
 from pathlib import Path
 from typing import Callable, Dict, Optional, OrderedDict, Tuple
 
 from thinc.api import Model, Ragged
 
-from ..errors import Errors
 from .types import Tok2PiecesBackpropT, Tok2PiecesInT, Tok2PiecesModelT, Tok2PiecesOutT
 
 
 def build_char_encoder_v1() -> Tok2PiecesModelT:
     """Construct a character piece encoder model that accepts a list
     of token sequences or documents and returns a corresponding list
     of piece identifiers.
@@ -41,15 +40,18 @@
     of piece identifiers.
 
     This model must be separately initialized using an appropriate
     loader.
     """
     vocab: Optional[Dict[str, int]] = model.attrs["vocab"]
     if vocab is None:
-        raise ValueError(Errors.E020)
+        raise ValueError(
+            "Character piece encoder vocabulary is not available. Use a loader "
+            "to initialize the encoder."
+        )
 
     bos_piece: str = model.attrs["bos_piece"]
     eos_piece: str = model.attrs["eos_piece"]
     unk_piece: str = model.attrs["unk_piece"]
     normalize: Optional[str] = model.attrs["normalize"]
     bos_id = vocab[bos_piece]
     eos_id = vocab[eos_piece]
@@ -98,15 +100,19 @@
 
     path (Path):
         Path to the serialized character model.
     """
 
     def load(model, X=None, Y=None):
         if model.name != "char_encoder":
-            raise ValueError(Errors.E021.format(model_name=model.name))
+            raise ValueError(
+                "Attempting to use the `CharEncoderLoader` piece encoder loader with an "
+                f"incompatible model ('{model.name}'). It can only be used with the "
+                "`CharEncoder` piece encoder"
+            )
 
         model.attrs["bos_piece"] = bos_piece
         model.attrs["eos_piece"] = eos_piece
         model.attrs["unk_piece"] = unk_piece
         model.attrs["normalize"] = normalize
 
         vocab = OrderedDict()
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/hf_loader.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/hf_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from typing import Callable, Optional
 
 from .._compat import has_hf_transformers, transformers
-from ..errors import Errors
 from .bbpe_encoder import ByteBPEProcessor
 from .sentencepiece_encoder import SentencePieceProcessor
 from .types import Tok2PiecesInT, Tok2PiecesModelT
 from .wordpiece_encoder import WordPieceProcessor
 
 if has_hf_transformers:
     SUPPORTED_TOKENIZERS = (
@@ -16,37 +15,49 @@
         transformers.CamembertTokenizerFast,
         transformers.BertJapaneseTokenizer,
     )
 else:
     SUPPORTED_TOKENIZERS = ()  # type: ignore
 
 
+class _HFPieceEncoderLoader:
+    """This was formerly an inline function. However, only proper objects
+    can be pickled."""
+
+    def __init__(self, *, name: str, revision: str):
+        self.name = name
+        self.revision = revision
+
+    def __call__(self, model, X=None, Y=None):
+        if not has_hf_transformers:
+            raise ValueError(
+                "`HFPieceEncoderLoader` requires the Hugging Face `transformers` package to be installed"
+            )
+
+        tokenizer = transformers.AutoTokenizer.from_pretrained(
+            self.name, revision=self.revision
+        )
+        return _convert_encoder(model, tokenizer)
+
+
 def build_hf_piece_encoder_loader_v1(
     *, name: str, revision: str = "main"
 ) -> Callable[
     [Tok2PiecesModelT, Optional[Tok2PiecesInT], Optional[Tok2PiecesInT]],
     Tok2PiecesModelT,
 ]:
     """Construct a callback that initializes a HuggingFace piece encoder
     model. Used in conjunction with the HuggingFace model loader.
 
     name (str):
         Name of the HuggingFace model.
     revision (str):
         Name of the model revision/branch.
     """
-
-    def load(model, X=None, Y=None):
-        if not has_hf_transformers:
-            raise ValueError(Errors.E011.format(loader_name="HFPieceEncoderLoader"))
-
-        tokenizer = transformers.AutoTokenizer.from_pretrained(name, revision=revision)
-        return _convert_encoder(model, tokenizer)
-
-    return load
+    return _HFPieceEncoderLoader(name=name, revision=revision)
 
 
 def _convert_encoder(
     model: Tok2PiecesModelT, tokenizer: "transformers.PreTrainedTokenizerBase"
 ) -> Tok2PiecesModelT:
     if isinstance(tokenizer, transformers.BertTokenizerFast):
         return _convert_wordpiece_encoder(model, tokenizer)
@@ -57,18 +68,16 @@
         (transformers.XLMRobertaTokenizerFast, transformers.CamembertTokenizerFast),
     ):
         return _convert_sentencepiece_encoder(model, tokenizer)  # type: ignore
     elif isinstance(tokenizer, transformers.BertJapaneseTokenizer):
         return _convert_bert_japanese_encoder(model, tokenizer)
     else:
         raise ValueError(
-            Errors.E022.format(
-                unsupported_tokenizer=type(tokenizer),
-                supported_tokenizers=SUPPORTED_TOKENIZERS,
-            )
+            "Attempting to load an unsupported Hugging Face tokenizer "
+            f"({type(tokenizer)}). Currently supported tokenizers: {SUPPORTED_TOKENIZERS}"
         )
 
 
 def _convert_byte_bpe_encoder(
     model: Tok2PiecesModelT,
     tokenizer: "transformers.RobertaTokenizerFast",
 ) -> Tok2PiecesModelT:
@@ -128,17 +137,23 @@
 def _convert_bert_japanese_encoder(
     model: Tok2PiecesModelT, tokenizer: "transformers.BertJapaneseTokenizer"
 ) -> Tok2PiecesModelT:
     if not isinstance(
         tokenizer.subword_tokenizer,
         transformers.models.bert_japanese.CharacterTokenizer,
     ):
-        raise ValueError(Errors.E023)
+        raise ValueError(
+            "Japanese BERT models currently only support character subword encoding"
+        )
     if model.name != "char_encoder":
-        raise ValueError(Errors.E024.format(model_name=model.name))
+        raise ValueError(
+            f"Attempting to initialize an incompatible piece encoder ('{model.name}') "
+            "with the Hugging Face Japanese BERT tokenizer. It can only be used with the "
+            "`CharEncoder` piece encoder"
+        )
 
     model.attrs["bos_piece"] = tokenizer.cls_token
     model.attrs["eos_piece"] = tokenizer.sep_token
     model.attrs["unk_piece"] = tokenizer.unk_token
     model.attrs["normalize"] = (
         "NFKC" if tokenizer.subword_tokenizer.normalize_text else None
     )
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/types.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/tokenization/wordpiece_encoder.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers/util.py` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import itertools
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable
 
 import thinc
 from spacy.language import Language
 
-from .errors import Errors
-
 if TYPE_CHECKING:
     from .pipeline.transformer import CuratedTransformer
 
 thinc.registry.create("model_loaders", entry_points=True)
 registry = thinc.registry
 
 
@@ -32,15 +30,18 @@
     from .pipeline.transformer import CuratedTransformer
 
     for name, pipe in nlp.components:
         unfreeze_step = freeze_params.get(name)
         if unfreeze_step is None:
             continue
         elif not isinstance(pipe, CuratedTransformer):
-            raise TypeError(Errors.E025.format(pipe_name=name))
+            raise TypeError(
+                "Attempting to perform gradual unfreezing of a non-transformer pipe "
+                f"('{name}'. Only transformer pipes support this feature"
+            )
 
         pipe.frozen = current_step < unfreeze_step
 
 
 def gradual_transformer_unfreezing_all_pipes(
     nlp: Language, callback_args: Dict[str, Any], unfreeze_step: int
 ):
@@ -65,15 +66,18 @@
 
     target_pipes (Dict[str, int]):
         A dictionary whose keys and values correspond to the names of Transformer
         components and the training step at which they should be unfrozen respectively.
     """
     unfreeze_step_all_pipes = target_pipes.get("*")
     if unfreeze_step_all_pipes is not None and len(target_pipes) > 1:
-        raise ValueError(Errors.E013)
+        raise ValueError(
+            "The target pipe names for gradual transformer unfreezing contain both the "
+            "wild-card operator ('*') and individual names. Use either of the two but not both"
+        )
 
     if unfreeze_step_all_pipes is not None:
         return partial(
             gradual_transformer_unfreezing_all_pipes,
             unfreeze_step=unfreeze_step_all_pipes,
         )
     else:
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/PKG-INFO` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Curated transformer models for spaCy pipelines
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curated-transformers<0.2.0,>=0.1.0
-Requires-Dist: curated-tokenizers<0.1.0,>=0.0.7
+Requires-Dist: curated-tokenizers<0.1.0,>=0.0.9
 Requires-Dist: spacy<4.0.0,>=3.7.0.dev0
 Requires-Dist: torch>=1.12.0
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # 💫 🤖 spaCy Curated Transformers
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 0.2.2 Summary:
 Curated transformer models for spaCy pipelines Home-page: https://github.com/
 explosion/spacy-curated-transformers Author: Explosion Author-email:
 contact@explosion.ai License: MIT Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: curated-
-transformers<0.2.0,>=0.1.0 Requires-Dist: curated-tokenizers<0.1.0,>=0.0.7
+transformers<0.2.0,>=0.1.0 Requires-Dist: curated-tokenizers<0.1.0,>=0.0.9
 Requires-Dist: spacy<4.0.0,>=3.7.0.dev0 Requires-Dist: torch>=1.12.0 _[_h_t_t_p_s_:_/_/
 _e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# ð« ð¤ spaCy Curated Transformers This
 package provides [spaCy](https://github.com/explosion/spaCy) components and
 architectures to use a curated set of transformer models via [`curated-
 transformers`](https://github.com/explosion/curated-transformers) in spaCy. [!
 [PyPi](https://img.shields.io/pypi/v/spacy-curated-transformers.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-curated-
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/SOURCES.txt` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 spacy_curated_transformers/__init__.py
 spacy_curated_transformers/_compat.py
-spacy_curated_transformers/errors.py
 spacy_curated_transformers/util.py
 spacy_curated_transformers.egg-info/PKG-INFO
 spacy_curated_transformers.egg-info/SOURCES.txt
 spacy_curated_transformers.egg-info/dependency_links.txt
 spacy_curated_transformers.egg-info/entry_points.txt
 spacy_curated_transformers.egg-info/requires.txt
 spacy_curated_transformers.egg-info/top_level.txt
```

### Comparing `spacy-curated-transformers-0.2.1/spacy_curated_transformers.egg-info/entry_points.txt` & `spacy-curated-transformers-0.2.2/spacy_curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

