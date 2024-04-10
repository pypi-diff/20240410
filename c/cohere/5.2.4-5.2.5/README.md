# Comparing `tmp/cohere-5.2.4.tar.gz` & `tmp/cohere-5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.2.4.tar", max compression
+gzip compressed data, was "cohere-5.2.5.tar", max compression
```

## Comparing `cohere-5.2.4.tar` & `cohere-5.2.5.tar`

### file list

```diff
@@ -1,174 +1,176 @@
--rw-r--r--   0        0        0     1062 2024-04-08 21:30:12.679398 cohere-5.2.4/LICENSE
--rw-r--r--   0        0        0     2359 2024-04-08 21:30:12.679398 cohere-5.2.4/README.md
--rw-r--r--   0        0        0      679 2024-04-08 21:30:12.687398 cohere-5.2.4/pyproject.toml
--rw-r--r--   0        0        0     7869 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/__init__.py
--rw-r--r--   0        0        0   203898 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/base_client.py
--rw-r--r--   0        0        0    19312 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    50199 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/connectors/client.py
--rw-r--r--   0        0        0     1006 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/core/unchecked_base_model.py
--rw-r--r--   0        0        0      289 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    34988 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      417 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0     1002 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0      959 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1057 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      998 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-04-08 21:30:12.687398 cohere-5.2.4/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    31599 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      169 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      253 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    62127 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1475 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      305 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1175 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1083 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1400 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2357 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1171 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1823 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1489 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1532 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1463 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1577 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      402 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      193 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1390 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1177 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     1948 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    13071 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/py.typed
--rw-r--r--   0        0        0    10138 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1167 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1011 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1434 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0      168 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1929 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1127 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1861 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1297 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1644 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      168 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      170 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1708 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      189 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1011 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1180 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1247 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1653 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1055 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1417 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1861 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      225 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      893 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      176 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1714 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      195 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1017 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1102 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1068 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1040 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1004 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      971 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      171 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1137 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2560 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      214 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      971 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      220 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3383 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/connector.py
--rw-r--r--   0        0        0      163 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1660 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1725 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      960 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1195 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1047 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2209 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1648 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      471 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      222 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1068 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1416 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2271 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1364 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      211 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1864 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      201 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      156 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      168 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1057 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      184 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1735 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      222 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      185 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      171 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1197 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1101 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1311 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      897 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      191 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      177 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1312 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1456 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1254 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/generation.py
--rw-r--r--   0        0        0      957 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     1975 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1256 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1095 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      993 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1187 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1024 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     2701 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1080 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      974 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0     1001 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1200 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1342 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1056 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1818 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1819 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1248 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      952 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     3157 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      179 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      170 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      173 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1201 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1127 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1928 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1221 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1331 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      960 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10025 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-04-08 21:30:12.691398 cohere-5.2.4/src/cohere/version.py
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 cohere-5.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-10 16:01:41.721135 cohere-5.2.5/LICENSE
+-rw-r--r--   0        0        0     2359 2024-04-10 16:01:41.721135 cohere-5.2.5/README.md
+-rw-r--r--   0        0        0      679 2024-04-10 16:01:41.729135 cohere-5.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8012 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/__init__.py
+-rw-r--r--   0        0        0   205304 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/base_client.py
+-rw-r--r--   0        0        0    19312 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    50199 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1006 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      411 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    34990 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      565 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1002 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0     1398 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/types/datasets_create_response_dataset_parts.py
+-rw-r--r--   0        0        0      959 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1057 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      998 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    31599 2024-04-10 16:01:41.729135 cohere-5.2.5/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      253 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    62127 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      305 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1175 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1083 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1400 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2357 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1171 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1823 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1489 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1532 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1463 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1577 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1390 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1177 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     1948 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    13071 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/py.typed
+-rw-r--r--   0        0        0    10202 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1011 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1434 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0     1177 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/api_meta_tokens.py
+-rw-r--r--   0        0        0      168 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1929 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1127 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1861 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1297 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1644 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      168 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      170 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1708 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1011 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1180 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1247 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1653 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1055 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1417 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1861 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      893 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1714 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1017 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1102 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1068 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1040 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1004 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      971 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1137 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2560 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      971 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3383 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1660 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1725 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      960 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1195 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1047 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2209 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1648 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      471 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1068 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1416 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2271 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1364 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1864 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1057 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1735 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1197 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1101 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1311 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      897 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1312 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1456 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1254 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      957 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     1975 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1256 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1095 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      993 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1187 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1024 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     2774 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1080 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      974 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1001 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1200 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1342 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1056 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1818 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1819 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1248 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      952 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     3157 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1201 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1127 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1928 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1221 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1331 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      960 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10025 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-04-10 16:01:41.733135 cohere-5.2.5/src/cohere/version.py
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 cohere-5.2.5/PKG-INFO
```

### Comparing `cohere-5.2.4/LICENSE` & `cohere-5.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/README.md` & `cohere-5.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/pyproject.toml` & `cohere-5.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "5.2.4"
+version = "5.2.5"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "cohere", from = "src"}
 ]
```

### Comparing `cohere-5.2.4/src/cohere/__init__.py` & `cohere-5.2.5/src/cohere/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     ApiMeta,
     ApiMetaApiVersion,
     ApiMetaBilledUnits,
+    ApiMetaTokens,
     AuthTokenType,
     ChatCitation,
     ChatCitationGenerationEvent,
     ChatConnector,
     ChatDataMetrics,
     ChatDocument,
     ChatMessage,
@@ -124,23 +125,30 @@
     NotFoundError,
     ServiceUnavailableError,
     TooManyRequestsError,
     UnauthorizedError,
 )
 from . import connectors, datasets, embed_jobs, finetuning, models
 from .client import AsyncClient, Client
-from .datasets import DatasetsCreateResponse, DatasetsGetResponse, DatasetsGetUsageResponse, DatasetsListResponse
+from .datasets import (
+    DatasetsCreateResponse,
+    DatasetsCreateResponseDatasetParts,
+    DatasetsGetResponse,
+    DatasetsGetUsageResponse,
+    DatasetsListResponse,
+)
 from .embed_jobs import CreateEmbedJobRequestTruncate
 from .environment import ClientEnvironment
 from .version import __version__
 
 __all__ = [
     "ApiMeta",
     "ApiMetaApiVersion",
     "ApiMetaBilledUnits",
+    "ApiMetaTokens",
     "AsyncClient",
     "AuthTokenType",
     "BadRequestError",
     "ChatCitation",
     "ChatCitationGenerationEvent",
     "ChatConnector",
     "ChatDataMetrics",
@@ -185,14 +193,15 @@
     "CreateEmbedJobRequestTruncate",
     "CreateEmbedJobResponse",
     "Dataset",
     "DatasetPart",
     "DatasetType",
     "DatasetValidationStatus",
     "DatasetsCreateResponse",
+    "DatasetsCreateResponseDatasetParts",
     "DatasetsGetResponse",
     "DatasetsGetUsageResponse",
     "DatasetsListResponse",
     "DeleteConnectorResponse",
     "DetokenizeResponse",
     "EmbedByTypeResponse",
     "EmbedByTypeResponseEmbeddings",
```

### Comparing `cohere-5.2.4/src/cohere/base_client.py` & `cohere-5.2.5/src/cohere/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1160,14 +1160,15 @@
     def rerank(
         self,
         *,
         model: typing.Optional[str] = OMIT,
         query: str,
         documents: typing.Sequence[RerankRequestDocumentsItem],
         top_n: typing.Optional[int] = OMIT,
+        rank_fields: typing.Optional[typing.Sequence[str]] = OMIT,
         return_documents: typing.Optional[bool] = OMIT,
         max_chunks_per_doc: typing.Optional[int] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankResponse:
         """
         This endpoint takes in a query and a list of texts and produces an ordered array with each text assigned a relevance score.
 
@@ -1180,14 +1181,16 @@
                                                                       If a document is provided the text fields is required and all other fields will be preserved in the response.
 
                                                                       The total max chunks (length of documents * max_chunks_per_doc) must be less than 10000.
 
                                                                       We recommend a maximum of 1,000 documents for optimal endpoint performance.
             - top_n: typing.Optional[int]. The number of most relevant documents or indices to return, defaults to the length of the documents
 
+            - rank_fields: typing.Optional[typing.Sequence[str]]. If a JSON object is provided, you can specify which keys you would like to have considered for reranking. The model will rerank based on order of the fields passed in (i.e. rank_fields=['title','author','text'] will rerank using the values in title, author, text  sequentially. If the length of title, author, and text exceeds the context length of the model, the chunking will not re-consider earlier fields). If not provided, the model will use the default text field for ranking.
+
             - return_documents: typing.Optional[bool]. - If false, returns results without the doc text - the api will return a list of {index, relevance score} where index is inferred from the list passed into the request.
                                                        - If true, returns results with the doc text passed in - the api will return an ordered list of {index, text, relevance score} where index + text refers to the list passed into the request.
             - max_chunks_per_doc: typing.Optional[int]. The maximum number of chunks to produce internally from a document
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
@@ -1208,14 +1211,16 @@
         )
         """
         _request: typing.Dict[str, typing.Any] = {"query": query, "documents": documents}
         if model is not OMIT:
             _request["model"] = model
         if top_n is not OMIT:
             _request["top_n"] = top_n
+        if rank_fields is not OMIT:
+            _request["rank_fields"] = rank_fields
         if return_documents is not OMIT:
             _request["return_documents"] = return_documents
         if max_chunks_per_doc is not OMIT:
             _request["max_chunks_per_doc"] = max_chunks_per_doc
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "rerank"),
@@ -2721,14 +2726,15 @@
     async def rerank(
         self,
         *,
         model: typing.Optional[str] = OMIT,
         query: str,
         documents: typing.Sequence[RerankRequestDocumentsItem],
         top_n: typing.Optional[int] = OMIT,
+        rank_fields: typing.Optional[typing.Sequence[str]] = OMIT,
         return_documents: typing.Optional[bool] = OMIT,
         max_chunks_per_doc: typing.Optional[int] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankResponse:
         """
         This endpoint takes in a query and a list of texts and produces an ordered array with each text assigned a relevance score.
 
@@ -2741,14 +2747,16 @@
                                                                       If a document is provided the text fields is required and all other fields will be preserved in the response.
 
                                                                       The total max chunks (length of documents * max_chunks_per_doc) must be less than 10000.
 
                                                                       We recommend a maximum of 1,000 documents for optimal endpoint performance.
             - top_n: typing.Optional[int]. The number of most relevant documents or indices to return, defaults to the length of the documents
 
+            - rank_fields: typing.Optional[typing.Sequence[str]]. If a JSON object is provided, you can specify which keys you would like to have considered for reranking. The model will rerank based on order of the fields passed in (i.e. rank_fields=['title','author','text'] will rerank using the values in title, author, text  sequentially. If the length of title, author, and text exceeds the context length of the model, the chunking will not re-consider earlier fields). If not provided, the model will use the default text field for ranking.
+
             - return_documents: typing.Optional[bool]. - If false, returns results without the doc text - the api will return a list of {index, relevance score} where index is inferred from the list passed into the request.
                                                        - If true, returns results with the doc text passed in - the api will return an ordered list of {index, text, relevance score} where index + text refers to the list passed into the request.
             - max_chunks_per_doc: typing.Optional[int]. The maximum number of chunks to produce internally from a document
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
@@ -2769,14 +2777,16 @@
         )
         """
         _request: typing.Dict[str, typing.Any] = {"query": query, "documents": documents}
         if model is not OMIT:
             _request["model"] = model
         if top_n is not OMIT:
             _request["top_n"] = top_n
+        if rank_fields is not OMIT:
+            _request["rank_fields"] = rank_fields
         if return_documents is not OMIT:
             _request["return_documents"] = return_documents
         if max_chunks_per_doc is not OMIT:
             _request["max_chunks_per_doc"] = max_chunks_per_doc
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "rerank"),
```

### Comparing `cohere-5.2.4/src/cohere/client.py` & `cohere-5.2.5/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/connectors/client.py` & `cohere-5.2.5/src/cohere/connectors/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/__init__.py` & `cohere-5.2.5/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/client_wrapper.py` & `cohere-5.2.5/src/cohere/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.2.4",
+            "X-Fern-SDK-Version": "5.2.5",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.2.4/src/cohere/core/datetime_utils.py` & `cohere-5.2.5/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/file.py` & `cohere-5.2.5/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/http_client.py` & `cohere-5.2.5/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/jsonable_encoder.py` & `cohere-5.2.5/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/request_options.py` & `cohere-5.2.5/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/core/unchecked_base_model.py` & `cohere-5.2.5/src/cohere/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/datasets/client.py` & `cohere-5.2.5/src/cohere/datasets/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 
             - optional_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, Datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `optional_fields` are missing from the uploaded file, Dataset validation will pass.
 
             - text_separator: typing.Optional[str]. Raw .txt uploads will be split into entries using the text_separator value.
 
             - csv_delimiter: typing.Optional[str]. The delimiter used for .csv uploads.
 
+
             - data: core.File. See core.File for more documentation
 
             - eval_data: typing.Optional[core.File]. See core.File for more documentation
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
@@ -486,14 +487,15 @@
 
             - optional_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, Datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `optional_fields` are missing from the uploaded file, Dataset validation will pass.
 
             - text_separator: typing.Optional[str]. Raw .txt uploads will be split into entries using the text_separator value.
 
             - csv_delimiter: typing.Optional[str]. The delimiter used for .csv uploads.
 
+
             - data: core.File. See core.File for more documentation
 
             - eval_data: typing.Optional[core.File]. See core.File for more documentation
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
```

### Comparing `cohere-5.2.4/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.2.5/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.2.5/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.2.5/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.2.5/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/embed_jobs/client.py` & `cohere-5.2.5/src/cohere/embed_jobs/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/errors/__init__.py` & `cohere-5.2.5/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/__init__.py` & `cohere-5.2.5/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/client.py` & `cohere-5.2.5/src/cohere/finetuning/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.2.5/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/manually_maintained/cache.py` & `cohere-5.2.5/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.2.5/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/models/client.py` & `cohere-5.2.5/src/cohere/models/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/overrides.py` & `cohere-5.2.5/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/__init__.py` & `cohere-5.2.5/src/cohere/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .api_meta import ApiMeta
 from .api_meta_api_version import ApiMetaApiVersion
 from .api_meta_billed_units import ApiMetaBilledUnits
+from .api_meta_tokens import ApiMetaTokens
 from .auth_token_type import AuthTokenType
 from .chat_citation import ChatCitation
 from .chat_citation_generation_event import ChatCitationGenerationEvent
 from .chat_connector import ChatConnector
 from .chat_data_metrics import ChatDataMetrics
 from .chat_document import ChatDocument
 from .chat_message import ChatMessage
@@ -120,14 +121,15 @@
 from .tool_parameter_definitions_value import ToolParameterDefinitionsValue
 from .update_connector_response import UpdateConnectorResponse
 
 __all__ = [
     "ApiMeta",
     "ApiMetaApiVersion",
     "ApiMetaBilledUnits",
+    "ApiMetaTokens",
     "AuthTokenType",
     "ChatCitation",
     "ChatCitationGenerationEvent",
     "ChatConnector",
     "ChatDataMetrics",
     "ChatDocument",
     "ChatMessage",
```

### Comparing `cohere-5.2.4/src/cohere/types/api_meta.py` & `cohere-5.2.5/src/cohere/types/api_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta_api_version import ApiMetaApiVersion
 from .api_meta_billed_units import ApiMetaBilledUnits
+from .api_meta_tokens import ApiMetaTokens
 
 
 class ApiMeta(UncheckedBaseModel):
     api_version: typing.Optional[ApiMetaApiVersion] = None
     billed_units: typing.Optional[ApiMetaBilledUnits] = None
+    tokens: typing.Optional[ApiMetaTokens] = None
     warnings: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.2.4/src/cohere/types/api_meta_api_version.py` & `cohere-5.2.5/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/api_meta_billed_units.py` & `cohere-5.2.5/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_citation.py` & `cohere-5.2.5/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.2.5/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_connector.py` & `cohere-5.2.5/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_data_metrics.py` & `cohere-5.2.5/src/cohere/types/chat_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_message.py` & `cohere-5.2.5/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.2.5/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.2.5/src/cohere/types/chat_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.2.5/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_search_query.py` & `cohere-5.2.5/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_search_result.py` & `cohere-5.2.5/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_search_result_connector.py` & `cohere-5.2.5/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_search_results_event.py` & `cohere-5.2.5/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_stream_end_event.py` & `cohere-5.2.5/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_stream_event.py` & `cohere-5.2.5/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.2.5/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.2.5/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_stream_start_event.py` & `cohere-5.2.5/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_text_generation_event.py` & `cohere-5.2.5/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.2.5/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/classify_data_metrics.py` & `cohere-5.2.5/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/classify_example.py` & `cohere-5.2.5/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/classify_response.py` & `cohere-5.2.5/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.2.5/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.2.5/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/connector.py` & `cohere-5.2.5/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/connector_o_auth.py` & `cohere-5.2.5/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/create_connector_o_auth.py` & `cohere-5.2.5/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/create_connector_response.py` & `cohere-5.2.5/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/create_connector_service_auth.py` & `cohere-5.2.5/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/create_embed_job_response.py` & `cohere-5.2.5/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/dataset.py` & `cohere-5.2.5/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/dataset_part.py` & `cohere-5.2.5/src/cohere/types/dataset_part.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/detokenize_response.py` & `cohere-5.2.5/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/embed_by_type_response.py` & `cohere-5.2.5/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.2.5/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/embed_floats_response.py` & `cohere-5.2.5/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/embed_job.py` & `cohere-5.2.5/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/embed_response.py` & `cohere-5.2.5/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.2.5/src/cohere/types/finetune_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generate_stream_end.py` & `cohere-5.2.5/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generate_stream_end_response.py` & `cohere-5.2.5/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generate_stream_error.py` & `cohere-5.2.5/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generate_stream_event.py` & `cohere-5.2.5/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generate_stream_text.py` & `cohere-5.2.5/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generate_streamed_response.py` & `cohere-5.2.5/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/generation.py` & `cohere-5.2.5/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/get_connector_response.py` & `cohere-5.2.5/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/get_model_response.py` & `cohere-5.2.5/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/label_metric.py` & `cohere-5.2.5/src/cohere/types/label_metric.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/list_connectors_response.py` & `cohere-5.2.5/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/list_embed_job_response.py` & `cohere-5.2.5/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/list_models_response.py` & `cohere-5.2.5/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/metrics.py` & `cohere-5.2.5/src/cohere/types/metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.2.5/src/cohere/types/non_streamed_chat_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
 from .chat_citation import ChatCitation
 from .chat_document import ChatDocument
 from .chat_message import ChatMessage
 from .chat_search_query import ChatSearchQuery
 from .chat_search_result import ChatSearchResult
 from .finish_reason import FinishReason
 from .tool_call import ToolCall
@@ -54,14 +55,16 @@
     finish_reason: typing.Optional[FinishReason] = None
     tool_calls: typing.Optional[typing.List[ToolCall]] = None
     chat_history: typing.Optional[typing.List[ChatMessage]] = pydantic_v1.Field(default=None)
     """
     A list of previous messages between the user and the model, meant to give the model conversational context for responding to the user's `message`.
     """
 
+    meta: typing.Optional[ApiMeta] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `cohere-5.2.4/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.2.5/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/parse_info.py` & `cohere-5.2.5/src/cohere/types/parse_info.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.2.5/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/rerank_response.py` & `cohere-5.2.5/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/rerank_response_results_item.py` & `cohere-5.2.5/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.2.5/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/reranker_data_metrics.py` & `cohere-5.2.5/src/cohere/types/reranker_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/single_generation.py` & `cohere-5.2.5/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/single_generation_in_stream.py` & `cohere-5.2.5/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.2.5/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/streamed_chat_response.py` & `cohere-5.2.5/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/summarize_response.py` & `cohere-5.2.5/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/tokenize_response.py` & `cohere-5.2.5/src/cohere/types/tokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/tool.py` & `cohere-5.2.5/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/tool_call.py` & `cohere-5.2.5/src/cohere/types/tool_call.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/tool_parameter_definitions_value.py` & `cohere-5.2.5/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/types/update_connector_response.py` & `cohere-5.2.5/src/cohere/types/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/src/cohere/utils.py` & `cohere-5.2.5/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.2.4/PKG-INFO` & `cohere-5.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.2.4
+Version: 5.2.5
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

