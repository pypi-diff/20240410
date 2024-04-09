# Comparing `tmp/azure-ai-formrecognizer-3.3.2.tar.gz` & `tmp/azure-ai-formrecognizer-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-ai-formrecognizer-3.3.2.tar", last modified: Tue Nov  7 20:50:34 2023, max compression
+gzip compressed data, was "azure-ai-formrecognizer-3.3.3.tar", last modified: Tue Apr  9 22:33:46 2024, max compression
```

## Comparing `azure-ai-formrecognizer-3.3.2.tar` & `azure-ai-formrecognizer-3.3.3.tar`

### file list

```diff
@@ -1,342 +1,347 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.802127 azure-ai-formrecognizer-3.3.2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26213 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      197 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32449 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/MIGRATION_GUIDE.md
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    63890 2023-11-07 20:50:34.802127 azure-ai-formrecognizer-3.3.2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36549 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4696 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/TROUBLESHOOTING.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.762126 azure-ai-formrecognizer-3.3.2/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.762126 azure-ai-formrecognizer-3.3.2/azure/ai/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.766126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3733 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2458 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_api_versions.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16108 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_document_analysis_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40238 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_document_model_administration_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6510 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_form_base_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    45405 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23263 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_form_training_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.766126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      662 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3229 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8141 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    76680 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_operations_mixin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      344 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.766126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      561 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3181 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8263 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    77099 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/_operations_mixin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      448 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/models.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.766126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3490 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3956 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1708 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.766126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3502 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4024 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1029 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    52751 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_form_recognizer_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4348 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4090 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/_form_recognizer_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   112396 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    65028 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_form_recognizer_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3490 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4916 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1197 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3502 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5001 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1025 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28791 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_classifiers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44957 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_models_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10866 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_miscellaneous_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.770126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5380 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10216 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/_form_recognizer_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   144656 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1025 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35253 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_classifiers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    55223 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_models_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13198 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_miscellaneous_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3192 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3781 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1708 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3204 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3849 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1029 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56894 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_form_recognizer_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2742 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2275 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/_form_recognizer_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    60322 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    67701 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/_form_recognizer_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.774126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3192 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3781 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1708 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3204 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3849 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_form_recognizer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1029 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   102413 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_form_recognizer_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3260 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4433 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/_form_recognizer_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70714 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   120902 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/_form_recognizer_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6676 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_helpers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   178425 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8937 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_polling.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5624 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_response_handlers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      227 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_user_agent.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      170 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      703 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_async_polling.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16550 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_document_analysis_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41330 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_document_model_administration_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5292 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_form_base_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46257 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_form_recognizer_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24135 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_form_training_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      856 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_helpers_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    63890 2023-11-07 20:50:34.000000 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16256 2023-11-07 20:50:34.000000 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-11-07 20:50:34.000000 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-11-07 20:50:34.000000 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       84 2023-11-07 20:50:34.000000 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-11-07 20:50:34.000000 azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       66 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.778126 azure-ai-formrecognizer-3.3.2/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31149 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.782127 azure-ai-formrecognizer-3.3.2/samples/v3.1/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.782127 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5023 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_authentication_v3_1_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3478 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_convert_to_and_from_dict_v3_1_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4793 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_copy_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6042 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_create_composed_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8309 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_differentiate_output_labeled_tables_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8549 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_differentiate_output_models_trained_with_and_without_labels_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7537 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_get_bounding_boxes_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4058 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_manage_custom_models_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5321 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_business_cards_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4660 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_content_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6492 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_custom_forms_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4063 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_identity_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10226 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_invoices_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4939 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_receipts_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4912 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_receipts_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5784 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_strongly_typing_recognized_form_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4107 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_train_model_with_labels_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3431 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_train_model_without_labels_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4547 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_authentication_v3_1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3254 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_convert_to_and_from_dict_v3_1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4440 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_copy_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5716 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_create_composed_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7830 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_differentiate_output_labeled_tables.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8202 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_differentiate_output_models_trained_with_and_without_labels.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7004 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_get_bounding_boxes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3691 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_manage_custom_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5126 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_business_cards.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4328 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_content.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6037 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_custom_forms.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3768 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_identity_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9646 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_invoices.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4619 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_receipts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4600 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_receipts_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5629 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_strongly_typing_recognized_form.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3792 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_train_model_with_labels.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3180 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_train_model_without_labels.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.786126 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.790127 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4720 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_barcodes_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6999 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_fonts_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5245 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_formulas_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5920 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_highres_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4597 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_languages_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6156 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_business_cards_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6570 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_custom_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_general_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4736 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_identity_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11097 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_invoices_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5313 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_layout_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5781 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_read_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5688 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_receipts_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5683 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_receipts_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13115 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_tax_us_w2_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5991 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_authentication_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3145 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_build_classifier_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3855 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_build_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5413 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_classify_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5355 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_classify_document_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6436 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_compose_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4013 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_convert_to_and_from_dict_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5882 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_copy_model_to_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6170 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_get_elements_with_spans_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4869 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_get_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4181 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_get_words_on_document_line_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5096 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_manage_classifiers_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5091 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_manage_models_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7922 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_send_request_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4485 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_barcodes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6777 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_fonts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5056 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_formulas.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5699 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_highres.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4394 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_languages.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5966 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_business_cards.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6312 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_custom_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5879 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_general_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4546 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_identity_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10895 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_invoices.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5179 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_layout.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5563 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_read.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5558 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_receipts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5499 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_receipts_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12928 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_tax_us_w2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5518 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_authentication.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2854 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_build_classifier.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3650 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_build_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5166 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_classify_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5133 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_classify_document_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6031 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_compose_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3784 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_convert_to_and_from_dict.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5607 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_copy_model_to.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_get_elements_with_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4469 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_get_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3991 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_get_words_on_document_line.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4644 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_manage_classifiers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_manage_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7514 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_send_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-11-07 20:50:34.802127 azure-ai-formrecognizer-3.3.2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2698 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.802127 azure-ai-formrecognizer-3.3.2/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1298 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/asynctestcase.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3159 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:50:34.802127 azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3139 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_custom_forms.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1967 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_dac_analyze_document_from_url_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1930 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_dac_analyze_document_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1935 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_dmac_build_model_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3294 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/preparers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2117 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_content_type.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10891 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11940 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8119 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8610 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7556 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_general_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7972 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_general_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8722 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_layout.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9319 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_layout_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6337 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilt_read.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6727 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilt_read_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29611 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30196 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20129 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21838 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5836 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_classify_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6486 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dac_classify_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8986 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_classifiers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9921 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_classifiers_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6214 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_compose_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6824 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_compose_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9947 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_copy_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11157 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_copy_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10173 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_mgmt.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11238 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_mgmt_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13798 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_training.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13646 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_dmac_training_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9316 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6265 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3848 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4014 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13013 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_content.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14638 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_content_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11045 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_content_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10626 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_content_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13615 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11368 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12257 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13595 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7537 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8206 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5700 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6159 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15248 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16297 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6586 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6563 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5180 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5578 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4590 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4840 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3015 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_compose_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3337 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_compose_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8476 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_copy_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9347 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_copy_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6508 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_mgmt.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6970 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_mgmt_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12585 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_training.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13314 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_ftc_training_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2118 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_get_children.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5834 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7014 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_logging_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14986 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_multiapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15850 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_multiapi_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33621 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_repr.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1720 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_resolve_elements.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5552 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_send_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6107 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_send_request_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37919 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_to_dict_v2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    84949 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/test_to_dict_v3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42294 2023-11-07 20:49:47.000000 azure-ai-formrecognizer-3.3.2/tests/testcase.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.946604 azure-ai-formrecognizer-3.3.3/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26419 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      197 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32449 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/MIGRATION_GUIDE.md
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    64552 2024-04-09 22:33:46.946604 azure-ai-formrecognizer-3.3.3/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37011 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4696 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/TROUBLESHOOTING.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.890603 azure-ai-formrecognizer-3.3.3/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.890603 azure-ai-formrecognizer-3.3.3/azure/ai/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.890603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3733 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2458 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_api_versions.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16108 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_document_analysis_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40238 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_document_model_administration_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6510 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_form_base_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    45405 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23263 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_form_training_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.894603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      662 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3229 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8141 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    76680 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_operations_mixin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      344 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.894603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      561 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3181 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8263 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    77099 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/_operations_mixin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      448 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.894603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3490 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3956 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1708 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.894603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3502 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4024 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1029 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.898604 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    52751 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_form_recognizer_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.898604 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4348 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4090 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/_form_recognizer_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   112396 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.898604 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    65028 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_form_recognizer_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.898604 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3490 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4916 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1197 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.898604 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3502 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5001 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.902603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1025 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28791 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_classifiers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44957 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_models_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10866 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_miscellaneous_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.902603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5380 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10216 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/_form_recognizer_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   144656 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.902603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1025 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35253 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_classifiers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    55223 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_models_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13198 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_miscellaneous_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.902603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3192 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3781 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1708 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.902603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3204 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3849 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1029 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.906603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56894 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_form_recognizer_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.906603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2742 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2275 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/_form_recognizer_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    60322 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.906603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    67701 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/_form_recognizer_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.906603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3192 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3781 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1708 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.906603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      854 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3204 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3849 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_form_recognizer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1029 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.910603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   102413 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_form_recognizer_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.910603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3260 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4433 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/_form_recognizer_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70714 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.910603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   120902 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/_form_recognizer_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/py.typed
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6676 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_helpers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   178425 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8937 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_polling.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5624 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_response_handlers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      227 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_user_agent.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      170 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.910603 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      703 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_async_polling.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16550 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_document_analysis_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41330 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_document_model_administration_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5292 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_form_base_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46257 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_form_recognizer_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24135 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_form_training_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      856 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_helpers_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.946604 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    64552 2024-04-09 22:33:46.000000 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16510 2024-04-09 22:33:46.000000 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-09 22:33:46.000000 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-09 22:33:46.000000 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       77 2024-04-09 22:33:46.000000 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-09 22:33:46.000000 azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      102 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.914604 azure-ai-formrecognizer-3.3.3/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31149 2024-04-09 22:32:12.000000 azure-ai-formrecognizer-3.3.3/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.918604 azure-ai-formrecognizer-3.3.3/samples/v3.1/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.918604 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5023 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_authentication_v3_1_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3478 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_convert_to_and_from_dict_v3_1_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4793 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_copy_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6042 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_create_composed_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8309 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_differentiate_output_labeled_tables_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8549 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_differentiate_output_models_trained_with_and_without_labels_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7537 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_get_bounding_boxes_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4058 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_manage_custom_models_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5321 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_business_cards_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4660 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_content_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6492 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_custom_forms_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4063 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_identity_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10226 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_invoices_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4939 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_receipts_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4912 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_receipts_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5784 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_strongly_typing_recognized_form_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4107 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_train_model_with_labels_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3431 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_train_model_without_labels_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4547 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_authentication_v3_1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3254 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_convert_to_and_from_dict_v3_1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4440 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_copy_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5716 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_create_composed_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7830 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_differentiate_output_labeled_tables.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8202 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_differentiate_output_models_trained_with_and_without_labels.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7004 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_get_bounding_boxes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3691 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_manage_custom_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5126 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_business_cards.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4328 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_content.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6037 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_custom_forms.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3768 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_identity_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9646 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_invoices.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4619 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_receipts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4600 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_receipts_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5629 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_strongly_typing_recognized_form.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3792 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_train_model_with_labels.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3180 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_train_model_without_labels.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.926603 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.930604 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4713 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_barcodes_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6999 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_fonts_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5245 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_formulas_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5920 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_highres_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4597 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_languages_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6156 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_business_cards_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6570 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_custom_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_general_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4736 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_identity_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11097 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_invoices_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5313 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_layout_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5781 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_read_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5688 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_receipts_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5683 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_receipts_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13115 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_tax_us_w2_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5991 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_authentication_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3145 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_build_classifier_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3855 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_build_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5413 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_classify_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5355 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_classify_document_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6436 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_compose_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4013 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_convert_to_and_from_dict_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5882 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_copy_model_to_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6170 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_get_elements_with_spans_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4869 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_get_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4181 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_get_words_on_document_line_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5096 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_manage_classifiers_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5091 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_manage_models_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7800 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_send_request_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4485 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_barcodes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6777 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_fonts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5056 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_formulas.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5699 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_highres.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4394 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_languages.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5966 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_business_cards.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6312 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_custom_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5879 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_general_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4546 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_identity_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10895 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_invoices.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5179 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_layout.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5563 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_read.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5558 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_receipts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5499 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_receipts_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12928 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_tax_us_w2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5518 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_authentication.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2854 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_build_classifier.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3650 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_build_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5166 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_classify_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5133 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_classify_document_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6031 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_compose_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3784 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_convert_to_and_from_dict.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5607 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_copy_model_to.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_get_elements_with_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4469 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_get_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3991 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_get_words_on_document_line.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4644 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_manage_classifiers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_manage_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7235 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_send_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-09 22:33:46.946604 azure-ai-formrecognizer-3.3.3/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2692 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.946604 azure-ai-formrecognizer-3.3.3/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1298 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/asynctestcase.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3159 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:33:46.946604 azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3143 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_custom_forms.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1971 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_dac_analyze_document_from_url_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1934 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_dac_analyze_document_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1939 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_dmac_build_model_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3294 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/preparers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2117 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_content_type.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10891 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11940 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8119 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8610 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7556 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_general_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7972 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_general_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8722 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_layout.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9319 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_layout_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6337 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilt_read.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6727 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilt_read_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29615 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30200 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20133 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21842 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5836 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_classify_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6486 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dac_classify_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8986 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_classifiers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9921 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_classifiers_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6218 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_compose_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6828 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_compose_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9951 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_copy_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11161 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_copy_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10173 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_mgmt.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11238 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_mgmt_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13802 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_training.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13650 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_dmac_training_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9316 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6265 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3848 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4014 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13017 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_content.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14642 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_content_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11049 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_content_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10630 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_content_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13619 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11372 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12261 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13599 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7541 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8210 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5704 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6163 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15252 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16301 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6590 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6567 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5180 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5578 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4590 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4840 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3015 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_compose_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3337 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_compose_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8476 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_copy_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9347 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_copy_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6508 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_mgmt.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6970 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_mgmt_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12585 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_training.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13314 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_ftc_training_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2118 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_get_children.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5834 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7014 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_logging_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14986 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_multiapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15850 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_multiapi_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33621 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_repr.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1720 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_resolve_elements.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5943 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_send_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6510 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_send_request_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37919 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_to_dict_v2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    84949 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/test_to_dict_v3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42294 2024-04-09 22:32:13.000000 azure-ai-formrecognizer-3.3.3/tests/testcase.py
```

### Comparing `azure-ai-formrecognizer-3.3.2/CHANGELOG.md` & `azure-ai-formrecognizer-3.3.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 3.3.3 (2024-04-09)
+
+### Other Changes
+- Added support for Python 3.12.
+- Python 3.7 is no longer supported. Please use Python version 3.8 or later.
+- Changed the default polling interval from 5s to 1s.
+
 ## 3.3.2 (2023-11-07)
 
 ### Bugs Fixed
 - Fixed incorrect data type for returned formula objects.
 
 ## 3.3.1 (2023-10-10)
```

### Comparing `azure-ai-formrecognizer-3.3.2/LICENSE` & `azure-ai-formrecognizer-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/MIGRATION_GUIDE.md` & `azure-ai-formrecognizer-3.3.3/MIGRATION_GUIDE.md`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/PKG-INFO` & `azure-ai-formrecognizer-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: azure-ai-formrecognizer
-Version: 3.3.2
+Version: 3.3.3
 Summary: Microsoft Azure Form Recognizer Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,form recognizer,cognitive services,document analyzer,document analysis,applied ai,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core<2.0.0,>=1.23.0
+Requires-Dist: azure-core>=1.23.0
 Requires-Dist: msrest>=0.6.21
-Requires-Dist: azure-common~=1.1
+Requires-Dist: azure-common>=1.1
 Requires-Dist: typing-extensions>=4.0.1
 
 # Azure Form Recognizer client library for Python
 
 Azure Document Intelligence ([previously known as Form Recognizer][service-rename]) is a cloud service that uses machine learning to analyze text and structured data from your documents. It includes the following main features:
 
 - Layout - Extract content and structure (ex. words, selection marks, tables) from documents.
@@ -41,19 +41,24 @@
 | [Package (PyPI)][python-fr-pypi]
 | [Package (Conda)](https://anaconda.org/microsoft/azure-ai-formrecognizer/)
 | [API reference documentation][python-fr-ref-docs]
 | [Product documentation][python-fr-product-docs]
 | [Samples][python-fr-samples]
 
 
+## _Disclaimer_
+
+_This package supports the following service API versions: 2.0, 2.1, 2022-08-31 and 2023-07-31. Service API version 2023-10-31-preview and later are supported in package `azure-ai-documentintelligence`. Please refer this [doc][fr_to_di_migration_guideline] for migration details._
+
+
 ## Getting started
 
 ### Prerequisites
 
-* Python 3.7 or later is required to use this package.
+* Python 3.8 or later is required to use this package.
 * You must have an [Azure subscription][azure_subscription] and a
 [Cognitive Services or Form Recognizer resource][FR_or_CS_resource] to use this package.
 
 ### Install the package
 
 Install the Azure Form Recognizer client library for Python with [pip][pip]:
 
@@ -776,14 +781,15 @@
 [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
 [labeling-tool]: https://aka.ms/azsdk/formrecognizer/labelingtool
 [fr-studio]: https://aka.ms/azsdk/formrecognizer/formrecognizerstudio
 [fr-build-model]: https://aka.ms/azsdk/formrecognizer/buildmodel
 [fr-build-training-set]: https://aka.ms/azsdk/formrecognizer/buildtrainingset
 [fr-models]: https://aka.ms/azsdk/formrecognizer/models
 [fr-errors]: https://aka.ms/azsdk/formrecognizer/errors
+[fr_to_di_migration_guideline]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/documentintelligence/azure-ai-documentintelligence/MIGRATION_GUIDE.md
 
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [python_logging]: https://docs.python.org/3/library/logging.html
 [multi_and_single_service]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows
 [azure_cli_endpoint_lookup]: https://docs.microsoft.com/cli/azure/cognitiveservices/account?view=azure-cli-latest#az-cognitiveservices-account-show
 [azure_portal_get_endpoint]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows#get-the-keys-for-your-resource
@@ -814,14 +820,21 @@
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
 
 
 # Release History
 
+## 3.3.3 (2024-04-09)
+
+### Other Changes
+- Added support for Python 3.12.
+- Python 3.7 is no longer supported. Please use Python version 3.8 or later.
+- Changed the default polling interval from 5s to 1s.
+
 ## 3.3.2 (2023-11-07)
 
 ### Bugs Fixed
 - Fixed incorrect data type for returned formula objects.
 
 ## 3.3.1 (2023-10-10)
```

### Comparing `azure-ai-formrecognizer-3.3.2/README.md` & `azure-ai-formrecognizer-3.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,24 @@
 | [Package (PyPI)][python-fr-pypi]
 | [Package (Conda)](https://anaconda.org/microsoft/azure-ai-formrecognizer/)
 | [API reference documentation][python-fr-ref-docs]
 | [Product documentation][python-fr-product-docs]
 | [Samples][python-fr-samples]
 
 
+## _Disclaimer_
+
+_This package supports the following service API versions: 2.0, 2.1, 2022-08-31 and 2023-07-31. Service API version 2023-10-31-preview and later are supported in package `azure-ai-documentintelligence`. Please refer this [doc][fr_to_di_migration_guideline] for migration details._
+
+
 ## Getting started
 
 ### Prerequisites
 
-* Python 3.7 or later is required to use this package.
+* Python 3.8 or later is required to use this package.
 * You must have an [Azure subscription][azure_subscription] and a
 [Cognitive Services or Form Recognizer resource][FR_or_CS_resource] to use this package.
 
 ### Install the package
 
 Install the Azure Form Recognizer client library for Python with [pip][pip]:
 
@@ -749,14 +754,15 @@
 [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
 [labeling-tool]: https://aka.ms/azsdk/formrecognizer/labelingtool
 [fr-studio]: https://aka.ms/azsdk/formrecognizer/formrecognizerstudio
 [fr-build-model]: https://aka.ms/azsdk/formrecognizer/buildmodel
 [fr-build-training-set]: https://aka.ms/azsdk/formrecognizer/buildtrainingset
 [fr-models]: https://aka.ms/azsdk/formrecognizer/models
 [fr-errors]: https://aka.ms/azsdk/formrecognizer/errors
+[fr_to_di_migration_guideline]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/documentintelligence/azure-ai-documentintelligence/MIGRATION_GUIDE.md
 
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [python_logging]: https://docs.python.org/3/library/logging.html
 [multi_and_single_service]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows
 [azure_cli_endpoint_lookup]: https://docs.microsoft.com/cli/azure/cognitiveservices/account?view=azure-cli-latest#az-cognitiveservices-account-show
 [azure_portal_get_endpoint]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows#get-the-keys-for-your-resource
```

### Comparing `azure-ai-formrecognizer-3.3.2/TROUBLESHOOTING.md` & `azure-ai-formrecognizer-3.3.3/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_api_versions.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_api_versions.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_document_analysis_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_document_analysis_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_document_model_administration_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_document_model_administration_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_form_base_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_form_base_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_form_training_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_form_training_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/_operations_mixin.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/_operations_mixin.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/aio/_operations_mixin.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/aio/_operations_mixin.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_form_recognizer_client_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_form_recognizer_client_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/_form_recognizer_client_enums.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/_form_recognizer_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/_models_py3.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/models/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_form_recognizer_client_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_form_recognizer_client_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2022_08_31/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_classifiers_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_classifiers_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_models_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_models_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_miscellaneous_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_miscellaneous_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/_form_recognizer_client_enums.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/_form_recognizer_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/_models_py3.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/models/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_classifiers_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_classifiers_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_models_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_document_models_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_miscellaneous_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_miscellaneous_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2023_07_31/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_form_recognizer_client_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_form_recognizer_client_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/_form_recognizer_client_enums.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/_form_recognizer_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/_models_py3.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/models/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/_form_recognizer_client_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/_form_recognizer_client_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_0/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_0/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_configuration.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_form_recognizer_client.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_form_recognizer_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/_vendor.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_form_recognizer_client_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_form_recognizer_client_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/_form_recognizer_client_enums.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/_form_recognizer_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/_models_py3.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/models/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/_form_recognizer_client_operations.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/_form_recognizer_client_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_generated/v2_1/operations/_patch.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_generated/v2_1/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_helpers.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Optional
 from azure.core.credentials import AzureKeyCredential
 from azure.core.pipeline.policies import AzureKeyCredentialPolicy, SansIOHTTPPolicy
 from azure.core.pipeline.transport import HttpTransport
 from azure.core.exceptions import HttpResponseError
 
 
-POLLING_INTERVAL = 5
+POLLING_INTERVAL = 1
 COGNITIVE_KEY_HEADER = "Ocp-Apim-Subscription-Key"
 
 
 def _get_deserialize(api_version):
     if api_version == "2.0":
         from ._generated.v2_0 import FormRecognizerClient
     elif api_version == "2.1":
```

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_models.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_models.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_polling.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_polling.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/_response_handlers.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/_response_handlers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/__init__.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_async_polling.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_async_polling.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_document_analysis_client_async.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_document_analysis_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_document_model_administration_client_async.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_document_model_administration_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_form_base_client_async.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_form_base_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_form_recognizer_client_async.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_form_recognizer_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_form_training_client_async.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_form_training_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure/ai/formrecognizer/aio/_helpers_async.py` & `azure-ai-formrecognizer-3.3.3/azure/ai/formrecognizer/aio/_helpers_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/PKG-INFO` & `azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: azure-ai-formrecognizer
-Version: 3.3.2
+Version: 3.3.3
 Summary: Microsoft Azure Form Recognizer Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,form recognizer,cognitive services,document analyzer,document analysis,applied ai,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core<2.0.0,>=1.23.0
+Requires-Dist: azure-core>=1.23.0
 Requires-Dist: msrest>=0.6.21
-Requires-Dist: azure-common~=1.1
+Requires-Dist: azure-common>=1.1
 Requires-Dist: typing-extensions>=4.0.1
 
 # Azure Form Recognizer client library for Python
 
 Azure Document Intelligence ([previously known as Form Recognizer][service-rename]) is a cloud service that uses machine learning to analyze text and structured data from your documents. It includes the following main features:
 
 - Layout - Extract content and structure (ex. words, selection marks, tables) from documents.
@@ -41,19 +41,24 @@
 | [Package (PyPI)][python-fr-pypi]
 | [Package (Conda)](https://anaconda.org/microsoft/azure-ai-formrecognizer/)
 | [API reference documentation][python-fr-ref-docs]
 | [Product documentation][python-fr-product-docs]
 | [Samples][python-fr-samples]
 
 
+## _Disclaimer_
+
+_This package supports the following service API versions: 2.0, 2.1, 2022-08-31 and 2023-07-31. Service API version 2023-10-31-preview and later are supported in package `azure-ai-documentintelligence`. Please refer this [doc][fr_to_di_migration_guideline] for migration details._
+
+
 ## Getting started
 
 ### Prerequisites
 
-* Python 3.7 or later is required to use this package.
+* Python 3.8 or later is required to use this package.
 * You must have an [Azure subscription][azure_subscription] and a
 [Cognitive Services or Form Recognizer resource][FR_or_CS_resource] to use this package.
 
 ### Install the package
 
 Install the Azure Form Recognizer client library for Python with [pip][pip]:
 
@@ -776,14 +781,15 @@
 [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
 [labeling-tool]: https://aka.ms/azsdk/formrecognizer/labelingtool
 [fr-studio]: https://aka.ms/azsdk/formrecognizer/formrecognizerstudio
 [fr-build-model]: https://aka.ms/azsdk/formrecognizer/buildmodel
 [fr-build-training-set]: https://aka.ms/azsdk/formrecognizer/buildtrainingset
 [fr-models]: https://aka.ms/azsdk/formrecognizer/models
 [fr-errors]: https://aka.ms/azsdk/formrecognizer/errors
+[fr_to_di_migration_guideline]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/documentintelligence/azure-ai-documentintelligence/MIGRATION_GUIDE.md
 
 [azure_core_ref_docs]: https://aka.ms/azsdk/python/core/docs
 [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
 [python_logging]: https://docs.python.org/3/library/logging.html
 [multi_and_single_service]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows
 [azure_cli_endpoint_lookup]: https://docs.microsoft.com/cli/azure/cognitiveservices/account?view=azure-cli-latest#az-cognitiveservices-account-show
 [azure_portal_get_endpoint]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows#get-the-keys-for-your-resource
@@ -814,14 +820,21 @@
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
 
 
 # Release History
 
+## 3.3.3 (2024-04-09)
+
+### Other Changes
+- Added support for Python 3.12.
+- Python 3.7 is no longer supported. Please use Python version 3.8 or later.
+- Changed the default polling interval from 5s to 1s.
+
 ## 3.3.2 (2023-11-07)
 
 ### Bugs Fixed
 - Fixed incorrect data type for returned formula objects.
 
 ## 3.3.1 (2023-10-10)
```

### Comparing `azure-ai-formrecognizer-3.3.2/azure_ai_formrecognizer.egg-info/SOURCES.txt` & `azure-ai-formrecognizer-3.3.3/azure_ai_formrecognizer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 azure/ai/formrecognizer/py.typed
 azure/ai/formrecognizer/_generated/__init__.py
 azure/ai/formrecognizer/_generated/_configuration.py
 azure/ai/formrecognizer/_generated/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/_operations_mixin.py
 azure/ai/formrecognizer/_generated/_version.py
 azure/ai/formrecognizer/_generated/models.py
+azure/ai/formrecognizer/_generated/py.typed
 azure/ai/formrecognizer/_generated/aio/__init__.py
 azure/ai/formrecognizer/_generated/aio/_configuration.py
 azure/ai/formrecognizer/_generated/aio/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/aio/_operations_mixin.py
 azure/ai/formrecognizer/_generated/v2022_08_31/__init__.py
 azure/ai/formrecognizer/_generated/v2022_08_31/_configuration.py
 azure/ai/formrecognizer/_generated/v2022_08_31/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2022_08_31/_patch.py
 azure/ai/formrecognizer/_generated/v2022_08_31/_vendor.py
+azure/ai/formrecognizer/_generated/v2022_08_31/py.typed
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/__init__.py
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/_configuration.py
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/_patch.py
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/_vendor.py
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/__init__.py
 azure/ai/formrecognizer/_generated/v2022_08_31/aio/operations/_form_recognizer_client_operations.py
@@ -53,14 +55,15 @@
 azure/ai/formrecognizer/_generated/v2022_08_31/operations/_form_recognizer_client_operations.py
 azure/ai/formrecognizer/_generated/v2022_08_31/operations/_patch.py
 azure/ai/formrecognizer/_generated/v2023_07_31/__init__.py
 azure/ai/formrecognizer/_generated/v2023_07_31/_configuration.py
 azure/ai/formrecognizer/_generated/v2023_07_31/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2023_07_31/_patch.py
 azure/ai/formrecognizer/_generated/v2023_07_31/_vendor.py
+azure/ai/formrecognizer/_generated/v2023_07_31/py.typed
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/__init__.py
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/_configuration.py
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/_patch.py
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/__init__.py
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_classifiers_operations.py
 azure/ai/formrecognizer/_generated/v2023_07_31/aio/operations/_document_models_operations.py
@@ -76,14 +79,15 @@
 azure/ai/formrecognizer/_generated/v2023_07_31/operations/_miscellaneous_operations.py
 azure/ai/formrecognizer/_generated/v2023_07_31/operations/_patch.py
 azure/ai/formrecognizer/_generated/v2_0/__init__.py
 azure/ai/formrecognizer/_generated/v2_0/_configuration.py
 azure/ai/formrecognizer/_generated/v2_0/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2_0/_patch.py
 azure/ai/formrecognizer/_generated/v2_0/_vendor.py
+azure/ai/formrecognizer/_generated/v2_0/py.typed
 azure/ai/formrecognizer/_generated/v2_0/aio/__init__.py
 azure/ai/formrecognizer/_generated/v2_0/aio/_configuration.py
 azure/ai/formrecognizer/_generated/v2_0/aio/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2_0/aio/_patch.py
 azure/ai/formrecognizer/_generated/v2_0/aio/_vendor.py
 azure/ai/formrecognizer/_generated/v2_0/aio/operations/__init__.py
 azure/ai/formrecognizer/_generated/v2_0/aio/operations/_form_recognizer_client_operations.py
@@ -96,14 +100,15 @@
 azure/ai/formrecognizer/_generated/v2_0/operations/_form_recognizer_client_operations.py
 azure/ai/formrecognizer/_generated/v2_0/operations/_patch.py
 azure/ai/formrecognizer/_generated/v2_1/__init__.py
 azure/ai/formrecognizer/_generated/v2_1/_configuration.py
 azure/ai/formrecognizer/_generated/v2_1/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2_1/_patch.py
 azure/ai/formrecognizer/_generated/v2_1/_vendor.py
+azure/ai/formrecognizer/_generated/v2_1/py.typed
 azure/ai/formrecognizer/_generated/v2_1/aio/__init__.py
 azure/ai/formrecognizer/_generated/v2_1/aio/_configuration.py
 azure/ai/formrecognizer/_generated/v2_1/aio/_form_recognizer_client.py
 azure/ai/formrecognizer/_generated/v2_1/aio/_patch.py
 azure/ai/formrecognizer/_generated/v2_1/aio/_vendor.py
 azure/ai/formrecognizer/_generated/v2_1/aio/operations/__init__.py
 azure/ai/formrecognizer/_generated/v2_1/aio/operations/_form_recognizer_client_operations.py
```

### Comparing `azure-ai-formrecognizer-3.3.2/samples/README.md` & `azure-ai-formrecognizer-3.3.3/samples/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 |[sample_convert_to_and_from_dict.py][sample_convert_to_and_from_dict_v3_1] and [sample_convert_to_and_from_dict_async.py][sample_convert_to_and_from_dict_async_v3_1]|Convert model types to a dictionary that can be used to create JSON content, then convert the same dictionary back to the original model type|
 
 ## Samples for client library versions 3.0.0 and below
 
 Please see the samples [here][v3.0.0-samples-tag].
 
 ## Prerequisites
-* Python 3.7 or later is required to use this package
+* Python 3.8 or later is required to use this package
 * You must have an [Azure subscription][azure_subscription] and an
 [Azure Form Recognizer account][azure_form_recognizer_account] to run these samples.
 
 ## Setup
 
 1. Install the Azure Form Recognizer client library for Python with [pip][pip]:
```

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_authentication_v3_1_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_authentication_v3_1_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_convert_to_and_from_dict_v3_1_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_convert_to_and_from_dict_v3_1_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_copy_model_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_copy_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_create_composed_model_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_create_composed_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_differentiate_output_labeled_tables_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_differentiate_output_labeled_tables_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_differentiate_output_models_trained_with_and_without_labels_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_differentiate_output_models_trained_with_and_without_labels_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_get_bounding_boxes_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_get_bounding_boxes_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_manage_custom_models_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_manage_custom_models_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_business_cards_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_business_cards_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_content_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_content_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_custom_forms_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_custom_forms_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_identity_documents_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_identity_documents_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_invoices_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_invoices_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_receipts_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_receipts_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_recognize_receipts_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_recognize_receipts_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_strongly_typing_recognized_form_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_strongly_typing_recognized_form_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_train_model_with_labels_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_train_model_with_labels_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/async_samples/sample_train_model_without_labels_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/async_samples/sample_train_model_without_labels_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_authentication_v3_1.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_authentication_v3_1.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_convert_to_and_from_dict_v3_1.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_convert_to_and_from_dict_v3_1.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_copy_model.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_copy_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_create_composed_model.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_create_composed_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_differentiate_output_labeled_tables.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_differentiate_output_labeled_tables.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_differentiate_output_models_trained_with_and_without_labels.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_differentiate_output_models_trained_with_and_without_labels.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_get_bounding_boxes.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_get_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_manage_custom_models.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_manage_custom_models.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_business_cards.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_business_cards.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_content.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_content.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_custom_forms.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_custom_forms.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_identity_documents.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_identity_documents.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_invoices.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_invoices.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_receipts.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_receipts.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_recognize_receipts_from_url.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_recognize_receipts_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_strongly_typing_recognized_form.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_strongly_typing_recognized_form.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_train_model_with_labels.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_train_model_with_labels.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.1/sample_train_model_without_labels.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.1/sample_train_model_without_labels.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_barcodes_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_barcodes_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         endpoint=endpoint, credential=AzureKeyCredential(key)
     )
 
     async with document_analysis_client:
         # Specify which add-on capabilities to enable.
         with open(path_to_sample_documents, "rb") as f:
             poller = await document_analysis_client.begin_analyze_document(
-                "prebuilt-layout", document=f, features=[AnalysisFeature.barcode/QR code]
+                "prebuilt-layout", document=f, features=[AnalysisFeature.BARCODES]
             )
         result = await poller.result()
 
     # Iterate over extracted barcodes on each page.
     for page in result.pages:
         print(f"----Barcodes detected from page #{page.page_number}----")
         print(f"Detected {len(page.barcodes)} barcodes:")
```

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_fonts_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_fonts_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_formulas_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_formulas_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_highres_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_highres_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_addon_languages_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_addon_languages_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_business_cards_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_business_cards_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_custom_documents_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_custom_documents_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_general_documents_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_general_documents_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_identity_documents_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_identity_documents_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_invoices_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_invoices_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_layout_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_layout_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_read_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_read_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_receipts_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_receipts_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_receipts_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_receipts_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_analyze_tax_us_w2_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_analyze_tax_us_w2_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_authentication_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_authentication_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_build_classifier_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_build_classifier_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_build_model_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_build_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_classify_document_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_classify_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_classify_document_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_classify_document_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_compose_model_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_compose_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_convert_to_and_from_dict_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_convert_to_and_from_dict_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_copy_model_to_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_copy_model_to_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_get_elements_with_spans_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_get_elements_with_spans_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_get_operations_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_get_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_get_words_on_document_line_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_get_words_on_document_line_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_manage_classifiers_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_manage_classifiers_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_manage_models_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_manage_models_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/async_samples/sample_send_request_async.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/async_samples/sample_send_request_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,107 +31,108 @@
     endpoint = os.environ["AZURE_FORM_RECOGNIZER_ENDPOINT"]
     key = os.environ["AZURE_FORM_RECOGNIZER_KEY"]
 
     client = DocumentModelAdministrationClient(
         endpoint=endpoint, credential=AzureKeyCredential(key)
     )
     
-    # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
-    # while adding convenience for endpoint construction and service API versioning.
-    # Now let's use the `send_request` method to make a resource details fetching request.
-    # The URL of the request can be relative (your endpoint is the default base URL),
-    # and the API version of your client will automatically be used for the request.
-    request = HttpRequest(method="GET", url="info")
     async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(
-        f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
-        f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
-        f"The quota limit for custom neural document models is {response_body['customNeuralDocumentModelBuilds']['quota']} and the resource has"
-        f"used {response_body['customNeuralDocumentModelBuilds']['used']}. The resource quota will reset on {response_body['customNeuralDocumentModelBuilds']['quotaResetDateTime']}"
-    )
-    
-    # pass with absolute url and override the API version
-    request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/info?api-version=2022-08-31")
-    async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(
-        f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
-        f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
-        f"The quota limit for custom neural document models is {response_body['customNeuralDocumentModelBuilds']['quota']} and the resource has"
-        f"used {response_body['customNeuralDocumentModelBuilds']['used']}. The resource quota will reset on {response_body['customNeuralDocumentModelBuilds']['quotaResetDateTime']}"
-    )
-    
-    # override the API version to v2.1
-    request = HttpRequest(method="GET", url="v2.1/custom/models?op=summary")
-    async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
-    
-    # pass with absolute url and override the API version to v2.1
-    request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/v2.1/custom/models?op=summary")
-    async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
+        # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
+        # while adding convenience for endpoint construction and service API versioning.
+        # Now let's use the `send_request` method to make a resource details fetching request.
+        # The URL of the request can be relative (your endpoint is the default base URL),
+        # and the API version of your client will automatically be used for the request.
+        request = HttpRequest(method="GET", url="info")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
+            f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
+            f"The quota limit for custom neural document models is {response_body['customNeuralDocumentModelBuilds']['quota']} and the resource has"
+            f"used {response_body['customNeuralDocumentModelBuilds']['used']}. The resource quota will reset on {response_body['customNeuralDocumentModelBuilds']['quotaResetDateTime']}"
+        )
+    
+        # pass with absolute url and override the API version
+        request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/info?api-version=2022-08-31")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
+            f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
+        )
+    
+        # override the API version to v2.1
+        request = HttpRequest(method="GET", url="v2.1/custom/models?op=summary")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our account has {response_body['summary']['count']} custom models, "
+            f"and we can have at most {response_body['summary']['limit']} custom models."
+        )
+    
+        # pass with absolute url and override the API version to v2.1
+        request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/v2.1/custom/models?op=summary")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our account has {response_body['summary']['count']} custom models, "
+            f"and we can have at most {response_body['summary']['limit']} custom models."
+        )
 
 
 async def sample_send_request_v2():
     endpoint = os.environ["AZURE_FORM_RECOGNIZER_ENDPOINT"]
     key = os.environ["AZURE_FORM_RECOGNIZER_KEY"]
 
     # The default FormTrainingClient API version is v2.1
     client = FormTrainingClient(
         endpoint=endpoint, credential=AzureKeyCredential(key)
     )
-    
-    # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
-    # while adding convenience for endpoint construction and service API versioning.
-    # Now let's use the `send_request` method to make a resource details fetching request.
-    # The URL of the request can be relative (your endpoint is the default base URL),
-    # and the API version of your client will automatically be used for the request.
-    request = HttpRequest(method="GET", url="custom/models?op=summary")
-    async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
-    
-    # pass with absolute  url and override the API version
-    request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/v2.0/custom/models?op=summary")
-    async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
-    
-    # override the API version to 2023-07-31
-    # can only override the API version to 2022-08-31 or later with absolute url
-    request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/info?api-version=2023-07-31")
+
     async with client:
-        response = await client.send_request(request)
-    response.raise_for_status()
-    response_body = response.json()
-    print(
-        f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
-        f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
-        f"The quota limit for custom neural document models is {response_body['customNeuralDocumentModelBuilds']['quota']} and the resource has"
-        f"used {response_body['customNeuralDocumentModelBuilds']['used']}. The resource quota will reset on {response_body['customNeuralDocumentModelBuilds']['quotaResetDateTime']}"
-    )
+        # The `send_request` method can send custom HTTP requests that share the client's existing pipeline,
+        # while adding convenience for endpoint construction and service API versioning.
+        # Now let's use the `send_request` method to make a resource details fetching request.
+        # The URL of the request can be relative (your endpoint is the default base URL),
+        # and the API version of your client will automatically be used for the request.
+        request = HttpRequest(method="GET", url="custom/models?op=summary")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our account has {response_body['summary']['count']} custom models, "
+            f"and we can have at most {response_body['summary']['limit']} custom models."
+        )
+    
+        # pass with absolute  url and override the API version
+        request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/v2.0/custom/models?op=summary")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our account has {response_body['summary']['count']} custom models, "
+            f"and we can have at most {response_body['summary']['limit']} custom models."
+        )
+    
+        # override the API version to 2023-07-31
+        # can only override the API version to 2022-08-31 or later with absolute url
+        request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/info?api-version=2023-07-31")
+        response = await client.send_request(request)
+        response.raise_for_status()
+        response_body = response.json()
+        print(
+            f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
+            f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
+            f"The quota limit for custom neural document models is {response_body['customNeuralDocumentModelBuilds']['quota']} and the resource has"
+            f"used {response_body['customNeuralDocumentModelBuilds']['used']}. The resource quota will reset on {response_body['customNeuralDocumentModelBuilds']['quotaResetDateTime']}"
+        )
 
 
 async def main():
     await sample_send_request()
     await sample_send_request_v2()
```

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_barcodes.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_barcodes.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_fonts.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_fonts.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_formulas.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_formulas.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_highres.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_highres.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_addon_languages.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_addon_languages.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_business_cards.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_business_cards.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_custom_documents.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_custom_documents.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_general_documents.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_general_documents.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_identity_documents.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_identity_documents.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_invoices.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_invoices.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_layout.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_layout.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_read.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_read.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_receipts.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_receipts.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_receipts_from_url.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_receipts_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_analyze_tax_us_w2.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_analyze_tax_us_w2.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_authentication.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_authentication.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_build_classifier.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_build_classifier.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_build_model.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_build_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_classify_document.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_classify_document.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_classify_document_from_url.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_classify_document_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_compose_model.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_compose_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_convert_to_and_from_dict.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_convert_to_and_from_dict.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_copy_model_to.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_copy_model_to.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_get_elements_with_spans.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_get_elements_with_spans.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_get_operations.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_get_operations.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_get_words_on_document_line.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_get_words_on_document_line.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_manage_classifiers.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_manage_classifiers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_manage_models.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_manage_models.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/samples/v3.2_and_later/sample_send_request.py` & `azure-ai-formrecognizer-3.3.3/samples/v3.2_and_later/sample_send_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,33 +54,35 @@
     request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/info?api-version=2022-08-31")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
     print(
         f"Our resource has {response_body['customDocumentModels']['count']} custom models, "
         f"and we can have at most {response_body['customDocumentModels']['limit']} custom models."
-        f"The quota limit for custom neural document models is {response_body['customNeuralDocumentModelBuilds']['quota']} and the resource has"
-        f"used {response_body['customNeuralDocumentModelBuilds']['used']}. The resource quota will reset on {response_body['customNeuralDocumentModelBuilds']['quotaResetDateTime']}"
     )
     
     # override the API version to v2.1
     request = HttpRequest(method="GET", url="v2.1/custom/models?op=summary")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
+    print(
+        f"Our account has {response_body['summary']['count']} custom models, "
+        f"and we can have at most {response_body['summary']['limit']} custom models."
+    )
     
     # pass with absolute url and override the API version to v2.1
     request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/v2.1/custom/models?op=summary")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
+    print(
+        f"Our account has {response_body['summary']['count']} custom models, "
+        f"and we can have at most {response_body['summary']['limit']} custom models."
+    )
 
 
 def sample_send_request_v2():
     endpoint = os.environ["AZURE_FORM_RECOGNIZER_ENDPOINT"]
     key = os.environ["AZURE_FORM_RECOGNIZER_KEY"]
 
     # The default FormTrainingClient API version is v2.1
@@ -93,24 +95,28 @@
     # Now let's use the `send_request` method to make a resource details fetching request.
     # The URL of the request can be relative (your endpoint is the default base URL),
     # and the API version of your client will automatically be used for the request.
     request = HttpRequest(method="GET", url="custom/models?op=summary")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
+    print(
+        f"Our account has {response_body['summary']['count']} custom models, "
+        f"and we can have at most {response_body['summary']['limit']} custom models."
+    )
     
     # pass with absolute url and override the API version
     request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/v2.0/custom/models?op=summary")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
-    print(f"Our account has {response_body['summary']['count']} custom models, "
-          f"and we can have at most {response_body['summary']['limit']} custom models.")
+    print(
+        f"Our account has {response_body['summary']['count']} custom models, "
+        f"and we can have at most {response_body['summary']['limit']} custom models."
+    )
     
     # override the API version to 2023-07-31
     request = HttpRequest(method="GET", url=f"{endpoint}/formrecognizer/info?api-version=2023-07-31")
     response = client.send_request(request)
     response.raise_for_status()
     response_body = response.json()
     print(
```

### Comparing `azure-ai-formrecognizer-3.3.2/setup.py` & `azure-ai-formrecognizer-3.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,32 +46,32 @@
     url='https://github.com/Azure/azure-sdk-for-python',
     keywords="azure, form recognizer, cognitive services, document analyzer, document analysis, applied ai, azure sdk",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.ai',
     ]),
     package_data={
         'azure.ai.formrecognizer': ['py.typed'],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
-        "azure-core<2.0.0,>=1.23.0",
+        "azure-core>=1.23.0",
         "msrest>=0.6.21",
-        'azure-common~=1.1',
+        'azure-common>=1.1',
         "typing-extensions>=4.0.1",
     ]
 )
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/asynctestcase.py` & `azure-ai-formrecognizer-3.3.3/tests/asynctestcase.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/conftest.py` & `azure-ai-formrecognizer-3.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_custom_forms.py` & `azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_custom_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # ------------------------------------
 
 import os
 import pytest
 import functools
 from io import BytesIO
 from datetime import date, time
-from azure_devtools.perfstress_tests import PerfStressTest
+from devtools_testutils.perfstress_tests import PerfStressTest
 from azure.core.credentials import AzureKeyCredential
 from azure.ai.formrecognizer import FormRecognizerClient, FormContentType
 from azure.ai.formrecognizer.aio import FormRecognizerClient as AsyncFormRecognizerClient, FormTrainingClient as AsyncFormTrainingClient
 
 class RecognizeCustomForms(PerfStressTest):   
 
     def __init__(self, arguments):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_dac_analyze_document_from_url_requests.py` & `azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_dac_analyze_document_from_url_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 
 import os
-from azure_devtools.perfstress_tests import PerfStressTest
+from devtools_testutils.perfstress_tests import PerfStressTest
 from azure.core.credentials import AzureKeyCredential
 from azure.ai.formrecognizer import DocumentAnalysisClient
 from azure.ai.formrecognizer.aio import DocumentAnalysisClient as AsyncDocumentAnalysisClient
 
 class AnalyzeDocumentFromUrlRequestPreparation(PerfStressTest):   
 
     def __init__(self, arguments):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_dac_analyze_document_requests.py` & `azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_dac_analyze_document_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 
 import os
-from azure_devtools.perfstress_tests import PerfStressTest
+from devtools_testutils.perfstress_tests import PerfStressTest
 from azure.core.credentials import AzureKeyCredential
 from azure.ai.formrecognizer import DocumentAnalysisClient
 from azure.ai.formrecognizer.aio import DocumentAnalysisClient as AsyncDocumentAnalysisClient
 
 class AnalyzeDocumentRequestPreparation(PerfStressTest):   
 
     def __init__(self, arguments):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/perfstress_tests/perf_dmac_build_model_requests.py` & `azure-ai-formrecognizer-3.3.3/tests/perfstress_tests/perf_dmac_build_model_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 
 import os
-from azure_devtools.perfstress_tests import PerfStressTest
+from devtools_testutils.perfstress_tests import PerfStressTest
 from azure.core.credentials import AzureKeyCredential
 from azure.ai.formrecognizer import DocumentModelAdministrationClient
 from azure.ai.formrecognizer.aio import DocumentModelAdministrationClient as AsyncDocumentModelAdministrationClient
 
 class BuildModelRequestPreparation(PerfStressTest):   
 
     def __init__(self, arguments):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/preparers.py` & `azure-ai-formrecognizer-3.3.3/tests/preparers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_content_type.py` & `azure-ai-formrecognizer-3.3.3/tests/test_content_type.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_custom_model_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_custom_model_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_general_document.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_general_document.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_general_document_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_general_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_layout.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_layout.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_layout_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_layout_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilt_read.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilt_read.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilt_read_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilt_read_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,15 +572,15 @@
             receipt = fd.read()
 
         initial_poller = client.begin_analyze_document("prebuilt-receipt", receipt)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_analyze_document("prebuilt-receipt", None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentAnalysisClientPreparer()
     @recorded_by_proxy
     def test_receipt_locale_specified(self, client):
         with open(self.receipt_jpg, "rb") as fd:
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
         async with client:
             initial_poller = await client.begin_analyze_document("prebuilt-receipt", receipt)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_analyze_document("prebuilt-receipt", None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentAnalysisClientPreparer()
     @recorded_by_proxy_async
     async def test_receipt_locale_specified(self, client):
         with open(self.receipt_jpg, "rb") as fd:
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts_from_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         client = kwargs.pop("client")
 
         initial_poller = client.begin_analyze_document_from_url("prebuilt-receipt", self.receipt_url_jpg)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_analyze_document_from_url(None, None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentAnalysisClientPreparer()
     @recorded_by_proxy
     def test_receipt_locale_specified(self, client):
         poller = client.begin_analyze_document_from_url("prebuilt-receipt", self.receipt_url_jpg, locale="en-IN")
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_analyze_prebuilts_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_analyze_prebuilts_from_url_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,15 @@
 
         async with client:
             initial_poller = await client.begin_analyze_document_from_url("prebuilt-receipt", self.receipt_url_jpg)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_analyze_document_from_url("prebuilt-receipt", None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentAnalysisClientPreparer()
     @recorded_by_proxy_async
     async def test_receipt_locale_specified(self, client):
         async with client:
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_classify_document.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_classify_document.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dac_classify_document_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dac_classify_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_classifiers.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_classifiers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_classifiers_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_classifiers_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_compose_model.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_compose_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         initial_poller = client.begin_compose_document_model([model_1.model_id, model_2.model_id])
         cont_token = initial_poller.continuation_token()
 
         poller = client.begin_compose_document_model(None, continuation_token=cont_token)
         result = poller.result()
         assert result
 
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy
     def test_poller_metadata(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_compose_model_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_compose_model_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             initial_poller = await client.begin_compose_document_model([model_1.model_id, model_2.model_id])
             cont_token = initial_poller.continuation_token()
 
             poller = await client.begin_compose_document_model(None, continuation_token=cont_token)
             result = await poller.result()
             assert result
 
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy_async
     async def test_poller_metadata(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_copy_model.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_copy_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         initial_poller = client.begin_copy_document_model_to(model.model_id, target=target)
         cont_token = initial_poller.continuation_token()
 
         poller = client.begin_copy_document_model_to(model.model_id, None, continuation_token=cont_token)
         result = poller.result()
         assert result
 
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy
     def test_poller_metadata(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_copy_model_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_copy_model_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
             initial_poller = await client.begin_copy_document_model_to(model.model_id, target=target)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_copy_document_model_to(model.model_id, None, continuation_token=cont_token)
             result = await poller.result()
             assert result
 
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy_async
     async def test_poller_metadata(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_mgmt.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_mgmt.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_mgmt_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_mgmt_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_training.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy
     def test_build_model_polling_interval(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
         def check_poll_value(poll):
             if self.is_live:
-                assert poll == 5
+                assert poll == 1
             else:
                 assert poll == 0
         check_poll_value(client._client._config.polling_interval)
         poller = client.begin_build_document_model(blob_container_url=formrecognizer_storage_container_sas_url, build_mode="template", polling_interval=6)
         poller.wait()
         assert poller._polling_method._timeout == 6
         poller2 = client.begin_build_document_model(blob_container_url=formrecognizer_storage_container_sas_url, build_mode="template")
@@ -266,15 +266,15 @@
         client = kwargs.pop("client")
         formrecognizer_storage_container_sas_url = kwargs.pop("formrecognizer_storage_container_sas_url")
         initial_poller = client.begin_build_document_model("template", blob_container_url=formrecognizer_storage_container_sas_url)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_build_document_model("template", blob_container_url=None, continuation_token=cont_token)
         result = poller.result()
         assert result
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy
     def test_build_model_poller_metadata(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_dmac_training_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_dmac_training_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy_async
     async def test_build_model_polling_interval(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
         def check_poll_value(poll):
             if self.is_live:
-                assert poll == 5
+                assert poll == 1
             else:
                 assert poll == 0
         check_poll_value(client._client._config.polling_interval)
         poller = await client.begin_build_document_model(blob_container_url=formrecognizer_storage_container_sas_url, build_mode="template", polling_interval=6)
         await poller.wait()
         assert poller._polling_method._timeout == 6
         poller2 = await client.begin_build_document_model(blob_container_url=formrecognizer_storage_container_sas_url, build_mode="template")
@@ -247,15 +247,15 @@
         formrecognizer_storage_container_sas_url = kwargs.pop("formrecognizer_storage_container_sas_url")
         async with client:
             initial_poller = await client.begin_build_document_model("template", blob_container_url=formrecognizer_storage_container_sas_url)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_build_document_model("template", blob_container_url=None, continuation_token=cont_token)
             result = await poller.result()
             assert result
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy_async
     async def test_build_model_poller_metadata(self, client, formrecognizer_storage_container_sas_url, **kwargs):
         set_bodiless_matcher()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_business_card_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_business_card_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_content.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             my_file = fd.read()
         initial_poller = client.begin_recognize_content(my_file)
         cont_token = initial_poller.continuation_token()
 
         poller = client.begin_recognize_content(None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @pytest.mark.live_test_only
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer()
     @recorded_by_proxy
     def test_content_multipage_table_span_transform(self, client):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_content_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_content_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             my_file = fd.read()
         async with client:
             initial_poller = await client.begin_recognize_content(my_file)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_recognize_content(None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
 
     @pytest.mark.live_test_only
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer()
     @recorded_by_proxy_async
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_content_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_content_from_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         client = kwargs.pop("client")
         initial_poller = client.begin_recognize_content_from_url(self.form_url_jpg)
         cont_token = initial_poller.continuation_token()
 
         poller = client.begin_recognize_content_from_url(None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer()
     @recorded_by_proxy
     def test_content_multipage_table_span_pdf(self, client):
         poller = client.begin_recognize_content_from_url(self.multipage_table_url_pdf)
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_content_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_content_from_url_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         async with client:
             initial_poller = await client.begin_recognize_content_from_url(self.form_url_jpg)
             cont_token = initial_poller.continuation_token()
 
             poller = await client.begin_recognize_content_from_url(None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer()
     @recorded_by_proxy_async
     async def test_content_multipage_table_span_pdf(self, client):
         async with client:
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         poller = fr_client.begin_recognize_custom_forms(
             model.model_id,
             None,
             continuation_token=cont_token
         )
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @pytest.mark.live_test_only
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormTrainingClientPreparer()
     @recorded_by_proxy
     def test_custom_form_multipage_vendor_set_unlabeled_transform(self, client, formrecognizer_multipage_storage_container_sas_url_2_v2, **kwargs):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                 poller = await fr_client.begin_recognize_custom_forms(
                     model.model_id,
                     None,
                     continuation_token=cont_token
                 )
                 result = await poller.result()
                 assert result is not None
-                await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+                await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @pytest.mark.live_test_only
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormTrainingClientPreparer()
     @recorded_by_proxy_async
     async def test_custom_form_multipage_vendor_set_unlabeled_transform(self, client, formrecognizer_multipage_storage_container_sas_url_2_v2, **kwargs):
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms_from_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         poller = fr_client.begin_recognize_custom_forms_from_url(
             model.model_id,
             None,
             continuation_token=cont_token
         )
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormTrainingClientPreparer()
     @recorded_by_proxy
     def test_custom_form_multipage_vendor_set_unlabeled_transform(self, client, formrecognizer_multipage_storage_container_sas_url_2_v2, **kwargs):
         fr_client = client.get_form_recognizer_client()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_custom_forms_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_custom_forms_from_url_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                 poller = await fr_client.begin_recognize_custom_forms_from_url(
                     model.model_id,
                     None,
                     continuation_token=cont_token
                 )
                 result = await poller.result()
                 assert result is not None
-                await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+                await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @skip_flaky_test
     @FormRecognizerPreparer()
     @FormTrainingClientPreparer()
     @recorded_by_proxy_async
     async def test_custom_form_multipage_vendor_set_unlabeled_transform(self, client, formrecognizer_multipage_storage_container_sas_url_2_v2, **kwargs):
         fr_client = client.get_form_recognizer_client()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             id_document = fd.read()
 
         initial_poller = client.begin_recognize_identity_documents(id_document)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_recognize_identity_documents(None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     def test_identity_document_v2(self, **kwargs):
         client = kwargs.pop("client")
         with open(self.identity_document_license_jpg, "rb") as fd:
             id_document = fd.read()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             id_document = fd.read()
         async with client:
             initial_poller = await client.begin_recognize_identity_documents(id_document)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_recognize_identity_documents(None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     async def test_identity_document_v2(self, **kwargs):
         client = kwargs.pop("client")
         with open(self.identity_document_license_jpg, "rb") as fd:
             id_document = fd.read()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents_from_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     def test_identity_document_continuation_token(self, **kwargs):
         client = kwargs.pop("client")
         initial_poller = client.begin_recognize_identity_documents_from_url(self.identity_document_url_jpg)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_recognize_identity_documents_from_url(None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     def test_identity_document_v2(self, **kwargs):
         client = kwargs.pop("client")
         with pytest.raises(ValueError) as e:
             client.begin_recognize_identity_documents_from_url(self.identity_document_url_jpg)
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_identity_documents_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_identity_documents_from_url_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         client = kwargs.pop("client")
         async with client:
             initial_poller = await client.begin_recognize_identity_documents_from_url(self.identity_document_url_jpg)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_recognize_identity_documents_from_url(None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     async def test_identity_document_v2(self, **kwargs):
         client = kwargs.pop("client")
         with pytest.raises(ValueError) as e:
             async with client:
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             invoice = fd.read()
 
         initial_poller = client.begin_recognize_invoices(invoice)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_recognize_invoices(None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     def test_invoice_v2(self, **kwargs):
         client = kwargs.pop("client")
         with open(self.invoice_pdf, "rb") as fd:
             invoice = fd.read()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             invoice = fd.read()
         async with client:
             initial_poller = await client.begin_recognize_invoices(invoice)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_recognize_invoices(None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     async def test_invoice_v2(self, **kwargs):
         client = kwargs.pop("client")
         with open(self.invoice_pdf, "rb") as fd:
             invoice = fd.read()
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice_from_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         client = kwargs.pop("client")
 
         initial_poller = client.begin_recognize_invoices_from_url(self.invoice_url_tiff)
         cont_token = initial_poller.continuation_token()
         poller = client.begin_recognize_invoices_from_url(None, continuation_token=cont_token)
         result = poller.result()
         assert result is not None
-        initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+        initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     def test_invoice_v2(self, **kwargs):
         client = kwargs.pop("client")
         with pytest.raises(ValueError) as e:
             client.begin_recognize_invoices_from_url(self.invoice_url_tiff)
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_invoice_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_invoice_from_url_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         client = kwargs.pop("client")
         async with client:
             initial_poller = await client.begin_recognize_invoices_from_url(self.invoice_url_tiff)
             cont_token = initial_poller.continuation_token()
             poller = await client.begin_recognize_invoices_from_url(None, continuation_token=cont_token)
             result = await poller.result()
             assert result is not None
-            await initial_poller.wait()  # necessary so azure-devtools doesn't throw assertion error
+            await initial_poller.wait()  # necessary so devtools_testutils doesn't throw assertion error
 
     @FormRecognizerPreparer()
     @FormRecognizerClientPreparer(client_kwargs={"api_version": FormRecognizerApiVersion.V2_0})
     async def test_invoice_v2(self, **kwargs):
         client = kwargs.pop("client")
         with pytest.raises(ValueError) as e:
             async with client:
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt_from_url.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_frc_receipt_from_url_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_frc_receipt_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_compose_model.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_compose_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_compose_model_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_compose_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_copy_model.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_copy_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_copy_model_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_copy_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_mgmt.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_mgmt.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_mgmt_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_mgmt_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_training.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_training.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_ftc_training_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_ftc_training_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_get_children.py` & `azure-ai-formrecognizer-3.3.3/tests/test_get_children.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_logging.py` & `azure-ai-formrecognizer-3.3.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_logging_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_logging_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_multiapi.py` & `azure-ai-formrecognizer-3.3.3/tests/test_multiapi.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_multiapi_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_multiapi_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_repr.py` & `azure-ai-formrecognizer-3.3.3/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_resolve_elements.py` & `azure-ai-formrecognizer-3.3.3/tests/test_resolve_elements.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_send_request.py` & `azure-ai-formrecognizer-3.3.3/tests/test_send_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,59 +18,61 @@
 
 class TestSendRequest(FormRecognizerTest):
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy
     def test_get_resource_details(self, client, **kwargs):
         set_bodiless_matcher()
+        resource_details = client.get_resource_details()
+
         request = HttpRequest(
             method="GET",
             url="info",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info1 = result.json()
         assert received_info1
         assert received_info1["customDocumentModels"]
-        assert received_info1["customDocumentModels"]["count"] == 0
-        assert received_info1["customDocumentModels"]["limit"] == 250
+        assert received_info1["customDocumentModels"]["count"] == resource_details.custom_document_models.count
+        assert received_info1["customDocumentModels"]["limit"] == resource_details.custom_document_models.limit
 
         request = HttpRequest(
             method="GET",
             url="info?api-version=2022-08-31",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info2 = result.json()
         assert received_info2["customDocumentModels"]["count"] == received_info1["customDocumentModels"]["count"]
         assert received_info2["customDocumentModels"]["limit"] == received_info1["customDocumentModels"]["limit"]
-        
+
         # test with absolute url
         request = HttpRequest(
             method="GET",
             url=f"{client._endpoint}/formrecognizer/info?api-version=2022-08-31",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info3 = result.json()
         assert received_info3["customDocumentModels"]["count"] == received_info1["customDocumentModels"]["count"]
         assert received_info3["customDocumentModels"]["limit"] == received_info1["customDocumentModels"]["limit"]
-        
+
         # test with v2 API version
         request = HttpRequest(
             method="GET",
             url="v2.1/custom/models?op=summary",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info4 = result.json()
         assert received_info4
-        assert received_info4["summary"]["count"] == 0
-        assert received_info4["summary"]["limit"]
-        
+        assert received_info4["summary"]["count"] == resource_details.custom_document_models.count
+        assert received_info4["summary"]["limit"] == resource_details.custom_document_models.limit
+
         # test with v2 API version with absolute url
         request = HttpRequest(
             method="GET",
             url=f"{client._endpoint}/formrecognizer/v2.1/custom/models?op=summary",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
@@ -79,52 +81,54 @@
         assert received_info5["summary"]["limit"] == received_info4["summary"]["limit"]
 
     @FormRecognizerPreparer()
     @FormTrainingClientPreparer(client_kwargs={"api_version": "2.1"})
     @recorded_by_proxy
     def test_get_account_properties_v2(self, client):
         set_bodiless_matcher()
+        account_properties = client.get_account_properties()
+
         request = HttpRequest(
             method="GET",
             url="custom/models?op=summary",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info1 = result.json()
         assert received_info1
         assert received_info1["summary"]
-        assert received_info1["summary"]["count"] == 0
-        assert received_info1["summary"]["limit"] == 250
-        
+        assert received_info1["summary"]["count"] == account_properties.custom_model_count
+        assert received_info1["summary"]["limit"] == account_properties.custom_model_limit
+
         # test with absolute url
         request = HttpRequest(
             method="GET",
             url=f"{client._endpoint}/formrecognizer/v2.0/custom/models?op=summary",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info3 = result.json()
         assert received_info3["summary"]["count"] == received_info1["summary"]["count"]
         assert received_info3["summary"]["limit"] == received_info1["summary"]["limit"]
-        
+
         # relative URLs can't override the API version on 2.x clients
         request = HttpRequest(
             method="GET",
             url="info?api-version=2022-08-31",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info4 = result.json()
         assert received_info4["error"]["code"] == "404"
         assert received_info4["error"]["message"] == "Resource not found"
-        
+
         # test with v2 API version with absolute url
         request = HttpRequest(
             method="GET",
             url=f"{client._endpoint}/formrecognizer/info?api-version=2022-08-31",
             headers={"Accept": "application/json"},
         )
         result = client.send_request(request)
         received_info5 = result.json()
         assert received_info5
-        assert received_info5["customDocumentModels"]["count"] == 0
-        assert received_info5["customDocumentModels"]["limit"] == 250
+        assert received_info5["customDocumentModels"]["count"] == account_properties.custom_model_count
+        assert received_info5["customDocumentModels"]["limit"] == account_properties.custom_model_limit
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_send_request_async.py` & `azure-ai-formrecognizer-3.3.3/tests/test_send_request_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 from asynctestcase import AsyncFormRecognizerTest
 
 DocumentModelAdministrationClientPreparer = functools.partial(_GlobalClientPreparer, DocumentModelAdministrationClient)
 FormTrainingClientPreparer = functools.partial(_GlobalClientPreparer, FormTrainingClient)
 
 
 class TestSendRequestAsync(AsyncFormRecognizerTest):
-
     @FormRecognizerPreparer()
     @DocumentModelAdministrationClientPreparer()
     @recorded_by_proxy_async
     async def test_get_resource_details(self, client, **kwargs):
         set_bodiless_matcher()
         async with client:
+            resource_details = await client.get_resource_details()
+
             request = HttpRequest(
                 method="GET",
                 url="info",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
             received_info1 = result.json()
             assert received_info1
             assert received_info1["customDocumentModels"]
-            assert received_info1["customDocumentModels"]["count"] == 0
-            assert received_info1["customDocumentModels"]["limit"] == 250
+            assert received_info1["customDocumentModels"]["count"] == resource_details.custom_document_models.count
+            assert received_info1["customDocumentModels"]["limit"] == resource_details.custom_document_models.limit
 
             request = HttpRequest(
                 method="GET",
                 url="info?api-version=2022-08-31",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
@@ -62,17 +63,17 @@
                 method="GET",
                 url="v2.1/custom/models?op=summary",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
             received_info4 = result.json()
             assert received_info4
-            assert received_info4["summary"]["count"] == 0
-            assert received_info4["summary"]["limit"] == 250
-            
+            assert received_info4["summary"]["count"] == resource_details.custom_document_models.count
+            assert received_info4["summary"]["limit"] == resource_details.custom_document_models.limit
+
             # test with v2 API version with absolute url
             request = HttpRequest(
                 method="GET",
                 url=f"{client._endpoint}/formrecognizer/v2.1/custom/models?op=summary",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
@@ -82,52 +83,54 @@
 
     @FormRecognizerPreparer()
     @FormTrainingClientPreparer(client_kwargs={"api_version": "2.1"})
     @recorded_by_proxy_async
     async def test_get_account_properties_v2(self, client):
         set_bodiless_matcher()
         async with client:
+            account_properties = await client.get_account_properties()
+
             request = HttpRequest(
                 method="GET",
                 url="custom/models?op=summary",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
             received_info1 = result.json()
             assert received_info1
             assert received_info1["summary"]
-            assert received_info1["summary"]["count"] == 0
-            assert received_info1["summary"]["limit"] == 250
-            
+            assert received_info1["summary"]["count"] == account_properties.custom_model_count
+            assert received_info1["summary"]["limit"] == account_properties.custom_model_limit
+
             # test with absolute url
             request = HttpRequest(
                 method="GET",
                 url=f"{client._endpoint}/formrecognizer/v2.0/custom/models?op=summary",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
             received_info3 = result.json()
             assert received_info3["summary"]["count"] == received_info1["summary"]["count"]
             assert received_info3["summary"]["limit"] == received_info1["summary"]["limit"]
-            
+
             # relative URLs can't override the API version on 2.x clients
             request = HttpRequest(
                 method="GET",
                 url="info?api-version=2022-08-31",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
             received_info4 = result.json()
             assert received_info4["error"]["code"] == "404"
             assert received_info4["error"]["message"] == "Resource not found"
-            
+
             # test with v2 API version with absolute url
             request = HttpRequest(
                 method="GET",
                 url=f"{client._endpoint}/formrecognizer/info?api-version=2022-08-31",
                 headers={"Accept": "application/json"},
             )
             result = await client.send_request(request)
             received_info5 = result.json()
             assert received_info5
-            assert received_info5["customDocumentModels"]["count"] == 0
-            assert received_info5["customDocumentModels"]["limit"] == 250
+            assert received_info5["customDocumentModels"]["count"] == account_properties.custom_model_count
+            assert received_info5["customDocumentModels"]["limit"] == account_properties.custom_model_limit
```

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_to_dict_v2.py` & `azure-ai-formrecognizer-3.3.3/tests/test_to_dict_v2.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/test_to_dict_v3.py` & `azure-ai-formrecognizer-3.3.3/tests/test_to_dict_v3.py`

 * *Files identical despite different names*

### Comparing `azure-ai-formrecognizer-3.3.2/tests/testcase.py` & `azure-ai-formrecognizer-3.3.3/tests/testcase.py`

 * *Files identical despite different names*

