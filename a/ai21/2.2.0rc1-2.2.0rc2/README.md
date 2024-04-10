# Comparing `tmp/ai21-2.2.0rc1.tar.gz` & `tmp/ai21-2.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-2.2.0rc1.tar", max compression
+gzip compressed data, was "ai21-2.2.0rc2.tar", max compression
```

## Comparing `ai21-2.2.0rc1.tar` & `ai21-2.2.0rc2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    11357 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/LICENSE
--rw-r--r--   0        0        0     9133 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/README.md
--rw-r--r--   0        0        0     1575 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/__init__.py
--rw-r--r--   0        0        0     1014 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/ai21_env_config.py
--rw-r--r--   0        0        0     2626 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/ai21_http_client.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/clients/bedrock/__init__.py
--rw-r--r--   0        0        0      844 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/clients/bedrock/ai21_bedrock_client.py
--rw-r--r--   0        0        0       92 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/clients/bedrock/bedrock_model_id.py
--rw-r--r--   0        0        0     2414 2024-03-27 13:26:34.427976 ai21-2.2.0rc1/ai21/clients/bedrock/bedrock_session.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/bedrock/resources/__init__.py
--rw-r--r--   0        0        0     1996 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/bedrock/resources/bedrock_completion.py
--rw-r--r--   0        0        0      522 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/bedrock/resources/bedrock_resource.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/__init__.py
--rw-r--r--   0        0        0      829 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/answer_base.py
--rw-r--r--   0        0        0     3670 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/chat_base.py
--rw-r--r--   0        0        0     4172 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/completion_base.py
--rw-r--r--   0        0        0     1594 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/custom_model_base.py
--rw-r--r--   0        0        0     1846 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/dataset_base.py
--rw-r--r--   0        0        0      868 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/embed_base.py
--rw-r--r--   0        0        0      557 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/gec_base.py
--rw-r--r--   0        0        0      751 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/improvements_base.py
--rw-r--r--   0        0        0     1438 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/paraphrase_base.py
--rw-r--r--   0        0        0      786 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/segmentation_base.py
--rw-r--r--   0        0        0     1177 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/summarize_base.py
--rw-r--r--   0        0        0     1103 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/common/summarize_by_segment_base.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/ai21_sagemaker_client.py
--rw-r--r--   0        0        0      154 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/constants.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/__init__.py
--rw-r--r--   0        0        0      498 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_answer.py
--rw-r--r--   0        0        0     3194 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_completion.py
--rw-r--r--   0        0        0      399 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_gec.py
--rw-r--r--   0        0        0      789 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
--rw-r--r--   0        0        0      484 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_resource.py
--rw-r--r--   0        0        0      810 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_summarize.py
--rw-r--r--   0        0        0     2522 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/sagemaker/sagemaker_session.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/__init__.py
--rw-r--r--   0        0        0     3314 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/ai21_client.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/__init__.py
--rw-r--r--   0        0        0      101 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/chat/__init__.py
--rw-r--r--   0        0        0     2882 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/chat/chat_completions.py
--rw-r--r--   0        0        0      564 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_answer.py
--rw-r--r--   0        0        0     1722 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_chat.py
--rw-r--r--   0        0        0     1974 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_completion.py
--rw-r--r--   0        0        0     1268 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_custom_model.py
--rw-r--r--   0        0        0     1485 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_dataset.py
--rw-r--r--   0        0        0      574 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_embed.py
--rw-r--r--   0        0        0      462 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_gec.py
--rw-r--r--   0        0        0      729 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_improvements.py
--rw-r--r--   0        0        0     3594 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_library.py
--rw-r--r--   0        0        0      851 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_paraphrase.py
--rw-r--r--   0        0        0     1096 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_resource.py
--rw-r--r--   0        0        0      602 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_segmentation.py
--rw-r--r--   0        0        0      869 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_summarize.py
--rw-r--r--   0        0        0      760 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/clients/studio/resources/studio_summarize_by_segment.py
--rw-r--r--   0        0        0       64 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/constants.py
--rw-r--r--   0        0        0     2615 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/errors.py
--rw-r--r--   0        0        0     4864 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/http_client.py
--rw-r--r--   0        0        0      484 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/logger.py
--rw-r--r--   0        0        0     2633 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/__init__.py
--rw-r--r--   0        0        0      262 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/ai21_base_model_mixin.py
--rw-r--r--   0        0        0      343 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/chat/__init__.py
--rw-r--r--   0        0        0      592 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/chat/chat_completion_response.py
--rw-r--r--   0        0        0      220 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/chat/chat_message.py
--rw-r--r--   0        0        0       97 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/chat/role_type.py
--rw-r--r--   0        0        0      233 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/chat_message.py
--rw-r--r--   0        0        0       89 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/document_type.py
--rw-r--r--   0        0        0       96 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/embed_type.py
--rw-r--r--   0        0        0      286 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/improvement_type.py
--rw-r--r--   0        0        0      410 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/logprobs.py
--rw-r--r--   0        0        0      168 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/paraphrase_style_type.py
--rw-r--r--   0        0        0      503 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/penalty.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/__init__.py
--rw-r--r--   0        0        0      273 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/answer_response.py
--rw-r--r--   0        0        0      518 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/chat_response.py
--rw-r--r--   0        0        0      786 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/completion_response.py
--rw-r--r--   0        0        0      713 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/custom_model_response.py
--rw-r--r--   0        0        0      376 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/dataset_response.py
--rw-r--r--   0        0        0      300 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/embed_response.py
--rw-r--r--   0        0        0      550 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/file_response.py
--rw-r--r--   0        0        0      635 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/gec_response.py
--rw-r--r--   0        0        0      401 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/improvement_response.py
--rw-r--r--   0        0        0      469 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/library_answer_response.py
--rw-r--r--   0        0        0      450 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/library_search_response.py
--rw-r--r--   0        0        0      294 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/paraphrase_response.py
--rw-r--r--   0        0        0      317 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/segmentation_response.py
--rw-r--r--   0        0        0      564 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/summarize_by_segment_response.py
--rw-r--r--   0        0        0      187 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/responses/summarize_response.py
--rw-r--r--   0        0        0      139 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/summary_method.py
--rw-r--r--   0        0        0      222 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/models/usage_info.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/py.typed
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/services/__init__.py
--rw-r--r--   0        0        0     2296 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/services/sagemaker.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/tokenizers/__init__.py
--rw-r--r--   0        0        0      568 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/tokenizers/ai21_tokenizer.py
--rw-r--r--   0        0        0      535 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/tokenizers/factory.py
--rw-r--r--   0        0        0      722 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/types.py
--rw-r--r--   0        0        0        0 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/utils/__init__.py
--rw-r--r--   0        0        0      668 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/utils/typing.py
--rw-r--r--   0        0        0       23 2024-03-27 13:26:34.431976 ai21-2.2.0rc1/ai21/version.py
--rw-r--r--   0        0        0     2266 2024-03-27 13:26:34.435976 ai21-2.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     9848 1970-01-01 00:00:00.000000 ai21-2.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/LICENSE
+-rw-r--r--   0        0        0    11868 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/README.md
+-rw-r--r--   0        0        0     1575 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/ai21_env_config.py
+-rw-r--r--   0        0        0     2626 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/ai21_http_client.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/__init__.py
+-rw-r--r--   0        0        0      844 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/ai21_bedrock_client.py
+-rw-r--r--   0        0        0       92 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/bedrock_model_id.py
+-rw-r--r--   0        0        0     2414 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/bedrock_session.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/resources/__init__.py
+-rw-r--r--   0        0        0     1996 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/resources/bedrock_completion.py
+-rw-r--r--   0        0        0      522 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/bedrock/resources/bedrock_resource.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/answer_base.py
+-rw-r--r--   0        0        0     3670 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/chat_base.py
+-rw-r--r--   0        0        0     4172 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/completion_base.py
+-rw-r--r--   0        0        0     1594 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/custom_model_base.py
+-rw-r--r--   0        0        0     1846 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/dataset_base.py
+-rw-r--r--   0        0        0      868 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/embed_base.py
+-rw-r--r--   0        0        0      557 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/gec_base.py
+-rw-r--r--   0        0        0      751 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/improvements_base.py
+-rw-r--r--   0        0        0     1438 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/paraphrase_base.py
+-rw-r--r--   0        0        0      786 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/segmentation_base.py
+-rw-r--r--   0        0        0     1177 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/summarize_base.py
+-rw-r--r--   0        0        0     1103 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/common/summarize_by_segment_base.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/__init__.py
+-rw-r--r--   0        0        0     1545 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/ai21_sagemaker_client.py
+-rw-r--r--   0        0        0      154 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/constants.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_answer.py
+-rw-r--r--   0        0        0     3194 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_completion.py
+-rw-r--r--   0        0        0      399 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_gec.py
+-rw-r--r--   0        0        0      789 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
+-rw-r--r--   0        0        0      484 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_resource.py
+-rw-r--r--   0        0        0      810 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_summarize.py
+-rw-r--r--   0        0        0     2522 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/sagemaker/sagemaker_session.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/__init__.py
+-rw-r--r--   0        0        0     3496 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/ai21_client.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/chat/__init__.py
+-rw-r--r--   0        0        0     1999 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/chat/chat_completions.py
+-rw-r--r--   0        0        0      564 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_answer.py
+-rw-r--r--   0        0        0     1722 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_chat.py
+-rw-r--r--   0        0        0     1974 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_completion.py
+-rw-r--r--   0        0        0     1268 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_custom_model.py
+-rw-r--r--   0        0        0     1485 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_dataset.py
+-rw-r--r--   0        0        0      574 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_embed.py
+-rw-r--r--   0        0        0      462 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_gec.py
+-rw-r--r--   0        0        0      729 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_improvements.py
+-rw-r--r--   0        0        0     3594 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_library.py
+-rw-r--r--   0        0        0      851 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_paraphrase.py
+-rw-r--r--   0        0        0     1096 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_resource.py
+-rw-r--r--   0        0        0      602 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_segmentation.py
+-rw-r--r--   0        0        0      869 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_summarize.py
+-rw-r--r--   0        0        0      760 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/clients/studio/resources/studio_summarize_by_segment.py
+-rw-r--r--   0        0        0       64 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/constants.py
+-rw-r--r--   0        0        0     2615 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/errors.py
+-rw-r--r--   0        0        0     4864 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/http_client.py
+-rw-r--r--   0        0        0      484 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/logger.py
+-rw-r--r--   0        0        0     2633 2024-04-10 13:39:38.363638 ai21-2.2.0rc2/ai21/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/ai21_base_model_mixin.py
+-rw-r--r--   0        0        0      343 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/chat/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/chat/chat_completion_response.py
+-rw-r--r--   0        0        0      219 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/chat/chat_message.py
+-rw-r--r--   0        0        0       97 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/chat/role_type.py
+-rw-r--r--   0        0        0      233 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/chat_message.py
+-rw-r--r--   0        0        0       89 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/document_type.py
+-rw-r--r--   0        0        0       96 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/embed_type.py
+-rw-r--r--   0        0        0      286 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/improvement_type.py
+-rw-r--r--   0        0        0      410 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/logprobs.py
+-rw-r--r--   0        0        0      168 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/paraphrase_style_type.py
+-rw-r--r--   0        0        0      503 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/penalty.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/answer_response.py
+-rw-r--r--   0        0        0      518 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/chat_response.py
+-rw-r--r--   0        0        0      786 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/completion_response.py
+-rw-r--r--   0        0        0      713 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/custom_model_response.py
+-rw-r--r--   0        0        0      376 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/dataset_response.py
+-rw-r--r--   0        0        0      300 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/embed_response.py
+-rw-r--r--   0        0        0      550 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/file_response.py
+-rw-r--r--   0        0        0      635 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/gec_response.py
+-rw-r--r--   0        0        0      401 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/improvement_response.py
+-rw-r--r--   0        0        0      469 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/library_answer_response.py
+-rw-r--r--   0        0        0      450 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/library_search_response.py
+-rw-r--r--   0        0        0      294 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/paraphrase_response.py
+-rw-r--r--   0        0        0      317 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/segmentation_response.py
+-rw-r--r--   0        0        0      564 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/summarize_by_segment_response.py
+-rw-r--r--   0        0        0      187 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/responses/summarize_response.py
+-rw-r--r--   0        0        0      139 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/summary_method.py
+-rw-r--r--   0        0        0      222 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/models/usage_info.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/py.typed
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/services/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/services/sagemaker.py
+-rw-r--r--   0        0        0      123 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/tokenizers/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/tokenizers/ai21_tokenizer.py
+-rw-r--r--   0        0        0      628 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/tokenizers/factory.py
+-rw-r--r--   0        0        0      722 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/types.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/utils/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/utils/typing.py
+-rw-r--r--   0        0        0       23 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/ai21/version.py
+-rw-r--r--   0        0        0     2266 2024-04-10 13:39:38.367638 ai21-2.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    12584 1970-01-01 00:00:00.000000 ai21-2.2.0rc2/PKG-INFO
```

### Comparing `ai21-2.2.0rc1/LICENSE` & `ai21-2.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/README.md` & `ai21-2.2.0rc2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-    <a href="https://github.com/AI21Labs/ai21">AI21 Labs Python SDK</a>
+    <a href="https://github.com/AI21Labs/ai21-python">AI21 Labs Python SDK</a>
 </h1>
 
 [//]: # "Add when public"
 [//]: # '<a href="https://github.com/AI21Labs/ai21/actions?query=workflow%3ATest+event%3Apush+branch%3Amain"><img src="https://github.com/AI21Labs/ai21/actions/workflows/test.yaml/badge.svg" alt="Test"></a>'
 [//]: # '<a href="https://pypi.org/project/ai21" target="_blank"><img src="https://img.shields.io/pypi/pyversions/ai21?color=%2334D058" alt="Supported Python versions"></a>'
 
 <p align="center">
@@ -17,15 +17,15 @@
 </p>
 
 ---
 
 ## Migration from v1.3.4 and below
 
 In `v2.0.0` we introduced a new SDK that is not backwards compatible with the previous version.
-This version allows for Non static instances of the client, defined parameters to each resource, modelized responses and
+This version allows for non-static instances of the client, defined parameters to each resource, modelized responses and
 more.
 
 <details>
 <summary>Migration Examples</summary>
 
 ### Instance creation (not available in v1.3.4 and below)
 
@@ -109,72 +109,155 @@
 + from ai21 import AI21SageMakerClient
 + client = AI21SageMakerClient(endpoint_name="j2-mid-test-endpoint")
 + response = client.completion.create(prompt=prompt, max_tokens=1000)
 ```
 
 </details>
 
+## Documentation
+
+---
+
+The full documentation for the REST API can be found on [docs.ai21.com](https://docs.ai21.com/).
+
 ## Installation
 
-### pip
+---
 
 ```bash
 pip install ai21
 ```
 
 ## Usage
 
-### Model Types
+---
+
+```python
+from ai21 import AI21Client
+from ai21.models import RoleType
+from ai21.models.chat import ChatMessage
+
+client = AI21Client(
+    # defaults to os.enviorn.get('AI21_API_KEY')
+    api_key='my_api_key',
+)
+
+messages = [
+    # Could be a dict or a ChatMessage object
+    ChatMessage(content="Hello, this is a readme", role="user"),
+    ChatMessage(content="You are correct, how can I help you?", role="assistant"),
+]
+
+chat_completions = client.chat.completions.create(
+    messages=messages,
+    model="jamba-instruct-preview",
+)
+```
 
-Wherever you are required to pass a model name as a parameter, you can use any of the available AI21
-state-of-the-art models:
+A more detailed example can be found [here](examples/studio/chat/chat_completions.py).
+
+## Older Models Support Usage
+
+<details>
+<summary>Examples</summary>
+
+### Supported Models:
 
 - j2-light
 - j2-mid
 - j2-ultra
 
 you can read more about the models [here](https://docs.ai21.com/reference/j2-complete-api-ref#jurassic-2-models).
 
----
-
-### Client Instance Creation
+### Chat
 
 ```python
 from ai21 import AI21Client
+from ai21.models import RoleType
+from ai21.models import ChatMessage
 
-client = AI21Client(
-    # defaults to os.enviorn.get('AI21_API_KEY')
-    api_key='my_api_key',
+system = "You're a support engineer in a SaaS company"
+messages = [
+    ChatMessage(text="Hello, I need help with a signup process.", role=RoleType.USER),
+    ChatMessage(text="Hi Alice, I can help you with that. What seems to be the problem?", role=RoleType.ASSISTANT),
+    ChatMessage(text="I am having trouble signing up for your product with my Google account.", role=RoleType.USER),
+]
+
+
+client = AI21Client()
+chat_response = client.chat.create(
+    system=system,
+    messages=messages,
+    model="j2-ultra",
 )
+```
 
-response = client.completion.create(
-    prompt="<your prompt here>",
-    max_tokens=10,
+For a more detailed example, see the chat [examples](examples/studio/chat.py).
+
+### Completion
+
+```python
+from ai21 import AI21Client
+
+
+client = AI21Client()
+completion_response = client.completion.create(
+    prompt="This is a test prompt",
     model="j2-mid",
-    temperature=0.3,
-    top_p=1,
 )
+```
+
+</details>
+
+For a more detailed example, see the completion [examples](examples/studio/completion.py).
+
+---
+
+## TSMs
+
+AI21 Studio's Task-Specific Models offer a range of powerful tools. These models have been specifically designed for their respective tasks and provide high-quality results while optimizing efficiency.
+The full documentation and guides can be found [here](https://docs.ai21.com/docs/task-specific).
+
+### Contextual Answers
 
-print(response.completions)
-print(response.prompt)
+The `answer` API allows you to access our high-quality question answering model.
+
+```python
+from ai21 import AI21Client
+
+client = AI21Client()
+response = client.answer.create(
+    context="This is a text is for testing purposes",
+    question="Question about context",
+)
 ```
 
+A detailed explanation on Contextual Answers, can be found [here](https://docs.ai21.com/docs/contextual-answers-api)
+
 ### Token Counting
 
 ---
 
 By using the `count_tokens` method, you can estimate the billing for a given request.
 
 ```python
-from ai21 import AI21Client
+from ai21.tokenizers import get_tokenizer
 
-client = AI21Client()
-client.count_tokens(text="some text")  # returns int
+tokenizer = get_tokenizer(name="jamba-instruct-tokenizer")
+total_tokens = tokenizer.count_tokens(text="some text")  # returns int
+print(total_tokens)
 ```
 
+Available tokenizers are:
+
+- `jamba-instruct-tokenizer`
+- `j2-tokenizer`
+
+For more information on AI21 Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-tokenizer).
+
 ### File Upload
 
 ---
 
 ```python
 from ai21 import AI21Client
 
@@ -323,7 +406,17 @@
 
 response = client.completion.create(
     prompt="Your prompt here",
     model_id=BedrockModelID.J2_MID_V1,
     max_tokens=10,
 )
 ```
+
+## Examples
+
+Explore our examples to see our models in action! We've put together a variety of use cases and demonstrations to showcase the capabilities and functionality of our models.
+
+### [Check out the Examples](examples/)
+
+Feel free to dive in, experiment, and adapt these examples to suit your needs. We believe they'll help you get up and running quickly.
+
+Happy prompting! 🚀
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                       ************ _AA_II_22_11_ _LL_aa_bb_ss_ _PP_yy_tt_hh_oo_nn_ _SS_DD_KK ************
 [//]: # "Add when public" [//]: # '_[_T_e_s_t_]' [//]: # '_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
 _v_e_r_s_i_o_n_s_]'
  _[_T_e_s_t_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                       _[_S_e_m_a_n_t_i_c_ _R_e_l_e_a_s_e_ _S_u_p_p_o_r_t_]_[_L_i_c_e_n_s_e_]
 --- ## Migration from v1.3.4 and below In `v2.0.0` we introduced a new SDK that
 is not backwards compatible with the previous version. This version allows for
-Non static instances of the client, defined parameters to each resource,
+non-static instances of the client, defined parameters to each resource,
 modelized responses and more. Migration Examples ### Instance creation (not
 available in v1.3.4 and below) ```python from ai21 import AI21Client client =
 AI21Client(api_key='my_api_key') # or set api_key in environment variable -
 AI21_API_KEY and then client = AI21Client() ``` We No longer support static
 methods for each resource, instead we have a client instance that has a method
 for each allowing for more flexibility and better control. ### Completion
 before/after ```diff prompt = "some prompt" - import ai21 - response =
@@ -35,65 +35,100 @@
 AI21BedrockClient, BedrockModelID + client = AI21BedrockClient() + response =
 client.completion.create(prompt=prompt, max_tokens=1000,
 model_id=BedrockModelID.J2_MID_V1) ``` ### SageMaker Client creation before/
 after ```diff - import ai21 - destination = ai21.SageMakerDestination("j2-mid-
 test-endpoint") - response = ai21.Completion.execute(prompt=prompt,
 maxTokens=1000, destination=destination) + from ai21 import AI21SageMakerClient
 + client = AI21SageMakerClient(endpoint_name="j2-mid-test-endpoint") + response
-= client.completion.create(prompt=prompt, max_tokens=1000) ``` ## Installation
-### pip ```bash pip install ai21 ``` ## Usage ### Model Types Wherever you are
-required to pass a model name as a parameter, you can use any of the available
-AI21 state-of-the-art models: - j2-light - j2-mid - j2-ultra you can read more
-about the models [here](https://docs.ai21.com/reference/j2-complete-api-
-ref#jurassic-2-models). --- ### Client Instance Creation ```python from ai21
-import AI21Client client = AI21Client( # defaults to os.enviorn.get
-('AI21_API_KEY') api_key='my_api_key', ) response = client.completion.create
-( prompt="", max_tokens=10, model="j2-mid", temperature=0.3, top_p=1, ) print
-(response.completions) print(response.prompt) ``` ### Token Counting --- By
-using the `count_tokens` method, you can estimate the billing for a given
-request. ```python from ai21 import AI21Client client = AI21Client()
-client.count_tokens(text="some text") # returns int ``` ### File Upload --
-- ```python from ai21 import AI21Client client = AI21Client() file_id =
-client.library.files.create( file_path="path/to/file", path="path/to/file/in/
-library", labels=["label1", "label2"], public_url="www.example.com", )
-uploaded_file = client.library.files.get(file_id) ``` ## Environment Variables
---- You can set several environment variables to configure the client. ###
-Logging We use the standard library [`logging`](https://docs.python.org/3/
-library/logging.html) module. To enable logging, set the `AI21_LOG_LEVEL`
-environment variable. ```bash $ export AI21_LOG_LEVEL=debug ``` ### Other
-Important Environment Variables - `AI21_API_KEY` - Your API key. If not set,
-you must pass it to the client constructor. - `AI21_API_VERSION` - The API
-version. Defaults to `v1`. - `AI21_API_HOST` - The API host. Defaults to
-`https://api.ai21.com/v1/`. - `AI21_TIMEOUT_SEC` - The timeout for API
-requests. - `AI21_NUM_RETRIES` - The maximum number of retries for API
-requests. Defaults to `3` retries. - `AI21_AWS_REGION` - The AWS region to use
-for AWS clients. Defaults to `us-east-1`. ## Error Handling --- ```python from
-ai21 import errors as ai21_errors from ai21 import AI21Client, AI21APIError
-from ai21.models import ChatMessage client = AI21Client() system = "You're a
-support engineer in a SaaS company" messages = [ # Notice the given role does
-not exist and will be the reason for the raised error ChatMessage(text="Hello,
-I need help with a signup process.", role="Non-Existent-Role"), ] try:
-chat_completion = client.chat.create( messages=messages, model="j2-ultra",
-system=system ) except ai21_errors.AI21ServerError as e: print("Server error
-and could not be reached") print(e.details) except
-ai21_errors.TooManyRequestsError as e: print("A 429 status code was returned.
-Slow down on the requests") except AI21APIError as e: print("A non 200 status
-code error. For more error types see ai21.errors") ``` ## AWS Clients --- AI21
-Library provides convenient ways to interact with two AWS clients for use with
-AWS SageMaker and AWS Bedrock. ### Installation --- ```bash pip install "ai21
-[AWS]" ``` This will make sure you have the required dependencies installed,
-including `boto3 >= 1.28.82`. ### Usage --- #### SageMaker ```python from ai21
-import AI21SageMakerClient client = AI21SageMakerClient(endpoint_name="j2-
-endpoint-name") response = client.summarize.create( source="Text to summarize",
-source_type="TEXT", ) print(response.summary) ``` #### With Boto3 Session
-```python from ai21 import AI21SageMakerClient import boto3 boto_session =
-boto3.Session(region_name="us-east-1") client = AI21SageMakerClient
-( session=boto_session, endpoint_name="j2-endpoint-name", ) ``` #### Bedrock --
-- ```python from ai21 import AI21BedrockClient, BedrockModelID client =
-AI21BedrockClient(region='us-east-1') # region is optional, as you can use the
-env variable instead response = client.completion.create( prompt="Your prompt
-here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print
-(response.completions[0].data.text) ``` #### With Boto3 Session ```python from
-ai21 import AI21BedrockClient, BedrockModelID import boto3 boto_session =
-boto3.Session(region_name="us-east-1") client = AI21BedrockClient
-( session=boto_session, ) response = client.completion.create( prompt="Your
-prompt here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ```
+= client.completion.create(prompt=prompt, max_tokens=1000) ``` ## Documentation
+--- The full documentation for the REST API can be found on [docs.ai21.com]
+(https://docs.ai21.com/). ## Installation --- ```bash pip install ai21 ``` ##
+Usage --- ```python from ai21 import AI21Client from ai21.models import
+RoleType from ai21.models.chat import ChatMessage client = AI21Client( #
+defaults to os.enviorn.get('AI21_API_KEY') api_key='my_api_key', ) messages =
+[ # Could be a dict or a ChatMessage object ChatMessage(content="Hello, this is
+a readme", role="user"), ChatMessage(content="You are correct, how can I help
+you?", role="assistant"), ] chat_completions = client.chat.completions.create
+( messages=messages, model="jamba-instruct-preview", ) ``` A more detailed
+example can be found [here](examples/studio/chat/chat_completions.py). ## Older
+Models Support Usage Examples ### Supported Models: - j2-light - j2-mid - j2-
+ultra you can read more about the models [here](https://docs.ai21.com/
+reference/j2-complete-api-ref#jurassic-2-models). ### Chat ```python from ai21
+import AI21Client from ai21.models import RoleType from ai21.models import
+ChatMessage system = "You're a support engineer in a SaaS company" messages =
+[ ChatMessage(text="Hello, I need help with a signup process.",
+role=RoleType.USER), ChatMessage(text="Hi Alice, I can help you with that. What
+seems to be the problem?", role=RoleType.ASSISTANT), ChatMessage(text="I am
+having trouble signing up for your product with my Google account.",
+role=RoleType.USER), ] client = AI21Client() chat_response = client.chat.create
+( system=system, messages=messages, model="j2-ultra", ) ``` For a more detailed
+example, see the chat [examples](examples/studio/chat.py). ### Completion
+```python from ai21 import AI21Client client = AI21Client() completion_response
+= client.completion.create( prompt="This is a test prompt", model="j2-mid", )
+``` For a more detailed example, see the completion [examples](examples/studio/
+completion.py). --- ## TSMs AI21 Studio's Task-Specific Models offer a range of
+powerful tools. These models have been specifically designed for their
+respective tasks and provide high-quality results while optimizing efficiency.
+The full documentation and guides can be found [here](https://docs.ai21.com/
+docs/task-specific). ### Contextual Answers The `answer` API allows you to
+access our high-quality question answering model. ```python from ai21 import
+AI21Client client = AI21Client() response = client.answer.create( context="This
+is a text is for testing purposes", question="Question about context", ) ``` A
+detailed explanation on Contextual Answers, can be found [here](https://
+docs.ai21.com/docs/contextual-answers-api) ### Token Counting --- By using the
+`count_tokens` method, you can estimate the billing for a given request.
+```python from ai21.tokenizers import get_tokenizer tokenizer = get_tokenizer
+(name="jamba-instruct-tokenizer") total_tokens = tokenizer.count_tokens
+(text="some text") # returns int print(total_tokens) ``` Available tokenizers
+are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For more information on AI21
+Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-
+tokenizer). ### File Upload --- ```python from ai21 import AI21Client client =
+AI21Client() file_id = client.library.files.create( file_path="path/to/file",
+path="path/to/file/in/library", labels=["label1", "label2"],
+public_url="www.example.com", ) uploaded_file = client.library.files.get
+(file_id) ``` ## Environment Variables --- You can set several environment
+variables to configure the client. ### Logging We use the standard library
+[`logging`](https://docs.python.org/3/library/logging.html) module. To enable
+logging, set the `AI21_LOG_LEVEL` environment variable. ```bash $ export
+AI21_LOG_LEVEL=debug ``` ### Other Important Environment Variables -
+`AI21_API_KEY` - Your API key. If not set, you must pass it to the client
+constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
+`AI21_API_HOST` - The API host. Defaults to `https://api.ai21.com/v1/`. -
+`AI21_TIMEOUT_SEC` - The timeout for API requests. - `AI21_NUM_RETRIES` - The
+maximum number of retries for API requests. Defaults to `3` retries. -
+`AI21_AWS_REGION` - The AWS region to use for AWS clients. Defaults to `us-
+east-1`. ## Error Handling --- ```python from ai21 import errors as ai21_errors
+from ai21 import AI21Client, AI21APIError from ai21.models import ChatMessage
+client = AI21Client() system = "You're a support engineer in a SaaS company"
+messages = [ # Notice the given role does not exist and will be the reason for
+the raised error ChatMessage(text="Hello, I need help with a signup process.",
+role="Non-Existent-Role"), ] try: chat_completion = client.chat.create
+( messages=messages, model="j2-ultra", system=system ) except
+ai21_errors.AI21ServerError as e: print("Server error and could not be
+reached") print(e.details) except ai21_errors.TooManyRequestsError as e: print
+("A 429 status code was returned. Slow down on the requests") except
+AI21APIError as e: print("A non 200 status code error. For more error types see
+ai21.errors") ``` ## AWS Clients --- AI21 Library provides convenient ways to
+interact with two AWS clients for use with AWS SageMaker and AWS Bedrock. ###
+Installation --- ```bash pip install "ai21[AWS]" ``` This will make sure you
+have the required dependencies installed, including `boto3 >= 1.28.82`. ###
+Usage --- #### SageMaker ```python from ai21 import AI21SageMakerClient client
+= AI21SageMakerClient(endpoint_name="j2-endpoint-name") response =
+client.summarize.create( source="Text to summarize", source_type="TEXT", )
+print(response.summary) ``` #### With Boto3 Session ```python from ai21 import
+AI21SageMakerClient import boto3 boto_session = boto3.Session(region_name="us-
+east-1") client = AI21SageMakerClient( session=boto_session, endpoint_name="j2-
+endpoint-name", ) ``` #### Bedrock --- ```python from ai21 import
+AI21BedrockClient, BedrockModelID client = AI21BedrockClient(region='us-east-
+1') # region is optional, as you can use the env variable instead response =
+client.completion.create( prompt="Your prompt here",
+model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print(response.completions
+[0].data.text) ``` #### With Boto3 Session ```python from ai21 import
+AI21BedrockClient, BedrockModelID import boto3 boto_session = boto3.Session
+(region_name="us-east-1") client = AI21BedrockClient( session=boto_session, )
+response = client.completion.create( prompt="Your prompt here",
+model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ``` ## Examples Explore our
+examples to see our models in action! We've put together a variety of use cases
+and demonstrations to showcase the capabilities and functionality of our
+models. ### [Check out the Examples](examples/) Feel free to dive in,
+experiment, and adapt these examples to suit your needs. We believe they'll
+help you get up and running quickly. Happy prompting! ð
```

### Comparing `ai21-2.2.0rc1/ai21/__init__.py` & `ai21-2.2.0rc2/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/ai21_env_config.py` & `ai21-2.2.0rc2/ai21/ai21_env_config.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/ai21_http_client.py` & `ai21-2.2.0rc2/ai21/ai21_http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/bedrock/ai21_bedrock_client.py` & `ai21-2.2.0rc2/ai21/clients/bedrock/ai21_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/bedrock/bedrock_session.py` & `ai21-2.2.0rc2/ai21/clients/bedrock/bedrock_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/bedrock/resources/bedrock_completion.py` & `ai21-2.2.0rc2/ai21/clients/bedrock/resources/bedrock_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/bedrock/resources/bedrock_resource.py` & `ai21-2.2.0rc2/ai21/clients/bedrock/resources/bedrock_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/answer_base.py` & `ai21-2.2.0rc2/ai21/clients/common/answer_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/chat_base.py` & `ai21-2.2.0rc2/ai21/clients/common/chat_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/completion_base.py` & `ai21-2.2.0rc2/ai21/clients/common/completion_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/custom_model_base.py` & `ai21-2.2.0rc2/ai21/clients/common/custom_model_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/dataset_base.py` & `ai21-2.2.0rc2/ai21/clients/common/dataset_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/embed_base.py` & `ai21-2.2.0rc2/ai21/clients/common/embed_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/gec_base.py` & `ai21-2.2.0rc2/ai21/clients/common/gec_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/improvements_base.py` & `ai21-2.2.0rc2/ai21/clients/common/improvements_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/paraphrase_base.py` & `ai21-2.2.0rc2/ai21/clients/common/paraphrase_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/segmentation_base.py` & `ai21-2.2.0rc2/ai21/clients/common/segmentation_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/summarize_base.py` & `ai21-2.2.0rc2/ai21/clients/common/summarize_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/common/summarize_by_segment_base.py` & `ai21-2.2.0rc2/ai21/clients/common/summarize_by_segment_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/sagemaker/ai21_sagemaker_client.py` & `ai21-2.2.0rc2/ai21/clients/sagemaker/ai21_sagemaker_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_completion.py` & `ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py` & `ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/sagemaker/resources/sagemaker_summarize.py` & `ai21-2.2.0rc2/ai21/clients/sagemaker/resources/sagemaker_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/sagemaker/sagemaker_session.py` & `ai21-2.2.0rc2/ai21/clients/sagemaker/sagemaker_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/ai21_client.py` & `ai21-2.2.0rc2/ai21/clients/studio/ai21_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import warnings
 from typing import Optional, Any, Dict
 
+from ai21_tokenizer import PreTrainedTokenizers
+
 from ai21.ai21_env_config import _AI21EnvConfig, AI21EnvConfig
 from ai21.ai21_http_client import AI21HTTPClient
 from ai21.clients.studio.resources.studio_answer import StudioAnswer
 from ai21.clients.studio.resources.studio_chat import StudioChat
 from ai21.clients.studio.resources.studio_completion import StudioCompletion
 from ai21.clients.studio.resources.studio_custom_model import StudioCustomModel
 from ai21.clients.studio.resources.studio_dataset import StudioDataset
@@ -59,13 +62,15 @@
         self.summarize_by_segment = StudioSummarizeBySegment(self._http_client)
         self.custom_model = StudioCustomModel(self._http_client)
         self.dataset = StudioDataset(self._http_client)
         self.answer = StudioAnswer(self._http_client)
         self.library = StudioLibrary(self._http_client)
         self.segmentation = StudioSegmentation(self._http_client)
 
-    def count_tokens(self, text: str) -> int:
-        # We might want to cache the tokenizer instance within the class
-        # and not globally as it might be used by other instances
+    def count_tokens(self, text: str, tokenizer_name: str = PreTrainedTokenizers.J2_TOKENIZER) -> int:
+        warnings.warn(
+            "Please use the global get_tokenizer() method directly instead of the AI21Client().count_tokens() method.",
+            DeprecationWarning,
+        )
 
-        tokenizer = get_tokenizer()
+        tokenizer = get_tokenizer(tokenizer_name)
         return tokenizer.count_tokens(text)
```

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/chat/chat_completions.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/chat/chat_completions.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,77 +7,57 @@
 from ai21.types import NotGiven, NOT_GIVEN
 from ai21.utils.typing import remove_not_given
 
 __all__ = ["ChatCompletions"]
 
 
 class ChatCompletions(StudioResource):
-    _module_name = "chat/complete"
+    _module_name = "chat/completions"
 
     def create(
         self,
         model: str,
         messages: List[ChatMessage],
-        n: int | NotGiven = NOT_GIVEN,
-        logprobs: bool | NotGiven = NOT_GIVEN,
-        top_logprobs: int | NotGiven = NOT_GIVEN,
         max_tokens: int | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
         stop: str | List[str] | NotGiven = NOT_GIVEN,
-        frequency_penalty: float | NotGiven = NOT_GIVEN,
-        presence_penalty: float | NotGiven = NOT_GIVEN,
         **kwargs: Any,
     ) -> ChatCompletionResponse:
         body = self._create_body(
             model=model,
             messages=messages,
-            n=n,
-            logprobs=logprobs,
-            top_logprobs=top_logprobs,
             stop=stop,
             temperature=temperature,
             max_tokens=max_tokens,
             top_p=top_p,
-            frequency_penalty=frequency_penalty,
-            presence_penalty=presence_penalty,
             **kwargs,
         )
 
         url = f"{self._client.get_base_url()}/{self._module_name}"
         response = self._post(url=url, body=body)
         return self._json_to_response(response)
 
     def _create_body(
         self,
         model: str,
         messages: List[ChatMessage],
-        n: Optional[int] | NotGiven,
-        logprobs: Optional[bool] | NotGiven,
-        top_logprobs: Optional[int] | NotGiven,
         max_tokens: Optional[int] | NotGiven,
         temperature: Optional[float] | NotGiven,
         top_p: Optional[float] | NotGiven,
         stop: Optional[Union[str, List[str]]] | NotGiven,
-        frequency_penalty: Optional[float] | NotGiven,
-        presence_penalty: Optional[float] | NotGiven,
         **kwargs: Any,
     ) -> Dict[str, Any]:
         return remove_not_given(
             {
                 "model": model,
                 "messages": [message.to_dict() for message in messages],
                 "temperature": temperature,
                 "maxTokens": max_tokens,
-                "n": n,
                 "topP": top_p,
-                "logprobs": logprobs,
-                "topLogprobs": top_logprobs,
                 "stop": stop,
-                "frequencyPenalty": frequency_penalty,
-                "presencePenalty": presence_penalty,
                 **kwargs,
             }
         )
 
     def _json_to_response(self, json: Dict[str, Any]) -> ChatCompletionResponse:
         return ChatCompletionResponse.from_dict(json)
```

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_answer.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_answer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_chat.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_chat.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_completion.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_custom_model.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_dataset.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_embed.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_embed.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_improvements.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_library.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_library.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_paraphrase.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_resource.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_segmentation.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_summarize.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/clients/studio/resources/studio_summarize_by_segment.py` & `ai21-2.2.0rc2/ai21/clients/studio/resources/studio_summarize_by_segment.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/errors.py` & `ai21-2.2.0rc2/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/http_client.py` & `ai21-2.2.0rc2/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/__init__.py` & `ai21-2.2.0rc2/ai21/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/chat/chat_completion_response.py` & `ai21-2.2.0rc2/ai21/models/chat/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/responses/chat_response.py` & `ai21-2.2.0rc2/ai21/models/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/responses/completion_response.py` & `ai21-2.2.0rc2/ai21/models/responses/completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/responses/custom_model_response.py` & `ai21-2.2.0rc2/ai21/models/responses/custom_model_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/responses/file_response.py` & `ai21-2.2.0rc2/ai21/models/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/responses/gec_response.py` & `ai21-2.2.0rc2/ai21/models/responses/gec_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/models/responses/summarize_by_segment_response.py` & `ai21-2.2.0rc2/ai21/models/responses/summarize_by_segment_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/services/sagemaker.py` & `ai21-2.2.0rc2/ai21/services/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/tokenizers/ai21_tokenizer.py` & `ai21-2.2.0rc2/ai21/tokenizers/ai21_tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Any
 
 from ai21_tokenizer import BaseTokenizer
 
 
 class AI21Tokenizer:
     """
     A class that wraps a tokenizer and provides additional functionality.
@@ -12,11 +12,11 @@
         self._tokenizer = tokenizer
 
     def count_tokens(self, text: str) -> int:
         encoded_text = self._tokenizer.encode(text)
 
         return len(encoded_text)
 
-    def tokenize(self, text: str) -> List[str]:
-        encoded_text = self._tokenizer.encode(text)
+    def tokenize(self, text: str, **kwargs: Any) -> List[str]:
+        encoded_text = self._tokenizer.encode(text, **kwargs)
 
-        return self._tokenizer.convert_ids_to_tokens(encoded_text)
+        return self._tokenizer.convert_ids_to_tokens(encoded_text, **kwargs)
```

### Comparing `ai21-2.2.0rc1/ai21/tokenizers/factory.py` & `ai21-2.2.0rc2/ai21/tokenizers/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Optional
+from typing import Dict
 
-from ai21_tokenizer import Tokenizer
+from ai21_tokenizer import Tokenizer, PreTrainedTokenizers
 
 from ai21.tokenizers.ai21_tokenizer import AI21Tokenizer
 
-_cached_tokenizer: Optional[AI21Tokenizer] = None
+_cached_tokenizers: Dict[str, AI21Tokenizer] = {}
 
 
-def get_tokenizer() -> AI21Tokenizer:
+def get_tokenizer(name: str = PreTrainedTokenizers.J2_TOKENIZER) -> AI21Tokenizer:
     """
     Get the tokenizer instance.
 
     If the tokenizer instance is not cached, it will be created using the Tokenizer.get_tokenizer() method.
     """
-    global _cached_tokenizer
+    global _cached_tokenizers
 
-    if _cached_tokenizer is None:
-        _cached_tokenizer = AI21Tokenizer(Tokenizer.get_tokenizer())
+    if _cached_tokenizers.get(name) is None:
+        _cached_tokenizers[name] = AI21Tokenizer(Tokenizer.get_tokenizer(name))
 
-    return _cached_tokenizer
+    return _cached_tokenizers[name]
```

### Comparing `ai21-2.2.0rc1/ai21/types.py` & `ai21-2.2.0rc2/ai21/types.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/ai21/utils/typing.py` & `ai21-2.2.0rc2/ai21/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.0rc1/pyproject.toml` & `ai21-2.2.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,26 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "if typing.TYPE_CHECKING:"
 ]
 
 [tool.poetry]
 name = "ai21"
-version = "2.2.0-rc.1"
+version = "2.2.0-rc.2"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
-ai21-tokenizer = "^0.3.9"
+ai21-tokenizer = "^0.9.0"
 boto3 = { version = "^1.28.82", optional = true }
 dataclasses-json = "^0.6.3"
 typing-extensions = "^4.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
```

### Comparing `ai21-2.2.0rc1/PKG-INFO` & `ai21-2.2.0rc2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 2.2.0rc1
+Version: 2.2.0rc2
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aws
-Requires-Dist: ai21-tokenizer (>=0.3.9,<0.4.0)
+Requires-Dist: ai21-tokenizer (>=0.9.0,<0.10.0)
 Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
-    <a href="https://github.com/AI21Labs/ai21">AI21 Labs Python SDK</a>
+    <a href="https://github.com/AI21Labs/ai21-python">AI21 Labs Python SDK</a>
 </h1>
 
 [//]: # "Add when public"
 [//]: # '<a href="https://github.com/AI21Labs/ai21/actions?query=workflow%3ATest+event%3Apush+branch%3Amain"><img src="https://github.com/AI21Labs/ai21/actions/workflows/test.yaml/badge.svg" alt="Test"></a>'
 [//]: # '<a href="https://pypi.org/project/ai21" target="_blank"><img src="https://img.shields.io/pypi/pyversions/ai21?color=%2334D058" alt="Supported Python versions"></a>'
 
 <p align="center">
@@ -37,15 +37,15 @@
 </p>
 
 ---
 
 ## Migration from v1.3.4 and below
 
 In `v2.0.0` we introduced a new SDK that is not backwards compatible with the previous version.
-This version allows for Non static instances of the client, defined parameters to each resource, modelized responses and
+This version allows for non-static instances of the client, defined parameters to each resource, modelized responses and
 more.
 
 <details>
 <summary>Migration Examples</summary>
 
 ### Instance creation (not available in v1.3.4 and below)
 
@@ -129,72 +129,155 @@
 + from ai21 import AI21SageMakerClient
 + client = AI21SageMakerClient(endpoint_name="j2-mid-test-endpoint")
 + response = client.completion.create(prompt=prompt, max_tokens=1000)
 ```
 
 </details>
 
+## Documentation
+
+---
+
+The full documentation for the REST API can be found on [docs.ai21.com](https://docs.ai21.com/).
+
 ## Installation
 
-### pip
+---
 
 ```bash
 pip install ai21
 ```
 
 ## Usage
 
-### Model Types
+---
+
+```python
+from ai21 import AI21Client
+from ai21.models import RoleType
+from ai21.models.chat import ChatMessage
+
+client = AI21Client(
+    # defaults to os.enviorn.get('AI21_API_KEY')
+    api_key='my_api_key',
+)
+
+messages = [
+    # Could be a dict or a ChatMessage object
+    ChatMessage(content="Hello, this is a readme", role="user"),
+    ChatMessage(content="You are correct, how can I help you?", role="assistant"),
+]
+
+chat_completions = client.chat.completions.create(
+    messages=messages,
+    model="jamba-instruct-preview",
+)
+```
 
-Wherever you are required to pass a model name as a parameter, you can use any of the available AI21
-state-of-the-art models:
+A more detailed example can be found [here](examples/studio/chat/chat_completions.py).
+
+## Older Models Support Usage
+
+<details>
+<summary>Examples</summary>
+
+### Supported Models:
 
 - j2-light
 - j2-mid
 - j2-ultra
 
 you can read more about the models [here](https://docs.ai21.com/reference/j2-complete-api-ref#jurassic-2-models).
 
----
-
-### Client Instance Creation
+### Chat
 
 ```python
 from ai21 import AI21Client
+from ai21.models import RoleType
+from ai21.models import ChatMessage
 
-client = AI21Client(
-    # defaults to os.enviorn.get('AI21_API_KEY')
-    api_key='my_api_key',
+system = "You're a support engineer in a SaaS company"
+messages = [
+    ChatMessage(text="Hello, I need help with a signup process.", role=RoleType.USER),
+    ChatMessage(text="Hi Alice, I can help you with that. What seems to be the problem?", role=RoleType.ASSISTANT),
+    ChatMessage(text="I am having trouble signing up for your product with my Google account.", role=RoleType.USER),
+]
+
+
+client = AI21Client()
+chat_response = client.chat.create(
+    system=system,
+    messages=messages,
+    model="j2-ultra",
 )
+```
 
-response = client.completion.create(
-    prompt="<your prompt here>",
-    max_tokens=10,
+For a more detailed example, see the chat [examples](examples/studio/chat.py).
+
+### Completion
+
+```python
+from ai21 import AI21Client
+
+
+client = AI21Client()
+completion_response = client.completion.create(
+    prompt="This is a test prompt",
     model="j2-mid",
-    temperature=0.3,
-    top_p=1,
 )
+```
+
+</details>
+
+For a more detailed example, see the completion [examples](examples/studio/completion.py).
+
+---
+
+## TSMs
+
+AI21 Studio's Task-Specific Models offer a range of powerful tools. These models have been specifically designed for their respective tasks and provide high-quality results while optimizing efficiency.
+The full documentation and guides can be found [here](https://docs.ai21.com/docs/task-specific).
+
+### Contextual Answers
 
-print(response.completions)
-print(response.prompt)
+The `answer` API allows you to access our high-quality question answering model.
+
+```python
+from ai21 import AI21Client
+
+client = AI21Client()
+response = client.answer.create(
+    context="This is a text is for testing purposes",
+    question="Question about context",
+)
 ```
 
+A detailed explanation on Contextual Answers, can be found [here](https://docs.ai21.com/docs/contextual-answers-api)
+
 ### Token Counting
 
 ---
 
 By using the `count_tokens` method, you can estimate the billing for a given request.
 
 ```python
-from ai21 import AI21Client
+from ai21.tokenizers import get_tokenizer
 
-client = AI21Client()
-client.count_tokens(text="some text")  # returns int
+tokenizer = get_tokenizer(name="jamba-instruct-tokenizer")
+total_tokens = tokenizer.count_tokens(text="some text")  # returns int
+print(total_tokens)
 ```
 
+Available tokenizers are:
+
+- `jamba-instruct-tokenizer`
+- `j2-tokenizer`
+
+For more information on AI21 Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-tokenizer).
+
 ### File Upload
 
 ---
 
 ```python
 from ai21 import AI21Client
 
@@ -344,7 +427,17 @@
 response = client.completion.create(
     prompt="Your prompt here",
     model_id=BedrockModelID.J2_MID_V1,
     max_tokens=10,
 )
 ```
 
+## Examples
+
+Explore our examples to see our models in action! We've put together a variety of use cases and demonstrations to showcase the capabilities and functionality of our models.
+
+### [Check out the Examples](examples/)
+
+Feel free to dive in, experiment, and adapt these examples to suit your needs. We believe they'll help you get up and running quickly.
+
+Happy prompting! 🚀
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: ai21 Version: 2.2.0rc1 Summary: Author: AI21 Labs
+Metadata-Version: 2.1 Name: ai21 Version: 2.2.0rc2 Summary: Author: AI21 Labs
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: aws Requires-Dist: ai21-tokenizer
-(>=0.3.9,<0.4.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
+(>=0.9.0,<0.10.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
                       ************ _AA_II_22_11_ _LL_aa_bb_ss_ _PP_yy_tt_hh_oo_nn_ _SS_DD_KK ************
 [//]: # "Add when public" [//]: # '_[_T_e_s_t_]' [//]: # '_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
 _v_e_r_s_i_o_n_s_]'
  _[_T_e_s_t_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                       _[_S_e_m_a_n_t_i_c_ _R_e_l_e_a_s_e_ _S_u_p_p_o_r_t_]_[_L_i_c_e_n_s_e_]
 --- ## Migration from v1.3.4 and below In `v2.0.0` we introduced a new SDK that
 is not backwards compatible with the previous version. This version allows for
-Non static instances of the client, defined parameters to each resource,
+non-static instances of the client, defined parameters to each resource,
 modelized responses and more. Migration Examples ### Instance creation (not
 available in v1.3.4 and below) ```python from ai21 import AI21Client client =
 AI21Client(api_key='my_api_key') # or set api_key in environment variable -
 AI21_API_KEY and then client = AI21Client() ``` We No longer support static
 methods for each resource, instead we have a client instance that has a method
 for each allowing for more flexibility and better control. ### Completion
 before/after ```diff prompt = "some prompt" - import ai21 - response =
@@ -45,65 +45,100 @@
 AI21BedrockClient, BedrockModelID + client = AI21BedrockClient() + response =
 client.completion.create(prompt=prompt, max_tokens=1000,
 model_id=BedrockModelID.J2_MID_V1) ``` ### SageMaker Client creation before/
 after ```diff - import ai21 - destination = ai21.SageMakerDestination("j2-mid-
 test-endpoint") - response = ai21.Completion.execute(prompt=prompt,
 maxTokens=1000, destination=destination) + from ai21 import AI21SageMakerClient
 + client = AI21SageMakerClient(endpoint_name="j2-mid-test-endpoint") + response
-= client.completion.create(prompt=prompt, max_tokens=1000) ``` ## Installation
-### pip ```bash pip install ai21 ``` ## Usage ### Model Types Wherever you are
-required to pass a model name as a parameter, you can use any of the available
-AI21 state-of-the-art models: - j2-light - j2-mid - j2-ultra you can read more
-about the models [here](https://docs.ai21.com/reference/j2-complete-api-
-ref#jurassic-2-models). --- ### Client Instance Creation ```python from ai21
-import AI21Client client = AI21Client( # defaults to os.enviorn.get
-('AI21_API_KEY') api_key='my_api_key', ) response = client.completion.create
-( prompt="", max_tokens=10, model="j2-mid", temperature=0.3, top_p=1, ) print
-(response.completions) print(response.prompt) ``` ### Token Counting --- By
-using the `count_tokens` method, you can estimate the billing for a given
-request. ```python from ai21 import AI21Client client = AI21Client()
-client.count_tokens(text="some text") # returns int ``` ### File Upload --
-- ```python from ai21 import AI21Client client = AI21Client() file_id =
-client.library.files.create( file_path="path/to/file", path="path/to/file/in/
-library", labels=["label1", "label2"], public_url="www.example.com", )
-uploaded_file = client.library.files.get(file_id) ``` ## Environment Variables
---- You can set several environment variables to configure the client. ###
-Logging We use the standard library [`logging`](https://docs.python.org/3/
-library/logging.html) module. To enable logging, set the `AI21_LOG_LEVEL`
-environment variable. ```bash $ export AI21_LOG_LEVEL=debug ``` ### Other
-Important Environment Variables - `AI21_API_KEY` - Your API key. If not set,
-you must pass it to the client constructor. - `AI21_API_VERSION` - The API
-version. Defaults to `v1`. - `AI21_API_HOST` - The API host. Defaults to
-`https://api.ai21.com/v1/`. - `AI21_TIMEOUT_SEC` - The timeout for API
-requests. - `AI21_NUM_RETRIES` - The maximum number of retries for API
-requests. Defaults to `3` retries. - `AI21_AWS_REGION` - The AWS region to use
-for AWS clients. Defaults to `us-east-1`. ## Error Handling --- ```python from
-ai21 import errors as ai21_errors from ai21 import AI21Client, AI21APIError
-from ai21.models import ChatMessage client = AI21Client() system = "You're a
-support engineer in a SaaS company" messages = [ # Notice the given role does
-not exist and will be the reason for the raised error ChatMessage(text="Hello,
-I need help with a signup process.", role="Non-Existent-Role"), ] try:
-chat_completion = client.chat.create( messages=messages, model="j2-ultra",
-system=system ) except ai21_errors.AI21ServerError as e: print("Server error
-and could not be reached") print(e.details) except
-ai21_errors.TooManyRequestsError as e: print("A 429 status code was returned.
-Slow down on the requests") except AI21APIError as e: print("A non 200 status
-code error. For more error types see ai21.errors") ``` ## AWS Clients --- AI21
-Library provides convenient ways to interact with two AWS clients for use with
-AWS SageMaker and AWS Bedrock. ### Installation --- ```bash pip install "ai21
-[AWS]" ``` This will make sure you have the required dependencies installed,
-including `boto3 >= 1.28.82`. ### Usage --- #### SageMaker ```python from ai21
-import AI21SageMakerClient client = AI21SageMakerClient(endpoint_name="j2-
-endpoint-name") response = client.summarize.create( source="Text to summarize",
-source_type="TEXT", ) print(response.summary) ``` #### With Boto3 Session
-```python from ai21 import AI21SageMakerClient import boto3 boto_session =
-boto3.Session(region_name="us-east-1") client = AI21SageMakerClient
-( session=boto_session, endpoint_name="j2-endpoint-name", ) ``` #### Bedrock --
-- ```python from ai21 import AI21BedrockClient, BedrockModelID client =
-AI21BedrockClient(region='us-east-1') # region is optional, as you can use the
-env variable instead response = client.completion.create( prompt="Your prompt
-here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print
-(response.completions[0].data.text) ``` #### With Boto3 Session ```python from
-ai21 import AI21BedrockClient, BedrockModelID import boto3 boto_session =
-boto3.Session(region_name="us-east-1") client = AI21BedrockClient
-( session=boto_session, ) response = client.completion.create( prompt="Your
-prompt here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ```
+= client.completion.create(prompt=prompt, max_tokens=1000) ``` ## Documentation
+--- The full documentation for the REST API can be found on [docs.ai21.com]
+(https://docs.ai21.com/). ## Installation --- ```bash pip install ai21 ``` ##
+Usage --- ```python from ai21 import AI21Client from ai21.models import
+RoleType from ai21.models.chat import ChatMessage client = AI21Client( #
+defaults to os.enviorn.get('AI21_API_KEY') api_key='my_api_key', ) messages =
+[ # Could be a dict or a ChatMessage object ChatMessage(content="Hello, this is
+a readme", role="user"), ChatMessage(content="You are correct, how can I help
+you?", role="assistant"), ] chat_completions = client.chat.completions.create
+( messages=messages, model="jamba-instruct-preview", ) ``` A more detailed
+example can be found [here](examples/studio/chat/chat_completions.py). ## Older
+Models Support Usage Examples ### Supported Models: - j2-light - j2-mid - j2-
+ultra you can read more about the models [here](https://docs.ai21.com/
+reference/j2-complete-api-ref#jurassic-2-models). ### Chat ```python from ai21
+import AI21Client from ai21.models import RoleType from ai21.models import
+ChatMessage system = "You're a support engineer in a SaaS company" messages =
+[ ChatMessage(text="Hello, I need help with a signup process.",
+role=RoleType.USER), ChatMessage(text="Hi Alice, I can help you with that. What
+seems to be the problem?", role=RoleType.ASSISTANT), ChatMessage(text="I am
+having trouble signing up for your product with my Google account.",
+role=RoleType.USER), ] client = AI21Client() chat_response = client.chat.create
+( system=system, messages=messages, model="j2-ultra", ) ``` For a more detailed
+example, see the chat [examples](examples/studio/chat.py). ### Completion
+```python from ai21 import AI21Client client = AI21Client() completion_response
+= client.completion.create( prompt="This is a test prompt", model="j2-mid", )
+``` For a more detailed example, see the completion [examples](examples/studio/
+completion.py). --- ## TSMs AI21 Studio's Task-Specific Models offer a range of
+powerful tools. These models have been specifically designed for their
+respective tasks and provide high-quality results while optimizing efficiency.
+The full documentation and guides can be found [here](https://docs.ai21.com/
+docs/task-specific). ### Contextual Answers The `answer` API allows you to
+access our high-quality question answering model. ```python from ai21 import
+AI21Client client = AI21Client() response = client.answer.create( context="This
+is a text is for testing purposes", question="Question about context", ) ``` A
+detailed explanation on Contextual Answers, can be found [here](https://
+docs.ai21.com/docs/contextual-answers-api) ### Token Counting --- By using the
+`count_tokens` method, you can estimate the billing for a given request.
+```python from ai21.tokenizers import get_tokenizer tokenizer = get_tokenizer
+(name="jamba-instruct-tokenizer") total_tokens = tokenizer.count_tokens
+(text="some text") # returns int print(total_tokens) ``` Available tokenizers
+are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For more information on AI21
+Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-
+tokenizer). ### File Upload --- ```python from ai21 import AI21Client client =
+AI21Client() file_id = client.library.files.create( file_path="path/to/file",
+path="path/to/file/in/library", labels=["label1", "label2"],
+public_url="www.example.com", ) uploaded_file = client.library.files.get
+(file_id) ``` ## Environment Variables --- You can set several environment
+variables to configure the client. ### Logging We use the standard library
+[`logging`](https://docs.python.org/3/library/logging.html) module. To enable
+logging, set the `AI21_LOG_LEVEL` environment variable. ```bash $ export
+AI21_LOG_LEVEL=debug ``` ### Other Important Environment Variables -
+`AI21_API_KEY` - Your API key. If not set, you must pass it to the client
+constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
+`AI21_API_HOST` - The API host. Defaults to `https://api.ai21.com/v1/`. -
+`AI21_TIMEOUT_SEC` - The timeout for API requests. - `AI21_NUM_RETRIES` - The
+maximum number of retries for API requests. Defaults to `3` retries. -
+`AI21_AWS_REGION` - The AWS region to use for AWS clients. Defaults to `us-
+east-1`. ## Error Handling --- ```python from ai21 import errors as ai21_errors
+from ai21 import AI21Client, AI21APIError from ai21.models import ChatMessage
+client = AI21Client() system = "You're a support engineer in a SaaS company"
+messages = [ # Notice the given role does not exist and will be the reason for
+the raised error ChatMessage(text="Hello, I need help with a signup process.",
+role="Non-Existent-Role"), ] try: chat_completion = client.chat.create
+( messages=messages, model="j2-ultra", system=system ) except
+ai21_errors.AI21ServerError as e: print("Server error and could not be
+reached") print(e.details) except ai21_errors.TooManyRequestsError as e: print
+("A 429 status code was returned. Slow down on the requests") except
+AI21APIError as e: print("A non 200 status code error. For more error types see
+ai21.errors") ``` ## AWS Clients --- AI21 Library provides convenient ways to
+interact with two AWS clients for use with AWS SageMaker and AWS Bedrock. ###
+Installation --- ```bash pip install "ai21[AWS]" ``` This will make sure you
+have the required dependencies installed, including `boto3 >= 1.28.82`. ###
+Usage --- #### SageMaker ```python from ai21 import AI21SageMakerClient client
+= AI21SageMakerClient(endpoint_name="j2-endpoint-name") response =
+client.summarize.create( source="Text to summarize", source_type="TEXT", )
+print(response.summary) ``` #### With Boto3 Session ```python from ai21 import
+AI21SageMakerClient import boto3 boto_session = boto3.Session(region_name="us-
+east-1") client = AI21SageMakerClient( session=boto_session, endpoint_name="j2-
+endpoint-name", ) ``` #### Bedrock --- ```python from ai21 import
+AI21BedrockClient, BedrockModelID client = AI21BedrockClient(region='us-east-
+1') # region is optional, as you can use the env variable instead response =
+client.completion.create( prompt="Your prompt here",
+model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print(response.completions
+[0].data.text) ``` #### With Boto3 Session ```python from ai21 import
+AI21BedrockClient, BedrockModelID import boto3 boto_session = boto3.Session
+(region_name="us-east-1") client = AI21BedrockClient( session=boto_session, )
+response = client.completion.create( prompt="Your prompt here",
+model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ``` ## Examples Explore our
+examples to see our models in action! We've put together a variety of use cases
+and demonstrations to showcase the capabilities and functionality of our
+models. ### [Check out the Examples](examples/) Feel free to dive in,
+experiment, and adapt these examples to suit your needs. We believe they'll
+help you get up and running quickly. Happy prompting! ð
```

