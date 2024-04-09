# Comparing `tmp/everyvoice-0.1.0a0.dev0.tar.gz` & `tmp/everyvoice-0.1.20230307.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everyvoice-0.1.0a0.dev0.tar", last modified: Tue Apr  9 22:29:19 2024, max compression
+gzip compressed data, was "everyvoice-0.1.20230307.tar", last modified: Tue Mar  7 20:38:03 2023, max compression
```

## Comparing `everyvoice-0.1.0a0.dev0.tar` & `everyvoice-0.1.20230307.tar`

### file list

```diff
@@ -1,154 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.363699 everyvoice-0.1.0a0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-09 22:29:19.363699 everyvoice-0.1.0a0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.339699 everyvoice-0.1.0a0.dev0/everyvoice/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.343699 everyvoice-0.1.0a0.dev0/everyvoice/base_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/base_cli/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/base_cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/base_cli/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.343699 everyvoice-0.1.0a0.dev0/everyvoice/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/config/preprocessing_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/config/shared_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/config/text_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.343699 everyvoice-0.1.0a0.dev0/everyvoice/dataloader/
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/dataloader/imbalanced_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.343699 everyvoice-0.1.0a0.dev0/everyvoice/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.343699 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.335699 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.347699 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.347699 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/duration_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-09 22:29:13.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/DeepForcedAligner/dfaligner/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.335699 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.347699 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/aligner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/aligner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/aligner/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/aligner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/aligner/heavy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/aligner/wav2vec2aligner/aligner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.347699 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.347699 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.347699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.335699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.351699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.351699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/attn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/attn/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/attn/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/attn/attention_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.351699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/check_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/synthesize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/cli/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.351699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/config/
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    16549 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/noam.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/prediction_writing_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3545 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/synthesize_text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.355699 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/tests/test_writing_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-09 22:29:14.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2/variance_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/feature_prediction/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.355699 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.335699 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.355699 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:15.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-09 22:29:15.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.355699 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/config/
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-09 22:29:15.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-09 22:29:15.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    26829 2024-04-09 22:29:15.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-09 22:29:15.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.355699 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/original_hifigan_helper/
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/original_hifigan_helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.355699 everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/attention_prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    35487 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/preprocessor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3871 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.359699 everyvoice-0.1.0a0.dev0/everyvoice/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/basic_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/stubs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10802 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30327 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_dataloader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3420 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21193 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_preprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9595 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_text.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5338 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    49966 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/tests/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.359699 everyvoice-0.1.0a0.dev0/everyvoice/text/
--rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/text/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/text/lookups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.359699 everyvoice-0.1.0a0.dev0/everyvoice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/utils/heavy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.359699 everyvoice-0.1.0a0.dev0/everyvoice/wizard/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/main_tour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/everyvoice/wizard/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:29:19.359699 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 22:29:19.000000 everyvoice-0.1.0a0.dev0/everyvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/requirements.torch.txt
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 22:29:19.363699 everyvoice-0.1.0a0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 22:29:10.000000 everyvoice-0.1.0a0.dev0/setup.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.209197 everyvoice-0.1.20230307/
+-rw-r--r--   0 pinea      (502) staff       (20)     1067 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/LICENSE
+-rw-r--r--   0 pinea      (502) staff       (20)     2957 2023-03-07 20:38:03.209261 everyvoice-0.1.20230307/PKG-INFO
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.199669 everyvoice-0.1.20230307/everyvoice/
+-rw-r--r--   0 pinea      (502) staff       (20)      990 2023-03-07 17:54:58.000000 everyvoice-0.1.20230307/everyvoice/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)       16 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/_version.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.201157 everyvoice-0.1.20230307/everyvoice/base_cli/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/base_cli/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     5916 2023-03-07 17:57:45.000000 everyvoice-0.1.20230307/everyvoice/base_cli/helpers.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3126 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/base_cli/interfaces.py
+-rw-r--r--   0 pinea      (502) staff       (20)    16204 2023-03-07 17:57:42.000000 everyvoice-0.1.20230307/everyvoice/cli.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.202333 everyvoice-0.1.20230307/everyvoice/config/
+-rw-r--r--   0 pinea      (502) staff       (20)      506 2023-03-07 17:55:11.000000 everyvoice-0.1.20230307/everyvoice/config/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3531 2023-03-07 17:53:49.000000 everyvoice-0.1.20230307/everyvoice/config/preprocessing_config.py
+-rw-r--r--   0 pinea      (502) staff       (20)     5307 2023-03-07 17:55:11.000000 everyvoice-0.1.20230307/everyvoice/config/shared_types.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1035 2023-03-07 17:53:50.000000 everyvoice-0.1.20230307/everyvoice/config/text_config.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1855 2023-03-07 17:53:51.000000 everyvoice-0.1.20230307/everyvoice/config/utils.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.202874 everyvoice-0.1.20230307/everyvoice/dataloader/
+-rw-r--r--   0 pinea      (502) staff       (20)     3040 2023-03-07 17:59:03.000000 everyvoice-0.1.20230307/everyvoice/dataloader/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2123 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/dataloader/imbalanced_sampler.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.203188 everyvoice-0.1.20230307/everyvoice/model/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.203606 everyvoice-0.1.20230307/everyvoice/model/aligner/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/aligner/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      121 2023-03-07 17:53:58.000000 everyvoice-0.1.20230307/everyvoice/model/aligner/config.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.204479 everyvoice-0.1.20230307/everyvoice/model/e2e/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/e2e/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      924 2023-03-07 17:57:49.000000 everyvoice-0.1.20230307/everyvoice/model/e2e/cli.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.204749 everyvoice-0.1.20230307/everyvoice/model/e2e/config/
+-rw-r--r--   0 pinea      (502) staff       (20)     1629 2023-03-07 17:57:55.000000 everyvoice-0.1.20230307/everyvoice/model/e2e/config/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     7777 2023-03-07 17:57:51.000000 everyvoice-0.1.20230307/everyvoice/model/e2e/dataset.py
+-rw-r--r--   0 pinea      (502) staff       (20)    12284 2023-03-07 17:57:53.000000 everyvoice-0.1.20230307/everyvoice/model/e2e/model.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.205070 everyvoice-0.1.20230307/everyvoice/model/feature_prediction/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/feature_prediction/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      218 2023-03-07 17:53:58.000000 everyvoice-0.1.20230307/everyvoice/model/feature_prediction/config.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1175 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/utils.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.205405 everyvoice-0.1.20230307/everyvoice/model/vocoder/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/vocoder/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)      118 2023-03-07 17:53:58.000000 everyvoice-0.1.20230307/everyvoice/model/vocoder/config.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.205639 everyvoice-0.1.20230307/everyvoice/model/vocoder/original_hifigan_helper/
+-rw-r--r--   0 pinea      (502) staff       (20)     7159 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/model/vocoder/original_hifigan_helper/__init__.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.206285 everyvoice-0.1.20230307/everyvoice/preprocessor/
+-rw-r--r--   0 pinea      (502) staff       (20)    27518 2023-03-07 17:57:20.000000 everyvoice-0.1.20230307/everyvoice/preprocessor/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3116 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/preprocessor/attention_prior.py
+-rw-r--r--   0 pinea      (502) staff       (20)     1860 2023-03-07 17:53:43.000000 everyvoice-0.1.20230307/everyvoice/run_tests.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.207557 everyvoice-0.1.20230307/everyvoice/tests/
+-rw-r--r--   0 pinea      (502) staff       (20)        0 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/tests/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3641 2023-03-07 17:58:07.000000 everyvoice-0.1.20230307/everyvoice/tests/test_configs.py
+-rw-r--r--   0 pinea      (502) staff       (20)     2559 2023-03-07 17:58:07.000000 everyvoice-0.1.20230307/everyvoice/tests/test_dataloader.py
+-rw-r--r--   0 pinea      (502) staff       (20)      594 2023-03-07 17:58:07.000000 everyvoice-0.1.20230307/everyvoice/tests/test_model.py
+-rw-r--r--   0 pinea      (502) staff       (20)    11265 2023-03-07 17:58:07.000000 everyvoice-0.1.20230307/everyvoice/tests/test_preprocessing.py
+-rw-r--r--   0 pinea      (502) staff       (20)     6137 2023-03-07 17:58:07.000000 everyvoice-0.1.20230307/everyvoice/tests/test_text.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.208267 everyvoice-0.1.20230307/everyvoice/text/
+-rw-r--r--   0 pinea      (502) staff       (20)     5616 2023-03-07 17:53:57.000000 everyvoice-0.1.20230307/everyvoice/text/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)     3118 2023-03-07 17:51:35.000000 everyvoice-0.1.20230307/everyvoice/text/features.py
+-rw-r--r--   0 pinea      (502) staff       (20)      725 2023-03-07 17:58:07.000000 everyvoice-0.1.20230307/everyvoice/text/lookups.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.208973 everyvoice-0.1.20230307/everyvoice/utils/
+-rw-r--r--   0 pinea      (502) staff       (20)     8141 2023-03-07 17:53:57.000000 everyvoice-0.1.20230307/everyvoice/utils/__init__.py
+-rw-r--r--   0 pinea      (502) staff       (20)    12946 2023-03-07 17:53:57.000000 everyvoice-0.1.20230307/everyvoice/utils/cli_wizard.py
+-rw-r--r--   0 pinea      (502) staff       (20)     4342 2023-03-07 17:53:57.000000 everyvoice-0.1.20230307/everyvoice/utils/heavy.py
+drwxr-xr-x   0 pinea      (502) staff       (20)        0 2023-03-07 20:38:03.200677 everyvoice-0.1.20230307/everyvoice.egg-info/
+-rw-r--r--   0 pinea      (502) staff       (20)     2957 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/PKG-INFO
+-rw-r--r--   0 pinea      (502) staff       (20)     1657 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        1 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 pinea      (502) staff       (20)       51 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/entry_points.txt
+-rw-r--r--   0 pinea      (502) staff       (20)        1 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/not-zip-safe
+-rw-r--r--   0 pinea      (502) staff       (20)      402 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/requires.txt
+-rw-r--r--   0 pinea      (502) staff       (20)       11 2023-03-07 20:38:03.000000 everyvoice-0.1.20230307/everyvoice.egg-info/top_level.txt
+-rw-r--r--   0 pinea      (502) staff       (20)      374 2023-03-07 20:38:03.209551 everyvoice-0.1.20230307/setup.cfg
+-rw-r--r--   0 pinea      (502) staff       (20)     1532 2023-03-07 18:08:00.000000 everyvoice-0.1.20230307/setup.py
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/dataloader/__init__.py` & `everyvoice-0.1.20230307/everyvoice/dataloader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,41 +45,41 @@
             if self.use_weighted_sampler
             else None
         )
         return DataLoader(
             self.train_dataset,
             batch_size=self.batch_size,
             num_workers=self.config.training.train_data_workers,
-            pin_memory=False,
+            pin_memory=True,
             drop_last=True,
             collate_fn=self.collate_fn,
             sampler=sampler,
         )
 
     def predict_dataloader(self):
         return DataLoader(
             self.train_dataset + self.val_dataset,
             batch_size=self.batch_size,
             num_workers=self.config.training.train_data_workers,
-            pin_memory=False,
+            pin_memory=True,
             drop_last=False,
             collate_fn=self.collate_fn,
         )
 
     def val_dataloader(self):
         sampler = (
             ImbalancedDatasetSampler(self.val_dataset)
             if self.use_weighted_sampler
             else None
         )
         return DataLoader(
             self.val_dataset,
             batch_size=1,
             num_workers=0,
-            pin_memory=False,
+            pin_memory=True,
             drop_last=True,
             collate_fn=self.collate_fn,
             sampler=sampler,
         )
 
     def prepare_data(self):
         # Override this method
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/dataloader/imbalanced_sampler.py` & `everyvoice-0.1.20230307/everyvoice/dataloader/imbalanced_sampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Adapted from https://github.com/ufoym/imbalanced-dataset-sampler
 
-from typing import Callable, Optional
+from typing import Callable
 
 import pandas as pd
 import torch
 import torch.utils.data
 
 
 class ImbalancedDatasetSampler(torch.utils.data.sampler.Sampler):
@@ -15,18 +15,18 @@
         num_samples: number of samples to draw
         callback_get_label: a callback-like function which takes two arguments - dataset and index
     """
 
     def __init__(
         self,
         dataset,
-        labels: Optional[list] = None,
-        indices: Optional[list] = None,
-        num_samples: Optional[int] = None,
-        callback_get_label: Optional[Callable] = None,
+        labels: list = None,
+        indices: list = None,
+        num_samples: int = None,
+        callback_get_label: Callable = None,
     ):
         # if indices is not provided, all elements in the dataset will be considered
         self.indices = list(range(len(dataset))) if indices is None else indices
 
         # define custom callback
         self.callback_get_label = callback_get_label
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/cli.py` & `everyvoice-0.1.20230307/everyvoice/model/e2e/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from enum import Enum
+
 import typer
 from merge_args import merge_args
 
 from everyvoice.base_cli.interfaces import train_base_command_interface
+from everyvoice.model.e2e.config import CONFIGS, EveryVoiceConfig
+
+app = typer.Typer(pretty_exceptions_show_locals=False)
+
+_config_keys = {k: k for k in CONFIGS.keys()}
 
-app = typer.Typer(
-    pretty_exceptions_show_locals=False,
-    help="End-to-end training: jointly train the FastSpeech2 and HiFiGAN networks",
-)
+CONFIGS_ENUM = Enum("CONFIGS", _config_keys)  # type: ignore
 
 
 @app.command()
 @merge_args(train_base_command_interface)
-def train(**kwargs):
+def train(name: CONFIGS_ENUM = typer.Option(None, "--name", "-n"), **kwargs):
     from everyvoice.base_cli.helpers import train_base_command
-    from everyvoice.model.e2e.config import EveryVoiceConfig
     from everyvoice.model.e2e.dataset import E2EDataModule
     from everyvoice.model.e2e.model import EveryVoice
 
     train_base_command(
+        name=name,
         model_config=EveryVoiceConfig,
+        configs=CONFIGS,
         model=EveryVoice,
         data_module=E2EDataModule,
         monitor="validation/mel_spec_error",
         **kwargs
     )
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/dataset.py` & `everyvoice-0.1.20230307/everyvoice/model/e2e/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,46 @@
+import random
 from pathlib import Path
 
 import numpy as np
 import torch
 from torch.nn.utils.rnn import pad_sequence
-from torch.utils.data import Dataset
+from torch.utils.data import Dataset, random_split
 
 from everyvoice.dataloader import BaseDataModule
 from everyvoice.model.e2e.config import EveryVoiceConfig
 from everyvoice.text import TextProcessor
 from everyvoice.text.lookups import LookupTables
-from everyvoice.utils import _flatten, check_dataset_size
-from everyvoice.utils.heavy import get_segments
+from everyvoice.utils import check_dataset_size
+from everyvoice.utils.heavy import _flatten, get_segments
 
 
 class E2EDataset(Dataset):
     def __init__(self, dataset, config: EveryVoiceConfig, use_segments=True):
         self.dataset = dataset
         self.config = config
         self.use_segments = use_segments
         self.lookup = LookupTables(config)
-        self.sep = "--"
+        self.sep = config.feature_prediction.preprocessing.value_separator
         self.text_processor = TextProcessor(config.feature_prediction)
         self.preprocessed_dir = Path(
             self.config.feature_prediction.preprocessing.save_dir
         )
+        random.seed(self.config.training.seed)
         self.output_sampling_rate = (
             self.config.vocoder.preprocessing.audio.output_sampling_rate
         )
         self.input_sampling_rate = (
             self.config.feature_prediction.preprocessing.audio.input_sampling_rate
         )
         self.sampling_rate_change = (
             self.output_sampling_rate // self.input_sampling_rate
         )
         self.output_hop_size = (
-            self.config.vocoder.preprocessing.audio.fft_hop_size
+            self.config.vocoder.preprocessing.audio.fft_hop_frames
             * self.sampling_rate_change
         )
         self.frame_segment_size = (
             self.config.vocoder.preprocessing.audio.vocoder_segment_size
             // self.output_hop_size
         )
         self.speaker2id = self.lookup.speaker2id
@@ -155,16 +157,17 @@
         self.collate_fn = self.collate_method
         self.use_weighted_sampler = (
             config.feature_prediction.training.use_weighted_sampler
         )
         self.batch_size = (
             config.training.batch_size
         )  # TODO: should this be set somewhere else?
+        self.train_split = config.training.train_split
         self.load_dataset()
-        self.dataset_length = len(self.train_dataset) + len(self.val_dataset)
+        self.dataset_length = len(self.dataset)
 
     @staticmethod
     def collate_method(data):
         data = [_flatten(x) for x in data]
         data = {k: [dic[k] for dic in data] for k in data[0]}
         text_lens = torch.LongTensor([text.size(0) for text in data["text"]])
         mel_lens = torch.LongTensor([mel.size(0) for mel in data["mel"]])
@@ -180,24 +183,24 @@
         data["src_lens"] = text_lens
         data["mel_lens"] = mel_lens
         data["max_src_len"] = max_text
         data["max_mel_len"] = max_mel
         return data
 
     def load_dataset(self):
-        self.train_dataset = self.config.training.filelist_loader(
-            self.config.training.training_filelist
-        )
-        self.val_dataset = self.config.training.filelist_loader(
-            self.config.training.validation_filelist
+        self.dataset = self.config.training.filelist_loader(
+            self.config.training.filelist
         )
 
     def prepare_data(self):
-        train_samples = len(self.train_dataset)
-        val_samples = len(self.val_dataset)
+        train_samples = int(self.dataset_length * self.train_split)
+        val_samples = self.dataset_length - train_samples
+        self.train_dataset, self.val_dataset = random_split(
+            self.dataset, [train_samples, val_samples]
+        )
         check_dataset_size(self.batch_size, train_samples, "training")
         check_dataset_size(self.batch_size, val_samples, "validation")
         self.train_dataset = E2EDataset(self.train_dataset, self.config)
         self.val_dataset = E2EDataset(self.val_dataset, self.config)
         # save it to disk
         torch.save(self.train_dataset, self.train_path)
         torch.save(self.val_dataset, self.val_path)
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/model/e2e/model.py` & `everyvoice-0.1.20230307/everyvoice/model/e2e/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from loguru import logger
 
 from everyvoice.model.e2e.config import EveryVoiceConfig
-from everyvoice.model.feature_prediction.FastSpeech2_lightning.fs2.model import (
-    FastSpeech2,
-)
+from everyvoice.model.feature_prediction.FastSpeech2_lightning.fs2.model import FastSpeech2
 from everyvoice.model.feature_prediction.FastSpeech2_lightning.fs2.type_definitions import (
     Stats,
 )
 from everyvoice.model.feature_prediction.FastSpeech2_lightning.fs2.utils import plot_mel
 from everyvoice.model.vocoder.HiFiGAN_iSTFT_lightning.hfgl.model import HiFiGAN
 from everyvoice.utils.heavy import dynamic_range_compression_torch, expand
 
@@ -48,21 +46,21 @@
         )
         with open(
             self.config.feature_prediction.preprocessing.save_dir / "stats.json"
         ) as f:
             self.stats: Stats = Stats(**json.load(f))
         self.input_frame_segment_size = (
             self.config.vocoder.preprocessing.audio.vocoder_segment_size
-            // self.config.vocoder.preprocessing.audio.fft_hop_size
+            // self.config.vocoder.preprocessing.audio.fft_hop_frames
         )
         self.use_segments = True
 
     def forward(self, batch, inference=False):
         feature_prediction = self.feature_prediction.forward(batch)
-        vocoder_x = feature_prediction[self.feature_prediction.output_key]
+        vocoder_x = feature_prediction["postnet_output"]
         if not inference and self.use_segments:
             vocoder_x = torch.stack(
                 [
                     x[
                         batch["segment_start_frame"][i] : batch["segment_start_frame"][
                             i
                         ]
@@ -194,15 +192,15 @@
             batch["audio_mel"], generated_mel_spec
         ).item()
         self.log("validation/mel_spec_error", val_err_tot, prog_bar=False)
         if self.global_step == 0:
             audio = torch.load(
                 self.config.feature_prediction.preprocessing.save_dir
                 / "audio"
-                / "--".join(
+                / self.config.feature_prediction.preprocessing.value_separator.join(
                     [
                         batch["basename"][0],
                         batch["speaker"][0],
                         batch["language"][0],
                         f"audio-{self.config.feature_prediction.preprocessing.audio.input_sampling_rate}.pt",
                     ]
                 )
@@ -228,19 +226,15 @@
                             ),
                             "energy": expand(
                                 batch["energy"][0].cpu().numpy(), duration_np
                             ),
                         },
                         {
                             "mel": np.swapaxes(
-                                fp_output[self.feature_prediction.output_key][0]
-                                .cpu()
-                                .numpy(),
-                                0,
-                                1,
+                                fp_output["postnet_output"][0].cpu().numpy(), 0, 1
                             ),
                             "pitch": expand(
                                 fp_output["pitch_prediction"][0].cpu().numpy(),
                                 duration_np,
                             ),
                             "energy": expand(
                                 fp_output["energy_prediction"][0].cpu().numpy(),
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/model/utils.py` & `everyvoice-0.1.20230307/everyvoice/model/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,40 @@
 
 def create_depthwise_separable_convolution(
     in_channels,
     out_channels,
     kernel_size,
     stride=1,
     padding=0,
-    output_padding=0,
     dilation=1,
     groups=1,
     bias=True,
     padding_mode="zeros",
     transpose=False,
     weight_norm=True,
 ):
     if transpose:
         depth = ConvTranspose1d(
             in_channels,
             in_channels,
             kernel_size=kernel_size,
             stride=stride,
             padding=padding,
-            output_padding=output_padding,
             dilation=dilation,
             bias=bias,
             groups=in_channels,
         )
         point = ConvTranspose1d(in_channels, out_channels, kernel_size=1)
     else:
         depth = Conv1d(
             in_channels,
             in_channels,
             kernel_size=kernel_size,
             stride=stride,
             padding=padding,
-            output_padding=output_padding,
             dilation=dilation,
             bias=bias,
             groups=in_channels,
         )
         point = Conv1d(in_channels, out_channels, kernel_size=1)
     if weight_norm:
         return Sequential(wnorm(depth), wnorm(point))
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/model/vocoder/original_hifigan_helper/__init__.py` & `everyvoice-0.1.20230307/everyvoice/model/vocoder/original_hifigan_helper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import Conv1d, ConvTranspose1d
 from torch.nn.utils import remove_weight_norm, weight_norm
 
 LRELU_SLOPE = 0.1
@@ -221,14 +220,20 @@
     vocoder.eval()
     vocoder.remove_weight_norm()
     vocoder.to(device)
 
     return vocoder
 
 
-def vocoder_infer(mels, vocoder) -> np.ndarray:
+def vocoder_infer(mels, vocoder, max_wav_value, lengths=None):
     # mels (1, 80, 111) normal
     # mels small (1, 80, 5)
     with torch.no_grad():
         wavs = vocoder(mels.transpose(1, 2)).squeeze(1)
-    wavs = wavs.cpu().numpy()  # B, T
+    wavs = wavs.cpu().numpy()
+    wavs = [wav for wav in wavs]
+
+    for i in range(len(mels)):
+        if lengths is not None:
+            wavs[i] = wavs[i][: lengths[i]]
+
     return wavs
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/attention_prior.py` & `everyvoice-0.1.20230307/everyvoice/preprocessor/attention_prior.py`

 * *Files identical despite different names*

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/preprocessor/preprocessor.py` & `everyvoice-0.1.20230307/everyvoice/preprocessor/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,196 +1,241 @@
 """ Preprocessor Module that given a filelist containing text, wav, textgrid:
     - extracts log Mel spectral features
     - extracts pitch (phone-level or frame-level)
     - extracts energy
     - extracts inputs (ex. phonological feats)
 """
-
 import functools
 import multiprocessing as mp
-import random
-import sys
-from collections import Counter
-from glob import glob
-from multiprocessing import Manager
+import os
 from pathlib import Path
-from typing import Optional
+from typing import List, Tuple, Union
 
 import numpy as np
 import torch
-import torchaudio
-from clipdetect import detect_clipping
-from joblib import Parallel, delayed
 from loguru import logger
-from rich import print as rich_print
+from pathos.multiprocessing import ProcessingPool as Pool
+from pydantic import BaseModel
+from rich import print
 from rich.panel import Panel
 from rich.style import Style
 from tabulate import tabulate
-from torchaudio.functional import resample
+from torch import Tensor, linalg, mean, tensor
+from torchaudio import load as load_audio
+from torchaudio import save as save_audio
+from torchaudio.functional import compute_kaldi_pitch, resample
 from torchaudio.sox_effects import apply_effects_tensor
 from tqdm import tqdm
 
-from everyvoice.exceptions import ConfigError
+from everyvoice.config import ConfigError
 from everyvoice.model.aligner.config import AlignerConfig
 from everyvoice.model.feature_prediction.config import FeaturePredictionConfig
 from everyvoice.model.vocoder.config import VocoderConfig
 from everyvoice.preprocessor.attention_prior import BetaBinomialInterpolator
-from everyvoice.preprocessor.helpers import Counters, Scaler, save_tensor
 from everyvoice.text import TextProcessor
-from everyvoice.utils import (
-    generic_dict_loader,
-    n_times,
-    tqdm_joblib_context,
-    write_filelist,
-)
-from everyvoice.utils.heavy import (
-    dynamic_range_compression_torch,
-    get_spectral_transform,
-)
+from everyvoice.utils import generic_dict_loader, write_filelist
+from everyvoice.utils.heavy import dynamic_range_compression_torch, get_spectral_transform
+
+
+class Scaler:
+    def __init__(self):
+        self._data = []
+        self._tensor_data = None
+        self.min = None
+        self.max = None
+        self.std = None
+        self.mean = None
+        self.norm_min = None
+        self.norm_max = None
+
+    def __len__(self):
+        return len(self.data)
+
+    @property
+    def data(self):
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        raise ValueError(
+            f"Sorry, you tried to change the data to {value} but it cannot be changed directly. Either Scaler.append(data), or Scaler.clear_data()"
+        )
+
+    def append(self, value):
+        self._data += value
+
+    def clear_data(self):
+        """Clear data"""
+        self.__init__()
+
+    def normalize(self, data):
+        """Remove mean and normalize to unit variance"""
+        return (data - self.mean) / self.std
+
+    def denormalize(self, data):
+        """Get de-normalized value"""
+        return (data * self.std) + self.mean
+
+    def calculate_stats(self):
+        if not len(self):
+            return
+        if self._tensor_data is None:
+            self._tensor_data = torch.cat(self.data)
+        non_nan_data = self._tensor_data[~torch.isnan(self._tensor_data)]
+        self.min = torch.min(non_nan_data)
+        self.max = torch.max(non_nan_data)
+        self.mean = torch.nanmean(self._tensor_data)
+        self.std = torch.std(non_nan_data)
+        self.norm_max = self.normalize(self.max)
+        self.norm_min = self.normalize(self.min)
+        return {
+            "sample_size": len(self),
+            "norm_min": float(self.norm_min),
+            "norm_max": float(self.norm_max),
+            "min": float(self.min),
+            "max": float(self.max),
+            "mean": float(self.mean),
+            "std": float(self.std),
+        }
+
+
+# TODO: make work with multiprocessing: https://stackoverflow.com/questions/2080660/how-to-increment-a-shared-counter-from-multiple-processes
+class Counters(BaseModel):
+    duration: float = 0.0
+    nans: List[str] = []
+    audio_too_long: List[str] = []
+    audio_too_short: List[str] = []
+    skipped_processes: int = 0
+    missing_files: List[str] = []
 
 
 class Preprocessor:
-    def __init__(self, config: AlignerConfig | FeaturePredictionConfig | VocoderConfig):
+    def __init__(
+        self, config: Union[AlignerConfig, FeaturePredictionConfig, VocoderConfig]
+    ):
         self.config = config
-        self.counters = Counters(Manager())
-        self.cpus = 0
         self.pitch_scaler = Scaler()
         self.energy_scaler = Scaler()
         self.datasets = config.preprocessing.source_data
         self.save_dir = Path(config.preprocessing.save_dir)
+        self.save_dir.mkdir(parents=True, exist_ok=True)
+        self.counters = Counters()
         self.audio_config = config.preprocessing.audio
-        self.sep = "--"
+        self.sep = config.preprocessing.value_separator
         self.text_processor = (
             None if isinstance(config, VocoderConfig) else TextProcessor(config)
         )
         self.overwrite = False
         self.input_sampling_rate = self.audio_config.input_sampling_rate
         self.output_sampling_rate = self.audio_config.output_sampling_rate
         self.sampling_rate_change = (
             self.output_sampling_rate // self.input_sampling_rate
         )
         # Define Spectral Transform
         # Gah, so many ways to do this: https://github.com/CookiePPP/VocoderComparisons/issues/3
+
         self.input_spectral_transform = get_spectral_transform(
             self.audio_config.spec_type,
             self.audio_config.n_fft,
-            self.audio_config.fft_window_size,
-            self.audio_config.fft_hop_size,
+            self.audio_config.fft_window_frames,
+            self.audio_config.fft_hop_frames,
             sample_rate=self.input_sampling_rate,
             n_mels=self.audio_config.n_mels,
             f_min=self.audio_config.f_min,
             f_max=self.audio_config.f_max,
         )
         self.output_spectral_transform = get_spectral_transform(
             self.audio_config.spec_type,
             self.audio_config.n_fft * self.sampling_rate_change,
-            self.audio_config.fft_window_size * self.sampling_rate_change,
-            self.audio_config.fft_hop_size * self.sampling_rate_change,
+            self.audio_config.fft_window_frames * self.sampling_rate_change,
+            self.audio_config.fft_hop_frames * self.sampling_rate_change,
             sample_rate=self.input_sampling_rate,
             n_mels=self.audio_config.n_mels,
             f_min=self.audio_config.f_min,
             f_max=self.audio_config.f_max,
         )
 
         if (
             self.input_spectral_transform is None
             or self.output_spectral_transform is None
         ):
             raise ConfigError(
-                f"Spectral feature specification '{self.audio_config.spec_type}' is not supported. Please edit your config file."
+                f"Spectral feature specification {self.audio_config.spec_type} is not supported. Please edit your config file."
             )
 
-    def load_audio(self, audio_path: Path) -> tuple[torch.Tensor, int, float]:
-        """
-        Load an audio file and calculate its duration.
+    def load_audio_tensor(self, audio_path: Union[Path, str]):
+        """Load audio tensor from file
 
         Args:
-            audio_path: path to audio file
-
-        Returns: (audio as a Tensor, sampling rate, duration in seconds)
+            audio_path (str): path to audio file
         """
-        audio, sr = torchaudio.load(str(audio_path))
-        seconds = len(audio[0]) / sr
-        return audio, sr, seconds
+        try:
+            return torch.load(audio_path)
+        except FileNotFoundError:
+            logger.error("Audio file not found. Please process audio first.")
+            exit()
 
     def process_audio(
         self,
-        wav_path: Path,
+        wav_path: str,
         normalize=True,
-        use_effects=True,
+        use_effects=False,
         resample_rate=None,
         sox_effects=None,
         save_wave=False,
-        update_counters=True,  # unset this when processing the same file a second time
-    ) -> tuple[torch.Tensor, int] | tuple[None, None]:
+    ) -> Union[Tuple[Tensor, int], Tuple[None, None]]:
         """Process audio
 
         Args:
-            wav_path (Path): path to wav file
+            wav_path (str): path to wav file
             normalize (bool): volume normalization
         Returns:
-            Tensor: (audio as a Tensor, sampling rate)
+            [Tensor, int]: audio Tensor, sampling rate
         """
-        audio, sr, seconds = self.load_audio(wav_path)
-
-        if seconds > self.audio_config.max_audio_length:
-            logger.warning(
-                f"Audio too long: {wav_path} ({seconds} seconds - we will skip this file)"
-            )
-            if update_counters:
-                self.counters.increment("audio_too_long")
-            return None, None
-        if seconds < self.audio_config.min_audio_length:
-            logger.warning(
-                f"Audio too short: {wav_path} ({seconds} seconds - we will skip this file)"
-            )
-            if update_counters:
-                self.counters.increment("audio_too_short")
-            return None, None
-
-        loudness_transform = torchaudio.transforms.Loudness(sr)
-        loudness = loudness_transform(audio)
-        if (
-            torch.isnan(loudness) or loudness < -36
-        ):  # This is a conservative threshold, so some very quiet/silent files may still get through
-            logger.warning(f"Audio empty: {wav_path} - we will skip this file")
-            if update_counters:
-                self.counters.increment("audio_empty")
-            return None, None
 
+        audio, sr = load_audio(wav_path, normalize=normalize)
         if use_effects and sox_effects:
             audio, sr = apply_effects_tensor(
                 audio,
                 sr,
                 sox_effects,
             )
-
         if resample_rate is not None and resample_rate != sr:
             audio = resample(audio, sr, resample_rate)
             sr = resample_rate
         if normalize:
             audio /= torch.max(torch.abs(audio))
             audio *= 0.95
-
-        if update_counters:
-            self.counters.increment("processed_files")
-            self.counters.increment("duration", seconds)
+        seconds = len(audio[0]) / sr
+        if seconds > self.audio_config.max_audio_length:
+            logger.warning(
+                f"Audio too long: {wav_path} ({seconds} seconds - we will skip this file)"
+            )
+            self.counters.audio_too_long.append(os.path.basename(wav_path))
+            return None, None
+        if seconds < self.audio_config.min_audio_length:
+            logger.warning(
+                f"Audio too short: {wav_path} ({seconds} seconds - we will skip this file)"
+            )
+            self.counters.audio_too_short.append(os.path.basename(wav_path))
+            return None, None
+        self.counters.duration += seconds
         if save_wave:
-            torchaudio.save(
-                str(wav_path) + ".processed.wav",
+            save_audio(
+                wav_path + ".processed.wav",
                 audio,
                 sr,
                 encoding="PCM_S",
-                bits_per_sample=self.audio_config.target_bit_depth,
+                bits_per_sample=self.audio_config.alignment_bit_depth,
             )
         audio = audio.squeeze()  # get rid of channels dimension
-        return audio, sr
+        return (audio, sr)
 
     def extract_spectral_features(
-        self, audio_tensor: torch.Tensor, transform, normalize=True
+        self, audio_tensor: Tensor, transform, normalize=True
     ):
         """Given an audio tensor, extract the log Mel spectral features
         from the given start and end points
 
         Args:
             audio_tensor (Tensor): Tensor trimmed according
             transform (torchaudio.transforms): transform to apply; use either Preprocessor.input_spectral_transform or Preprocessor.output_spectral_transform
@@ -205,456 +250,377 @@
         def nan_helper(y):
             return np.isnan(y), lambda z: z.nonzero()[0]
 
         nans, y = nan_helper(x)
         x[nans] = np.interp(y(nans), y(~nans), x[~nans])
         return x
 
-    def extract_pitch(self, audio_tensor: torch.Tensor):
+    def extract_pitch(self, audio_tensor: Tensor):
         """Given an audio tensor, extract the pitch
 
         TODO: consider CWT and Parselmouth
 
         Comparison with other implementations:
             - ming024 & Christoph Minxhoffer use the pyworld implementation and interpolate along with phone averaging
             - the Lightspeech implementation seems to use pyworld implementation and not interpolate or average
             - Christoph Minxhoffer reported no significant differences with continuous wavelet transform so it is not implemented here
 
         Args:
-            audio_tensor (Tensor): 1D tensor of audio samples
+            spectral_feature_tensor (Tensor): tensor of spectral features extracted from audio
         """
-        import pyworld as pw  # This isn't a very good place for an import,
+        if self.config.preprocessing.pitch_type == "pyworld":
+            import pyworld as pw  # This isn't a very good place for an import,
 
-        # but also pyworld is very annoying to install so this is a compromise
-        pitch, t = pw.dio(
-            audio_tensor.squeeze(0)
-            .numpy()
-            .astype(
-                np.float64
-            ),  # TODO: why are these np.float64, maybe it's just what pw expects?
-            self.input_sampling_rate,
-            frame_period=self.audio_config.fft_hop_size
-            / self.input_sampling_rate
-            * 1000,
-            speed=4,
-        )
-        pitch = pw.stonemask(
-            audio_tensor.squeeze(0).numpy().astype(np.float64),
-            pitch,
-            t,
-            self.input_sampling_rate,
-        )
-        pitch[pitch == 0] = np.nan
-        try:
+            # but also pyworld is very annoying to install so this is a compromise
+            pitch, t = pw.dio(
+                audio_tensor.squeeze(0)
+                .numpy()
+                .astype(
+                    np.float64
+                ),  # TODO: why are these np.float64, maybe it's just what pw expects?
+                self.input_sampling_rate,
+                frame_period=self.audio_config.fft_hop_frames
+                / self.input_sampling_rate
+                * 1000,
+                speed=4,
+            )
+            pitch = pw.stonemask(
+                audio_tensor.squeeze(0).numpy().astype(np.float64),
+                pitch,
+                t,
+                self.input_sampling_rate,
+            )
+            pitch[pitch == 0] = np.nan
             pitch = self._interpolate(pitch)
-        except ValueError:
-            # TODO: we should warn the user about pitch-less samples
-            pitch[np.isnan(pitch)] = 0
-        pitch = torch.tensor(pitch).float()
+            pitch = tensor(pitch).float()
+        elif self.config.preprocessing.pitch_type == "kaldi":
+            pitch = compute_kaldi_pitch(
+                waveform=audio_tensor,
+                sample_rate=self.input_sampling_rate,
+                frame_length=self.audio_config.fft_window_frames
+                / self.input_sampling_rate
+                * 1000,
+                frame_shift=self.audio_config.fft_hop_frames
+                / self.input_sampling_rate
+                * 1000,
+                min_f0=50,
+                max_f0=400,
+            )[0][
+                ..., 1
+            ]  # TODO: the docs and C Minxhoffer implementation take [..., 0] but this doesn't appear to be the pitch, at least for this version of torchaudio.
+        else:
+            raise ConfigError(
+                f"Sorry, the pitch estimation type '{self.config.preprocessing.pitch_type}' is not supported. Please edit your config file."
+            )
         return pitch
 
     def average_data_by_durations(self, data, durations):
         current_frame_position = 0
         new_data = []
         for duration in durations.numpy().tolist():
             if duration > 0:
                 new_data.append(
-                    torch.mean(
+                    mean(
                         data[current_frame_position : current_frame_position + duration]
                     )
                 )
             else:
                 new_data.append(1e-7)
             current_frame_position += duration
-        return torch.tensor(new_data)
+        return tensor(new_data)
 
-    def extract_energy(self, spectral_feature_tensor: torch.Tensor):
+    def extract_energy(self, spectral_feature_tensor: Tensor):
         """Given a spectral feature tensor, and durations extract the energy averaged across a phone
 
         Args:
             spectral_feature_tensor (Tensor): tensor of spectral features extracted from audio
             durations (_type_): _descriptiont    #TODO
         """
-        return torch.linalg.norm(spectral_feature_tensor, dim=0)
+        return linalg.norm(spectral_feature_tensor, dim=0)
 
-    # This method is static because we want to use it in Datasets without setting the Preprocessor as an attribute
-    @staticmethod
-    def extract_text_inputs(
-        text, text_processor: TextProcessor, use_pfs=False, quiet=False
-    ) -> torch.Tensor:
-        """
-        Given some text and a text_processor, normalize it, g2p it, and save as one-hot or multi-hot phonological feature vectors
+    def extract_text_inputs(self, text, use_pfs=False) -> Tensor:
+        """Given some text, normalize it, g2p it, and save as one-hot or multi-hot phonological feature vectors
 
         Args:
             text (str): text
-            text_processor (TextProcessor): a text processor
-            use_pfs:
-            quiet: suppress warnings
         """
-        if text_processor is None:
+        if self.text_processor is None:
             raise ValueError("Text processor not initialized")
         if use_pfs:
             return torch.Tensor(
-                text_processor.text_to_phonological_features(text, quiet)
+                self.text_processor.text_to_phonological_features(text)
             ).long()
         else:
-            return torch.Tensor(text_processor.text_to_sequence(text, quiet)).long()
+            return torch.Tensor(self.text_processor.text_to_sequence(text)).long()
 
     def print_duration(self):
         """Convert seconds to a human readable format"""
-        seconds = int(self.counters.value("duration"))
+        seconds = int(self.counters.duration)
         hours = seconds // 3600
         seconds %= 3600
         minutes = seconds // 60
         seconds %= 60
         return f"{hours}h {minutes}m {seconds}s"
 
     def report(self, tablefmt="simple"):
         """Print a report of the dataset processing"""
         headers = ["type", "quantity"]
         table = [
-            ["processed files", self.counters.value("processed_files")],
-            [
-                "previously processed files",
-                self.counters.value("previously_processed_files"),
-            ],
-            ["missing files", self.counters.value("missing_files")],
+            ["missing files", len(self.counters.missing_files)],
             [
                 "missing symbols",
                 len(self.text_processor.missing_symbols) if self.text_processor else 0,
             ],
             [
                 "duplicate symbols",
-                (
-                    len(self.text_processor.duplicate_symbols)
-                    if self.text_processor
-                    else 0
-                ),
+                len(self.text_processor.duplicate_symbols)
+                if self.text_processor
+                else 0,
             ],
-            ["skipped processes", self.counters.value("skipped_processes")],
-            ["nans", self.counters.value("nans")],
-            ["audio_empty", self.counters.value("audio_empty")],
-            ["audio_too_short", self.counters.value("audio_too_short")],
-            ["audio_too_long", self.counters.value("audio_too_long")],
+            ["skipped processes", self.counters.skipped_processes],
+            ["nans", self.counters.nans],
+            ["audio_too_short", len(self.counters.audio_too_short)],
+            ["audio_too_long", len(self.counters.audio_too_long)],
             ["duration", self.print_duration()],
         ]
         return tabulate(table, headers, tablefmt=tablefmt)
 
     def get_speaker_and_language(self, item):
         """Unless the dataset already has values for speaker and language, set them to 'default'"""
         if "speaker" in item and "language" in item:
             return item
         speaker = "default" if "speaker" not in item else item["speaker"]
         language = "default" if "language" not in item else item["language"]
         return {**item, **{"speaker": speaker, "language": language}}
 
     def compute_stats(
         self, energy=True, pitch=True
-    ) -> tuple[Optional[Scaler], Optional[Scaler]]:
-        if self.cpus > 1:
-            parallel = Parallel(n_jobs=self.cpus, backend="loky", batch_size=500)
+    ) -> Tuple[Union[Scaler, None], Union[Scaler, None]]:
         if energy:
             energy_scaler = Scaler()
-            # Until Python 3.13, pathlib.Path.glob() doesn't work with symlinks: https://github.com/python/cpython/issues/77609
-            paths = glob(
-                str(self.config.preprocessing.save_dir / "energy/**/*energy*"),
-                recursive=True,
-            )
-            if self.cpus > 1:
-                logger.info("Gathering energy values")
-                with tqdm_joblib_context(tqdm(desc="Gathering energy values")):
-                    for energy_data in parallel(
-                        delayed(torch.load)(path) for path in paths
-                    ):
-                        energy_scaler.data.append(energy_data)
-            else:
-                for path in tqdm(paths, desc="Gathering energy values"):
-                    energy_data = torch.load(path)
-                    energy_scaler.data.append(energy_data)
+            for path in tqdm(
+                (self.config.preprocessing.save_dir / "energy").glob("*energy*"),
+                desc="Gathering energy values",
+            ):
+                energy_data = torch.load(path)
+                energy_scaler.data.append(energy_data)
         if pitch:
             pitch_scaler = Scaler()
-            # Until Python 3.13, pathlib.Path.glob() doesn't work with symlinks: https://github.com/python/cpython/issues/77609
-            paths = glob(
-                str(self.config.preprocessing.save_dir / "pitch/**/*pitch*"),
-                recursive=True,
-            )
-            if self.cpus > 1:
-                logger.info("Gathering pitch values")
-                with tqdm_joblib_context(tqdm(desc="Gathering pitch values")):
-                    for pitch_data in parallel(
-                        delayed(torch.load)(path) for path in paths
-                    ):
-                        pitch_scaler.data.append(pitch_data)
-            else:
-                for path in tqdm(paths, desc="Gathering pitch values"):
-                    pitch_data = torch.load(path)
-                    pitch_scaler.data.append(pitch_data)
+            for path in tqdm(
+                (self.config.preprocessing.save_dir / "pitch").glob("*pitch*"),
+                desc="Gathering pitch values",
+            ):
+                pitch_data = torch.load(path)
+                pitch_scaler.data.append(pitch_data)
         return energy_scaler if energy else energy, pitch_scaler if pitch else pitch
 
     def normalize_stats(self, energy_scaler: Scaler, pitch_scaler: Scaler):
         """Normalize pitch and energy to unit variance"""
-        # Note: this function is IO bound, because it is a tight loop writing small files.
-        # Attempts to parallelize it make it much slower, even with only 2 threads.
         logger.info("Scaling dataset statistics...")
         stats = {}
         if energy_scaler:
             energy_stats = energy_scaler.calculate_stats()
             for path in tqdm(
-                # Until Python 3.13, pathlib.Path.glob() doesn't work with symlinks: https://github.com/python/cpython/issues/77609
-                glob(
-                    str(self.config.preprocessing.save_dir / "energy/**/*energy*"),
-                    recursive=True,
-                ),
+                (self.config.preprocessing.save_dir / "energy").glob("*energy*"),
                 desc="Normalizing energy values",
             ):
                 energy = torch.load(path)
                 energy = energy_scaler.normalize(energy)
-                save_tensor(energy, path)
+                torch.save(energy, path)
             stats["energy"] = energy_stats
         if pitch_scaler:
             pitch_stats = pitch_scaler.calculate_stats()
             for path in tqdm(
-                # Until Python 3.13, pathlib.Path.glob() doesn't work with symlinks: https://github.com/python/cpython/issues/77609
-                glob(
-                    str(self.config.preprocessing.save_dir / "pitch/**/*pitch*"),
-                    recursive=True,
-                ),
+                (self.config.preprocessing.save_dir / "pitch").glob("*pitch*"),
                 desc="Normalizing pitch values",
             ):
                 pitch = torch.load(path)
                 pitch = pitch_scaler.normalize(pitch)
-                save_tensor(pitch, path)
+                torch.save(pitch, path)
             stats["pitch"] = pitch_stats
 
         return stats
 
     def dataset_sanity_checks(self):
         """Before processing datasets, we should do some sanity checks."""
         for dataset in self.datasets:
             data_dir = Path(dataset.data_dir)
             if not data_dir.exists():
                 logger.error(
                     f"Data directory '{data_dir}' does not exist. Please check your config file."
                 )
-                sys.exit(1)
+                exit()
+
+    def _collect_non_missing_files_from_filelist(self, filelist, data_dir):
+        for f in filelist:
+            audio_path = data_dir / (f["basename"] + ".wav")
+            if not audio_path.exists():
+                logger.warning(f"File '{f}' is missing and will not be processed.")
+                self.counters.missing_files.append(f)
+            else:
+                yield f
 
-    def create_path(self, item: dict, folder: str, fn: str) -> Path:
+    def create_path(self, item: dict, folder: str, fn: str):
         return (
             self.save_dir
             / folder
             / self.sep.join([item["basename"], item["speaker"], item["language"], fn])
         )
 
-    def process_one_audio(
-        self, item: dict, data_dir, sox_effects: list[list]
-    ) -> Optional[dict]:
-        """Process one audio item
-
-        Return:
-           - item if it is found and processed successfully
-           - None otherwise, indicating it should be skipped from further processing
-        """
-        extension = "" if item["basename"].endswith(".wav") else ".wav"
-        audio_path = data_dir / (item["basename"] + extension)
-        if not audio_path.exists():
-            logger.warning(f"File '{item}' is missing and will not be processed.")
-            self.counters.increment("missing_files")
-            return None
-
-        item = self.get_speaker_and_language(item)
-        input_audio_save_path = self.create_path(
-            item, "audio", f"audio-{self.input_sampling_rate}.pt"
-        )
-        output_audio_save_path = self.create_path(
-            item, "audio", f"audio-{self.output_sampling_rate}.pt"
-        )
-        if (
-            input_audio_save_path.exists()
-            and output_audio_save_path.exists()
-            and not self.overwrite
-        ):
-            audio, sr, seconds = self.load_audio(audio_path)
-            self.counters.increment("previously_processed_files")
-            self.counters.increment("duration", seconds)
-            return item
-        if not input_audio_save_path.exists() or self.overwrite:
-            input_audio, _ = self.process_audio(
-                audio_path,
-                resample_rate=self.input_sampling_rate,
-                sox_effects=sox_effects,
-            )
-            if input_audio is None:
-                return None
-            else:
-                save_tensor(input_audio, input_audio_save_path)
-        if (
-            self.input_sampling_rate != self.output_sampling_rate
-            and not output_audio_save_path.exists()
-            or self.overwrite
-        ):
-            output_audio, _ = self.process_audio(
-                audio_path,
-                resample_rate=self.output_sampling_rate,
-                sox_effects=sox_effects,
-                update_counters=False,
-            )
-            if output_audio is not None:
-                save_tensor(output_audio, output_audio_save_path)
-        return item
-
-    def process_all_audio(self) -> list[dict]:
+    def process_all_audio(self, debug=False):
         """Process all audio across datasets, create a combined, filtered filelist and return it"""
         self.dataset_sanity_checks()
-        filtered_filelist: list[dict] = []
-        for dataset in tqdm(self.datasets, total=len(self.datasets), desc="Dataset"):
+        filtered_filelist = []
+        for dataset in tqdm(self.datasets, total=len(self.datasets)):
             data_dir = Path(dataset.data_dir)
             filelist = dataset.filelist_loader(dataset.filelist)
-            sox_effects = dataset.sox_effects
-            if self.debug:
+            if debug:
                 filelist = filelist[:10]
                 logger.info(
                     "Debug flag was set to true, only processing first 10 files"
                 )
-            logger.info(f"Collecting files for {dataset.label} and processing audio")
-            if self.cpus * 3 > len(filelist):
-                self.cpus = len(filelist) // 3
-            if self.cpus > 1:
-                logger.info("Launching parallel processes may take a moment...")
-                batch_size = min(100, 1 + len(filelist) // (self.cpus * 2))
-                with tqdm_joblib_context(
-                    tqdm(
-                        desc=f"Processing audio on {self.cpus} CPUs",
-                        total=len(filelist),
+            logger.info(f"Collecting files for {dataset.label}")
+            non_missing_files = list(
+                self._collect_non_missing_files_from_filelist(filelist, data_dir)
+            )
+            for item in tqdm(non_missing_files):
+                item = self.get_speaker_and_language(item)
+                input_audio_save_path = self.create_path(
+                    item, "audio", f"audio-{self.input_sampling_rate}.pt"
+                )
+                output_audio_save_path = self.create_path(
+                    item, "audio", f"audio-{self.output_sampling_rate}.pt"
+                )
+                if (
+                    input_audio_save_path.exists()
+                    and output_audio_save_path.exists()
+                    and not self.overwrite
+                ):
+                    self.counters.skipped_processes += 1
+                    continue
+                if not input_audio_save_path.exists() or self.overwrite:
+                    input_audio, _ = self.process_audio(
+                        data_dir / (item["basename"] + ".wav"),
+                        resample_rate=self.input_sampling_rate,
                     )
+                    if input_audio is None:
+                        continue
+                    else:
+                        filtered_filelist.append(item)
+                        torch.save(input_audio, input_audio_save_path)
+                if (
+                    self.input_sampling_rate != self.output_sampling_rate
+                    and not output_audio_save_path.exists()
+                    or self.overwrite
                 ):
-                    processed_items = Parallel(
-                        n_jobs=self.cpus,
-                        # verbose=10,
-                        backend="loky",
-                        batch_size=batch_size,
-                    )(
-                        delayed(self.process_one_audio)(item, data_dir, sox_effects)
-                        for item in filelist
+                    output_audio, _ = self.process_audio(
+                        data_dir / (item["basename"] + ".wav"),
+                        resample_rate=self.output_sampling_rate,
                     )
-                filtered_filelist.extend(
-                    item for item in processed_items if item is not None
-                )
-            else:
-                for item in tqdm(filelist, desc="Processing Audio on 1 CPU"):
-                    processed_item = self.process_one_audio(item, data_dir, sox_effects)
-                    if processed_item is not None:
-                        filtered_filelist.append(processed_item)
+                    if output_audio is None:
+                        continue
+                    else:
+                        torch.save(output_audio, output_audio_save_path)
         return filtered_filelist
 
     def process_energy(self, item):
-        energy_path = self.create_path(item, "energy", "energy.pt")
-        # Always reprocess energy even without self.overwrite, since its results
-        # depend on the stats of the whole fileset.
         spec_path = self.create_path(
             item,
             "spec",
             f"spec-{self.input_sampling_rate}-{self.audio_config.spec_type}.pt",
         )
+        energy_path = self.create_path(item, "energy", "energy.pt")
         spec = torch.load(spec_path)
         energy = self.extract_energy(spec)
         if (
             isinstance(self.config, FeaturePredictionConfig)
-            and self.config.model.variance_predictors.energy.level == "phone"
+            and self.config.model.variance_adaptor.variance_predictors.energy.level
+            == "phone"
             and not self.config.model.learn_alignment
         ):
             dur_path = self.create_path(item, "duration", "duration.pt")
             durs = torch.load(dur_path)
             energy = self.average_data_by_durations(energy, durs)
-        save_tensor(energy, energy_path)
+        torch.save(energy, energy_path)
 
     def process_pitch(self, item):
-        pitch_path = self.create_path(item, "pitch", "pitch.pt")
-        # Always reprocess pitch even without self.overwrite, since its results
-        # depend on the stats of the whole fileset.
         audio_path = self.create_path(
             item, "audio", f"audio-{self.input_sampling_rate}.pt"
         )
+        pitch_path = self.create_path(item, "pitch", "pitch.pt")
         audio = torch.load(audio_path)
         pitch = self.extract_pitch(audio)
         if (
             isinstance(self.config, FeaturePredictionConfig)
-            and self.config.model.variance_predictors.pitch.level == "phone"
+            and self.config.model.variance_adaptor.variance_predictors.pitch.level
+            == "phone"
             and not self.config.model.learn_alignment
         ):
             dur_path = self.create_path(item, "duration", "duration.pt")
             durs = torch.load(dur_path)
             pitch = self.average_data_by_durations(pitch, durs)
-        save_tensor(pitch, pitch_path)
+        torch.save(pitch, pitch_path)
 
     def process_attn_prior(self, item):
-        attn_prior_path = self.create_path(item, "attn", "attn-prior.pt")
-        if attn_prior_path.exists() and not self.overwrite:
-            return
         binomial_interpolator = BetaBinomialInterpolator()
-        text = self.extract_text_inputs(
-            item["text"], self.text_processor, use_pfs=False, quiet=True
-        )
+        text = self.extract_text_inputs(item["text"], use_pfs=False)
         input_spec_path = self.create_path(
             item,
             "spec",
             f"spec-{self.input_sampling_rate}-{self.audio_config.spec_type}.pt",
         )
+        attn_prior_path = self.create_path(item, "attn", "attn-prior.pt")
         input_spec = torch.load(input_spec_path)
         attn_prior = torch.from_numpy(
             binomial_interpolator(input_spec.size(1), text.size(0))
         )
         assert input_spec.size(1) == attn_prior.size(0)
-        save_tensor(attn_prior, attn_prior_path)
+        torch.save(attn_prior, attn_prior_path)
 
     def process_text(self, item, use_pfs=False):
         basename = "pfs.pt" if use_pfs else "text.pt"
         text_path = self.create_path(item, "text", basename)
-        if text_path.exists() and not self.overwrite:
-            return
-        text = self.extract_text_inputs(
-            item["text"], self.text_processor, use_pfs=use_pfs, quiet=True
-        )
-        save_tensor(text, text_path)
+        text = self.extract_text_inputs(item["text"], use_pfs=use_pfs)
+        torch.save(text, text_path)
 
     def process_spec(self, item):
         input_audio_path = self.create_path(
             item, "audio", f"audio-{self.input_sampling_rate}.pt"
         )
         if not input_audio_path.exists():
-            self.counters.increment("skipped_processes")
+            self.counters.skipped_processes += 1
             logger.info(f"Audio at {input_audio_path} is missing. Skipping...")
             return
         output_audio_path = self.create_path(
             item, "audio", f"audio-{self.output_sampling_rate}.pt"
         )
         input_spec_path = self.create_path(
             item,
             "spec",
             f"spec-{self.input_sampling_rate}-{self.audio_config.spec_type}.pt",
         )
 
+        input_audio = torch.load(input_audio_path)
         if input_audio_path != output_audio_path:
+            output_audio = torch.load(output_audio_path)
             output_spec_path = self.create_path(
                 item,
                 "spec",
                 f"spec-{self.output_sampling_rate}-{self.audio_config.spec_type}.pt",
             )
-            if not output_spec_path.exists() or self.overwrite:
-                output_audio = torch.load(output_audio_path)
-                output_spec = self.extract_spectral_features(
-                    output_audio, self.output_spectral_transform
-                )
-                save_tensor(output_spec, output_spec_path)
-
-        if not input_spec_path.exists() or self.overwrite:
-            input_audio = torch.load(input_audio_path)
-            input_spec = self.extract_spectral_features(
-                input_audio, self.input_spectral_transform
+            output_spec = self.extract_spectral_features(
+                output_audio, self.output_spectral_transform
             )
-            save_tensor(input_spec, input_spec_path)
+            torch.save(output_spec, output_spec_path)
+        else:
+            output_audio = input_audio
+        input_spec = self.extract_spectral_features(
+            input_audio, self.input_spectral_transform
+        )
+        torch.save(input_spec, input_spec_path)
 
     def get_process_fn(self, process):
         if process == "text":
             return functools.partial(self.process_text, use_pfs=False)
         if process == "pfs":
             return functools.partial(self.process_text, use_pfs=True)
         if process == "energy":
@@ -662,180 +628,66 @@
         if process == "pitch":
             return self.process_pitch
         if process == "spec":
             return functools.partial(self.process_spec)
         if process == "attn":
             return self.process_attn_prior
 
-    def check_data(self, filelist, word_seg_token=" ", heavy_clip_detction=False):
-        data = []
-        # speaking rate (words/second, float, scatterplot or bar chart)
-        # speaking rate (characters/second, float, scatterplot or bar chart)
-        # articulation level (mean energy/speaking rate)
-        # unrecognized symbols (bool, list)
-        # duration (float, box plot)
-        # clipping (float, box plot)
-        # silence % (float, box plot)
-        for item in tqdm(filelist, desc="Checking Data"):
-            data_point = {k: v for k, v in item.items()}
-            raw_text = item["text"]
-            n_words = len(raw_text.split(word_seg_token))
-            n_chars = len(self.text_processor.text_to_sequence(raw_text))
-            audio = torch.load(
-                self.create_path(item, "audio", f"audio-{self.input_sampling_rate}.pt")
-            )
-            if heavy_clip_detction:
-                _, total_clipping = detect_clipping(audio)
-            else:
-                # this isn't a great way of detecting clipping,
-                # but it's a lot faster than clipdetect
-                audio_max = audio.max()
-                audio_min = audio.min()
-                total_clipping = (
-                    audio[audio >= audio_max].size(0)
-                    + audio[audio <= audio_min].size(0)
-                    - 2
-                )
-            pitch = torch.load(self.create_path(item, "pitch", "pitch.pt"))
-            energy = torch.load(self.create_path(item, "energy", "energy.pt"))
-            audio_length_s = len(audio) / self.input_sampling_rate
-            data_point["total_clipped_samples"] = total_clipping
-            data_point["pitch_min"] = float(pitch.min())
-            data_point["pitch_max"] = float(pitch.max())
-            data_point["pitch_mean"] = float(pitch.mean())
-            data_point["pitch_std"] = float(pitch.std())
-            data_point["energy_min"] = float(energy.min())
-            data_point["energy_max"] = float(energy.max())
-            data_point["energy_mean"] = float(energy.mean())
-            data_point["energy_std"] = float(energy.std())
-            data_point["duration"] = audio_length_s
-            data_point["speaking_rate_word"] = n_words / audio_length_s
-            data_point["speaking_rate_char"] = n_chars / audio_length_s
-            data_point["articulation_rate_word"] = (
-                data_point["energy_mean"] / data_point["speaking_rate_word"]
-            )
-            data_point["articulation_rate_char"] = (
-                data_point["energy_mean"] / data_point["speaking_rate_char"]
-            )
-            data_point["n_missing_symbols"] = len(
-                self.text_processor.get_missing_symbols(raw_text)
-            )
-            data_point["n_words"] = n_words
-            data_point["n_chars"] = n_chars
-            data.append(data_point)
-        return data
-
-    def load_filelist(self, path: Path):
-        try:
-            filelist = generic_dict_loader(path)
-            if self.debug:
-                logger.info(
-                    "Debug flag was set to true, only processing first 10 files"
-                )
-                filelist = filelist[:10]
-        except FileNotFoundError:
-            logger.error(
-                f"A filelist was not found at {path}. "
-                "Please try processing your audio again."
-            )
-            sys.exit(1)
-        return filelist
-
     def preprocess(
         self,
-        output_path="filelist.psv",
+        output_path="processed_filelist.psv",
         cpus=min(5, mp.cpu_count()),
-        to_process=list[str],
+        to_process=List[str],
         overwrite=False,
         debug=False,
     ):
         self.overwrite = overwrite
-        self.cpus = cpus
-        self.debug = debug
-        if not isinstance(output_path, Path):
-            output_path = Path(output_path)
-        processing_order = ("audio", "text", "pfs", "spec", "attn", "energy", "pitch")
-        random.seed(self.config.preprocessing.dataset_split_seed)
-        processed_filelist = self.save_dir / output_path.name
+        processing_order = ["audio", "text", "pfs", "spec", "attn", "energy", "pitch"]
+
         for process in processing_order:
             if process not in to_process:
                 continue
             (self.save_dir / process).mkdir(parents=True, exist_ok=True)
             if process == "audio":
-                if filelist := self.process_all_audio():
-                    write_filelist(filelist, processed_filelist)
-                    # sample the validation set and subtract it from the whole dataset to determine the training set
-                    random.shuffle(filelist)
-                    train_split = int(
-                        len(filelist) * self.config.preprocessing.train_split
-                    )
-                    write_filelist(
-                        filelist[:train_split],
-                        self.save_dir / f"training_{output_path.name}",
-                    )
-                    write_filelist(
-                        filelist[train_split:],
-                        self.save_dir / f"validation_{output_path.name}",
-                    )
+                if filelist := self.process_all_audio(debug=debug):
+                    write_filelist(filelist, self.save_dir / output_path)
                     report = self.report()
                     with open(self.save_dir / "summary.txt", "w", encoding="utf8") as f:
                         f.write(report)
-                    rich_print(report)
-                else:
-                    logger.error(
-                        "Your filtered audio filelist is empty. Nothing to process."
-                    )
-                    sys.exit(1)
-                # logger.info(f"Audio Filelist len={len(filelist or [])}")
-            elif process in ["text", "pfs"]:
-                # We split out the "text" step to issue the missing symbol warnings
-                filelist = self.load_filelist(processed_filelist)
-                process_fn = self.get_process_fn(process)
-                missing_symbols_before = Counter(self.text_processor.missing_symbols)
-                for f in tqdm(filelist, desc=f"Processing {process} on 1 CPU"):
-                    process_fn(f)
-                # if only one of "pfs" or "text" is specified, missing_symbols_before
-                # will always be empty, but if both are specified this makes sure
-                # each process gets only its own missing symbols logged.
-                new_missing_symbols = (
-                    self.text_processor.missing_symbols - missing_symbols_before
-                )
-                for symbol, count in new_missing_symbols.items():
-                    logger.warning(
-                        f"Symbol '{symbol}' occurs {n_times(count)} but was not declared in your configuration so it is being ignored."
-                    )
+                    print(report)
             else:
                 # If audio has already been processed, then just read the processed_filelist
-                filelist = self.load_filelist(processed_filelist)
-                process_fn = self.get_process_fn(process)
-                logger.info(f"Processing {process} on {self.cpus} CPUs...")
-                # logger.info(f"Filelist len={len(filelist or [])}")
-                if self.cpus > 1:
-                    batch_size = min(100, 1 + len(filelist) // (self.cpus * 2))
-                    with tqdm_joblib_context(
-                        tqdm(
-                            desc=f"Processing {process} on {self.cpus} CPUs",
-                            total=len(filelist),
+                try:
+                    filelist = generic_dict_loader(self.save_dir / output_path)
+                    if debug:
+                        logger.info(
+                            "Debug flag was set to true, only processing first 10 files"
                         )
+                        filelist = filelist[:10]
+                except FileNotFoundError:
+                    logger.error(
+                        f"A filelist was not found at {self.save_dir / output_path}. Please try processing your audio again."
+                    )
+                    exit()
+                process_fn = self.get_process_fn(process)
+                logger.info(f"Processing {process} on {cpus} CPUs...")
+                if cpus:
+                    pool = Pool(nodes=cpus)
+                    for _ in tqdm(
+                        pool.uimap(process_fn, filelist), total=len(filelist)
                     ):
-                        Parallel(
-                            n_jobs=self.cpus,
-                            backend="loky",
-                            batch_size=batch_size,
-                        )(delayed(process_fn)(file) for file in filelist)
+                        pass
                 else:
-                    for f in tqdm(filelist, desc=f"Processing {process} on 1 CPU"):
+                    for f in tqdm(filelist):
                         process_fn(f)
         if "audio" in to_process:
             report = f"Here is a report:\n {self.report()}"
-            if not self.counters.value("duration"):
-                report += "\n\nWARNING: No audio files were processed."
         else:
             report = ""
-        rich_print(
+        print(
             Panel(
                 f"You've finished preprocessing: {', '.join(to_process)}. Your files are located at {self.save_dir.absolute()}. {report}",
                 title="Congratulations 🎉",
                 subtitle="Next Steps Documentation: https://roedoejet.github.io/EveryVoice/guides/custom.html",
                 border_style=Style(color="#0B4F19"),
             )
         )
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/tests/test_dataloader.py` & `everyvoice-0.1.20230307/everyvoice/tests/test_configs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,85 @@
-#!/usr/bin/env python
+import json
+from pathlib import Path
+from unittest import TestCase, main
 
-from tqdm import tqdm
+import yaml
 
-from everyvoice.dataloader import BaseDataModule
-from everyvoice.dataloader.imbalanced_sampler import ImbalancedDatasetSampler
-from everyvoice.model.aligner.config import AlignerConfig
+from everyvoice.config import CONFIGS
+from everyvoice.config import __file__ as everyvoice_file
 from everyvoice.model.e2e.config import EveryVoiceConfig
-from everyvoice.model.feature_prediction.config import FeaturePredictionConfig
-from everyvoice.model.vocoder.config import VocoderConfig
-from everyvoice.model.vocoder.HiFiGAN_iSTFT_lightning.hfgl.config import (
-    HiFiGANTrainingConfig,
-)
-from everyvoice.model.vocoder.HiFiGAN_iSTFT_lightning.hfgl.dataset import (
-    HiFiGANDataModule,
-    SpecDataset,
-)
-from everyvoice.tests.basic_test_case import BasicTestCase
-from everyvoice.tests.test_preprocessing import PreprocessingTest
+from everyvoice.utils import expand_config_string_syntax, lower
 
 
-class DataLoaderTest(BasicTestCase):
-    """Basic test for dataloaders"""
+class ConfigTest(TestCase):
+    """Basic test for hyperparameter configuration"""
 
-    lj_preprocessed = PreprocessingTest.lj_preprocessed
+    data_dir = Path(__file__).parent / "data"
 
     def setUp(self) -> None:
-        super().setUp()
-        PreprocessingTest.preprocess()  # Generate some preprocessed test data
-        self.config = EveryVoiceConfig(
-            contact=self.contact,
-            aligner=AlignerConfig(contact=self.contact),
-            feature_prediction=FeaturePredictionConfig(contact=self.contact),
-            vocoder=VocoderConfig(
-                contact=self.contact,
-                training=HiFiGANTrainingConfig(
-                    training_filelist=self.lj_preprocessed
-                    / "training_preprocessed_filelist.psv",
-                    validation_filelist=self.lj_preprocessed
-                    / "validation_preprocessed_filelist.psv",
-                ),
-            ),
+        with open(Path(everyvoice_file).parent / "base" / "base_composed.yaml") as f:
+            self.yaml_config = yaml.safe_load(f)
+            self.config = EveryVoiceConfig(**self.yaml_config)
+
+    def test_update_from_file(self):
+        """Test that updating the config from yaml/json works"""
+        with open(self.data_dir / "update.json") as f:
+            update = json.load(f)
+        self.config.update_config(update)
+        with open(self.data_dir / "update.yaml") as f:
+            update = yaml.safe_load(f)
+        self.config.update_config(update)
+        self.assertEqual(self.config.feature_prediction.training.batch_size, 123)
+        self.assertEqual(self.config.vocoder.training.batch_size, 456)
+
+    def test_string_to_dict(self):
+        base_config = EveryVoiceConfig.load_config_from_path()
+        test_string = "vocoder.training.gan_type=wgan"
+        test_bad_strings = [
+            "vocoder.training.gan_type==wgan",
+            "vocoder.training.gan_typewgan",
+        ]
+        # test_missing = ["training.foobar.gan_type=original"]
+        test_dict = expand_config_string_syntax(test_string)
+        self.assertEqual(test_dict, {"vocoder": {"training": {"gan_type": "wgan"}}})
+        for bs in test_bad_strings:
+            with self.assertRaises(ValueError):
+                expand_config_string_syntax(bs)
+
+        self.assertEqual(base_config.vocoder.training.gan_type, "original")
+        config = base_config.combine_configs(base_config, test_dict)
+        self.assertEqual(config["vocoder"]["training"]["gan_type"], "wgan")
+
+    def test_changes(self):
+        """Test that the changes to the config are correct"""
+        self.config.update_config(
+            {"feature_prediction": {"text": {"symbols": {"pad": "FOO"}}}}
         )
-        self.config.vocoder.preprocessing.save_dir = self.lj_preprocessed
-        self.config.vocoder.training.training_filelist = (
-            self.lj_preprocessed / "preprocessed_filelist.psv"
+        self.assertEqual(self.config.feature_prediction.text.symbols.pad, "FOO")
+        self.config.update_config(
+            {"feature_prediction": {"text": {"cleaners": ["everyvoice.utils.lower"]}}}
         )
+        self.assertEqual(self.config.feature_prediction.text.cleaners, [lower])
+        self.assertEqual(self.config.feature_prediction.text.symbols.pad, "FOO")
 
-    def test_base_data_loader(self):
-        bdm = BaseDataModule(self.config.aligner)
-        with self.assertRaises(NotImplementedError):
-            bdm.load_dataset()
-
-    def test_spec_dataset(self):
-        dataset = SpecDataset(
-            self.config.vocoder.training.filelist_loader(
-                self.config.vocoder.training.training_filelist
-            ),
-            self.config.vocoder,
-            use_segments=True,
+    def test_shared_sox(self):
+        """Test that the shared sox config is correct"""
+        config: EveryVoiceConfig = EveryVoiceConfig.load_config_from_path(CONFIGS["openslr"])
+        sox_effects = config.vocoder.preprocessing.source_data[0].sox_effects
+        self.assertEqual(len(config.vocoder.preprocessing.source_data), 4)
+        for d_other in config.vocoder.preprocessing.source_data[1:]:
+            self.assertEqual(sox_effects, d_other.sox_effects)
+            self.assertEqual(sox_effects[0], ["channels", "1"])
+
+    def test_correct_number_typing(self):
+        batch_size = 64.0
+        config = EveryVoiceConfig.load_config_from_path()
+        config.update_config(
+            {"feature_prediction": {"training": {"batch_size": batch_size}}}
         )
-        for sample in tqdm(dataset):
-            spec, audio, basename, spec_from_audio = sample
-            self.assertTrue(isinstance(basename, str))
-            self.assertEqual(spec.size(), spec_from_audio.size())
-            self.assertEqual(
-                spec.size(0), self.config.vocoder.preprocessing.audio.n_mels
-            )
-            self.assertEqual(
-                spec.size(1),
-                self.config.vocoder.preprocessing.audio.vocoder_segment_size
-                / (
-                    self.config.vocoder.preprocessing.audio.fft_hop_size
-                    * (
-                        self.config.vocoder.preprocessing.audio.output_sampling_rate
-                        // self.config.vocoder.preprocessing.audio.input_sampling_rate
-                    )
-                ),
-            )
-
-    def test_hifi_data_loader(self):
-        hfgdm = HiFiGANDataModule(self.config.vocoder)
-        hfgdm.load_dataset()
-        self.assertEqual(len(hfgdm.train_dataset), 5)
-
-    def test_hifi_ft_data_loader(self):
-        """TODO: can't make this test until I generate some synthesized samples"""
-        pass
-
-    def test_feature_prediction_data_loader(self):
-        # TODO: once feature prediction is done
-        pass
-
-    def test_e2e_data_module(self):
-        # TODO: once e2e is done
-        pass
-
-    def test_imbalanced_sampler(self):
-        dataset = SpecDataset(
-            self.config.vocoder.training.filelist_loader(
-                self.config.vocoder.training.training_filelist
-            ),
-            self.config.vocoder,
-            use_segments=True,
-        )
-        sampler = ImbalancedDatasetSampler(dataset)
-        sample = list(sampler)
-        self.assertEqual(len(sample), 5)
+        self.assertIsInstance(batch_size, float)
+        self.assertEqual(config.feature_prediction.training.batch_size, 64)
+        self.assertIsInstance(config.feature_prediction.training.batch_size, int)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/text/__init__.py` & `everyvoice-0.1.20230307/everyvoice/text/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from collections import Counter
 from itertools import chain
 from typing import Dict, List, Union
 
 from loguru import logger
 from nltk.tokenize import RegexpTokenizer
 
-from everyvoice.exceptions import ConfigError
+from everyvoice.config import ConfigError
 from everyvoice.model.aligner.config import AlignerConfig
 from everyvoice.model.feature_prediction.config import FeaturePredictionConfig
 from everyvoice.text.features import get_features
 
 
 class TextProcessor:
     def __init__(self, config: Union[AlignerConfig, FeaturePredictionConfig]):
         self.config = config
-        self._all_symbols = self.config.text.symbols.model_dump()
+        self._all_symbols = self.config.text.symbols.dict()
         if "pad" in self._all_symbols:
             assert isinstance(self._all_symbols["pad"], str)
         self._pad_symbol = self._all_symbols["pad"]
         # apply longest characters first to apply multigraph symbols first
         self.symbols = sorted(
             list(
                 chain.from_iterable(
@@ -27,15 +27,15 @@
                 )
             ),
             key=len,
             reverse=True,
         )
         self.symbols.insert(0, self._pad_symbol)
 
-        self.to_replace = config.text.model_dump().get("to_replace", {})
+        self.to_replace = config.text.dict().get("to_replace", {})
         self.missing_symbols: Counter[str] = Counter()
         self.duplicate_symbols: Counter[str] = Counter()
 
         # Mappings from symbol to numeric ID and vice versa
         self._symbol_to_id: Dict[str, int] = {}
         self._id_to_symbol: Dict[int, str] = {}
         for i, s in enumerate(self.symbols):
@@ -53,93 +53,87 @@
         )
         self._missing_symbol_finder = RegexpTokenizer(
             "|".join([re.escape(x) for x in self.symbols]),
             gaps=True,
             discard_empty=True,
         )
 
-    def replace_cleaner(self, text: str) -> str:
+    def replace_cleaner(self, text):
         """Given some text and a list of replacement operations in the form of input/output key value pairs,
            return the transformed text.
         Args:
             text (str): The text to be converted
         Returns:
             str: the replaced text
         """
         for k, v in self.to_replace.items():
             text = re.sub(k, v, text)
         return text
 
-    def text_to_sequence(self, text: str, quiet: bool = False):
+    def text_to_sequence(self, text):
         """Converts a string of text to a sequence of IDs corresponding to the symbols in the text.
         Args:
         text: string to convert to a sequence
         cleaner_fns: a list of fns to clean text
         Returns:
         List of integers corresponding to the symbols in the text
         """
         sequence = []
-        clean_tokens = self.text_to_tokens(text, quiet)
+        clean_tokens = self.text_to_tokens(text)
         for symbol in clean_tokens:
             symbol_id = self._symbol_to_id[symbol]
             sequence += [symbol_id]
         return sequence
 
-    def text_to_phonological_features(self, text: str, quiet: bool = False):
+    def text_to_phonological_features(self, text):
         """Converts a string of text to a sequence of IDs corresponding to the symbols in the text.
         Args:
-            text: string to convert to a sequence
-            quiet: suppress warnings
+        text: string to convert to a sequence
+        cleaner_fns: a list of fns to clean text
         Returns:
-            List of phonological feature vectors
+        List of phonological feature vectors
         """
-        clean_text = self.text_to_tokens(text, quiet)
+        clean_text = self.text_to_tokens(text)
         return get_features(clean_text)
 
-    def clean_text(self, text: str) -> str:
+    def clean_text(self, text):
         """Converts some text to cleaned text"""
         text = self.replace_cleaner(text)
         for cleaner_fn in self.config.text.cleaners:
             try:
                 text = cleaner_fn(text)
             except Exception as e:
                 raise ConfigError(
                     f"Cleaner did not work and threw exception {e}"
                 ) from e
         return text
 
-    def text_to_tokens(self, text: str, quiet: bool = False):
+    def text_to_tokens(self, text):
         """Converts a string of text to a sequence of tokens.
         Args:
-            text: string to convert to a sequence
-            quiet: suppress warnings
+        text: string to convert to a sequence
+        cleaner_fns: a list of fns to clean text
         Returns:
-            List of symbols in the text
+        List of symbols in the text
         """
         clean_text = self.clean_text(text)
         clean_tokens = self._tokenizer.tokenize(clean_text)
         for symbol in self._missing_symbol_finder.tokenize(clean_text):
-            if not quiet:
-                logger.warning(
-                    f"Symbol '{symbol}' occurs in the text '{clean_text}' but was not declared in your configuration so it is being ignored."
-                )
+            logger.warning(
+                f"Symbol '{symbol}' occurs in the text '{clean_text}' but was not declared in your configuration so it is being ignored."
+            )
             self.missing_symbols[symbol] += 1
         return clean_tokens
 
-    def get_missing_symbols(self, text):
-        """Helper function to return a list of symbols missing from configuration."""
-        clean_text = self.clean_text(text)
-        return self._missing_symbol_finder.tokenize(clean_text)
-
     def cleaned_text_to_sequence(self, cleaned_text):
         """Converts a string of text to a sequence of IDs corresponding to the symbols in the text.
         Args:
-            text: string to convert to a sequence
+        text: string to convert to a sequence
         Returns:
-            List of integers corresponding to the symbols in the text
+        List of integers corresponding to the symbols in the text
         """
         cleaned_text = self._tokenizer.tokenize(cleaned_text)
         return [self._symbol_to_id[symbol] for symbol in cleaned_text]
 
     def token_sequence_to_text_sequence(self, sequence) -> List[str]:
         """Converts a sequence of IDs to a sequence of text characters"""
         return [self._id_to_symbol[symbol_id] for symbol_id in sequence]
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/text/features.py` & `everyvoice-0.1.20230307/everyvoice/text/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
             "í",
             "ṹː",
             "ṹ",
             "óː",
             "ó",
         ]
     ]
-    low_tone_chars = [normalize("NFC", x) for x in ["òː", "ũ̀ː", "ìː", "èː", "ʌ̃̀ː", "àː"]]
+    low_tone_chars = [
+        normalize("NFC", x) for x in ["òː", "ũ̀ː", "ìː", "èː", "ʌ̃̀ː", "àː"]
+    ]
     for char in text:
         char = normalize("NFC", char)
         if char in high_tone_chars:
             tone_features.append([-1, 1, -1, -1, -1, -1, -1])
         elif char in low_tone_chars:
             tone_features.append([-1, -1, -1, -1, -1, -1, -1])
         else:
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/utils/__init__.py` & `everyvoice-0.1.20230307/everyvoice/utils/cli_wizard.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,463 +1,342 @@
-import csv
+# This module contains helper functions for use with the configuration wizard CLI
+#
+#
 import json
-import os
-import re
+import string
 import sys
-from contextlib import contextmanager
-from datetime import datetime
-from itertools import islice
-from os.path import splitext
+from collections import Counter
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Dict, List, Tuple, Union
 from unicodedata import normalize
 
+import simple_term_menu
+import typer
 import yaml
+from g2p import make_g2p
+from g2p.exceptions import InvalidLanguageCode, NoPath
+from g2p.transducer import CompositeTransducer
 from loguru import logger
-from pydantic import ValidationInfo
+from pydantic import BaseModel
+from readalongs.util import get_langs
+from rich import print
+from rich.panel import Panel
+from tqdm import tqdm
+
+from everyvoice.utils import lower, nfc_normalize
 
-from everyvoice import exceptions
 
-# Regular expression matching whitespace:
-_whitespace_re = re.compile(r"\s+")
-# Regular expression matching non-slug characters:
-special_chars = re.compile(r"[\W]+")
+def get_single_lang_information(
+    supported_langs, unsupported_langs
+) -> Tuple[Union[None, Dict[str, str]], Union[None, Dict[str, str]]]:
+    """Get language information for the user's dataset through terminal prompts
 
+    Returns:
+        Tuple[Union[None, Dict[str, str]], Union[None, Dict[str, str]]]: A tuple containing the selected language or None
+    """
+    supported_langs_choices = ["[none]: my language isn't here"] + [
+        f"[{k}]: {v}" for k, v in supported_langs
+    ]
+    all_langs_choices = [f"[{lang.alpha_3}]: {lang.name}" for lang in unsupported_langs]
+    supported_langs_choice: int = get_menu_prompt(  # type: ignore
+        "Which of the following supported languages are in your dataset?",
+        supported_langs_choices,
+        multi=False,
+        search=True,
+    )
+    unsupported_langs_choice = None
+    if supported_langs_choice == 0:
+        unsupported_langs_choice: int = get_menu_prompt(  # type: ignore
+            "Please select all the languages in your dataset:",
+            all_langs_choices,
+            multi=False,
+            search=True,
+        )
+    return (
+        supported_langs[supported_langs_choice] if supported_langs_choice else None,
+        unsupported_langs[unsupported_langs_choice]
+        if unsupported_langs_choice
+        else None,
+    )
 
-def slugify(
-    text: str, repl: str = "-", limit_to_n_characters: Optional[int] = None
-) -> str:
-    """Create a slugified representation of input text
-       (i.e. without special characters) and optionally
-       limited to a specific number of characters.
-
-       >>> slugify('gya?a')
-       'gya-a'
-
-       >>> slugify('gya?a', repl='')
-       'gyaa'
-
-       >>> slugify('gya?a', limit_to_n_characters=3)
-       'gya'
 
-       >>> slugify('!@#$%^&*(){}<>? :;|+=/\\'"', limit_to_n_characters=3)
-       '-'
+def get_symbols_from_g2p_mapping(in_lang: str, out_lang: str) -> Dict[str, List[str]]:
+    try:
+        transducer = make_g2p(in_lang, out_lang)
+    except (InvalidLanguageCode, NoPath) as e:
+        logger.warning(e)
+        return {}
+    if isinstance(transducer, CompositeTransducer):
+        chars = transducer._transducers[-1].mapping.mapping
+    else:
+        chars = transducer.mapping.mapping
+    return {
+        f"{in_lang}_ipa": list({normalize("NFC", c["out"]) for c in chars}),
+        f"{in_lang}_char": list({normalize("NFC", c["in"]) for c in chars}),
+    }
 
-       >>> slugify('!@#$%^&*(){}<>? :;|+=/\\'"', repl='', limit_to_n_characters=3)
-       ''
 
-    Args:
-        text (str): text to slugify
-        repl (str): character to replace special character with. defaults to -
-        limit_to_n_characters (Optional[int]): return first n characters of output
+def get_lang_information() -> Tuple[Dict[str, str], Dict[str, str]]:
+    """Get language information for the user's dataset through terminal prompts
 
     Returns:
-        str: slugified string
+        Tuple[List[Dict[str, str]], List[Dict[str, str]]]: A tuple containing Supported Languages and Unsupported Languages - each are lists of dicts with iso code keys and language name values
     """
-    slugified_text = re.sub(special_chars, repl, text)
+    logger.info("Getting supported languages...")
+    from pycountry import languages
 
-    if limit_to_n_characters is None:
-        return slugified_text
-    else:
-        return slugified_text[:limit_to_n_characters]
+    supported_langs = get_langs()[1].items()
+    all_langs = list(languages)
+    supported_langs_choices = ["[none]: my language isn't here"] + [
+        f"[{k}]: {v}" for k, v in supported_langs
+    ]
+    all_langs_choices = [f"[{lang.alpha_3}]: {lang.name}" for lang in languages]
+    langs: List[int] = get_menu_prompt(  # type: ignore
+        "Which of the following supported languages are in your dataset?",
+        supported_langs_choices,
+        multi=True,
+        search=True,
+    )
+    unsupported_langs: List[int] = []
+    if 0 in langs:
+        unsupported_langs: List[int] = get_menu_prompt(  # type: ignore
+            "Please select all the languages in your dataset:",
+            all_langs_choices,
+            multi=True,
+            search=True,
+        )
+    langs = [x - 1 for x in langs if x]  # remove "none" index from count
+    supported_langs = list(supported_langs)
+    return {supported_langs[i][0]: supported_langs[i][1] for i in langs}, {
+        all_langs[i].alpha_3: all_langs[i].name for i in unsupported_langs
+    }
 
 
-def check_dataset_size(batch_size: int, number_of_samples: int, name: str):
-    if batch_size > number_of_samples:
-        reduce_train_split = (
-            "You can also decrease the train split to increase the number of samples in your validation dataset."
-            if "val" in name
-            else ""
+def get_symbol_set(
+    filelist_data: List[Dict[str, str]],
+    supported_langs,
+    unsupported_langs,
+    to_filter="-';:,.!?¡¿—…\"«»“” ",
+):
+    symbols = {}
+    for lang in supported_langs.keys():
+        if lang == "eng":
+            symbols["eng"] = list(string.ascii_letters)
+        else:
+            symbols = {**symbols, **get_symbols_from_g2p_mapping(lang, f"{lang}-ipa")}
+    for iso, lang in unsupported_langs.items():
+        logger.info(
+            f"We don't support [{iso}] - {lang} so we will just guess. You can always update/change the symbol set in your configuration file later."
         )
-        logger.error(
-            f"Your {name} dataset only has {number_of_samples} samples, but you have a defined batch size of {batch_size}. Please either add more data or decrease your batch size. {reduce_train_split}"
+        possible_values = [iso, lang, "default"]
+        possible_text_transformations = ["none", lower, nfc_normalize]
+        text_transformations: List[int] = get_menu_prompt(  # type: ignore
+            f"Please select all the text transformations to apply to [{iso}] - {lang} before determining symbol set:",
+            [
+                "None",
+                "Lowercase",
+                "NFC Normalization - See here for more information: https://withblue.ink/2019/03/11/why-you-need-to-normalize-unicode-strings.html",
+            ],
+            multi=True,
         )
-        sys.exit(1)
-
+        chars = set()
+        for row in tqdm(filelist_data):
+            row_lang = row["language"]
+            if row_lang in possible_values:
+                text = row["text"]
+                if 0 not in text_transformations:
+                    for t in text_transformations:
+                        text = possible_text_transformations[t](text)
+                for c in text:
+                    chars.add(c)
+        symbols[iso] = [
+            x for x in chars if x not in to_filter
+        ]  # filter default punctuation
+    return {k: sorted(v) for k, v in symbols.items()}
+
+
+def auto_check_audio(
+    filelist_data: List[Dict[str, str]], wavs_dir: Path
+) -> Tuple[int, float, float]:
+    """Check all audio with basenames from filelist in wavs_dir and return the sampling rate,
+    min length rounded down (seconds), and max length rounded up (seconds). Log warnings if less than
+    0.25 seconds or longer that 11 seconds.
+    """
+    import math
+
+    srs_counter: Counter[int] = Counter()
+    logger.info("🧙 is checking your audio. please wait...")
+    lengths = []
+    from scipy import signal
+    from scipy.io import wavfile
 
-def return_configs_from_dir(dir: Path) -> Dict[str, Path]:
-    return {os.path.basename(path)[:-5]: path for path in dir.glob("*.yaml")}
-
-
-def get_current_time():
-    return str(int(datetime.now().timestamp()))
-
-
-def _flatten(structure, key="", path="", flattened=None):
-    """
-    >>> _flatten({"a": {"b": 2, "c": {"d": "e"}, "f": 4}, "g": 5})
-    {'a_b': 2, 'a_c_d': 'e', 'a_f': 4, 'g': 5}
-    """
-    if flattened is None:
-        flattened = {}
-    if not isinstance(structure, dict):
-        flattened[(f"{path}_" if path else "") + key] = structure
-    else:
-        for new_key, value in structure.items():
-            _flatten(value, new_key, (f"{path}_" if path else "") + key, flattened)
-    return flattened
-
-
-def load_config_from_json_or_yaml_path(path: Path):
-    if not path.exists():
-        raise ValueError(f"Config file '{path}' does not exist")
-    with open(path, "r", encoding="utf8") as f:
-        config = json.load(f) if path.suffix == ".json" else yaml.safe_load(f)
-    if not config:
-        raise exceptions.InvalidConfiguration(f"Your configuration at {path} was empty")
-    return config
-
-
-def expand_config_string_syntax(config_arg: str) -> dict:
-    """Expand a string of the form "key1=value1" into a dict."""
-    config_dict: Any = {}
-    try:
-        key, value = config_arg.split("=")
-    except ValueError as e:
-        raise ValueError(f"Invalid config string: {config_arg} - missing '='") from e
-    current_dict = config_dict
-    keys = key.split(".")
-    for key in keys[:-1]:
-        current_dict[key] = {}
-        current_dict = current_dict[key]
-    current_dict[keys[-1]] = value
-    return config_dict
-
-
-def update_config_from_cli_args(arg_list: List[str], original_config):
-    if arg_list is None or not arg_list:
-        return original_config
-    for arg in arg_list:
-        key, value = arg.split("=")
-        logger.info(f"Updating config '{key}' to value '{value}'")
-        original_config = original_config.update_config(
-            expand_config_string_syntax(arg)
+    double_check = typer.confirm(
+        "The configuration wizard can double check that your declared sampling rate is correct by analyzing the spectrogram. Would you like to do this? It will mean that your processing takes longer."
+    )
+    for d in tqdm(filelist_data):
+        audio_path = wavs_dir / (d["basename"] + ".wav")
+        try:
+            samplerate, data = wavfile.read(audio_path)
+        except FileNotFoundError:
+            logger.warning(
+                f"File '{audio_path}' was not found. Please ensure the file exists and your filelist is created properly."
+            )
+            continue
+        if double_check:
+            frequencies, _, spectrogram = signal.spectrogram(data, samplerate)
+            energy_threshold = None
+            n_empty_bands = 0
+            for i, band in enumerate(spectrogram):
+                if sum(band) < 0.1:
+                    if n_empty_bands == 0:
+                        energy_threshold = int(frequencies[i])
+                    n_empty_bands += 1
+                    if n_empty_bands > 4:
+                        logger.warning(
+                            f"File '{audio_path} was labelled as having a sampling rate of {samplerate}, but it appears to lose energy at around {energy_threshold}Hz. We'll skip this file."
+                        )
+        srs_counter[samplerate] += 1
+        lengths.append(data.shape[0] / samplerate)
+    for k, v in srs_counter.items():
+        logger.info(f"{v} audio files found at {k}Hz sampling rate")
+    if not srs_counter:
+        logger.error(f"Couldn't read any files at {wavs_dir}. Please check your path.")
+        exit()
+    sr = min(srs_counter.keys())
+    logger.info(f"Using {sr}Hz sampling rate")
+    min_s = min(lengths)
+    if min_s < 0.25:
+        logger.warning(
+            f"Shortest sample was {min_s} seconds long - this is probably too short. Please remove all audio shorter than 0.25 seconds."
         )
-    return original_config
-
-
-def relative_to_absolute_path(
-    value: Any, info: Optional[ValidationInfo] = None
-) -> Path | None:
-    """
-    Helper function to annotate a type.
-    This function processes relative paths and either resolve them to absolute
-    paths or resolve them with respect to the configuration file they came
-    from.
-    """
-    if value is None:
-        return value
-
-    try:
-        # Make sure value is a path because it can be a string when we load a
-        # model that is not partial.
-        path = Path(value)
-        if (
-            not path.is_absolute()
-            and info
-            and info.context
-            and (config_path := info.context.get("config_path", None))
-        ):
-            path = (config_path.parent / path).resolve()
-        return path
-    except TypeError as e:
-        # Pydantic needs ValueErrors to raise its ValidationErrors
-        raise ValueError from e
-
-
-def directory_path_must_exist(
-    value: Any, info: Optional[ValidationInfo] = None
-) -> Path | None:
-    """
-    Helper function to annotate a type.
-    Creates a directory if it doesn't exist.
-    """
-    assert isinstance(value, Path)
-    if (
-        info
-        and info.context
-        and (writing_config := info.context.get("writing_config", None))
-    ):
-        # We are writing the original config and must temporarily resolve the path.
-        (writing_config.resolve() / value).mkdir(parents=True, exist_ok=True)
     else:
-        if not value.exists():
-            logger.info(f"Directory at {value} does not exist. Creating...")
-            value.mkdir(parents=True, exist_ok=True)
-
-    return value
-
-
-def path_is_a_directory(
-    value: Any, info: Optional[ValidationInfo] = None
-) -> Path | None:
-    """
-    Helper function to annotate a type.
-    Verifies ala `PathType("dir")` that `value` is a directory.
-    """
-    if (
-        info
-        and info.context
-        and (writing_config := info.context.get("writing_config", None))
-    ):
-        # We are writing the original config and must temporarily resolve the path.
-        tmp_path = writing_config.resolve() / value
-        if not tmp_path.is_dir():
-            raise ValueError(f"{tmp_path} is not a directory")
+        logger.info(f"Shortest sample was {min_s} seconds long")
+    max_s = max(lengths)
+    if max_s > 11:
+        logger.warning(
+            f"Longest sample was {max_s} seconds long - this is probably too long, and may result in longer training times or force you to use a reduced batch size. Please remove all audio longer than 11 seconds."
+        )
     else:
-        try:
-            # Make sure value is a path because it can be a string when we load a model that is not partial.
-            path = Path(value)
-            if not path.is_dir():
-                raise ValueError(f"{path} is not a directory")
-        except TypeError as e:
-            # Pydantic needs ValueErrors to raise its ValidationErrors
-            raise ValueError from e
-
-    return value
+        logger.info(f"Longest sample was {max_s} seconds long")
+    return sr, float(math.floor(min_s)), float(math.ceil(max_s))
 
 
-def original_hifigan_leaky_relu(x):
-    import torch.nn.functional as F
+def get_menu_prompt(
+    prompt_text: str, choices: List[str], multi=False, search=False
+) -> Union[int, List[int]]:
+    """Given some prompt text and a list of choices, create a simple terminal window
+       and return the index of the choice
 
-    return F.leaky_relu(x, 0.1)
-
-
-def plot_spectrogram(spectrogram):
-    import matplotlib.pylab as plt
+    Args:
+        prompt_text (str): rich prompt text to print before menu
+        choices (List[str]): choices to display
 
-    fig, ax = plt.subplots(figsize=(10, 2))
-    im = ax.imshow(spectrogram, aspect="auto", origin="lower", interpolation="none")
-    plt.colorbar(im, ax=ax)
+    Returns:
+        int: index of choice
+    """
+    print(Panel(prompt_text))
+    menu = simple_term_menu.TerminalMenu(
+        choices,
+        multi_select=multi,
+        show_multi_select_hint=multi,
+        show_search_hint=search,
+    )
+    index = menu.show()
+    sys.stdout.write("\033[K")
+    if index is None:
+        exit()
+    return index
 
-    fig.canvas.draw()
-    plt.close()
 
-    return fig
+def get_required_headers(headers: List[str], sample_data: List[List[str]]) -> List[str]:
+    """Given some headers and sample data, prompt the user to specify which column is text and which column is basenames
+       the basename should be unique for each audio file and should be without a file extension.
 
+    Args:
+        headers (List[str]): hypothesized list of headers
+        sample_data (List[List[str]]): sample data from reading in filelist in psv format (like LJSpeech metadata file)
 
-def write_filelist(files, path):
-    with open(path, "w", encoding="utf8") as f:
-        if not files:
-            logger.warning(f"Writing empty filelist file {path}")
-            print("", file=f)  # header line, empty because we don't know the fields
-            return
-        writer = csv.DictWriter(
-            f,
-            fieldnames=files[0].keys(),
-            delimiter="|",
-            quoting=csv.QUOTE_NONE,
-            escapechar="\\",
-        )
-        writer.writeheader()
-        for f in files:
-            writer.writerow(f)
+    Returns:
+        List[str]: revised list of headers
+    """
+    text_column: int = get_menu_prompt(  # type: ignore
+        "These are the values from the first row in your data. Which column contains the [bold blue]text?",
+        [str(f"{x}: {sample_data[0][x]}") for x in range(len(headers))],
+    )
+    bn_column: int = get_menu_prompt(  # type: ignore
+        "Which column contains the [bold blue]basenames?",
+        [
+            str(f"{x}: {sample_data[0][x]}")
+            for x in range(len(headers))
+            if str(x) != text_column
+        ],
+    )
+    headers[text_column] = "text"
+    headers[bn_column] = "basename"
+    return headers
 
 
-def lower(text):
-    """
-    >>> lower("MiXeD ÇÀSÉ")
-    'mixed çàsé'
-    """
-    return text.lower()
+def create_default_filelist(
+    data: List[List[str]], headers: List[str]
+) -> List[Dict[str, str]]:
+    """Given a list of row data (list of cell strings), and a list of headers, produce a list
+        of dicts that could be read by csv.DictReader and written by csv.DictWriter
 
+    Args:
+        data (List[List[str]]): spreadsheet row data
+        headers (List[str]): list of headers
 
-def nfc_normalize(text):
-    """
-    >>> nfc_normalize("éçà")
-    'éçà'
+    Returns:
+        List[Dict[str, str]]: List of spreadsheet data in dict format
     """
-    return normalize("NFC", text)
-
+    len_data = len(data[0])
+    new_data = []
+    for d in data:
+        data_dict = {
+            h: d[h_i] if h_i < len_data else "default" for h_i, h in enumerate(headers)
+        }
+        new_data.append(data_dict)
+    return new_data
 
-def load_lj_metadata_hifigan(path):
-    with open(path, "r", newline="", encoding="utf8") as f:
-        reader = csv.DictReader(
-            f,
-            fieldnames=["basename", "raw_text", "text"],
-            delimiter="|",
-            quoting=csv.QUOTE_NONE,
-            escapechar="\\",
-        )
-        files = list(reader)
-    return files
 
+def write_config_to_file(config: BaseModel, path: Path):
+    """Given a Pydantic model, convert it to a json object and write as yaml or json
 
-def read_festival(
-    path,
-    record_limit: int = 0,  # if non-zero, read only this many records
-):
-    """Read Festival format into filelist
     Args:
-        path (Path): Path to festival format filelist
-        record_limit: if non-zero, read only that many records
-    Raises:
-        ValueError: the file is not valid festival input
+        config (BaseModel): The Configuration to write
+        path (Path): The output path; must end with either json or yaml
     """
-    festival_pattern = re.compile(
-        r"""
-    (\s*
-    (?P<basename>[\w\d\-\_]*)
-    \s*
-    "(?P<text>[^"]*)"
-     )
-    """,
-        re.VERBOSE,
-    )
-    data = []
-    f: Iterable[str]
-    with open(path, encoding="utf-8") as f:
-        if record_limit:
-            f = islice(f, record_limit)
-        for line in f:
-            if match := re.search(festival_pattern, line.strip()):
-                basename = match["basename"].strip()
-                text = match["text"].strip()
-                data.append({"basename": basename, "text": text})
-            else:
-                raise ValueError(f'File {path} is not in the "festival" format.')
-    return data
-
-
-def sniff_and_return_filelist_data(path):
-    """Sniff csv, and return dialect if not festival format:
-    ( LJ0002 "this is the festival format" )
-    Args:
-        path (Path): path to filelist
-    Returns:
-        False if not csv
-    """
-    festival_pattern = re.compile(r'\( [\w\d_]* "[^"]*" \)')
-    with open(path, newline="", encoding="utf8") as f:
-        data = f.read(1024)
-        f.seek(0)
-        if re.search(festival_pattern, data):
-            return read_festival(path)
+    config = json.loads(config.json())
+    with open(path, "w", encoding="utf8") as f:
+        path_string = str(path)
+        if path_string.endswith("yaml"):
+            yaml.dump(config, f, default_flow_style=None, allow_unicode=True)
         else:
-            dialect = csv.Sniffer().sniff(data)
-            reader = csv.DictReader(f, dialect=dialect)
-            return list(reader)
+            json.dump(config, f, ensure_ascii=False)
 
 
-def generic_dict_loader(
-    path,
-    delimiter="|",
-    quoting=csv.QUOTE_NONE,
-    escapechar="\\",
-    fieldnames=None,
-    file_has_header_line=True,
-):
-    assert fieldnames is not None or file_has_header_line
-    with open(path, "r", newline="", encoding="utf8") as f:
-        reader = csv.DictReader(
-            f,
-            fieldnames=fieldnames,
-            delimiter=delimiter,
-            quoting=quoting,
-            escapechar=escapechar,
-        )
-        # When fieldnames is given, csv.DictReader assumes the first line is a data
-        # line.  Skip it if the file has a header line.
-        if fieldnames and file_has_header_line:
-            next(reader)
-        files = list(reader)
-    return files
-
-
-generic_psv_dict_reader = generic_dict_loader
-
-
-def generic_csv_reader(
-    path,
-    delimiter=",",
-    quoting=csv.QUOTE_NONE,
-    escapechar="\\",
-    record_limit: int = 0,  # if non-zero, read only this many records
-):
-    f: Iterable[str]
-    with open(path, "r", newline="", encoding="utf8") as f:
-        if record_limit:
-            f = islice(f, record_limit)
-        reader = csv.reader(
-            f,
-            delimiter=delimiter,
-            quoting=quoting,
-            escapechar=escapechar,
-        )
-        files = list(reader)
-    return files
-
+def write_dict_to_config(config: Dict, path: Path):
+    """Given an object, write it to file
 
-def collapse_whitespace(text):
-    """
-    >>> collapse_whitespace("  asdf  	   qwer   ")
-    ' asdf qwer '
-    """
-    return re.sub(_whitespace_re, " ", text)
-
-
-def read_filelist(
-    filelist_path: Union[str, os.PathLike],
-    filename_col: int = 0,
-    filename_suffix: str = "",
-    text_col: int = 1,
-    delimiter: str = "|",
-    speaker_col=None,
-    language_col=None,
-):
-    data = []
-    with open(filelist_path, encoding="utf8") as f:
-        reader = csv.reader(f, delimiter=delimiter)
-        for line in reader:
-            fn, _ = splitext(line[filename_col])
-            entry = {"text": line[text_col], "filename": fn + filename_suffix}
-            if speaker_col:
-                entry["speaker"] = line[speaker_col]
-            if language_col:
-                entry["language"] = line[language_col]
-            data.append(entry)
-    return data
-
-
-@contextmanager
-def tqdm_joblib_context(tqdm_instance):
-    """Context manager to make tqdm compatible with joblib.Parallel
-
-    Runs the parallel jobs using joblib, but displays the nicer tqdm progress bar
-    Only tested with tqdm.tqdm, but should also work with tqdm.notepad.tqdm and
-    other variants
-
-    Usage:
-        with tqdm_joblib_context(tqdm(desc="my description", total=len(job_list))):
-            joblib.Parallel(n_jobs=cpus)(delayed(fn)(item) for item in job_list)
+    Args:
+        config (Dict): The Configuration Dict to write
+        path (Path): The output path; must end with either json or yaml
     """
-    import joblib.parallel
-
-    class ParallelCallback(joblib.parallel.BatchCompletionCallBack):
-        def __call__(self, out):
-            tqdm_instance.update(n=self.batch_size)
-            super().__call__(out)
-
-    old_callback = joblib.parallel.BatchCompletionCallBack
-    joblib.parallel.BatchCompletionCallBack = ParallelCallback
-    try:
-        yield
-    finally:
-        tqdm_instance.close()
-        joblib.parallel.BatchCompletionCallBack = old_callback
+    with open(path, "w", encoding="utf8") as f:
+        path_string = str(path)
+        if path_string.endswith("yaml"):
+            yaml.dump(config, f, default_flow_style=None, allow_unicode=True)
+        else:
+            json.dump(config, f, ensure_ascii=False)
 
 
-def n_times(n: int) -> str:
-    """Return a grammatically correct version of n times for n > 0.
-
-    >>> n_times(1)
-    'once'
-    >>> n_times(2)
-    'twice'
-    >>> n_times(1001)
-    '1001 times'
-    """
-    if n == 1:
-        return "once"
-    if n == 2:
-        return "twice"
-    return f"{n} times"
+def create_sox_effects_list(indices: List[str], sr: int):
+    effects = [["channels", "1"]]
+    if "none" in indices:
+        return effects
+    if "resample" in indices:
+        effects.append(["rate", str(sr)])
+    if "norm" in indices:
+        effects.append(["norm", "-3.0"])
+    if "sil-start" in indices:
+        effects.append(["silence", "1", "0.1", "1.0%"])
+    return effects
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/utils/heavy.py` & `everyvoice-0.1.20230307/everyvoice/utils/heavy.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Tuple
 
 import numpy as np
 import torch
 import torchaudio.transforms as T
 from torch.nn.utils.rnn import pad_sequence
 
-from everyvoice.config.preprocessing_config import AudioSpecTypeEnum
 from everyvoice.utils import _flatten
 
 
 def expand(values, durations):
     out = []
     for value, d in zip(values, durations):
         out += [value] * max(0, int(d))
@@ -51,27 +50,27 @@
     win_length,
     hop_length,
     sample_rate=None,
     n_mels=None,
     f_min=0,
     f_max=8000,
 ):
-    if spec_type == AudioSpecTypeEnum.mel.value:
+    if spec_type == "mel-torch":
         return T.MelSpectrogram(
             sample_rate=sample_rate,
             n_fft=n_fft,
             f_min=f_min,
             f_max=f_max,
             win_length=win_length,
             hop_length=hop_length,
             n_mels=n_mels,
             norm="slaney",
             center=True,
         )
-    elif spec_type == AudioSpecTypeEnum.mel_librosa.value:
+    elif spec_type == "mel-librosa":
         from librosa.filters import mel as librosa_mel
 
         transform = T.Spectrogram(
             n_fft=n_fft,
             win_length=win_length,
             hop_length=hop_length,
             pad=0,
@@ -95,21 +94,21 @@
             transform.to(x.device)
             spec = transform(x)
             sine_windowed_spec = torch.sqrt(spec + 1e-9)
             mel = torch.matmul(mel_basis.to(x.device), sine_windowed_spec)
             return mel
 
         return mel_transform
-    elif spec_type == AudioSpecTypeEnum.linear.value:
+    elif spec_type == "linear":
         return T.Spectrogram(
             n_fft=n_fft,
             win_length=win_length,
             hop_length=hop_length,
         )
-    elif spec_type == AudioSpecTypeEnum.raw.value:
+    elif spec_type == "raw":
         return T.Spectrogram(
             n_fft=n_fft,
             win_length=win_length,
             hop_length=hop_length,
             power=None,
         )
     elif spec_type == "istft":
```

### Comparing `everyvoice-0.1.0a0.dev0/everyvoice/wizard/basic.py` & `everyvoice-0.1.20230307/everyvoice/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,451 +1,419 @@
 import json
+from enum import Enum
 from pathlib import Path
+from typing import List
 
 import questionary
-from email_validator import EmailNotValidError, validate_email
+import typer
+from loguru import logger
 from rich import print
 from rich.panel import Panel
+from rich.prompt import Prompt
 from rich.style import Style
+from slugify import slugify
 
-from everyvoice.config.preprocessing_config import Dataset, PreprocessingConfig
-from everyvoice.config.shared_types import (
-    BaseTrainingConfig,
-    ContactInformation,
-    LoggerConfig,
-    init_context,
-)
-from everyvoice.config.text_config import Symbols, TextConfig
-from everyvoice.model.aligner.config import AlignerConfig
-from everyvoice.model.e2e.config import E2ETrainingConfig, EveryVoiceConfig
-from everyvoice.model.feature_prediction.config import (
-    FastSpeech2ModelConfig,
-    FeaturePredictionConfig,
-)
-from everyvoice.model.vocoder.config import VocoderConfig
-from everyvoice.utils import generic_psv_dict_reader, slugify, write_filelist
-from everyvoice.wizard import (
-    ALIGNER_CONFIG_FILENAME_PREFIX,
-    PREPROCESSING_CONFIG_FILENAME_PREFIX,
-    SPEC_TO_WAV_CONFIG_FILENAME_PREFIX,
-    TEXT_CONFIG_FILENAME_PREFIX,
-    TEXT_TO_SPEC_CONFIG_FILENAME_PREFIX,
-    TEXT_TO_WAV_CONFIG_FILENAME_PREFIX,
-    Step,
-    StepNames,
-)
-from everyvoice.wizard.dataset import return_dataset_steps
-from everyvoice.wizard.prompts import (
-    CUSTOM_QUESTIONARY_STYLE,
-    get_response_from_menu_prompt,
-)
-from everyvoice.wizard.utils import write_dict_to_config
-
-
-class NameStep(Step):
-    DEFAULT_NAME = StepNames.name_step
-
-    def prompt(self):
-        return input(
-            "What would you like to call this project? This name should reflect the model you intend to train, e.g. 'my-sinhala-project' or 'english-french-model' or something similarly descriptive of your project: "
+from everyvoice.config import CONFIGS
+from everyvoice.model.aligner.DeepForcedAligner.dfaligner.cli import app as dfaligner_app
+from everyvoice.model.e2e.cli import app as e2e_app
+from everyvoice.model.feature_prediction.FastSpeech2_lightning.fs2.cli import app as fs2_app
+from everyvoice.model.vocoder.HiFiGAN_iSTFT_lightning.hfgl.cli import app as hfgl_app
+
+app = typer.Typer(pretty_exceptions_show_locals=False)
+app.add_typer(dfaligner_app, name="dfa")
+app.add_typer(e2e_app, name="e2e")
+app.add_typer(hfgl_app, name="hifigan")
+app.add_typer(fs2_app, name="fs2")
+
+_config_keys = {k: k for k in CONFIGS.keys()}
+
+CONFIGS_ENUM = Enum("CONFIGS", _config_keys)  # type: ignore
+
+
+class PreprocessCategories(str, Enum):
+    audio = "audio"
+    sox_audio = "sox_audio"
+    pitch = "pitch"
+    mel = "mel"
+    energy = "energy"
+    dur = "dur"
+    text = "text"
+    feats = "feats"
+
+
+class TestSuites(str, Enum):
+    all = "all"
+    configs = "configs"
+    dev = "dev"
+    model = "model"
+    preprocessing = "preprocessing"
+    text = "text"
+
+
+class Model(str, Enum):
+    aligner = "aligner"
+    e2e = "e2e"
+    hifigan = "hifigan"
+    feat = "feat"
+
+
+def output_callback(ctx: typer.Context, value: Path):
+    path = value / slugify(ctx.params["name"])
+    if path.exists():
+        raise typer.BadParameter(
+            f"Sorry, the path at '{path.absolute()}' already exists. Please choose another output directory."
         )
+    return value
 
-    def validate(self, response):
-        if len(response) == 0:
-            print("Sorry, your project needs a name. ")
-            return False
-        sanitized_path = slugify(response)
-        if not sanitized_path == response:
-            print(
-                f"Sorry, the project name '{response}' is not valid, since it will be used to create a folder and special characters are not permitted for folder names. Please re-type something like '{sanitized_path}' instead."
-            )
-            return False
-        return True
 
-    def effect(self):
-        print(
-            f"Great! Launching Configuration Wizard 🧙 for project named '{self.response}'."
-        )
+def questionary_callback(value: str, name: str):
+    path = Path(value)
+    if path.is_file():
+        return f"Sorry, the path at '{path.absolute()}' is a file. Please select a directory."
+    path = path / slugify(name)
+    if path.exists():
+        return f"Sorry, the path at '{path.absolute()}' already exists. Please choose another output directory."
+    return True
 
 
-class ContactNameStep(Step):
-    DEFAULT_NAME = StepNames.contact_name_step
+def questionary_file(value: str):
+    path = Path(value)
+    if path.is_dir():
+        return f"Sorry, the path at '{path.absolute()}' is a directory. Please select a file."
+    return True
 
-    def prompt(self):
-        return input("What is your full name? ")
 
-    def validate(self, response):
-        # Some languages don't use first and last names, so we can't necessarily check that response.split() > 1
-        # It would be nice to have a better check here though.
-        if len(response) < 3:
-            print("Sorry, EveryVoice requires a name to help prevent misuse.")
-            return False
-        return True
-
-    def effect(self):
-        print(f"Great! Nice to meet you, '{self.response}'.")
-
-
-class ContactEmailStep(Step):
-    DEFAULT_NAME = StepNames.contact_email_step
-
-    def prompt(self):
-        return input("Please provide a contact email address for your models. ")
-
-    def validate(self, response):
-        try:
-            # Check that the email address is valid. Turn on check_deliverability
-            # for first-time validations like on account creation pages (but not
-            # login pages).
-            validate_email(response, check_deliverability=True)
-        except EmailNotValidError as e:
-            # The exception message is a human-readable explanation of why it's
-            # not a valid (or deliverable) email address.
-            print("EveryVoice requires a valid email address to prevent misuse.")
-            print(str(e))
-            return False
-        return True
-
-    def effect(self):
-        emailinfo = validate_email(self.response, check_deliverability=False)
-        email = emailinfo.normalized
-        self.response = email
-        print(
-            f"Great! Your contact email '{self.response}' will be saved to your models."
-        )
+def questionary_dir(value: str):
+    path = Path(value)
+    if path.is_file():
+        return f"Sorry, the path at '{path.absolute()}' is a file. Please select a directory."
+    return True
 
 
-class OutputPathStep(Step):
-    DEFAULT_NAME = StepNames.output_step
+@app.command(
+    help="""This command will help you create all the configuration necessary for your using your dataset.
 
-    def prompt(self):
-        return questionary.path(
-            "Where should the Configuration Wizard save your files?",
-            default=".",
-            style=CUSTOM_QUESTIONARY_STYLE,
-            only_directories=True,
-        ).unsafe_ask()
-
-    def sanitize_input(self, response):
-        response = super().sanitize_input(response)
-        return response.strip()
-
-    def validate(self, response) -> bool:
-        path = Path(response)
-        if path.is_file():
-            print(f"Sorry, '{path}' is a file. Please select a directory.")
-            return False
-        assert self.state is not None, "OutputPathStep requires NameStep"
-        output_path = path / self.state.get(StepNames.name_step.value, "DEFAULT_NAME")
-        if output_path.exists():
-            print(
-                f"Sorry, '{output_path}' already exists. Please choose another output directory or start again and choose a different project name."
-            )
-            return False
-        return True
+In order to get started, please:
+ - have your audio data (in .wav format) together in a folder
+ - have a 'metadata' file that minimally has two columns, one for the text of the audio and one for the basename of the file
 
-    def effect(self):
-        assert self.state is not None, "OutputPathStep requires NameStep"
-        output_path = Path(self.response) / self.state.get(
-            StepNames.name_step.value, "DEFAULT_NAME"
-        )
-        output_path.mkdir(parents=True, exist_ok=True)
-        print(f"The Configuration Wizard 🧙 will put your files here: '{output_path}'")
+Inside /path/to/wavs/ you should have wav audio files like test0001.wav, test0002.wav etc - they can be called anything you want. but the part of the file (minus the .wav portion) must be in your metadata file.
 
+Example wavs directory: "/path/to/wavs/"
 
-class ConfigFormatStep(Step):
-    DEFAULT_NAME = StepNames.config_format_step
+Example metadata: https://github.com/roedoejet/EveryVoice/blob/main/everyvoice/filelists/lj_full.psv
 
-    def prompt(self):
-        return get_response_from_menu_prompt(
-            "Which format would you like to output the configuration to?",
-            ("yaml", "json"),
+"""
+)
+def config_wizard(
+    name: str = typer.Option(
+        ...,
+        prompt="What would you like to call this dataset?",
+        help="The name of your dataset.",
+    ),
+):
+    output_dir = Path(
+        questionary.path(
+            "Where should the wizard save your files?",
+            default=".",
+            validate=lambda x: questionary_callback(x, name),
+        ).ask()
+    )
+    wavs_dir = Path(
+        questionary.path("Where are your audio files?", validate=questionary_dir).ask()
+    )
+    filelist_path = Path(
+        questionary.path(
+            "Where is your data filelist?", validate=questionary_file
+        ).ask()
+    )
+    from everyvoice.config.preprocessing_config import (
+        AudioConfig,
+        Dataset,
+        PreprocessingConfig,
+    )
+    from everyvoice.config.shared_types import BaseTrainingConfig, LoggerConfig
+    from everyvoice.config.text_config import Symbols, TextConfig
+    from everyvoice.model.aligner.config import AlignerConfig
+    from everyvoice.model.e2e.config import EveryVoiceConfig
+    from everyvoice.model.feature_prediction.config import FeaturePredictionConfig
+    from everyvoice.model.vocoder.config import VocoderConfig
+    from everyvoice.utils import generic_csv_loader, read_festival, write_dict
+    from everyvoice.utils.cli_wizard import (
+        auto_check_audio,
+        create_default_filelist,
+        create_sox_effects_list,
+        get_lang_information,
+        get_menu_prompt,
+        get_required_headers,
+        get_single_lang_information,
+        get_symbol_set,
+        write_config_to_file,
+        write_dict_to_config,
+    )
+
+    logger.info(
+        f"Great! Launching Configuration Wizard 🧙 for dataset named {name} with audio files at {wavs_dir} and a filelist at {filelist_path}. Files will be output here: {output_dir.absolute()}"
+    )
+    output_path = output_dir / name
+    output_path.mkdir(parents=True, exist_ok=True)
+    # Determine file type
+    file_type_choices = ["psv", "tsv", "csv", "festival"]
+    file_type_choice = get_menu_prompt(
+        "Select which format your filelist is in:",
+        choices=file_type_choices,
+        multi=False,
+        search=False,
+    )
+    file_type = file_type_choices[file_type_choice]
+    if file_type == "csv":
+        delimiter = ","
+    elif file_type == "psv":
+        delimiter = "|"
+    elif file_type == "tsv":
+        delimiter = "\t"
+    filelist_data_dict = None
+    if file_type == "festival":
+        filelist_data_dict = read_festival(filelist_path)
+        headers = list(filelist_data_dict[0].keys())
+        filelist_data = [list(row.values()) for row in filelist_data_dict]
+    else:
+        # Check filelist headers
+        filelist_data = generic_csv_loader(filelist_path, delimiter=delimiter)
+        headers = list(filelist_data[0])
+    if "basename" not in headers or "text" not in headers:
+        logger.info(
+            "Your filelist must minimally contain a 'basename' and 'text' column, but yours does not."
         )
-
-    def validate(self, response):
-        return response in ("yaml", "json")
-
-    def effect(self):
-        output_path = (
-            Path(self.state[StepNames.output_step.value])
-            / self.state[StepNames.name_step.value]
-        ).expanduser()
-        # create_config_files
-        config_dir = output_path / "config"
-        config_dir.absolute().mkdir(exist_ok=True, parents=True)
-        # preprocessed dir
-        preprocessed_dir = output_path / "preprocessed"
-        preprocessed_dir.absolute().mkdir(parents=True, exist_ok=True)
-        # used in configs
-        preprocessed_dir_relative_to_configs = Path("..") / "preprocessed"
-        # log dir
-        log_dir = output_path / "logs_and_checkpoints"
-        log_dir.absolute().mkdir(parents=True, exist_ok=True)
-        log_dir_relative_to_configs = Path("..") / "logs_and_checkpoints"
-        datasets = []
-        # Text Configuration
-        punctuation = []
-        symbols = {}
-        multispeaker = False
-        multilingual = False
-        for dataset in [key for key in self.state.keys() if key.startswith("dataset_")]:
-            dataset_state = self.state[dataset]
-            # Gather Symbols for Text Configuration
-            punctuation += dataset_state[StepNames.symbol_set_step.value].punctuation
-            symbols[f"{dataset}-symbols"] = dataset_state[
-                StepNames.symbol_set_step.value
-            ].symbol_set
-            if (
-                dataset_state.get(StepNames.data_has_language_value_step.value, "no")
-                == "yes"
-            ):
-                multilingual = True
-            if (
-                dataset_state.get(StepNames.data_has_speaker_value_step.value, "no")
-                == "yes"
+        headers = get_required_headers(headers, sample_data=filelist_data[:5])
+    for i, h in enumerate(headers):
+        if h not in ["text", "basename", "speaker", "language"]:
+            headers[i] = f"unknown_{i}"
+    if "speaker" not in headers:
+        spkr_column = Prompt.ask(
+            "Do you have a column for speaker id?",
+            choices=["no"]
+            + [
+                str(x)
+                for x in range(len(headers))
+                if headers[x] not in ["text", "basename"]
+            ],
+            default="no",
+        )
+        if spkr_column != "no":
+            headers[int(spkr_column)] = "speaker"
+    langs_inferred_from_data = None
+    if "language" not in headers:
+        lang_column = Prompt.ask(
+            "Do you have a column for language id?",
+            choices=["no"]
+            + [
+                str(x)
+                for x in range(len(headers))
+                if headers[x] not in ["text", "basename", "speaker"]
+            ],
+            default="no",
+        )
+        if lang_column != "no":
+            headers[int(lang_column)] = "language"
+            langs_inferred_from_data = {x[int(lang_column)] for x in filelist_data}
+    # TODO: test with multilingual and monolingual labelled (with recognized and unrecognized) and unlabelled datasets
+    if langs_inferred_from_data is None:
+        # No language selected
+        ds_supported_langs, ds_unsupported_langs = get_lang_information()
+        number_of_languages = len(ds_supported_langs) + len(ds_unsupported_langs)
+        if number_of_languages > 1:
+            logger.info(
+                "Sorry, if your dataset has more than one language in it, you will have to add this information to your filelist, because the wizard can't guess!"
+            )
+    else:
+        langs_to_convert = (
+            {}
+        )  # we might need to convert some of the names of languages to the recognized iso code
+        logger.info("Getting supported languages...")
+        from pycountry import languages
+        from readalongs.util import get_langs
+
+        supported_langs = get_langs()[1]
+        all_langs = list(languages)
+        ds_supported_langs = {}
+        ds_unsupported_langs = {}
+        for lang in langs_inferred_from_data:
+            if lang in supported_langs and typer.confirm(
+                f"Is the lang in your data labelled {lang} the same as the language {supported_langs[lang]} with the iso code {lang}?"
             ):
-                multispeaker = True
-            # Dataset Configs
-            wavs_dir = Path(dataset_state[StepNames.wavs_dir_step.value]).expanduser()
-            if not wavs_dir.is_absolute():
-                if not output_path.is_absolute():
-                    for _ in config_dir.parts:
-                        wavs_dir = Path("..") / wavs_dir
-                else:
-                    wavs_dir = Path.cwd() / wavs_dir
-            new_filelist_path = (
-                Path("..")
-                / f"{dataset_state[StepNames.dataset_name_step.value]}-filelist.psv"
-            ).expanduser()
-            filelist_data = dataset_state["filelist_data"]
-            for i, entry in enumerate(filelist_data):
-                # Remove .wav if it was added to the basename
-                if entry["basename"].endswith(".wav"):
-                    entry["basename"] = entry["basename"].replace(".wav", "")
-                # Remove unknown columns
-                filelist_data[i] = {
-                    k: v
-                    for k, v in entry.items()
-                    if k is not None and not k.startswith("unknown")
-                }
-            write_filelist(filelist_data, (config_dir / new_filelist_path).absolute())
-            sox_effects = dataset_state["sox_effects"]
-            filelist_loader = generic_psv_dict_reader
-
-            datasets.append(
-                Dataset(
-                    label=dataset,
-                    data_dir=wavs_dir,
-                    filelist=new_filelist_path,
-                    filelist_loader=filelist_loader,
-                    sox_effects=sox_effects,
-                )
+                ds_supported_langs[lang] = supported_langs[lang]
+                continue
+            logger.info(
+                f"We couldn't recognize {lang}. Please choose it from our list:"
+            )
+            new_lang_sup, new_lang_unsup = get_single_lang_information(
+                supported_langs.items(), all_langs
+            )
+            if new_lang_sup:
+                ds_supported_langs = {**ds_supported_langs, **new_lang_sup}
+            if new_lang_unsup:
+                ds_unsupported_langs = {**ds_unsupported_langs, **new_lang_unsup}
+            langs_to_convert[lang] = (
+                supported_langs.keys()[new_lang_sup]
+                if new_lang_sup
+                else all_langs[new_lang_unsup].alpha_3  # type: ignore
+            )
+        if langs_to_convert:
+            # replace all unrecognized languages with recognized ones
+            for k, v in langs_to_convert.items():
+                for i, row in enumerate(filelist_data):
+                    if row[lang_column] == k:
+                        filelist_data[i][lang_column] = v
+    filelist_data = create_default_filelist(filelist_data, headers)
+    symbol_set = Symbols(
+        **get_symbol_set(filelist_data, ds_supported_langs, ds_unsupported_langs)
+    )
+    dataset_filelist = output_path / "filelist.psv"
+    write_dict(dataset_filelist, filelist_data, headers)
+    # Check Audio
+    auto_check = Prompt.ask(
+        "Config Wizard can try to determine the appropriate settings for your audio automatically. Would you like to do that or manually specify information (like sample rates etc)?",
+        choices=["auto", "manual"],
+        default="auto",
+    )
+    if auto_check == "auto":
+        input_sr, min_length, max_length = auto_check_audio(filelist_data, wavs_dir)
+    else:
+        input_sr = int(
+            Prompt.ask(
+                "What is the input sampling rate of your data in Hertz?",
+                default="22050",
             )
-        text_config = TextConfig(
-            symbols=Symbols(punctuation=list(set(punctuation)), **symbols)
         )
-        text_config_path = Path(f"{TEXT_CONFIG_FILENAME_PREFIX}.{self.response}")
-        write_dict_to_config(
-            json.loads(text_config.model_dump_json(exclude_none=False)),
-            (config_dir / text_config_path).absolute(),
+        min_length = 0.25
+        max_length = 11.0
+        logger.info(
+            "Note: the configuration wizard does not currently support super resolution. If you would like to synthesize to a different sampling rate than your input, please visit the docs: https://pathtodocs"
         )
-        # Contact
-        CONTACT_INFO = ContactInformation(
-            contact_name=self.state[StepNames.contact_name_step.value],
-            contact_email=self.state[StepNames.contact_email_step.value],
+    sox_effects = ["none", "resample", "norm", "sil-start"]
+    sox_indices: List[int] = get_menu_prompt(  # type: ignore
+        "Please select zero or more from the following audio preprocessing options:",
+        [
+            "none",
+            "resample_audio (will resample to previously defined sampling rate)",
+            "normalize to -3.0dB",
+            "remove silence at the beginning of each clip",
+        ],
+        multi=True,
+    )
+    sox_config = create_sox_effects_list(
+        [sox_effects[i] for i in sox_indices], input_sr
+    )
+    config_formats = ["yaml", "json"]
+    config_format_index: int = get_menu_prompt(  # type: ignore
+        "What kind of configuration would you like to generate?", config_formats
+    )
+    config_format = config_formats[config_format_index]
+    # create_config_files
+    config_dir = output_path / "config"
+    config_dir.mkdir(exist_ok=True, parents=True)
+    # log dir
+    log_dir = (output_path / "logs").absolute()
+    log_dir.mkdir(parents=True, exist_ok=True)
+    ## Create Preprocessing Config
+    preprocessed_filelist_path = output_path / "preprocessed" / "processed_filelist.psv"
+    audio_config = AudioConfig(
+        min_audio_length=min_length,
+        max_audio_length=max_length,
+        input_sampling_rate=input_sr,
+        output_sampling_rate=input_sr,
+        alignment_sampling_rate=input_sr,
+    )
+    dataset_config = Dataset(
+        label=name,
+        data_dir=wavs_dir.absolute(),
+        filelist=dataset_filelist.absolute(),
+        sox_effects=sox_config,
+    )
+    preprocessing_config = PreprocessingConfig(
+        dataset=name,
+        save_dir=(output_path / "preprocessed").absolute(),
+        audio=audio_config,
+        source_data=[dataset_config],
+    )
+    preprocessing_config_path = (
+        config_dir / f"preprocessing.{config_format}"
+    ).absolute()
+    write_config_to_file(preprocessing_config, preprocessing_config_path)
+    ## Create Text Config
+    text_config = TextConfig(symbols=symbol_set)
+    text_config_path = (config_dir / f"text.{config_format}").absolute()
+    write_config_to_file(text_config, text_config_path)
+    ## Create Aligner Config
+    aligner_logger = LoggerConfig(name="AlignerExperiment", save_dir=log_dir)
+    aligner_config = AlignerConfig(
+        training=BaseTrainingConfig(
+            filelist=preprocessed_filelist_path.absolute(), logger=aligner_logger
         )
-
-        with init_context({"writing_config": config_dir.resolve()}):
-            # Preprocessing Config
-            preprocessed_training_filelist_path = (
-                preprocessed_dir_relative_to_configs / "training_filelist.psv"
-            )
-            preprocessed_validation_filelist_path = (
-                preprocessed_dir_relative_to_configs / "validation_filelist.psv"
-            )
-            preprocessing_config = PreprocessingConfig(
-                dataset=self.state[StepNames.name_step.value],
-                save_dir=preprocessed_dir_relative_to_configs,
-                source_data=datasets,
-            )
-            preprocessing_config_path = Path(
-                f"{PREPROCESSING_CONFIG_FILENAME_PREFIX}.{self.response}"
-            )
-            write_dict_to_config(
-                json.loads(preprocessing_config.model_dump_json(exclude_none=False)),
-                (config_dir / preprocessing_config_path).absolute(),
-            )
-
-            ## Create Aligner Config
-            aligner_logger = LoggerConfig(
-                name="AlignerExperiment", save_dir=log_dir_relative_to_configs
-            ).model_dump()
-            aligner_config = AlignerConfig(
-                contact=CONTACT_INFO,
-                # This isn't the actual AlignerTrainingConfig, but we can use it because we just
-                # inherit the defaults if we pass a dict to the AlignerConfig.training field
-                training=BaseTrainingConfig(
-                    training_filelist=preprocessed_training_filelist_path,
-                    validation_filelist=preprocessed_validation_filelist_path,
-                    logger=aligner_logger,
-                ).model_dump(),
-            )
-            aligner_config_path = Path(
-                f"{ALIGNER_CONFIG_FILENAME_PREFIX}.{self.response}"
-            )
-            aligner_config_json = json.loads(
-                aligner_config.model_dump_json(
-                    exclude_none=False, exclude={"preprocessing": True, "text": True}
-                )
-            )
-            aligner_config_json["path_to_preprocessing_config_file"] = str(
-                preprocessing_config_path
-            )
-            aligner_config_json["path_to_text_config_file"] = str(text_config_path)
-            write_dict_to_config(
-                aligner_config_json,
-                (config_dir / aligner_config_path).absolute(),
-            )
-
-            # Create Feature Prediction Config
-            fp_logger = LoggerConfig(
-                name="FeaturePredictionExperiment", save_dir=log_dir_relative_to_configs
-            )
-            fp_config = FeaturePredictionConfig(
-                contact=CONTACT_INFO,
-                model=FastSpeech2ModelConfig(
-                    multilingual=multilingual,
-                    multispeaker=multispeaker,
-                ),
-                training=BaseTrainingConfig(
-                    training_filelist=preprocessed_training_filelist_path,
-                    validation_filelist=preprocessed_validation_filelist_path,
-                    logger=fp_logger,
-                ).model_dump(),
-            )
-            fp_config_path = Path(
-                f"{TEXT_TO_SPEC_CONFIG_FILENAME_PREFIX}.{self.response}"
-            )
-            fp_config_json = json.loads(
-                fp_config.model_dump_json(
-                    exclude_none=False, exclude={"preprocessing": True, "text": True}
-                )
-            )
-            fp_config_json["path_to_preprocessing_config_file"] = str(
-                preprocessing_config_path
-            )
-            fp_config_json["path_to_text_config_file"] = str(text_config_path)
-            write_dict_to_config(
-                fp_config_json,
-                (config_dir / fp_config_path).absolute(),
-            )
-
-            # Create Vocoder Config
-            vocoder_logger = LoggerConfig(
-                name="VocoderExperiment", save_dir=log_dir_relative_to_configs
-            )
-            vocoder_config = VocoderConfig(
-                contact=CONTACT_INFO,
-                training=BaseTrainingConfig(
-                    training_filelist=preprocessed_training_filelist_path,
-                    validation_filelist=preprocessed_validation_filelist_path,
-                    logger=vocoder_logger,
-                ).model_dump(),
-            )
-            vocoder_config_path = Path(
-                f"{SPEC_TO_WAV_CONFIG_FILENAME_PREFIX}.{self.response}"
-            )
-            vocoder_config_json = json.loads(
-                vocoder_config.model_dump_json(
-                    exclude_none=False, exclude={"preprocessing": True}
-                )
-            )
-            vocoder_config_json["path_to_preprocessing_config_file"] = str(
-                preprocessing_config_path
-            )
-            write_dict_to_config(
-                vocoder_config_json,
-                (config_dir / vocoder_config_path).absolute(),
-            )
-
-            # E2E Config
-            e2e_logger = LoggerConfig(
-                name="E2E-Experiment", save_dir=log_dir_relative_to_configs
-            )
-            e2e_config = EveryVoiceConfig(
-                contact=CONTACT_INFO,
-                aligner=aligner_config,
-                feature_prediction=fp_config,
-                vocoder=vocoder_config,
-                training=E2ETrainingConfig(
-                    training_filelist=preprocessed_training_filelist_path,
-                    validation_filelist=preprocessed_validation_filelist_path,
-                    logger=e2e_logger,
-                ).model_dump(),
-            )
-            e2e_config_json = json.loads(
-                e2e_config.model_dump_json(
-                    exclude_none=False,
-                    exclude={
-                        "aligner": True,
-                        "feature_prediction": True,
-                        "vocoder": True,
-                    },
-                )
-            )
-            e2e_config_json["path_to_aligner_config_file"] = str(aligner_config_path)
-            e2e_config_json["path_to_feature_prediction_config_file"] = str(
-                fp_config_path
-            )
-            e2e_config_json["path_to_vocoder_config_file"] = str(vocoder_config_path)
-            e2e_config_path = Path(
-                f"{TEXT_TO_WAV_CONFIG_FILENAME_PREFIX}.{self.response}"
-            )
-            write_dict_to_config(
-                e2e_config_json,
-                (config_dir / e2e_config_path).absolute(),
-            )
-
-        print(
-            Panel(
-                f"You've finished configuring your dataset. Your files are located at {config_dir.absolute()}",
-                title="Congratulations 🎉",
-                subtitle="Next Steps Documentation: https://docs.everyvoice.ca/guides",
-                border_style=Style(color="#0B4F19"),
-            )
+    )
+    aligner_config_path = (config_dir / f"aligner.{config_format}").absolute()
+    aligner_config_json = json.loads(aligner_config.json())
+    aligner_config_json["preprocessing"] = str(preprocessing_config_path)
+    aligner_config_json["text"] = str(text_config_path)
+    write_dict_to_config(aligner_config_json, aligner_config_path)
+    ## Create Feature Prediction Config
+    fp_logger = LoggerConfig(name="FeaturePredictionExperiment", save_dir=log_dir)
+    fp_config = FeaturePredictionConfig(
+        training=BaseTrainingConfig(
+            filelist=preprocessed_filelist_path.absolute(), logger=fp_logger
         )
+    )
+    fp_config_path = (config_dir / f"feature_prediction.{config_format}").absolute()
+    fp_config_json = json.loads(fp_config.json())
+    fp_config_json["preprocessing"] = str(preprocessing_config_path)
+    fp_config_json["text"] = str(text_config_path)
+    write_dict_to_config(fp_config_json, fp_config_path)
+    ## Create Vocoder Config
+    vocoder_logger = LoggerConfig(name="VocoderExperiment", save_dir=log_dir)
+    vocoder_config = VocoderConfig(
+        training=BaseTrainingConfig(
+            filelist=preprocessed_filelist_path.absolute(), logger=vocoder_logger
+        )
+    )
+    vocoder_config_path = (config_dir / f"vocoder.{config_format}").absolute()
+    vocoder_config_json = json.loads(vocoder_config.json())
+    vocoder_config_json["preprocessing"] = str(preprocessing_config_path)
+    write_dict_to_config(vocoder_config_json, vocoder_config_path)
+    ## E2E Config
+    e2e_logger = LoggerConfig(name="E2E-Experiment", save_dir=log_dir)
+    e2e_config = EveryVoiceConfig(
+        vocoder=vocoder_config_path,
+        feature_prediction=fp_config_path,
+        aligner=aligner_config_path,
+        training=BaseTrainingConfig(
+            filelist=preprocessed_filelist_path.absolute(), logger=e2e_logger
+        ),
+    )
+    e2e_config_json = json.loads(e2e_config.json())
+    e2e_config_json["aligner"] = str(aligner_config_path)
+    e2e_config_json["feature_prediction"] = str(fp_config_path)
+    e2e_config_json["vocoder"] = str(vocoder_config_path)
+    e2e_config_path = (config_dir / f"e2e.{config_format}").absolute()
+    write_dict_to_config(e2e_config_json, e2e_config_path)
+    print(
+        Panel(
+            f"You've finished configuring your dataset. Your files are located at {config_dir.absolute()}",
+            title="Congratulations 🎉",
+            subtitle="Next Steps Documentation: http://localhost:8000/guides/index.html",
+            border_style=Style(color="#0B4F19"),
+        )
+    )
 
 
-class MoreDatasetsStep(Step):
-    DEFAULT_NAME = StepNames.more_datasets_step
+@app.command()
+def test(suite: TestSuites = typer.Argument(TestSuites.dev)):
+    """This command will run the test suite specified by the user"""
+    from everyvoice.run_tests import run_tests
 
-    def prompt(self):
-        return get_response_from_menu_prompt(
-            "Do you have more datasets to process?",
-            ("no", "yes"),
-        )
+    run_tests(suite)
 
-    def validate(self, response):
-        return response in ("yes", "no")
 
-    def effect(self):
-        if self.response == "yes":
-            new_dataset_index = (
-                max(
-                    [
-                        int(key.split("_")[1])
-                        for key in self.state.keys()
-                        if key.startswith("dataset_")
-                    ],
-                    default=0,
-                )
-                + 1
-            )
-            self.tour.add_step(
-                MoreDatasetsStep(name=StepNames.more_datasets_step.value), self
-            )
-            for step in reversed(return_dataset_steps(dataset_index=new_dataset_index)):
-                self.tour.add_step(step, self)
-        else:
-            self.tour.add_step(
-                ConfigFormatStep(name=StepNames.config_format_step.value), self
-            )
+CLICK_APP = typer.main.get_group(app)
+
+if __name__ == "__main__":
+    app()
```

### Comparing `everyvoice-0.1.0a0.dev0/setup.py` & `everyvoice-0.1.20230307/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,47 @@
 """ Setup for everyvoice
 """
-
+import datetime as dt
 from os import path
 
 from setuptools import find_packages, setup
 
-# Ugly hack to read the current version number without importing everyvoice:
+build_no = dt.datetime.now().strftime("%Y%m%d")
+
+# Ugly hack to read the current version number without importing g2p:
+# (works by )
 with open("everyvoice/_version.py", "r", encoding="utf8") as version_file:
-    namespace: dict = {}
+    namespace = {}  # type: ignore
     exec(version_file.read(), namespace)
-    VERSION = namespace["VERSION"]
-    # [N!]N(.N)*[{a|b|rc}N][.postN][.devN]
+    VERSION = namespace["VERSION"] + "." + build_no
 
 this_directory = path.abspath(path.dirname(__file__))
 
-with open(path.join(this_directory, "README.md"), encoding="utf8") as f:
+with open(path.join(this_directory, "readme.md"), encoding="utf8") as f:
     long_description = f.read()
 
 with open(path.join(this_directory, "requirements.txt"), encoding="utf8") as f:
     REQS = f.read().splitlines()
 
-# Get a list of submodules
-SUBMODULE_PATHS = [
-    "everyvoice/model/feature_prediction/FastSpeech2_lightning/fs2",
-    "everyvoice/model/vocoder/HiFiGAN_iSTFT_lightning/hfgl",
-    "everyvoice/model/aligner/DeepForcedAligner/dfaligner",
-    "everyvoice/model/aligner/wav2vec2aligner/aligner",
-]
-SUBMODULE_PACKAGES = []
-
-# For each submodule
-for submodule_path in SUBMODULE_PATHS:
-    # append the submodule path to the list of submodule packages
-    submodule = submodule_path.replace("/", ".")
-    SUBMODULE_PACKAGES.append(submodule)
-    # then use find_packages to automatically find the rest
-    packages = find_packages(submodule_path)
-    SUBMODULE_PACKAGES += [submodule + f".{pkg}" for pkg in packages]
-
 setup(
     name="everyvoice",
-    python_requires=">=3.10, <3.12",
+    python_requires=">=3.9",
     version=VERSION,
     author="Aidan Pine",
     author_email="hello@aidanpine.ca",
     license="MIT",
     url="https://github.com/roedoejet/EveryVoice",
     description="Text-to-Speech Synthesis for the Speech Generation for Indigenous Language Education Small Teams Project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platform=["any"],
-    packages=find_packages() + SUBMODULE_PACKAGES,
+    packages=find_packages(),
     include_package_data=True,
     install_requires=REQS,
     entry_points={"console_scripts": ["everyvoice = everyvoice.cli:app"]},
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: MacOS",
+        "Operating System :: OS Independent",
     ],
 )
```

