# Comparing `tmp/trieve_py_client-0.5.7-py3-none-any.whl.zip` & `tmp/trieve_py_client-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,225 +1,116 @@
-Zip file size: 406287 bytes, number of entries: 223
--rw-rw-r--  2.0 unx     8246 b- defN 24-Apr-03 03:54 trieve_py_client/__init__.py
--rw-rw-r--  2.0 unx    25843 b- defN 24-Apr-03 03:54 trieve_py_client/api_client.py
--rw-rw-r--  2.0 unx      652 b- defN 24-Apr-03 03:54 trieve_py_client/api_response.py
--rw-rw-r--  2.0 unx    15539 b- defN 24-Apr-03 03:54 trieve_py_client/configuration.py
--rw-rw-r--  2.0 unx     6012 b- defN 24-Apr-03 03:54 trieve_py_client/exceptions.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-03 03:54 trieve_py_client/py.typed
--rw-rw-r--  2.0 unx     9274 b- defN 24-Apr-03 03:54 trieve_py_client/rest.py
--rw-rw-r--  2.0 unx      767 b- defN 24-Apr-03 03:54 trieve_py_client/api/__init__.py
--rw-rw-r--  2.0 unx    39416 b- defN 24-Apr-03 03:54 trieve_py_client/api/auth_api.py
--rw-rw-r--  2.0 unx   134746 b- defN 24-Apr-03 03:54 trieve_py_client/api/chunk_api.py
--rw-rw-r--  2.0 unx   211320 b- defN 24-Apr-03 03:54 trieve_py_client/api/chunk_group_api.py
--rw-rw-r--  2.0 unx    71099 b- defN 24-Apr-03 03:54 trieve_py_client/api/dataset_api.py
--rw-rw-r--  2.0 unx    13295 b- defN 24-Apr-03 03:54 trieve_py_client/api/events_api.py
--rw-rw-r--  2.0 unx    50431 b- defN 24-Apr-03 03:54 trieve_py_client/api/file_api.py
--rw-rw-r--  2.0 unx    10344 b- defN 24-Apr-03 03:54 trieve_py_client/api/health_api.py
--rw-rw-r--  2.0 unx    13398 b- defN 24-Apr-03 03:54 trieve_py_client/api/invitation_api.py
--rw-rw-r--  2.0 unx    51855 b- defN 24-Apr-03 03:54 trieve_py_client/api/message_api.py
--rw-rw-r--  2.0 unx    71526 b- defN 24-Apr-03 03:54 trieve_py_client/api/organization_api.py
--rw-rw-r--  2.0 unx    44982 b- defN 24-Apr-03 03:54 trieve_py_client/api/stripe_api.py
--rw-rw-r--  2.0 unx    47374 b- defN 24-Apr-03 03:54 trieve_py_client/api/topic_api.py
--rw-rw-r--  2.0 unx    34606 b- defN 24-Apr-03 03:54 trieve_py_client/api/user_api.py
--rw-rw-r--  2.0 unx     6965 b- defN 24-Apr-03 03:54 trieve_py_client/models/__init__.py
--rw-rw-r--  2.0 unx     2625 b- defN 24-Apr-03 03:54 trieve_py_client/models/add_chunk_to_group_data.py
--rw-rw-r--  2.0 unx     2908 b- defN 24-Apr-03 03:54 trieve_py_client/models/api_key_dto.py
--rw-rw-r--  2.0 unx     3713 b- defN 24-Apr-03 03:54 trieve_py_client/models/auth_query.py
--rw-rw-r--  2.0 unx     3278 b- defN 24-Apr-03 03:54 trieve_py_client/models/batch_queued_chunk_response.py
--rw-rw-r--  2.0 unx     3463 b- defN 24-Apr-03 03:54 trieve_py_client/models/bookmark_data.py
--rw-rw-r--  2.0 unx     3119 b- defN 24-Apr-03 03:54 trieve_py_client/models/bookmark_group_result.py
--rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-03 03:54 trieve_py_client/models/chat_message_proxy.py
--rw-rw-r--  2.0 unx    10290 b- defN 24-Apr-03 03:54 trieve_py_client/models/chunk_data.py
--rw-rw-r--  2.0 unx     4960 b- defN 24-Apr-03 03:54 trieve_py_client/models/chunk_filter.py
--rw-rw-r--  2.0 unx     3288 b- defN 24-Apr-03 03:54 trieve_py_client/models/chunk_group.py
--rw-rw-r--  2.0 unx     3621 b- defN 24-Apr-03 03:54 trieve_py_client/models/chunk_group_and_file.py
--rw-rw-r--  2.0 unx     5262 b- defN 24-Apr-03 03:54 trieve_py_client/models/chunk_metadata.py
--rw-rw-r--  2.0 unx     5587 b- defN 24-Apr-03 03:54 trieve_py_client/models/chunk_metadata_with_file_data.py
--rw-rw-r--  2.0 unx     7083 b- defN 24-Apr-03 03:54 trieve_py_client/models/client_dataset_configuration.py
--rw-rw-r--  2.0 unx     5386 b- defN 24-Apr-03 03:54 trieve_py_client/models/create_chunk_data.py
--rw-rw-r--  2.0 unx     3341 b- defN 24-Apr-03 03:54 trieve_py_client/models/create_chunk_group_data.py
--rw-rw-r--  2.0 unx     4040 b- defN 24-Apr-03 03:54 trieve_py_client/models/create_dataset_request.py
--rw-rw-r--  2.0 unx     5235 b- defN 24-Apr-03 03:54 trieve_py_client/models/create_message_data.py
--rw-rw-r--  2.0 unx     2668 b- defN 24-Apr-03 03:54 trieve_py_client/models/create_organization_data.py
--rw-rw-r--  2.0 unx     3997 b- defN 24-Apr-03 03:54 trieve_py_client/models/create_topic_data.py
--rw-rw-r--  2.0 unx     3658 b- defN 24-Apr-03 03:54 trieve_py_client/models/dataset.py
--rw-rw-r--  2.0 unx     3251 b- defN 24-Apr-03 03:54 trieve_py_client/models/dataset_and_usage.py
--rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-03 03:54 trieve_py_client/models/dataset_dto.py
--rw-rw-r--  2.0 unx     2709 b- defN 24-Apr-03 03:54 trieve_py_client/models/dataset_usage_count.py
--rw-rw-r--  2.0 unx     2593 b- defN 24-Apr-03 03:54 trieve_py_client/models/delete_topic_data.py
--rw-rw-r--  2.0 unx     2635 b- defN 24-Apr-03 03:54 trieve_py_client/models/delete_user_api_key_request.py
--rw-rw-r--  2.0 unx     5414 b- defN 24-Apr-03 03:54 trieve_py_client/models/edit_message_data.py
--rw-rw-r--  2.0 unx     2536 b- defN 24-Apr-03 03:54 trieve_py_client/models/error_response_body.py
--rw-rw-r--  2.0 unx     3178 b- defN 24-Apr-03 03:54 trieve_py_client/models/event.py
--rw-rw-r--  2.0 unx     3025 b- defN 24-Apr-03 03:54 trieve_py_client/models/event_return.py
--rw-rw-r--  2.0 unx     4455 b- defN 24-Apr-03 03:54 trieve_py_client/models/field_condition.py
--rw-rw-r--  2.0 unx     4151 b- defN 24-Apr-03 03:54 trieve_py_client/models/file.py
--rw-rw-r--  2.0 unx     3514 b- defN 24-Apr-03 03:54 trieve_py_client/models/file_dto.py
--rw-rw-r--  2.0 unx     5366 b- defN 24-Apr-03 03:54 trieve_py_client/models/generate_chunks_request.py
--rw-rw-r--  2.0 unx     3738 b- defN 24-Apr-03 03:54 trieve_py_client/models/get_events_data.py
--rw-rw-r--  2.0 unx     2570 b- defN 24-Apr-03 03:54 trieve_py_client/models/get_groups_for_chunks_data.py
--rw-rw-r--  2.0 unx     3072 b- defN 24-Apr-03 03:54 trieve_py_client/models/group_data.py
--rw-rw-r--  2.0 unx     3492 b- defN 24-Apr-03 03:54 trieve_py_client/models/group_score_chunk_dto.py
--rw-rw-r--  2.0 unx     3105 b- defN 24-Apr-03 03:54 trieve_py_client/models/group_slim_chunks_dto.py
--rw-rw-r--  2.0 unx     3482 b- defN 24-Apr-03 03:54 trieve_py_client/models/invitation_data.py
--rw-rw-r--  2.0 unx     5286 b- defN 24-Apr-03 03:54 trieve_py_client/models/match_condition.py
--rw-rw-r--  2.0 unx     3932 b- defN 24-Apr-03 03:54 trieve_py_client/models/message.py
--rw-rw-r--  2.0 unx     3135 b- defN 24-Apr-03 03:54 trieve_py_client/models/organization.py
--rw-rw-r--  2.0 unx     3008 b- defN 24-Apr-03 03:54 trieve_py_client/models/organization_usage_count.py
--rw-rw-r--  2.0 unx     4407 b- defN 24-Apr-03 03:54 trieve_py_client/models/range.py
--rw-rw-r--  2.0 unx     5348 b- defN 24-Apr-03 03:54 trieve_py_client/models/range_condition.py
--rw-rw-r--  2.0 unx     7177 b- defN 24-Apr-03 03:54 trieve_py_client/models/reccomend_group_chunks_request.py
--rw-rw-r--  2.0 unx     6536 b- defN 24-Apr-03 03:54 trieve_py_client/models/recommend_chunks_request.py
--rw-rw-r--  2.0 unx     5946 b- defN 24-Apr-03 03:54 trieve_py_client/models/recommend_chunks_response_types.py
--rw-rw-r--  2.0 unx     6065 b- defN 24-Apr-03 03:54 trieve_py_client/models/recommend_group_chunk_response_types.py
--rw-rw-r--  2.0 unx     5019 b- defN 24-Apr-03 03:54 trieve_py_client/models/regenerate_message_data.py
--rw-rw-r--  2.0 unx     5760 b- defN 24-Apr-03 03:54 trieve_py_client/models/return_queued_chunk.py
--rw-rw-r--  2.0 unx     3155 b- defN 24-Apr-03 03:54 trieve_py_client/models/score_chunk_dto.py
--rw-rw-r--  2.0 unx     3129 b- defN 24-Apr-03 03:54 trieve_py_client/models/score_slim_chunks.py
--rw-rw-r--  2.0 unx     9055 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_chunk_data.py
--rw-rw-r--  2.0 unx     3209 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_chunk_query_response_body.py
--rw-rw-r--  2.0 unx     6006 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_chunk_response_types.py
--rw-rw-r--  2.0 unx     3508 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_group_slim_chunks_result.py
--rw-rw-r--  2.0 unx     3464 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_groups_result.py
--rw-rw-r--  2.0 unx     8460 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_over_groups_data.py
--rw-rw-r--  2.0 unx     3230 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_over_groups_response_body.py
--rw-rw-r--  2.0 unx     6149 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_over_groups_response_types.py
--rw-rw-r--  2.0 unx     3270 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_over_groups_slim_chunks_response_body.py
--rw-rw-r--  2.0 unx     3233 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_slim_chunk_query_response_body.py
--rw-rw-r--  2.0 unx     9683 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_within_group_data.py
--rw-rw-r--  2.0 unx     5796 b- defN 24-Apr-03 03:54 trieve_py_client/models/search_within_group_response_types.py
--rw-rw-r--  2.0 unx     3049 b- defN 24-Apr-03 03:54 trieve_py_client/models/set_user_api_key_request.py
--rw-rw-r--  2.0 unx     2681 b- defN 24-Apr-03 03:54 trieve_py_client/models/set_user_api_key_response.py
--rw-rw-r--  2.0 unx     3115 b- defN 24-Apr-03 03:54 trieve_py_client/models/single_queued_chunk_response.py
--rw-rw-r--  2.0 unx     4783 b- defN 24-Apr-03 03:54 trieve_py_client/models/slim_chunk_metadata.py
--rw-rw-r--  2.0 unx     2772 b- defN 24-Apr-03 03:54 trieve_py_client/models/slim_group.py
--rw-rw-r--  2.0 unx     3924 b- defN 24-Apr-03 03:54 trieve_py_client/models/slim_user.py
--rw-rw-r--  2.0 unx     3409 b- defN 24-Apr-03 03:54 trieve_py_client/models/stripe_plan.py
--rw-rw-r--  2.0 unx     2640 b- defN 24-Apr-03 03:54 trieve_py_client/models/suggested_queries_request.py
--rw-rw-r--  2.0 unx     2570 b- defN 24-Apr-03 03:54 trieve_py_client/models/suggested_queries_response.py
--rw-rw-r--  2.0 unx     2995 b- defN 24-Apr-03 03:54 trieve_py_client/models/topic.py
--rw-rw-r--  2.0 unx     6962 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_chunk_by_tracking_id_data.py
--rw-rw-r--  2.0 unx     8254 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_chunk_data.py
--rw-rw-r--  2.0 unx     4234 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_chunk_group_data.py
--rw-rw-r--  2.0 unx     4343 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_dataset_request.py
--rw-rw-r--  2.0 unx     3635 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_group_by_tracking_id_data.py
--rw-rw-r--  2.0 unx     3058 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_organization_data.py
--rw-rw-r--  2.0 unx     2767 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_topic_data.py
--rw-rw-r--  2.0 unx     4085 b- defN 24-Apr-03 03:54 trieve_py_client/models/update_user_data.py
--rw-rw-r--  2.0 unx     6484 b- defN 24-Apr-03 03:54 trieve_py_client/models/upload_file_data.py
--rw-rw-r--  2.0 unx     2837 b- defN 24-Apr-03 03:54 trieve_py_client/models/upload_file_result.py
--rw-rw-r--  2.0 unx     2980 b- defN 24-Apr-03 03:54 trieve_py_client/models/user_organization.py
--rw-rw-r--  2.0 unx     8682 b- defN 24-Apr-03 03:44 trieve_python_client/__init__.py
--rw-rw-r--  2.0 unx    25867 b- defN 24-Apr-03 03:44 trieve_python_client/api_client.py
--rw-rw-r--  2.0 unx      652 b- defN 24-Apr-03 03:44 trieve_python_client/api_response.py
--rw-rw-r--  2.0 unx    15547 b- defN 24-Apr-03 03:44 trieve_python_client/configuration.py
--rw-rw-r--  2.0 unx     6012 b- defN 24-Apr-03 03:44 trieve_python_client/exceptions.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-03 03:44 trieve_python_client/py.typed
--rw-rw-r--  2.0 unx     9278 b- defN 24-Apr-03 03:44 trieve_python_client/rest.py
--rw-rw-r--  2.0 unx      819 b- defN 24-Apr-03 03:44 trieve_python_client/api/__init__.py
--rw-rw-r--  2.0 unx    39436 b- defN 24-Apr-03 03:44 trieve_python_client/api/auth_api.py
--rw-rw-r--  2.0 unx   134806 b- defN 24-Apr-03 03:44 trieve_python_client/api/chunk_api.py
--rw-rw-r--  2.0 unx   211392 b- defN 24-Apr-03 03:44 trieve_python_client/api/chunk_group_api.py
--rw-rw-r--  2.0 unx    71131 b- defN 24-Apr-03 03:44 trieve_python_client/api/dataset_api.py
--rw-rw-r--  2.0 unx    13315 b- defN 24-Apr-03 03:44 trieve_python_client/api/events_api.py
--rw-rw-r--  2.0 unx    50459 b- defN 24-Apr-03 03:44 trieve_python_client/api/file_api.py
--rw-rw-r--  2.0 unx    10356 b- defN 24-Apr-03 03:44 trieve_python_client/api/health_api.py
--rw-rw-r--  2.0 unx    13414 b- defN 24-Apr-03 03:44 trieve_python_client/api/invitation_api.py
--rw-rw-r--  2.0 unx    51883 b- defN 24-Apr-03 03:44 trieve_python_client/api/message_api.py
--rw-rw-r--  2.0 unx    71558 b- defN 24-Apr-03 03:44 trieve_python_client/api/organization_api.py
--rw-rw-r--  2.0 unx    44998 b- defN 24-Apr-03 03:44 trieve_python_client/api/stripe_api.py
--rw-rw-r--  2.0 unx    47398 b- defN 24-Apr-03 03:44 trieve_python_client/api/topic_api.py
--rw-rw-r--  2.0 unx    34638 b- defN 24-Apr-03 03:44 trieve_python_client/api/user_api.py
--rw-rw-r--  2.0 unx     7313 b- defN 24-Apr-03 03:44 trieve_python_client/models/__init__.py
--rw-rw-r--  2.0 unx     2625 b- defN 24-Apr-03 03:44 trieve_python_client/models/add_chunk_to_group_data.py
--rw-rw-r--  2.0 unx     2908 b- defN 24-Apr-03 03:44 trieve_python_client/models/api_key_dto.py
--rw-rw-r--  2.0 unx     3713 b- defN 24-Apr-03 03:44 trieve_python_client/models/auth_query.py
--rw-rw-r--  2.0 unx     3282 b- defN 24-Apr-03 03:44 trieve_python_client/models/batch_queued_chunk_response.py
--rw-rw-r--  2.0 unx     3471 b- defN 24-Apr-03 03:44 trieve_python_client/models/bookmark_data.py
--rw-rw-r--  2.0 unx     3123 b- defN 24-Apr-03 03:44 trieve_python_client/models/bookmark_group_result.py
--rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-03 03:44 trieve_python_client/models/chat_message_proxy.py
--rw-rw-r--  2.0 unx    10290 b- defN 24-Apr-03 03:44 trieve_python_client/models/chunk_data.py
--rw-rw-r--  2.0 unx     4964 b- defN 24-Apr-03 03:44 trieve_python_client/models/chunk_filter.py
--rw-rw-r--  2.0 unx     3288 b- defN 24-Apr-03 03:44 trieve_python_client/models/chunk_group.py
--rw-rw-r--  2.0 unx     3621 b- defN 24-Apr-03 03:44 trieve_python_client/models/chunk_group_and_file.py
--rw-rw-r--  2.0 unx     5262 b- defN 24-Apr-03 03:44 trieve_python_client/models/chunk_metadata.py
--rw-rw-r--  2.0 unx     5587 b- defN 24-Apr-03 03:44 trieve_python_client/models/chunk_metadata_with_file_data.py
--rw-rw-r--  2.0 unx     7083 b- defN 24-Apr-03 03:44 trieve_python_client/models/client_dataset_configuration.py
--rw-rw-r--  2.0 unx     5390 b- defN 24-Apr-03 03:44 trieve_python_client/models/create_chunk_data.py
--rw-rw-r--  2.0 unx     3341 b- defN 24-Apr-03 03:44 trieve_python_client/models/create_chunk_group_data.py
--rw-rw-r--  2.0 unx     4040 b- defN 24-Apr-03 03:44 trieve_python_client/models/create_dataset_request.py
--rw-rw-r--  2.0 unx     5235 b- defN 24-Apr-03 03:44 trieve_python_client/models/create_message_data.py
--rw-rw-r--  2.0 unx     2668 b- defN 24-Apr-03 03:44 trieve_python_client/models/create_organization_data.py
--rw-rw-r--  2.0 unx     3997 b- defN 24-Apr-03 03:44 trieve_python_client/models/create_topic_data.py
--rw-rw-r--  2.0 unx     3658 b- defN 24-Apr-03 03:44 trieve_python_client/models/dataset.py
--rw-rw-r--  2.0 unx     3259 b- defN 24-Apr-03 03:44 trieve_python_client/models/dataset_and_usage.py
--rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-03 03:44 trieve_python_client/models/dataset_dto.py
--rw-rw-r--  2.0 unx     2709 b- defN 24-Apr-03 03:44 trieve_python_client/models/dataset_usage_count.py
--rw-rw-r--  2.0 unx     2632 b- defN 24-Apr-02 18:29 trieve_python_client/models/delete_dataset_request.py
--rw-rw-r--  2.0 unx     2593 b- defN 24-Apr-03 03:44 trieve_python_client/models/delete_topic_data.py
--rw-rw-r--  2.0 unx     2635 b- defN 24-Apr-03 03:44 trieve_python_client/models/delete_user_api_key_request.py
--rw-rw-r--  2.0 unx     5414 b- defN 24-Apr-03 03:44 trieve_python_client/models/edit_message_data.py
--rw-rw-r--  2.0 unx     2536 b- defN 24-Apr-03 03:44 trieve_python_client/models/error_response_body.py
--rw-rw-r--  2.0 unx     3178 b- defN 24-Apr-03 03:44 trieve_python_client/models/event.py
--rw-rw-r--  2.0 unx     3029 b- defN 24-Apr-03 03:44 trieve_python_client/models/event_return.py
--rw-rw-r--  2.0 unx     4463 b- defN 24-Apr-03 03:44 trieve_python_client/models/field_condition.py
--rw-rw-r--  2.0 unx     4151 b- defN 24-Apr-03 03:44 trieve_python_client/models/file.py
--rw-rw-r--  2.0 unx     3514 b- defN 24-Apr-03 03:44 trieve_python_client/models/file_dto.py
--rw-rw-r--  2.0 unx     5370 b- defN 24-Apr-03 03:44 trieve_python_client/models/generate_chunks_request.py
--rw-rw-r--  2.0 unx     3738 b- defN 24-Apr-03 03:44 trieve_python_client/models/get_events_data.py
--rw-rw-r--  2.0 unx     2570 b- defN 24-Apr-03 03:44 trieve_python_client/models/get_groups_for_chunks_data.py
--rw-rw-r--  2.0 unx     3076 b- defN 24-Apr-03 03:44 trieve_python_client/models/group_data.py
--rw-rw-r--  2.0 unx     3496 b- defN 24-Apr-03 03:44 trieve_python_client/models/group_score_chunk_dto.py
--rw-rw-r--  2.0 unx     3109 b- defN 24-Apr-03 03:44 trieve_python_client/models/group_slim_chunks_dto.py
--rw-rw-r--  2.0 unx     3482 b- defN 24-Apr-03 03:44 trieve_python_client/models/invitation_data.py
--rw-rw-r--  2.0 unx     5286 b- defN 24-Apr-03 03:44 trieve_python_client/models/match_condition.py
--rw-rw-r--  2.0 unx     3932 b- defN 24-Apr-03 03:44 trieve_python_client/models/message.py
--rw-rw-r--  2.0 unx     3135 b- defN 24-Apr-03 03:44 trieve_python_client/models/organization.py
--rw-rw-r--  2.0 unx     3008 b- defN 24-Apr-03 03:44 trieve_python_client/models/organization_usage_count.py
--rw-rw-r--  2.0 unx     4411 b- defN 24-Apr-03 03:44 trieve_python_client/models/range.py
--rw-rw-r--  2.0 unx     5348 b- defN 24-Apr-03 03:44 trieve_python_client/models/range_condition.py
--rw-rw-r--  2.0 unx     7181 b- defN 24-Apr-03 03:44 trieve_python_client/models/reccomend_group_chunks_request.py
--rw-rw-r--  2.0 unx     6540 b- defN 24-Apr-03 03:44 trieve_python_client/models/recommend_chunks_request.py
--rw-rw-r--  2.0 unx     5954 b- defN 24-Apr-03 03:44 trieve_python_client/models/recommend_chunks_response_types.py
--rw-rw-r--  2.0 unx     6073 b- defN 24-Apr-03 03:44 trieve_python_client/models/recommend_group_chunk_response_types.py
--rw-rw-r--  2.0 unx     5019 b- defN 24-Apr-03 03:44 trieve_python_client/models/regenerate_message_data.py
--rw-rw-r--  2.0 unx     5768 b- defN 24-Apr-03 03:44 trieve_python_client/models/return_queued_chunk.py
--rw-rw-r--  2.0 unx     3159 b- defN 24-Apr-03 03:44 trieve_python_client/models/score_chunk_dto.py
--rw-rw-r--  2.0 unx     3133 b- defN 24-Apr-03 03:44 trieve_python_client/models/score_slim_chunks.py
--rw-rw-r--  2.0 unx     9059 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_chunk_data.py
--rw-rw-r--  2.0 unx     3213 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_chunk_query_response_body.py
--rw-rw-r--  2.0 unx     6014 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_chunk_response_types.py
--rw-rw-r--  2.0 unx     3516 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_group_slim_chunks_result.py
--rw-rw-r--  2.0 unx     3472 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_groups_result.py
--rw-rw-r--  2.0 unx     8464 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_over_groups_data.py
--rw-rw-r--  2.0 unx     3234 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_over_groups_response_body.py
--rw-rw-r--  2.0 unx     6157 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_over_groups_response_types.py
--rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_over_groups_slim_chunks_response_body.py
--rw-rw-r--  2.0 unx     3237 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_slim_chunk_query_response_body.py
--rw-rw-r--  2.0 unx     9687 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_within_group_data.py
--rw-rw-r--  2.0 unx     5804 b- defN 24-Apr-03 03:44 trieve_python_client/models/search_within_group_response_types.py
--rw-rw-r--  2.0 unx     3049 b- defN 24-Apr-03 03:44 trieve_python_client/models/set_user_api_key_request.py
--rw-rw-r--  2.0 unx     2681 b- defN 24-Apr-03 03:44 trieve_python_client/models/set_user_api_key_response.py
--rw-rw-r--  2.0 unx     3119 b- defN 24-Apr-03 03:44 trieve_python_client/models/single_queued_chunk_response.py
--rw-rw-r--  2.0 unx     4783 b- defN 24-Apr-03 03:44 trieve_python_client/models/slim_chunk_metadata.py
--rw-rw-r--  2.0 unx     2772 b- defN 24-Apr-03 03:44 trieve_python_client/models/slim_group.py
--rw-rw-r--  2.0 unx     3932 b- defN 24-Apr-03 03:44 trieve_python_client/models/slim_user.py
--rw-rw-r--  2.0 unx     3409 b- defN 24-Apr-03 03:44 trieve_python_client/models/stripe_plan.py
--rw-rw-r--  2.0 unx     2640 b- defN 24-Apr-03 03:44 trieve_python_client/models/suggested_queries_request.py
--rw-rw-r--  2.0 unx     2570 b- defN 24-Apr-03 03:44 trieve_python_client/models/suggested_queries_response.py
--rw-rw-r--  2.0 unx     2995 b- defN 24-Apr-03 03:44 trieve_python_client/models/topic.py
--rw-rw-r--  2.0 unx     6962 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_chunk_by_tracking_id_data.py
--rw-rw-r--  2.0 unx     8254 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_chunk_data.py
--rw-rw-r--  2.0 unx     4234 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_chunk_group_data.py
--rw-rw-r--  2.0 unx     4343 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_dataset_request.py
--rw-rw-r--  2.0 unx     3635 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_group_by_tracking_id_data.py
--rw-rw-r--  2.0 unx     3058 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_organization_data.py
--rw-rw-r--  2.0 unx     2767 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_topic_data.py
--rw-rw-r--  2.0 unx     4085 b- defN 24-Apr-03 03:44 trieve_python_client/models/update_user_data.py
--rw-rw-r--  2.0 unx     6484 b- defN 24-Apr-03 03:44 trieve_python_client/models/upload_file_data.py
--rw-rw-r--  2.0 unx     2841 b- defN 24-Apr-03 03:44 trieve_python_client/models/upload_file_result.py
--rw-rw-r--  2.0 unx     2980 b- defN 24-Apr-03 03:44 trieve_python_client/models/user_organization.py
--rw-rw-r--  2.0 unx      523 b- defN 24-Apr-03 03:54 trieve_py_client-0.5.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-03 03:54 trieve_py_client-0.5.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 24-Apr-03 03:54 trieve_py_client-0.5.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    22911 b- defN 24-Apr-03 03:54 trieve_py_client-0.5.7.dist-info/RECORD
-223 files, 2503451 bytes uncompressed, 368851 bytes compressed:  85.3%
+Zip file size: 207090 bytes, number of entries: 114
+-rw-rw-r--  2.0 unx     8246 b- defN 24-Apr-09 04:57 trieve_py_client/__init__.py
+-rw-rw-r--  2.0 unx    25843 b- defN 24-Apr-09 04:57 trieve_py_client/api_client.py
+-rw-rw-r--  2.0 unx      652 b- defN 24-Apr-09 04:57 trieve_py_client/api_response.py
+-rw-rw-r--  2.0 unx    15539 b- defN 24-Apr-09 04:57 trieve_py_client/configuration.py
+-rw-rw-r--  2.0 unx     6012 b- defN 24-Apr-09 04:57 trieve_py_client/exceptions.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-09 04:57 trieve_py_client/py.typed
+-rw-rw-r--  2.0 unx     9274 b- defN 24-Apr-09 04:57 trieve_py_client/rest.py
+-rw-rw-r--  2.0 unx      767 b- defN 24-Apr-09 04:57 trieve_py_client/api/__init__.py
+-rw-rw-r--  2.0 unx    41292 b- defN 24-Apr-09 04:57 trieve_py_client/api/auth_api.py
+-rw-rw-r--  2.0 unx   135067 b- defN 24-Apr-09 04:57 trieve_py_client/api/chunk_api.py
+-rw-rw-r--  2.0 unx   211548 b- defN 24-Apr-09 04:57 trieve_py_client/api/chunk_group_api.py
+-rw-rw-r--  2.0 unx    70974 b- defN 24-Apr-09 04:57 trieve_py_client/api/dataset_api.py
+-rw-rw-r--  2.0 unx    12995 b- defN 24-Apr-09 04:57 trieve_py_client/api/events_api.py
+-rw-rw-r--  2.0 unx    49987 b- defN 24-Apr-09 04:57 trieve_py_client/api/file_api.py
+-rw-rw-r--  2.0 unx    10344 b- defN 24-Apr-09 04:57 trieve_py_client/api/health_api.py
+-rw-rw-r--  2.0 unx    13398 b- defN 24-Apr-09 04:57 trieve_py_client/api/invitation_api.py
+-rw-rw-r--  2.0 unx    51855 b- defN 24-Apr-09 04:57 trieve_py_client/api/message_api.py
+-rw-rw-r--  2.0 unx    71526 b- defN 24-Apr-09 04:57 trieve_py_client/api/organization_api.py
+-rw-rw-r--  2.0 unx    44982 b- defN 24-Apr-09 04:57 trieve_py_client/api/stripe_api.py
+-rw-rw-r--  2.0 unx    47374 b- defN 24-Apr-09 04:57 trieve_py_client/api/topic_api.py
+-rw-rw-r--  2.0 unx    34606 b- defN 24-Apr-09 04:57 trieve_py_client/api/user_api.py
+-rw-rw-r--  2.0 unx     6965 b- defN 24-Apr-09 04:57 trieve_py_client/models/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 24-Apr-09 04:57 trieve_py_client/models/add_chunk_to_group_data.py
+-rw-rw-r--  2.0 unx     2908 b- defN 24-Apr-09 04:57 trieve_py_client/models/api_key_dto.py
+-rw-rw-r--  2.0 unx     3713 b- defN 24-Apr-09 04:57 trieve_py_client/models/auth_query.py
+-rw-rw-r--  2.0 unx     3278 b- defN 24-Apr-09 04:57 trieve_py_client/models/batch_queued_chunk_response.py
+-rw-rw-r--  2.0 unx     3463 b- defN 24-Apr-09 04:57 trieve_py_client/models/bookmark_data.py
+-rw-rw-r--  2.0 unx     3119 b- defN 24-Apr-09 04:57 trieve_py_client/models/bookmark_group_result.py
+-rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-09 04:57 trieve_py_client/models/chat_message_proxy.py
+-rw-rw-r--  2.0 unx    10290 b- defN 24-Apr-09 04:57 trieve_py_client/models/chunk_data.py
+-rw-rw-r--  2.0 unx     4960 b- defN 24-Apr-09 04:57 trieve_py_client/models/chunk_filter.py
+-rw-rw-r--  2.0 unx     3900 b- defN 24-Apr-09 04:57 trieve_py_client/models/chunk_group.py
+-rw-rw-r--  2.0 unx     3621 b- defN 24-Apr-09 04:57 trieve_py_client/models/chunk_group_and_file.py
+-rw-rw-r--  2.0 unx     5262 b- defN 24-Apr-09 04:57 trieve_py_client/models/chunk_metadata.py
+-rw-rw-r--  2.0 unx     5587 b- defN 24-Apr-09 04:57 trieve_py_client/models/chunk_metadata_with_file_data.py
+-rw-rw-r--  2.0 unx     7083 b- defN 24-Apr-09 04:57 trieve_py_client/models/client_dataset_configuration.py
+-rw-rw-r--  2.0 unx     5386 b- defN 24-Apr-09 04:57 trieve_py_client/models/create_chunk_data.py
+-rw-rw-r--  2.0 unx     4332 b- defN 24-Apr-09 04:57 trieve_py_client/models/create_chunk_group_data.py
+-rw-rw-r--  2.0 unx     4040 b- defN 24-Apr-09 04:57 trieve_py_client/models/create_dataset_request.py
+-rw-rw-r--  2.0 unx     5235 b- defN 24-Apr-09 04:57 trieve_py_client/models/create_message_data.py
+-rw-rw-r--  2.0 unx     2668 b- defN 24-Apr-09 04:57 trieve_py_client/models/create_organization_data.py
+-rw-rw-r--  2.0 unx     3997 b- defN 24-Apr-09 04:57 trieve_py_client/models/create_topic_data.py
+-rw-rw-r--  2.0 unx     3658 b- defN 24-Apr-09 04:57 trieve_py_client/models/dataset.py
+-rw-rw-r--  2.0 unx     3251 b- defN 24-Apr-09 04:57 trieve_py_client/models/dataset_and_usage.py
+-rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-09 04:57 trieve_py_client/models/dataset_dto.py
+-rw-rw-r--  2.0 unx     2709 b- defN 24-Apr-09 04:57 trieve_py_client/models/dataset_usage_count.py
+-rw-rw-r--  2.0 unx     2593 b- defN 24-Apr-09 04:57 trieve_py_client/models/delete_topic_data.py
+-rw-rw-r--  2.0 unx     2635 b- defN 24-Apr-09 04:57 trieve_py_client/models/delete_user_api_key_request.py
+-rw-rw-r--  2.0 unx     5414 b- defN 24-Apr-09 04:57 trieve_py_client/models/edit_message_data.py
+-rw-rw-r--  2.0 unx     2536 b- defN 24-Apr-09 04:57 trieve_py_client/models/error_response_body.py
+-rw-rw-r--  2.0 unx     3178 b- defN 24-Apr-09 04:57 trieve_py_client/models/event.py
+-rw-rw-r--  2.0 unx     3025 b- defN 24-Apr-09 04:57 trieve_py_client/models/event_return.py
+-rw-rw-r--  2.0 unx     4455 b- defN 24-Apr-09 04:57 trieve_py_client/models/field_condition.py
+-rw-rw-r--  2.0 unx     4151 b- defN 24-Apr-09 04:57 trieve_py_client/models/file.py
+-rw-rw-r--  2.0 unx     3514 b- defN 24-Apr-09 04:57 trieve_py_client/models/file_dto.py
+-rw-rw-r--  2.0 unx     5366 b- defN 24-Apr-09 04:57 trieve_py_client/models/generate_chunks_request.py
+-rw-rw-r--  2.0 unx     3738 b- defN 24-Apr-09 04:57 trieve_py_client/models/get_events_data.py
+-rw-rw-r--  2.0 unx     2570 b- defN 24-Apr-09 04:57 trieve_py_client/models/get_groups_for_chunks_data.py
+-rw-rw-r--  2.0 unx     3072 b- defN 24-Apr-09 04:57 trieve_py_client/models/group_data.py
+-rw-rw-r--  2.0 unx     3492 b- defN 24-Apr-09 04:57 trieve_py_client/models/group_score_chunk_dto.py
+-rw-rw-r--  2.0 unx     3105 b- defN 24-Apr-09 04:57 trieve_py_client/models/group_slim_chunks_dto.py
+-rw-rw-r--  2.0 unx     3482 b- defN 24-Apr-09 04:57 trieve_py_client/models/invitation_data.py
+-rw-rw-r--  2.0 unx     5286 b- defN 24-Apr-09 04:57 trieve_py_client/models/match_condition.py
+-rw-rw-r--  2.0 unx     3932 b- defN 24-Apr-09 04:57 trieve_py_client/models/message.py
+-rw-rw-r--  2.0 unx     3135 b- defN 24-Apr-09 04:57 trieve_py_client/models/organization.py
+-rw-rw-r--  2.0 unx     3008 b- defN 24-Apr-09 04:57 trieve_py_client/models/organization_usage_count.py
+-rw-rw-r--  2.0 unx     4407 b- defN 24-Apr-09 04:57 trieve_py_client/models/range.py
+-rw-rw-r--  2.0 unx     5348 b- defN 24-Apr-09 04:57 trieve_py_client/models/range_condition.py
+-rw-rw-r--  2.0 unx     7177 b- defN 24-Apr-03 03:56 trieve_py_client/models/reccomend_group_chunks_request.py
+-rw-rw-r--  2.0 unx     7324 b- defN 24-Apr-09 04:57 trieve_py_client/models/recommend_chunks_request.py
+-rw-rw-r--  2.0 unx     5946 b- defN 24-Apr-09 04:57 trieve_py_client/models/recommend_chunks_response_types.py
+-rw-rw-r--  2.0 unx     6065 b- defN 24-Apr-09 04:57 trieve_py_client/models/recommend_group_chunk_response_types.py
+-rw-rw-r--  2.0 unx     8162 b- defN 24-Apr-09 04:57 trieve_py_client/models/recommend_group_chunks_request.py
+-rw-rw-r--  2.0 unx     5019 b- defN 24-Apr-09 04:57 trieve_py_client/models/regenerate_message_data.py
+-rw-rw-r--  2.0 unx     5760 b- defN 24-Apr-09 04:57 trieve_py_client/models/return_queued_chunk.py
+-rw-rw-r--  2.0 unx     3155 b- defN 24-Apr-09 04:57 trieve_py_client/models/score_chunk_dto.py
+-rw-rw-r--  2.0 unx     3129 b- defN 24-Apr-09 04:57 trieve_py_client/models/score_slim_chunks.py
+-rw-rw-r--  2.0 unx     8446 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_chunk_data.py
+-rw-rw-r--  2.0 unx     3209 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_chunk_query_response_body.py
+-rw-rw-r--  2.0 unx     6006 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_chunk_response_types.py
+-rw-rw-r--  2.0 unx     3508 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_group_slim_chunks_result.py
+-rw-rw-r--  2.0 unx     3464 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_groups_result.py
+-rw-rw-r--  2.0 unx     8226 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_over_groups_data.py
+-rw-rw-r--  2.0 unx     3230 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_over_groups_response_body.py
+-rw-rw-r--  2.0 unx     6149 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_over_groups_response_types.py
+-rw-rw-r--  2.0 unx     3270 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_over_groups_slim_chunks_response_body.py
+-rw-rw-r--  2.0 unx     3233 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_slim_chunk_query_response_body.py
+-rw-rw-r--  2.0 unx     9074 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_within_group_data.py
+-rw-rw-r--  2.0 unx     5796 b- defN 24-Apr-09 04:57 trieve_py_client/models/search_within_group_response_types.py
+-rw-rw-r--  2.0 unx     3049 b- defN 24-Apr-09 04:57 trieve_py_client/models/set_user_api_key_request.py
+-rw-rw-r--  2.0 unx     2681 b- defN 24-Apr-09 04:57 trieve_py_client/models/set_user_api_key_response.py
+-rw-rw-r--  2.0 unx     3115 b- defN 24-Apr-09 04:57 trieve_py_client/models/single_queued_chunk_response.py
+-rw-rw-r--  2.0 unx     4783 b- defN 24-Apr-09 04:57 trieve_py_client/models/slim_chunk_metadata.py
+-rw-rw-r--  2.0 unx     2772 b- defN 24-Apr-09 04:57 trieve_py_client/models/slim_group.py
+-rw-rw-r--  2.0 unx     3924 b- defN 24-Apr-09 04:57 trieve_py_client/models/slim_user.py
+-rw-rw-r--  2.0 unx     3409 b- defN 24-Apr-09 04:57 trieve_py_client/models/stripe_plan.py
+-rw-rw-r--  2.0 unx     2640 b- defN 24-Apr-09 04:57 trieve_py_client/models/suggested_queries_request.py
+-rw-rw-r--  2.0 unx     2570 b- defN 24-Apr-09 04:57 trieve_py_client/models/suggested_queries_response.py
+-rw-rw-r--  2.0 unx     2995 b- defN 24-Apr-09 04:57 trieve_py_client/models/topic.py
+-rw-rw-r--  2.0 unx     6962 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_chunk_by_tracking_id_data.py
+-rw-rw-r--  2.0 unx     8254 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_chunk_data.py
+-rw-rw-r--  2.0 unx     5225 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_chunk_group_data.py
+-rw-rw-r--  2.0 unx     4343 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_dataset_request.py
+-rw-rw-r--  2.0 unx     4626 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_group_by_tracking_id_data.py
+-rw-rw-r--  2.0 unx     3058 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_organization_data.py
+-rw-rw-r--  2.0 unx     2767 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_topic_data.py
+-rw-rw-r--  2.0 unx     4085 b- defN 24-Apr-09 04:57 trieve_py_client/models/update_user_data.py
+-rw-rw-r--  2.0 unx     6484 b- defN 24-Apr-09 04:57 trieve_py_client/models/upload_file_data.py
+-rw-rw-r--  2.0 unx     2837 b- defN 24-Apr-09 04:57 trieve_py_client/models/upload_file_result.py
+-rw-rw-r--  2.0 unx     2980 b- defN 24-Apr-09 04:57 trieve_py_client/models/user_organization.py
+-rw-rw-r--  2.0 unx      548 b- defN 24-Apr-09 05:02 trieve_py_client-0.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-09 05:02 trieve_py_client-0.6.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 24-Apr-09 05:02 trieve_py_client-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    11463 b- defN 24-Apr-09 05:02 trieve_py_client-0.6.0.dist-info/RECORD
+114 files, 1263343 bytes uncompressed, 188382 bytes compressed:  85.1%
```

## zipnote {}

```diff
@@ -210,14 +210,17 @@
 
 Filename: trieve_py_client/models/recommend_chunks_response_types.py
 Comment: 
 
 Filename: trieve_py_client/models/recommend_group_chunk_response_types.py
 Comment: 
 
+Filename: trieve_py_client/models/recommend_group_chunks_request.py
+Comment: 
+
 Filename: trieve_py_client/models/regenerate_message_data.py
 Comment: 
 
 Filename: trieve_py_client/models/return_queued_chunk.py
 Comment: 
 
 Filename: trieve_py_client/models/score_chunk_dto.py
@@ -321,350 +324,20 @@
 
 Filename: trieve_py_client/models/upload_file_result.py
 Comment: 
 
 Filename: trieve_py_client/models/user_organization.py
 Comment: 
 
-Filename: trieve_python_client/__init__.py
-Comment: 
-
-Filename: trieve_python_client/api_client.py
-Comment: 
-
-Filename: trieve_python_client/api_response.py
-Comment: 
-
-Filename: trieve_python_client/configuration.py
-Comment: 
-
-Filename: trieve_python_client/exceptions.py
-Comment: 
-
-Filename: trieve_python_client/py.typed
-Comment: 
-
-Filename: trieve_python_client/rest.py
-Comment: 
-
-Filename: trieve_python_client/api/__init__.py
-Comment: 
-
-Filename: trieve_python_client/api/auth_api.py
-Comment: 
-
-Filename: trieve_python_client/api/chunk_api.py
-Comment: 
-
-Filename: trieve_python_client/api/chunk_group_api.py
-Comment: 
-
-Filename: trieve_python_client/api/dataset_api.py
-Comment: 
-
-Filename: trieve_python_client/api/events_api.py
-Comment: 
-
-Filename: trieve_python_client/api/file_api.py
-Comment: 
-
-Filename: trieve_python_client/api/health_api.py
-Comment: 
-
-Filename: trieve_python_client/api/invitation_api.py
-Comment: 
-
-Filename: trieve_python_client/api/message_api.py
-Comment: 
-
-Filename: trieve_python_client/api/organization_api.py
-Comment: 
-
-Filename: trieve_python_client/api/stripe_api.py
-Comment: 
-
-Filename: trieve_python_client/api/topic_api.py
-Comment: 
-
-Filename: trieve_python_client/api/user_api.py
-Comment: 
-
-Filename: trieve_python_client/models/__init__.py
-Comment: 
-
-Filename: trieve_python_client/models/add_chunk_to_group_data.py
-Comment: 
-
-Filename: trieve_python_client/models/api_key_dto.py
-Comment: 
-
-Filename: trieve_python_client/models/auth_query.py
-Comment: 
-
-Filename: trieve_python_client/models/batch_queued_chunk_response.py
-Comment: 
-
-Filename: trieve_python_client/models/bookmark_data.py
-Comment: 
-
-Filename: trieve_python_client/models/bookmark_group_result.py
-Comment: 
-
-Filename: trieve_python_client/models/chat_message_proxy.py
-Comment: 
-
-Filename: trieve_python_client/models/chunk_data.py
-Comment: 
-
-Filename: trieve_python_client/models/chunk_filter.py
-Comment: 
-
-Filename: trieve_python_client/models/chunk_group.py
-Comment: 
-
-Filename: trieve_python_client/models/chunk_group_and_file.py
-Comment: 
-
-Filename: trieve_python_client/models/chunk_metadata.py
-Comment: 
-
-Filename: trieve_python_client/models/chunk_metadata_with_file_data.py
-Comment: 
-
-Filename: trieve_python_client/models/client_dataset_configuration.py
-Comment: 
-
-Filename: trieve_python_client/models/create_chunk_data.py
-Comment: 
-
-Filename: trieve_python_client/models/create_chunk_group_data.py
-Comment: 
-
-Filename: trieve_python_client/models/create_dataset_request.py
-Comment: 
-
-Filename: trieve_python_client/models/create_message_data.py
-Comment: 
-
-Filename: trieve_python_client/models/create_organization_data.py
-Comment: 
-
-Filename: trieve_python_client/models/create_topic_data.py
-Comment: 
-
-Filename: trieve_python_client/models/dataset.py
-Comment: 
-
-Filename: trieve_python_client/models/dataset_and_usage.py
-Comment: 
-
-Filename: trieve_python_client/models/dataset_dto.py
-Comment: 
-
-Filename: trieve_python_client/models/dataset_usage_count.py
-Comment: 
-
-Filename: trieve_python_client/models/delete_dataset_request.py
-Comment: 
-
-Filename: trieve_python_client/models/delete_topic_data.py
-Comment: 
-
-Filename: trieve_python_client/models/delete_user_api_key_request.py
-Comment: 
-
-Filename: trieve_python_client/models/edit_message_data.py
-Comment: 
-
-Filename: trieve_python_client/models/error_response_body.py
-Comment: 
-
-Filename: trieve_python_client/models/event.py
-Comment: 
-
-Filename: trieve_python_client/models/event_return.py
-Comment: 
-
-Filename: trieve_python_client/models/field_condition.py
-Comment: 
-
-Filename: trieve_python_client/models/file.py
-Comment: 
-
-Filename: trieve_python_client/models/file_dto.py
-Comment: 
-
-Filename: trieve_python_client/models/generate_chunks_request.py
-Comment: 
-
-Filename: trieve_python_client/models/get_events_data.py
-Comment: 
-
-Filename: trieve_python_client/models/get_groups_for_chunks_data.py
-Comment: 
-
-Filename: trieve_python_client/models/group_data.py
-Comment: 
-
-Filename: trieve_python_client/models/group_score_chunk_dto.py
-Comment: 
-
-Filename: trieve_python_client/models/group_slim_chunks_dto.py
-Comment: 
-
-Filename: trieve_python_client/models/invitation_data.py
-Comment: 
-
-Filename: trieve_python_client/models/match_condition.py
-Comment: 
-
-Filename: trieve_python_client/models/message.py
-Comment: 
-
-Filename: trieve_python_client/models/organization.py
-Comment: 
-
-Filename: trieve_python_client/models/organization_usage_count.py
-Comment: 
-
-Filename: trieve_python_client/models/range.py
-Comment: 
-
-Filename: trieve_python_client/models/range_condition.py
-Comment: 
-
-Filename: trieve_python_client/models/reccomend_group_chunks_request.py
-Comment: 
-
-Filename: trieve_python_client/models/recommend_chunks_request.py
-Comment: 
-
-Filename: trieve_python_client/models/recommend_chunks_response_types.py
-Comment: 
-
-Filename: trieve_python_client/models/recommend_group_chunk_response_types.py
-Comment: 
-
-Filename: trieve_python_client/models/regenerate_message_data.py
-Comment: 
-
-Filename: trieve_python_client/models/return_queued_chunk.py
-Comment: 
-
-Filename: trieve_python_client/models/score_chunk_dto.py
-Comment: 
-
-Filename: trieve_python_client/models/score_slim_chunks.py
-Comment: 
-
-Filename: trieve_python_client/models/search_chunk_data.py
-Comment: 
-
-Filename: trieve_python_client/models/search_chunk_query_response_body.py
-Comment: 
-
-Filename: trieve_python_client/models/search_chunk_response_types.py
-Comment: 
-
-Filename: trieve_python_client/models/search_group_slim_chunks_result.py
-Comment: 
-
-Filename: trieve_python_client/models/search_groups_result.py
-Comment: 
-
-Filename: trieve_python_client/models/search_over_groups_data.py
-Comment: 
-
-Filename: trieve_python_client/models/search_over_groups_response_body.py
-Comment: 
-
-Filename: trieve_python_client/models/search_over_groups_response_types.py
-Comment: 
-
-Filename: trieve_python_client/models/search_over_groups_slim_chunks_response_body.py
-Comment: 
-
-Filename: trieve_python_client/models/search_slim_chunk_query_response_body.py
-Comment: 
-
-Filename: trieve_python_client/models/search_within_group_data.py
-Comment: 
-
-Filename: trieve_python_client/models/search_within_group_response_types.py
-Comment: 
-
-Filename: trieve_python_client/models/set_user_api_key_request.py
-Comment: 
-
-Filename: trieve_python_client/models/set_user_api_key_response.py
-Comment: 
-
-Filename: trieve_python_client/models/single_queued_chunk_response.py
-Comment: 
-
-Filename: trieve_python_client/models/slim_chunk_metadata.py
-Comment: 
-
-Filename: trieve_python_client/models/slim_group.py
-Comment: 
-
-Filename: trieve_python_client/models/slim_user.py
-Comment: 
-
-Filename: trieve_python_client/models/stripe_plan.py
-Comment: 
-
-Filename: trieve_python_client/models/suggested_queries_request.py
-Comment: 
-
-Filename: trieve_python_client/models/suggested_queries_response.py
-Comment: 
-
-Filename: trieve_python_client/models/topic.py
-Comment: 
-
-Filename: trieve_python_client/models/update_chunk_by_tracking_id_data.py
-Comment: 
-
-Filename: trieve_python_client/models/update_chunk_data.py
-Comment: 
-
-Filename: trieve_python_client/models/update_chunk_group_data.py
-Comment: 
-
-Filename: trieve_python_client/models/update_dataset_request.py
-Comment: 
-
-Filename: trieve_python_client/models/update_group_by_tracking_id_data.py
-Comment: 
-
-Filename: trieve_python_client/models/update_organization_data.py
-Comment: 
-
-Filename: trieve_python_client/models/update_topic_data.py
-Comment: 
-
-Filename: trieve_python_client/models/update_user_data.py
-Comment: 
-
-Filename: trieve_python_client/models/upload_file_data.py
-Comment: 
-
-Filename: trieve_python_client/models/upload_file_result.py
-Comment: 
-
-Filename: trieve_python_client/models/user_organization.py
-Comment: 
-
-Filename: trieve_py_client-0.5.7.dist-info/METADATA
+Filename: trieve_py_client-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: trieve_py_client-0.5.7.dist-info/WHEEL
+Filename: trieve_py_client-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: trieve_py_client-0.5.7.dist-info/top_level.txt
+Filename: trieve_py_client-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: trieve_py_client-0.5.7.dist-info/RECORD
+Filename: trieve_py_client-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trieve_py_client/__init__.py

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.5.7"
+__version__ = "0.6.0"
 
 # import apis into sdk package
 from trieve_py_client.api.auth_api import AuthApi
 from trieve_py_client.api.chunk_api import ChunkApi
 from trieve_py_client.api.chunk_group_api import ChunkGroupApi
 from trieve_py_client.api.dataset_api import DatasetApi
 from trieve_py_client.api.events_api import EventsApi
@@ -86,18 +86,18 @@
 from trieve_py_client.models.invitation_data import InvitationData
 from trieve_py_client.models.match_condition import MatchCondition
 from trieve_py_client.models.message import Message
 from trieve_py_client.models.organization import Organization
 from trieve_py_client.models.organization_usage_count import OrganizationUsageCount
 from trieve_py_client.models.range import Range
 from trieve_py_client.models.range_condition import RangeCondition
-from trieve_py_client.models.reccomend_group_chunks_request import ReccomendGroupChunksRequest
 from trieve_py_client.models.recommend_chunks_request import RecommendChunksRequest
 from trieve_py_client.models.recommend_chunks_response_types import RecommendChunksResponseTypes
 from trieve_py_client.models.recommend_group_chunk_response_types import RecommendGroupChunkResponseTypes
+from trieve_py_client.models.recommend_group_chunks_request import RecommendGroupChunksRequest
 from trieve_py_client.models.regenerate_message_data import RegenerateMessageData
 from trieve_py_client.models.return_queued_chunk import ReturnQueuedChunk
 from trieve_py_client.models.score_chunk_dto import ScoreChunkDTO
 from trieve_py_client.models.score_slim_chunks import ScoreSlimChunks
 from trieve_py_client.models.search_chunk_data import SearchChunkData
 from trieve_py_client.models.search_chunk_query_response_body import SearchChunkQueryResponseBody
 from trieve_py_client.models.search_chunk_response_types import SearchChunkResponseTypes
```

## trieve_py_client/api_client.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.7/python'
+        self.user_agent = 'OpenAPI-Generator/0.6.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

## trieve_py_client/configuration.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -395,16 +395,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.5.7\n"\
-               "SDK Package Version: 0.5.7".\
+               "Version of the API: 0.6.0\n"\
+               "SDK Package Version: 0.6.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

## trieve_py_client/exceptions.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

## trieve_py_client/rest.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/api/auth_api.py

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field
+from pydantic import Field, StrictStr
+from typing import Optional
 from typing_extensions import Annotated
-from trieve_py_client.models.auth_query import AuthQuery
 from trieve_py_client.models.slim_user import SlimUser
 
 from trieve_py_client.api_client import ApiClient, RequestSerialized
 from trieve_py_client.api_response import ApiResponse
 from trieve_py_client.rest import RESTResponseType
 
 
@@ -530,15 +530,17 @@
 
 
 
 
     @validate_call
     def login(
         self,
-        content: Annotated[AuthQuery, Field(description="Query parameters for login to be included as kv pairs after ? on the request URL.")],
+        organization_id: Annotated[Optional[StrictStr], Field(description="ID of organization to authenticate into")] = None,
+        redirect_uri: Annotated[Optional[StrictStr], Field(description="URL to redirect to after successful login")] = None,
+        inv_code: Annotated[Optional[StrictStr], Field(description="Code sent via email as a result of successful call to send_invitation")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -548,16 +550,20 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """Login
 
         Login  This will redirect you to the OAuth provider for authentication with email/pass, SSO, Google, Github, etc.
 
-        :param content: Query parameters for login to be included as kv pairs after ? on the request URL. (required)
-        :type content: AuthQuery
+        :param organization_id: ID of organization to authenticate into
+        :type organization_id: str
+        :param redirect_uri: URL to redirect to after successful login
+        :type redirect_uri: str
+        :param inv_code: Code sent via email as a result of successful call to send_invitation
+        :type inv_code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -573,15 +579,17 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._login_serialize(
-            content=content,
+            organization_id=organization_id,
+            redirect_uri=redirect_uri,
+            inv_code=inv_code,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -598,15 +606,17 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def login_with_http_info(
         self,
-        content: Annotated[AuthQuery, Field(description="Query parameters for login to be included as kv pairs after ? on the request URL.")],
+        organization_id: Annotated[Optional[StrictStr], Field(description="ID of organization to authenticate into")] = None,
+        redirect_uri: Annotated[Optional[StrictStr], Field(description="URL to redirect to after successful login")] = None,
+        inv_code: Annotated[Optional[StrictStr], Field(description="Code sent via email as a result of successful call to send_invitation")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -616,16 +626,20 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """Login
 
         Login  This will redirect you to the OAuth provider for authentication with email/pass, SSO, Google, Github, etc.
 
-        :param content: Query parameters for login to be included as kv pairs after ? on the request URL. (required)
-        :type content: AuthQuery
+        :param organization_id: ID of organization to authenticate into
+        :type organization_id: str
+        :param redirect_uri: URL to redirect to after successful login
+        :type redirect_uri: str
+        :param inv_code: Code sent via email as a result of successful call to send_invitation
+        :type inv_code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -641,15 +655,17 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._login_serialize(
-            content=content,
+            organization_id=organization_id,
+            redirect_uri=redirect_uri,
+            inv_code=inv_code,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -666,15 +682,17 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def login_without_preload_content(
         self,
-        content: Annotated[AuthQuery, Field(description="Query parameters for login to be included as kv pairs after ? on the request URL.")],
+        organization_id: Annotated[Optional[StrictStr], Field(description="ID of organization to authenticate into")] = None,
+        redirect_uri: Annotated[Optional[StrictStr], Field(description="URL to redirect to after successful login")] = None,
+        inv_code: Annotated[Optional[StrictStr], Field(description="Code sent via email as a result of successful call to send_invitation")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -684,16 +702,20 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Login
 
         Login  This will redirect you to the OAuth provider for authentication with email/pass, SSO, Google, Github, etc.
 
-        :param content: Query parameters for login to be included as kv pairs after ? on the request URL. (required)
-        :type content: AuthQuery
+        :param organization_id: ID of organization to authenticate into
+        :type organization_id: str
+        :param redirect_uri: URL to redirect to after successful login
+        :type redirect_uri: str
+        :param inv_code: Code sent via email as a result of successful call to send_invitation
+        :type inv_code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -709,15 +731,17 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._login_serialize(
-            content=content,
+            organization_id=organization_id,
+            redirect_uri=redirect_uri,
+            inv_code=inv_code,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -729,15 +753,17 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _login_serialize(
         self,
-        content,
+        organization_id,
+        redirect_uri,
+        inv_code,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -750,17 +776,25 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if content is not None:
+        if organization_id is not None:
             
-            _query_params.append(('content', content))
+            _query_params.append(('organization_id', organization_id))
+            
+        if redirect_uri is not None:
+            
+            _query_params.append(('redirect_uri', redirect_uri))
+            
+        if inv_code is not None:
+            
+            _query_params.append(('inv_code', inv_code))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
```

## trieve_py_client/api/chunk_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -2906,15 +2906,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Update Chunk By Tracking Id
+        """(Deprecated) Update Chunk By Tracking Id
 
         Update Chunk By Tracking Id  Update a chunk by tracking_id. This is useful for when you are coordinating with an external system and want to use the tracking_id to identify the chunk.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param update_chunk_by_tracking_id_data: JSON request payload to update a chunk by tracking_id (chunks) (required)
         :type update_chunk_by_tracking_id_data: UpdateChunkByTrackingIdData
@@ -2935,14 +2935,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/chunk/tracking_id/update is deprecated.", DeprecationWarning)
 
         _param = self._update_chunk_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             update_chunk_by_tracking_id_data=update_chunk_by_tracking_id_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -2978,15 +2979,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Update Chunk By Tracking Id
+        """(Deprecated) Update Chunk By Tracking Id
 
         Update Chunk By Tracking Id  Update a chunk by tracking_id. This is useful for when you are coordinating with an external system and want to use the tracking_id to identify the chunk.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param update_chunk_by_tracking_id_data: JSON request payload to update a chunk by tracking_id (chunks) (required)
         :type update_chunk_by_tracking_id_data: UpdateChunkByTrackingIdData
@@ -3007,14 +3008,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/chunk/tracking_id/update is deprecated.", DeprecationWarning)
 
         _param = self._update_chunk_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             update_chunk_by_tracking_id_data=update_chunk_by_tracking_id_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -3050,15 +3052,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update Chunk By Tracking Id
+        """(Deprecated) Update Chunk By Tracking Id
 
         Update Chunk By Tracking Id  Update a chunk by tracking_id. This is useful for when you are coordinating with an external system and want to use the tracking_id to identify the chunk.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param update_chunk_by_tracking_id_data: JSON request payload to update a chunk by tracking_id (chunks) (required)
         :type update_chunk_by_tracking_id_data: UpdateChunkByTrackingIdData
@@ -3079,14 +3081,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/chunk/tracking_id/update is deprecated.", DeprecationWarning)
 
         _param = self._update_chunk_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             update_chunk_by_tracking_id_data=update_chunk_by_tracking_id_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
```

## trieve_py_client/api/chunk_group_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -23,16 +23,16 @@
 from trieve_py_client.models.add_chunk_to_group_data import AddChunkToGroupData
 from trieve_py_client.models.bookmark_data import BookmarkData
 from trieve_py_client.models.bookmark_group_result import BookmarkGroupResult
 from trieve_py_client.models.chunk_group import ChunkGroup
 from trieve_py_client.models.create_chunk_group_data import CreateChunkGroupData
 from trieve_py_client.models.get_groups_for_chunks_data import GetGroupsForChunksData
 from trieve_py_client.models.group_data import GroupData
-from trieve_py_client.models.reccomend_group_chunks_request import ReccomendGroupChunksRequest
 from trieve_py_client.models.recommend_group_chunk_response_types import RecommendGroupChunkResponseTypes
+from trieve_py_client.models.recommend_group_chunks_request import RecommendGroupChunksRequest
 from trieve_py_client.models.search_over_groups_data import SearchOverGroupsData
 from trieve_py_client.models.search_over_groups_response_types import SearchOverGroupsResponseTypes
 from trieve_py_client.models.search_within_group_data import SearchWithinGroupData
 from trieve_py_client.models.search_within_group_response_types import SearchWithinGroupResponseTypes
 from trieve_py_client.models.update_chunk_group_data import UpdateChunkGroupData
 from trieve_py_client.models.update_group_by_tracking_id_data import UpdateGroupByTrackingIDData
 
@@ -373,15 +373,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Add Chunk to Group by Tracking ID
+        """(Deprecated) Add Chunk to Group by Tracking ID
 
         Add Chunk to Group by Tracking ID  Route to add a chunk to a group by tracking id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param tracking_id: Id of the group to add the chunk to as a bookmark (required)
         :type tracking_id: str
@@ -404,14 +404,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("POST /api/chunk_group/tracking_id/{tracking_id} is deprecated.", DeprecationWarning)
 
         _param = self._add_chunk_to_group_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             tracking_id=tracking_id,
             add_chunk_to_group_data=add_chunk_to_group_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -449,15 +450,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Add Chunk to Group by Tracking ID
+        """(Deprecated) Add Chunk to Group by Tracking ID
 
         Add Chunk to Group by Tracking ID  Route to add a chunk to a group by tracking id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param tracking_id: Id of the group to add the chunk to as a bookmark (required)
         :type tracking_id: str
@@ -480,14 +481,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("POST /api/chunk_group/tracking_id/{tracking_id} is deprecated.", DeprecationWarning)
 
         _param = self._add_chunk_to_group_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             tracking_id=tracking_id,
             add_chunk_to_group_data=add_chunk_to_group_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -525,15 +527,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Add Chunk to Group by Tracking ID
+        """(Deprecated) Add Chunk to Group by Tracking ID
 
         Add Chunk to Group by Tracking ID  Route to add a chunk to a group by tracking id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param tracking_id: Id of the group to add the chunk to as a bookmark (required)
         :type tracking_id: str
@@ -556,14 +558,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("POST /api/chunk_group/tracking_id/{tracking_id} is deprecated.", DeprecationWarning)
 
         _param = self._add_chunk_to_group_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             tracking_id=tracking_id,
             add_chunk_to_group_data=add_chunk_to_group_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -968,15 +971,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """Delete Group
 
-        Delete Group  This will delete a chunk_group. This will not delete the chunks that are in the group. We will soon support deleting a chunk_group along with its member chunks.
+        Delete Group  This will delete a chunk_group. If you set delete_chunks to true, it will also delete the chunks within the group.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_id: Id of the group you want to fetch. (required)
         :type group_id: str
         :param delete_chunks: Delete the chunks within the group (required)
         :type delete_chunks: bool
@@ -1044,15 +1047,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """Delete Group
 
-        Delete Group  This will delete a chunk_group. This will not delete the chunks that are in the group. We will soon support deleting a chunk_group along with its member chunks.
+        Delete Group  This will delete a chunk_group. If you set delete_chunks to true, it will also delete the chunks within the group.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_id: Id of the group you want to fetch. (required)
         :type group_id: str
         :param delete_chunks: Delete the chunks within the group (required)
         :type delete_chunks: bool
@@ -1120,15 +1123,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Delete Group
 
-        Delete Group  This will delete a chunk_group. This will not delete the chunks that are in the group. We will soon support deleting a chunk_group along with its member chunks.
+        Delete Group  This will delete a chunk_group. If you set delete_chunks to true, it will also delete the chunks within the group.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_id: Id of the group you want to fetch. (required)
         :type group_id: str
         :param delete_chunks: Delete the chunks within the group (required)
         :type delete_chunks: bool
@@ -1813,15 +1816,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> BookmarkData:
         """Get Chunks in Group
 
-        Get Chunks in Group  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon.
+        Get Chunks in Group  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Page is 1-indexed.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_id: Id of the group you want to fetch. (required)
         :type group_id: str
         :param page: The page of chunks to get from the group (required)
         :type page: int
@@ -1889,15 +1892,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[BookmarkData]:
         """Get Chunks in Group
 
-        Get Chunks in Group  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon.
+        Get Chunks in Group  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Page is 1-indexed.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_id: Id of the group you want to fetch. (required)
         :type group_id: str
         :param page: The page of chunks to get from the group (required)
         :type page: int
@@ -1965,15 +1968,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Chunks in Group
 
-        Get Chunks in Group  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon.
+        Get Chunks in Group  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Page is 1-indexed.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_id: Id of the group you want to fetch. (required)
         :type group_id: str
         :param page: The page of chunks to get from the group (required)
         :type page: int
@@ -2104,15 +2107,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> BookmarkData:
         """Get Chunks in Group by Tracking ID
 
-        Get Chunks in Group by Tracking ID  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon.
+        Get Chunks in Group by Tracking ID  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon. Page is 1-indexed.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_tracking_id: The id of the group to get the chunks from (required)
         :type group_tracking_id: str
         :param page: The page of chunks to get from the group (required)
         :type page: int
@@ -2180,15 +2183,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[BookmarkData]:
         """Get Chunks in Group by Tracking ID
 
-        Get Chunks in Group by Tracking ID  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon.
+        Get Chunks in Group by Tracking ID  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon. Page is 1-indexed.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_tracking_id: The id of the group to get the chunks from (required)
         :type group_tracking_id: str
         :param page: The page of chunks to get from the group (required)
         :type page: int
@@ -2256,15 +2259,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Chunks in Group by Tracking ID
 
-        Get Chunks in Group by Tracking ID  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon.
+        Get Chunks in Group by Tracking ID  Route to get all chunks for a group. The response is paginated, with each page containing 10 chunks. Support for custom page size is coming soon. Page is 1-indexed.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param group_tracking_id: The id of the group to get the chunks from (required)
         :type group_tracking_id: str
         :param page: The page of chunks to get from the group (required)
         :type page: int
@@ -2943,15 +2946,15 @@
 
 
 
     @validate_call
     def get_recommended_groups(
         self,
         tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
-        reccomend_group_chunks_request: Annotated[ReccomendGroupChunksRequest, Field(description="JSON request payload to get recommendations of chunks similar to the chunks in the request")],
+        recommend_group_chunks_request: Annotated[RecommendGroupChunksRequest, Field(description="JSON request payload to get recommendations of chunks similar to the chunks in the request")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2963,16 +2966,16 @@
     ) -> RecommendGroupChunkResponseTypes:
         """Get Recommended Groups
 
         Get Recommended Groups  Route to get recommended groups. This route will return groups which are similar to the groups in the request body.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
-        :param reccomend_group_chunks_request: JSON request payload to get recommendations of chunks similar to the chunks in the request (required)
-        :type reccomend_group_chunks_request: ReccomendGroupChunksRequest
+        :param recommend_group_chunks_request: JSON request payload to get recommendations of chunks similar to the chunks in the request (required)
+        :type recommend_group_chunks_request: RecommendGroupChunksRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2989,15 +2992,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_recommended_groups_serialize(
             tr_dataset=tr_dataset,
-            reccomend_group_chunks_request=reccomend_group_chunks_request,
+            recommend_group_chunks_request=recommend_group_chunks_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3015,15 +3018,15 @@
         ).data
 
 
     @validate_call
     def get_recommended_groups_with_http_info(
         self,
         tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
-        reccomend_group_chunks_request: Annotated[ReccomendGroupChunksRequest, Field(description="JSON request payload to get recommendations of chunks similar to the chunks in the request")],
+        recommend_group_chunks_request: Annotated[RecommendGroupChunksRequest, Field(description="JSON request payload to get recommendations of chunks similar to the chunks in the request")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3035,16 +3038,16 @@
     ) -> ApiResponse[RecommendGroupChunkResponseTypes]:
         """Get Recommended Groups
 
         Get Recommended Groups  Route to get recommended groups. This route will return groups which are similar to the groups in the request body.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
-        :param reccomend_group_chunks_request: JSON request payload to get recommendations of chunks similar to the chunks in the request (required)
-        :type reccomend_group_chunks_request: ReccomendGroupChunksRequest
+        :param recommend_group_chunks_request: JSON request payload to get recommendations of chunks similar to the chunks in the request (required)
+        :type recommend_group_chunks_request: RecommendGroupChunksRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3061,15 +3064,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_recommended_groups_serialize(
             tr_dataset=tr_dataset,
-            reccomend_group_chunks_request=reccomend_group_chunks_request,
+            recommend_group_chunks_request=recommend_group_chunks_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3087,15 +3090,15 @@
         )
 
 
     @validate_call
     def get_recommended_groups_without_preload_content(
         self,
         tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
-        reccomend_group_chunks_request: Annotated[ReccomendGroupChunksRequest, Field(description="JSON request payload to get recommendations of chunks similar to the chunks in the request")],
+        recommend_group_chunks_request: Annotated[RecommendGroupChunksRequest, Field(description="JSON request payload to get recommendations of chunks similar to the chunks in the request")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3107,16 +3110,16 @@
     ) -> RESTResponseType:
         """Get Recommended Groups
 
         Get Recommended Groups  Route to get recommended groups. This route will return groups which are similar to the groups in the request body.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
-        :param reccomend_group_chunks_request: JSON request payload to get recommendations of chunks similar to the chunks in the request (required)
-        :type reccomend_group_chunks_request: ReccomendGroupChunksRequest
+        :param recommend_group_chunks_request: JSON request payload to get recommendations of chunks similar to the chunks in the request (required)
+        :type recommend_group_chunks_request: RecommendGroupChunksRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3133,15 +3136,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_recommended_groups_serialize(
             tr_dataset=tr_dataset,
-            reccomend_group_chunks_request=reccomend_group_chunks_request,
+            recommend_group_chunks_request=recommend_group_chunks_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3154,15 +3157,15 @@
         )
         return response_data.response
 
 
     def _get_recommended_groups_serialize(
         self,
         tr_dataset,
-        reccomend_group_chunks_request,
+        recommend_group_chunks_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3180,16 +3183,16 @@
         # process the path parameters
         # process the query parameters
         # process the header parameters
         if tr_dataset is not None:
             _header_params['TR-Dataset'] = tr_dataset
         # process the form parameters
         # process the body parameter
-        if reccomend_group_chunks_request is not None:
-            _body_params = reccomend_group_chunks_request
+        if recommend_group_chunks_request is not None:
+            _body_params = recommend_group_chunks_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -3233,15 +3236,15 @@
 
 
     @validate_call
     def get_specific_dataset_chunk_groups(
         self,
         tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
         dataset_id: Annotated[StrictStr, Field(description="The id of the dataset to fetch groups for.")],
-        page: Annotated[StrictInt, Field(description="The page of groups to fetch. Each page contains 10 groups. Support for custom page size is coming soon.")],
+        page: Annotated[StrictInt, Field(description="The page of groups to fetch. Page is 1-indexed.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3255,15 +3258,15 @@
 
         Get Groups for Dataset  Fetch the groups which belong to a dataset specified by its id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param dataset_id: The id of the dataset to fetch groups for. (required)
         :type dataset_id: str
-        :param page: The page of groups to fetch. Each page contains 10 groups. Support for custom page size is coming soon. (required)
+        :param page: The page of groups to fetch. Page is 1-indexed. (required)
         :type page: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -3309,15 +3312,15 @@
 
 
     @validate_call
     def get_specific_dataset_chunk_groups_with_http_info(
         self,
         tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
         dataset_id: Annotated[StrictStr, Field(description="The id of the dataset to fetch groups for.")],
-        page: Annotated[StrictInt, Field(description="The page of groups to fetch. Each page contains 10 groups. Support for custom page size is coming soon.")],
+        page: Annotated[StrictInt, Field(description="The page of groups to fetch. Page is 1-indexed.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3331,15 +3334,15 @@
 
         Get Groups for Dataset  Fetch the groups which belong to a dataset specified by its id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param dataset_id: The id of the dataset to fetch groups for. (required)
         :type dataset_id: str
-        :param page: The page of groups to fetch. Each page contains 10 groups. Support for custom page size is coming soon. (required)
+        :param page: The page of groups to fetch. Page is 1-indexed. (required)
         :type page: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -3385,15 +3388,15 @@
 
 
     @validate_call
     def get_specific_dataset_chunk_groups_without_preload_content(
         self,
         tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
         dataset_id: Annotated[StrictStr, Field(description="The id of the dataset to fetch groups for.")],
-        page: Annotated[StrictInt, Field(description="The page of groups to fetch. Each page contains 10 groups. Support for custom page size is coming soon.")],
+        page: Annotated[StrictInt, Field(description="The page of groups to fetch. Page is 1-indexed.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3407,15 +3410,15 @@
 
         Get Groups for Dataset  Fetch the groups which belong to a dataset specified by its id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param dataset_id: The id of the dataset to fetch groups for. (required)
         :type dataset_id: str
-        :param page: The page of groups to fetch. Each page contains 10 groups. Support for custom page size is coming soon. (required)
+        :param page: The page of groups to fetch. Page is 1-indexed. (required)
         :type page: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -4709,15 +4712,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Update Group by Tracking ID
+        """(Deprecated) Update Group by Tracking ID
 
         Update Group by Tracking ID  Update a chunk_group with the given tracking id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param tracking_id: Tracking id of the chunk_group to update (required)
         :type tracking_id: str
@@ -4740,14 +4743,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/chunk_group/tracking_id/{tracking_id} is deprecated.", DeprecationWarning)
 
         _param = self._update_group_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             tracking_id=tracking_id,
             update_group_by_tracking_id_data=update_group_by_tracking_id_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -4785,15 +4789,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Update Group by Tracking ID
+        """(Deprecated) Update Group by Tracking ID
 
         Update Group by Tracking ID  Update a chunk_group with the given tracking id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param tracking_id: Tracking id of the chunk_group to update (required)
         :type tracking_id: str
@@ -4816,14 +4820,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/chunk_group/tracking_id/{tracking_id} is deprecated.", DeprecationWarning)
 
         _param = self._update_group_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             tracking_id=tracking_id,
             update_group_by_tracking_id_data=update_group_by_tracking_id_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -4861,15 +4866,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update Group by Tracking ID
+        """(Deprecated) Update Group by Tracking ID
 
         Update Group by Tracking ID  Update a chunk_group with the given tracking id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param tracking_id: Tracking id of the chunk_group to update (required)
         :type tracking_id: str
@@ -4892,14 +4897,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/chunk_group/tracking_id/{tracking_id} is deprecated.", DeprecationWarning)
 
         _param = self._update_group_by_tracking_id_serialize(
             tr_dataset=tr_dataset,
             tracking_id=tracking_id,
             update_group_by_tracking_id_data=update_group_by_tracking_id_data,
             _request_auth=_request_auth,
             _content_type=_content_type,
```

## trieve_py_client/api/dataset_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -331,15 +331,15 @@
 
 
 
 
     @validate_call
     def delete_dataset(
         self,
-        tr_organization: Annotated[StrictStr, Field(description="The organization id to use for the request")],
+        tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
         dataset_id: Annotated[StrictStr, Field(description="The id of the dataset you want to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -350,16 +350,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """Delete Dataset
 
         Delete Dataset  Delete a dataset. The auth'ed user must be an owner of the organization to delete a dataset.
 
-        :param tr_organization: The organization id to use for the request (required)
-        :type tr_organization: str
+        :param tr_dataset: The dataset id to use for the request (required)
+        :type tr_dataset: str
         :param dataset_id: The id of the dataset you want to delete. (required)
         :type dataset_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -377,15 +377,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._delete_dataset_serialize(
-            tr_organization=tr_organization,
+            tr_dataset=tr_dataset,
             dataset_id=dataset_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -403,15 +403,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def delete_dataset_with_http_info(
         self,
-        tr_organization: Annotated[StrictStr, Field(description="The organization id to use for the request")],
+        tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
         dataset_id: Annotated[StrictStr, Field(description="The id of the dataset you want to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -422,16 +422,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """Delete Dataset
 
         Delete Dataset  Delete a dataset. The auth'ed user must be an owner of the organization to delete a dataset.
 
-        :param tr_organization: The organization id to use for the request (required)
-        :type tr_organization: str
+        :param tr_dataset: The dataset id to use for the request (required)
+        :type tr_dataset: str
         :param dataset_id: The id of the dataset you want to delete. (required)
         :type dataset_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -449,15 +449,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._delete_dataset_serialize(
-            tr_organization=tr_organization,
+            tr_dataset=tr_dataset,
             dataset_id=dataset_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -475,15 +475,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def delete_dataset_without_preload_content(
         self,
-        tr_organization: Annotated[StrictStr, Field(description="The organization id to use for the request")],
+        tr_dataset: Annotated[StrictStr, Field(description="The dataset id to use for the request")],
         dataset_id: Annotated[StrictStr, Field(description="The id of the dataset you want to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -494,16 +494,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Delete Dataset
 
         Delete Dataset  Delete a dataset. The auth'ed user must be an owner of the organization to delete a dataset.
 
-        :param tr_organization: The organization id to use for the request (required)
-        :type tr_organization: str
+        :param tr_dataset: The dataset id to use for the request (required)
+        :type tr_dataset: str
         :param dataset_id: The id of the dataset you want to delete. (required)
         :type dataset_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -521,15 +521,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._delete_dataset_serialize(
-            tr_organization=tr_organization,
+            tr_dataset=tr_dataset,
             dataset_id=dataset_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -542,15 +542,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _delete_dataset_serialize(
         self,
-        tr_organization,
+        tr_dataset,
         dataset_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
@@ -567,16 +567,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if dataset_id is not None:
             _path_params['dataset_id'] = dataset_id
         # process the query parameters
         # process the header parameters
-        if tr_organization is not None:
-            _header_params['TR-Organization'] = tr_organization
+        if tr_dataset is not None:
+            _header_params['TR-Dataset'] = tr_dataset
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
```

## trieve_py_client/api/events_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -56,15 +56,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> EventReturn:
         """Get events for the dataset
 
-        Get events for the dataset  Get events for the auth'ed user. Currently, this is only for events belonging to the auth'ed user. Soon, we plan to associate events to datasets instead of users.
+        Get events for the dataset  Get events for the dataset specified by the TR-Dataset header.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param get_events_data: JSON request payload to get events for a dataset (required)
         :type get_events_data: GetEventsData
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -128,15 +128,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[EventReturn]:
         """Get events for the dataset
 
-        Get events for the dataset  Get events for the auth'ed user. Currently, this is only for events belonging to the auth'ed user. Soon, we plan to associate events to datasets instead of users.
+        Get events for the dataset  Get events for the dataset specified by the TR-Dataset header.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param get_events_data: JSON request payload to get events for a dataset (required)
         :type get_events_data: GetEventsData
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -200,15 +200,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get events for the dataset
 
-        Get events for the dataset  Get events for the auth'ed user. Currently, this is only for events belonging to the auth'ed user. Soon, we plan to associate events to datasets instead of users.
+        Get events for the dataset  Get events for the dataset specified by the TR-Dataset header.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param get_events_data: JSON request payload to get events for a dataset (required)
         :type get_events_data: GetEventsData
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

## trieve_py_client/api/file_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -59,15 +59,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """Delete File
 
-        Delete File  Delete a file from S3 attached to the server based on its id. This will disassociate chunks from the file, but will not delete the chunks. We plan to add support for deleting chunks in a release soon. Auth'ed user must be an admin or owner of the dataset's organization to upload a file.
+        Delete File  Delete a file from S3 attached to the server based on its id. This will disassociate chunks from the file, but only delete them all together if you specify delete_chunks to be true. Auth'ed user must be an admin or owner of the dataset's organization to delete a file.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param file_id: The id of the file to delete (required)
         :type file_id: str
         :param delete_chunks: Whether or not to delete the chunks associated with the file (required)
         :type delete_chunks: bool
@@ -135,15 +135,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """Delete File
 
-        Delete File  Delete a file from S3 attached to the server based on its id. This will disassociate chunks from the file, but will not delete the chunks. We plan to add support for deleting chunks in a release soon. Auth'ed user must be an admin or owner of the dataset's organization to upload a file.
+        Delete File  Delete a file from S3 attached to the server based on its id. This will disassociate chunks from the file, but only delete them all together if you specify delete_chunks to be true. Auth'ed user must be an admin or owner of the dataset's organization to delete a file.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param file_id: The id of the file to delete (required)
         :type file_id: str
         :param delete_chunks: Whether or not to delete the chunks associated with the file (required)
         :type delete_chunks: bool
@@ -211,15 +211,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Delete File
 
-        Delete File  Delete a file from S3 attached to the server based on its id. This will disassociate chunks from the file, but will not delete the chunks. We plan to add support for deleting chunks in a release soon. Auth'ed user must be an admin or owner of the dataset's organization to upload a file.
+        Delete File  Delete a file from S3 attached to the server based on its id. This will disassociate chunks from the file, but only delete them all together if you specify delete_chunks to be true. Auth'ed user must be an admin or owner of the dataset's organization to delete a file.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param file_id: The id of the file to delete (required)
         :type file_id: str
         :param delete_chunks: Whether or not to delete the chunks associated with the file (required)
         :type delete_chunks: bool
@@ -642,15 +642,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> FileDTO:
         """Get File
 
-        Get File  Download a file from S3 attached to the server based on its id. We plan to add support for getting signed S3 URLs to download from S3 directly in a release soon.
+        Get File  Download a file based on its id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param file_id: The id of the file to fetch (required)
         :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -714,15 +714,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[FileDTO]:
         """Get File
 
-        Get File  Download a file from S3 attached to the server based on its id. We plan to add support for getting signed S3 URLs to download from S3 directly in a release soon.
+        Get File  Download a file based on its id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param file_id: The id of the file to fetch (required)
         :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -786,15 +786,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get File
 
-        Get File  Download a file from S3 attached to the server based on its id. We plan to add support for getting signed S3 URLs to download from S3 directly in a release soon.
+        Get File  Download a file based on its id.
 
         :param tr_dataset: The dataset id to use for the request (required)
         :type tr_dataset: str
         :param file_id: The id of the file to fetch (required)
         :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

## trieve_py_client/api/health_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/api/invitation_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/api/message_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/api/organization_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/api/stripe_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/api/topic_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/api/user_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

## trieve_py_client/models/__init__.py

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -57,18 +57,18 @@
 from trieve_py_client.models.invitation_data import InvitationData
 from trieve_py_client.models.match_condition import MatchCondition
 from trieve_py_client.models.message import Message
 from trieve_py_client.models.organization import Organization
 from trieve_py_client.models.organization_usage_count import OrganizationUsageCount
 from trieve_py_client.models.range import Range
 from trieve_py_client.models.range_condition import RangeCondition
-from trieve_py_client.models.reccomend_group_chunks_request import ReccomendGroupChunksRequest
 from trieve_py_client.models.recommend_chunks_request import RecommendChunksRequest
 from trieve_py_client.models.recommend_chunks_response_types import RecommendChunksResponseTypes
 from trieve_py_client.models.recommend_group_chunk_response_types import RecommendGroupChunkResponseTypes
+from trieve_py_client.models.recommend_group_chunks_request import RecommendGroupChunksRequest
 from trieve_py_client.models.regenerate_message_data import RegenerateMessageData
 from trieve_py_client.models.return_queued_chunk import ReturnQueuedChunk
 from trieve_py_client.models.score_chunk_dto import ScoreChunkDTO
 from trieve_py_client.models.score_slim_chunks import ScoreSlimChunks
 from trieve_py_client.models.search_chunk_data import SearchChunkData
 from trieve_py_client.models.search_chunk_query_response_body import SearchChunkQueryResponseBody
 from trieve_py_client.models.search_chunk_response_types import SearchChunkResponseTypes
```

## trieve_py_client/models/add_chunk_to_group_data.py

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AddChunkToGroupData(BaseModel):
     """
     AddChunkToGroupData
     """ # noqa: E501
-    chunk_id: StrictStr = Field(description="Id of the chunk to make a member of the group.")
-    __properties: ClassVar[List[str]] = ["chunk_id"]
+    chunk_id: Optional[StrictStr] = Field(default=None, description="Id of the chunk to make a member of the group.")
+    tracking_id: Optional[StrictStr] = Field(default=None, description="Tracking Id of the chunk to make a member of the group.")
+    __properties: ClassVar[List[str]] = ["chunk_id", "tracking_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -65,24 +66,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if chunk_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.chunk_id is None and "chunk_id" in self.model_fields_set:
+            _dict['chunk_id'] = None
+
+        # set to None if tracking_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.tracking_id is None and "tracking_id" in self.model_fields_set:
+            _dict['tracking_id'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of AddChunkToGroupData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "chunk_id": obj.get("chunk_id")
+            "chunk_id": obj.get("chunk_id"),
+            "tracking_id": obj.get("tracking_id")
         })
         return _obj
```

## trieve_py_client/models/api_key_dto.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/auth_query.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/batch_queued_chunk_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/bookmark_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/bookmark_group_result.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/chat_message_proxy.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/chunk_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/chunk_filter.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/chunk_group.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -28,18 +28,20 @@
     """
     ChunkGroup
     """ # noqa: E501
     created_at: datetime
     dataset_id: StrictStr
     description: StrictStr
     id: StrictStr
+    metadata: Optional[Any] = None
     name: StrictStr
+    tag_set: Optional[StrictStr] = None
     tracking_id: Optional[StrictStr] = None
     updated_at: datetime
-    __properties: ClassVar[List[str]] = ["created_at", "dataset_id", "description", "id", "name", "tracking_id", "updated_at"]
+    __properties: ClassVar[List[str]] = ["created_at", "dataset_id", "description", "id", "metadata", "name", "tag_set", "tracking_id", "updated_at"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -72,14 +74,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if metadata (nullable) is None
+        # and model_fields_set contains the field
+        if self.metadata is None and "metadata" in self.model_fields_set:
+            _dict['metadata'] = None
+
+        # set to None if tag_set (nullable) is None
+        # and model_fields_set contains the field
+        if self.tag_set is None and "tag_set" in self.model_fields_set:
+            _dict['tag_set'] = None
+
         # set to None if tracking_id (nullable) is None
         # and model_fields_set contains the field
         if self.tracking_id is None and "tracking_id" in self.model_fields_set:
             _dict['tracking_id'] = None
 
         return _dict
 
@@ -93,14 +105,16 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "created_at": obj.get("created_at"),
             "dataset_id": obj.get("dataset_id"),
             "description": obj.get("description"),
             "id": obj.get("id"),
+            "metadata": obj.get("metadata"),
             "name": obj.get("name"),
+            "tag_set": obj.get("tag_set"),
             "tracking_id": obj.get("tracking_id"),
             "updated_at": obj.get("updated_at")
         })
         return _obj
```

## trieve_py_client/models/chunk_group_and_file.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/chunk_metadata.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/chunk_metadata_with_file_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/client_dataset_configuration.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/create_chunk_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/create_chunk_group_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,17 +24,19 @@
 from typing_extensions import Self
 
 class CreateChunkGroupData(BaseModel):
     """
     CreateChunkGroupData
     """ # noqa: E501
     description: StrictStr = Field(description="Description to assign to the chunk_group. Convenience field for you to avoid having to remember what the group is for.")
+    metadata: Optional[Any] = Field(default=None, description="Optional metadata to assign to the chunk_group. This is a JSON object that can store any additional information you want to associate with the chunks inside of the chunk_group.")
     name: StrictStr = Field(description="Name to assign to the chunk_group. Does not need to be unique.")
+    tag_set: Optional[List[StrictStr]] = Field(default=None, description="Optional tags to assign to the chunk_group. This is a list of strings that can be used to categorize the chunks inside the chunk_group.")
     tracking_id: Optional[StrictStr] = Field(default=None, description="Optional tracking id to assign to the chunk_group. This is a unique identifier for the chunk_group.")
-    __properties: ClassVar[List[str]] = ["description", "name", "tracking_id"]
+    __properties: ClassVar[List[str]] = ["description", "metadata", "name", "tag_set", "tracking_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -67,14 +69,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if metadata (nullable) is None
+        # and model_fields_set contains the field
+        if self.metadata is None and "metadata" in self.model_fields_set:
+            _dict['metadata'] = None
+
+        # set to None if tag_set (nullable) is None
+        # and model_fields_set contains the field
+        if self.tag_set is None and "tag_set" in self.model_fields_set:
+            _dict['tag_set'] = None
+
         # set to None if tracking_id (nullable) is None
         # and model_fields_set contains the field
         if self.tracking_id is None and "tracking_id" in self.model_fields_set:
             _dict['tracking_id'] = None
 
         return _dict
 
@@ -85,13 +97,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "description": obj.get("description"),
+            "metadata": obj.get("metadata"),
             "name": obj.get("name"),
+            "tag_set": obj.get("tag_set"),
             "tracking_id": obj.get("tracking_id")
         })
         return _obj
```

## trieve_py_client/models/create_dataset_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/create_message_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/create_organization_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/create_topic_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/dataset.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/dataset_and_usage.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/dataset_dto.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/dataset_usage_count.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/delete_topic_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/delete_user_api_key_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/edit_message_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/error_response_body.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/event.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/event_return.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/field_condition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/file.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/file_dto.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/generate_chunks_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/get_events_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/get_groups_for_chunks_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/group_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/group_score_chunk_dto.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/group_slim_chunks_dto.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/invitation_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/match_condition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/message.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/organization.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/organization_usage_count.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/range.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/range_condition.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/recommend_chunks_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -32,15 +32,16 @@
     filters: Optional[ChunkFilter] = None
     limit: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The number of chunks to return. This is the number of chunks which will be returned in the response. The default is 10.")
     negative_chunk_ids: Optional[List[StrictStr]] = Field(default=None, description="The ids of the chunks to be used as negative examples for the recommendation. The chunks in this array will be used to filter out similar chunks.")
     negative_tracking_ids: Optional[List[StrictStr]] = Field(default=None, description="The tracking_ids of the chunks to be used as negative examples for the recommendation. The chunks in this array will be used to filter out similar chunks.")
     positive_chunk_ids: Optional[List[StrictStr]] = Field(default=None, description="The ids of the chunks to be used as positive examples for the recommendation. The chunks in this array will be used to find similar chunks.")
     positive_tracking_ids: Optional[List[StrictStr]] = Field(default=None, description="The tracking_ids of the chunks to be used as positive examples for the recommendation. The chunks in this array will be used to find similar chunks.")
     slim_chunks: Optional[StrictBool] = Field(default=None, description="Set slim_chunks to true to avoid returning the content and chunk_html of the chunks. This is useful for when you want to reduce amount of data over the wire for latency improvement. Default is false.")
-    __properties: ClassVar[List[str]] = ["filters", "limit", "negative_chunk_ids", "negative_tracking_ids", "positive_chunk_ids", "positive_tracking_ids", "slim_chunks"]
+    strategy: Optional[StrictStr] = Field(default=None, description="Strategy to use for recommendations, either \"average_vector\" or \"best_score\". The default is \"average_vector\". The \"average_vector\" strategy will construct a single average vector from the positive and negative samples then use it to perform a pseudo-search. The \"best_score\" strategy is more advanced and navigates the HNSW with a heuristic of picking edges where the point is closer to the positive samples than it is the negatives.")
+    __properties: ClassVar[List[str]] = ["filters", "limit", "negative_chunk_ids", "negative_tracking_ids", "positive_chunk_ids", "positive_tracking_ids", "slim_chunks", "strategy"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -111,14 +112,19 @@
             _dict['positive_tracking_ids'] = None
 
         # set to None if slim_chunks (nullable) is None
         # and model_fields_set contains the field
         if self.slim_chunks is None and "slim_chunks" in self.model_fields_set:
             _dict['slim_chunks'] = None
 
+        # set to None if strategy (nullable) is None
+        # and model_fields_set contains the field
+        if self.strategy is None and "strategy" in self.model_fields_set:
+            _dict['strategy'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of RecommendChunksRequest from a dict"""
         if obj is None:
             return None
@@ -129,12 +135,13 @@
         _obj = cls.model_validate({
             "filters": ChunkFilter.from_dict(obj["filters"]) if obj.get("filters") is not None else None,
             "limit": obj.get("limit"),
             "negative_chunk_ids": obj.get("negative_chunk_ids"),
             "negative_tracking_ids": obj.get("negative_tracking_ids"),
             "positive_chunk_ids": obj.get("positive_chunk_ids"),
             "positive_tracking_ids": obj.get("positive_tracking_ids"),
-            "slim_chunks": obj.get("slim_chunks")
+            "slim_chunks": obj.get("slim_chunks"),
+            "strategy": obj.get("strategy")
         })
         return _obj
```

## trieve_py_client/models/recommend_chunks_response_types.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/recommend_group_chunk_response_types.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/regenerate_message_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/return_queued_chunk.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/score_chunk_dto.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/score_slim_chunks.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_chunk_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -30,23 +30,22 @@
     SearchChunkData
     """ # noqa: E501
     date_bias: Optional[StrictBool] = Field(default=None, description="Set date_bias to true to bias search results towards more recent chunks. This will work best in hybrid search mode.")
     filters: Optional[ChunkFilter] = None
     get_collisions: Optional[StrictBool] = Field(default=None, description="Set get_collisions to true to get the collisions for each chunk. This will only apply if environment variable COLLISIONS_ENABLED is set to true.")
     highlight_delimiters: Optional[List[StrictStr]] = Field(default=None, description="Set highlight_delimiters to a list of strings to use as delimiters for highlighting. If not specified, this defaults to [\"?\", \",\", \".\", \"!\"].")
     highlight_results: Optional[StrictBool] = Field(default=None, description="Set highlight_results to true to highlight the results. If not specified, this defaults to true.")
-    page: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page of chunks to fetch. Each page is 10 chunks. Support for custom page size is coming soon.")
+    page: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page of chunks to fetch. Page is 1-indexed.")
     page_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page size is the number of chunks to fetch. This can be used to fetch more than 10 chunks at a time.")
     query: StrictStr = Field(description="Query is the search query. This can be any string. The query will be used to create an embedding vector and/or SPLADE vector which will be used to find the result set.")
-    quote_negated_words: Optional[StrictBool] = Field(default=None, description="Turn on quote words and negated words to search for exact phrases and exclude words from the search results. Default is false.")
     score_threshold: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="Set score_threshold to a float to filter out chunks with a score below the threshold.")
     search_type: StrictStr = Field(description="Can be either \"semantic\", \"fulltext\", or \"hybrid\". \"hybrid\" will pull in one page (10 chunks) of both semantic and full-text results then re-rank them using BAAI/bge-reranker-large. \"semantic\" will pull in one page (10 chunks) of the nearest cosine distant vectors. \"fulltext\" will pull in one page (10 chunks) of full-text results based on SPLADE.")
     slim_chunks: Optional[StrictBool] = Field(default=None, description="Set slim_chunks to true to avoid returning the content and chunk_html of the chunks. This is useful for when you want to reduce amount of data over the wire for latency improvement. Default is false.")
     use_weights: Optional[StrictBool] = Field(default=None, description="Set use_weights to true to use the weights of the chunks in the result set in order to sort them. If not specified, this defaults to true.")
-    __properties: ClassVar[List[str]] = ["date_bias", "filters", "get_collisions", "highlight_delimiters", "highlight_results", "page", "page_size", "query", "quote_negated_words", "score_threshold", "search_type", "slim_chunks", "use_weights"]
+    __properties: ClassVar[List[str]] = ["date_bias", "filters", "get_collisions", "highlight_delimiters", "highlight_results", "page", "page_size", "query", "score_threshold", "search_type", "slim_chunks", "use_weights"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -117,19 +116,14 @@
             _dict['page'] = None
 
         # set to None if page_size (nullable) is None
         # and model_fields_set contains the field
         if self.page_size is None and "page_size" in self.model_fields_set:
             _dict['page_size'] = None
 
-        # set to None if quote_negated_words (nullable) is None
-        # and model_fields_set contains the field
-        if self.quote_negated_words is None and "quote_negated_words" in self.model_fields_set:
-            _dict['quote_negated_words'] = None
-
         # set to None if score_threshold (nullable) is None
         # and model_fields_set contains the field
         if self.score_threshold is None and "score_threshold" in self.model_fields_set:
             _dict['score_threshold'] = None
 
         # set to None if slim_chunks (nullable) is None
         # and model_fields_set contains the field
@@ -157,15 +151,14 @@
             "filters": ChunkFilter.from_dict(obj["filters"]) if obj.get("filters") is not None else None,
             "get_collisions": obj.get("get_collisions"),
             "highlight_delimiters": obj.get("highlight_delimiters"),
             "highlight_results": obj.get("highlight_results"),
             "page": obj.get("page"),
             "page_size": obj.get("page_size"),
             "query": obj.get("query"),
-            "quote_negated_words": obj.get("quote_negated_words"),
             "score_threshold": obj.get("score_threshold"),
             "search_type": obj.get("search_type"),
             "slim_chunks": obj.get("slim_chunks"),
             "use_weights": obj.get("use_weights")
         })
         return _obj
```

## trieve_py_client/models/search_chunk_query_response_body.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_chunk_response_types.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_group_slim_chunks_result.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_groups_result.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_over_groups_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -27,25 +27,24 @@
 
 class SearchOverGroupsData(BaseModel):
     """
     SearchOverGroupsData
     """ # noqa: E501
     filters: Optional[ChunkFilter] = None
     get_collisions: Optional[StrictBool] = Field(default=None, description="Set get_collisions to true to get the collisions for each chunk. This will only apply if environment variable COLLISIONS_ENABLED is set to true.")
-    group_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = None
+    group_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Group_size is the number of chunks to fetch for each group. The default is 3. If a group has less than group_size chunks, all chunks will be returned. If this is set to a large number, we recommend setting slim_chunks to true to avoid returning the content and chunk_html of the chunks so as to lower the amount of time required for content download and serialization.")
     highlight_delimiters: Optional[List[StrictStr]] = Field(default=None, description="Set highlight_delimiters to a list of strings to use as delimiters for highlighting. If not specified, this defaults to [\"?\", \",\", \".\", \"!\"].")
     highlight_results: Optional[StrictBool] = Field(default=None, description="Set highlight_results to true to highlight the results. If not specified, this defaults to true.")
-    page: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page of chunks to fetch. Each page is 10 chunks. Support for custom page size is coming soon.")
-    page_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page size is the number of chunks to fetch. This can be used to fetch more than 10 chunks at a time.")
+    page: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page of group results to fetch. Page is 1-indexed.")
+    page_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="Page size is the number of group results to fetch. The default is 10.")
     query: StrictStr = Field(description="Query is the search query. This can be any string. The query will be used to create an embedding vector and/or SPLADE vector which will be used to find the result set.")
-    quote_negated_words: Optional[StrictBool] = Field(default=None, description="Turn on quote words and negated words to search for exact phrases and exclude words from the search results. Default is false.")
     score_threshold: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="Set score_threshold to a float to filter out chunks with a score below the threshold.")
     search_type: StrictStr = Field(description="Can be either \"semantic\", \"fulltext\", or \"hybrid\". \"hybrid\" will pull in one page (10 chunks) of both semantic and full-text results then re-rank them using BAAI/bge-reranker-large. \"semantic\" will pull in one page (10 chunks) of the nearest cosine distant vectors. \"fulltext\" will pull in one page (10 chunks) of full-text results based on SPLADE.")
     slim_chunks: Optional[StrictBool] = Field(default=None, description="Set slim_chunks to true to avoid returning the content and chunk_html of the chunks. This is useful for when you want to reduce amount of data over the wire for latency improvement. Default is false.")
-    __properties: ClassVar[List[str]] = ["filters", "get_collisions", "group_size", "highlight_delimiters", "highlight_results", "page", "page_size", "query", "quote_negated_words", "score_threshold", "search_type", "slim_chunks"]
+    __properties: ClassVar[List[str]] = ["filters", "get_collisions", "group_size", "highlight_delimiters", "highlight_results", "page", "page_size", "query", "score_threshold", "search_type", "slim_chunks"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -116,19 +115,14 @@
             _dict['page'] = None
 
         # set to None if page_size (nullable) is None
         # and model_fields_set contains the field
         if self.page_size is None and "page_size" in self.model_fields_set:
             _dict['page_size'] = None
 
-        # set to None if quote_negated_words (nullable) is None
-        # and model_fields_set contains the field
-        if self.quote_negated_words is None and "quote_negated_words" in self.model_fields_set:
-            _dict['quote_negated_words'] = None
-
         # set to None if score_threshold (nullable) is None
         # and model_fields_set contains the field
         if self.score_threshold is None and "score_threshold" in self.model_fields_set:
             _dict['score_threshold'] = None
 
         # set to None if slim_chunks (nullable) is None
         # and model_fields_set contains the field
@@ -151,15 +145,14 @@
             "get_collisions": obj.get("get_collisions"),
             "group_size": obj.get("group_size"),
             "highlight_delimiters": obj.get("highlight_delimiters"),
             "highlight_results": obj.get("highlight_results"),
             "page": obj.get("page"),
             "page_size": obj.get("page_size"),
             "query": obj.get("query"),
-            "quote_negated_words": obj.get("quote_negated_words"),
             "score_threshold": obj.get("score_threshold"),
             "search_type": obj.get("search_type"),
             "slim_chunks": obj.get("slim_chunks")
         })
         return _obj
```

## trieve_py_client/models/search_over_groups_response_body.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_over_groups_response_types.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_over_groups_slim_chunks_response_body.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_slim_chunk_query_response_body.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/search_within_group_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -31,23 +31,22 @@
     """ # noqa: E501
     date_bias: Optional[StrictBool] = Field(default=None, description="Set date_bias to true to bias search results towards more recent chunks. This will work best in hybrid search mode.")
     filters: Optional[ChunkFilter] = None
     group_id: Optional[StrictStr] = Field(default=None, description="Group specifies the group to search within. Results will only consist of chunks which are bookmarks within the specified group.")
     group_tracking_id: Optional[StrictStr] = Field(default=None, description="Group_tracking_id specifies the group to search within by tracking id. Results will only consist of chunks which are bookmarks within the specified group. If both group_id and group_tracking_id are provided, group_id will be used.")
     highlight_delimiters: Optional[List[StrictStr]] = Field(default=None, description="Set highlight_delimiters to a list of strings to use as delimiters for highlighting. If not specified, this defaults to [\"?\", \",\", \".\", \"!\"].")
     highlight_results: Optional[StrictBool] = Field(default=None, description="Set highlight_results to true to highlight the results. If not specified, this defaults to true.")
-    page: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The page of chunks to fetch. Each page is 10 chunks. Support for custom page size is coming soon.")
+    page: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The page of chunks to fetch. Page is 1-indexed.")
     page_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The page size is the number of chunks to fetch. This can be used to fetch more than 10 chunks at a time.")
     query: StrictStr = Field(description="The query is the search query. This can be any string. The query will be used to create an embedding vector and/or SPLADE vector which will be used to find the result set.")
-    quote_negated_words: Optional[StrictBool] = Field(default=None, description="Turn on quote words and negated words to search for exact phrases and exclude words from the search results. Default is false.")
     score_threshold: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="Set score_threshold to a float to filter out chunks with a score below the threshold.")
     search_type: StrictStr = Field(description="Search_type can be either \"semantic\", \"fulltext\", or \"hybrid\". \"hybrid\" will pull in one page (10 chunks) of both semantic and full-text results then re-rank them using BAAI/bge-reranker-large. \"semantic\" will pull in one page (10 chunks) of the nearest cosine distant vectors. \"fulltext\" will pull in one page (10 chunks) of full-text results based on SPLADE.")
     slim_chunks: Optional[StrictBool] = Field(default=None, description="Set slim_chunks to true to avoid returning the content and chunk_html of the chunks. This is useful for when you want to reduce amount of data over the wire for latency improvement. Default is false.")
     use_weights: Optional[StrictBool] = Field(default=None, description="Set use_weights to true to use the weights of the chunks in the result set in order to sort them. If not specified, this defaults to true.")
-    __properties: ClassVar[List[str]] = ["date_bias", "filters", "group_id", "group_tracking_id", "highlight_delimiters", "highlight_results", "page", "page_size", "query", "quote_negated_words", "score_threshold", "search_type", "slim_chunks", "use_weights"]
+    __properties: ClassVar[List[str]] = ["date_bias", "filters", "group_id", "group_tracking_id", "highlight_delimiters", "highlight_results", "page", "page_size", "query", "score_threshold", "search_type", "slim_chunks", "use_weights"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -123,19 +122,14 @@
             _dict['page'] = None
 
         # set to None if page_size (nullable) is None
         # and model_fields_set contains the field
         if self.page_size is None and "page_size" in self.model_fields_set:
             _dict['page_size'] = None
 
-        # set to None if quote_negated_words (nullable) is None
-        # and model_fields_set contains the field
-        if self.quote_negated_words is None and "quote_negated_words" in self.model_fields_set:
-            _dict['quote_negated_words'] = None
-
         # set to None if score_threshold (nullable) is None
         # and model_fields_set contains the field
         if self.score_threshold is None and "score_threshold" in self.model_fields_set:
             _dict['score_threshold'] = None
 
         # set to None if slim_chunks (nullable) is None
         # and model_fields_set contains the field
@@ -164,15 +158,14 @@
             "group_id": obj.get("group_id"),
             "group_tracking_id": obj.get("group_tracking_id"),
             "highlight_delimiters": obj.get("highlight_delimiters"),
             "highlight_results": obj.get("highlight_results"),
             "page": obj.get("page"),
             "page_size": obj.get("page_size"),
             "query": obj.get("query"),
-            "quote_negated_words": obj.get("quote_negated_words"),
             "score_threshold": obj.get("score_threshold"),
             "search_type": obj.get("search_type"),
             "slim_chunks": obj.get("slim_chunks"),
             "use_weights": obj.get("use_weights")
         })
         return _obj
```

## trieve_py_client/models/search_within_group_response_types.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/set_user_api_key_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/set_user_api_key_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/single_queued_chunk_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/slim_chunk_metadata.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/slim_group.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/slim_user.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/stripe_plan.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/suggested_queries_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/suggested_queries_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/topic.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/update_chunk_by_tracking_id_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/update_chunk_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/update_chunk_group_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -25,17 +25,19 @@
 
 class UpdateChunkGroupData(BaseModel):
     """
     UpdateChunkGroupData
     """ # noqa: E501
     description: Optional[StrictStr] = Field(default=None, description="Description to assign to the chunk_group. Convenience field for you to avoid having to remember what the group is for. If not provided, the description will not be updated.")
     group_id: Optional[StrictStr] = Field(default=None, description="Id of the chunk_group to update.")
+    metadata: Optional[Any] = Field(default=None, description="Optional metadata to assign to the chunk_group. This is a JSON object that can store any additional information you want to associate with the chunks inside of the chunk_group.")
     name: Optional[StrictStr] = Field(default=None, description="Name to assign to the chunk_group. Does not need to be unique. If not provided, the name will not be updated.")
+    tag_set: Optional[List[StrictStr]] = Field(default=None, description="Optional tags to assign to the chunk_group. This is a list of strings that can be used to categorize the chunks inside the chunk_group.")
     tracking_id: Optional[StrictStr] = Field(default=None, description="Tracking Id of the chunk_group to update.")
-    __properties: ClassVar[List[str]] = ["description", "group_id", "name", "tracking_id"]
+    __properties: ClassVar[List[str]] = ["description", "group_id", "metadata", "name", "tag_set", "tracking_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -78,19 +80,29 @@
             _dict['description'] = None
 
         # set to None if group_id (nullable) is None
         # and model_fields_set contains the field
         if self.group_id is None and "group_id" in self.model_fields_set:
             _dict['group_id'] = None
 
+        # set to None if metadata (nullable) is None
+        # and model_fields_set contains the field
+        if self.metadata is None and "metadata" in self.model_fields_set:
+            _dict['metadata'] = None
+
         # set to None if name (nullable) is None
         # and model_fields_set contains the field
         if self.name is None and "name" in self.model_fields_set:
             _dict['name'] = None
 
+        # set to None if tag_set (nullable) is None
+        # and model_fields_set contains the field
+        if self.tag_set is None and "tag_set" in self.model_fields_set:
+            _dict['tag_set'] = None
+
         # set to None if tracking_id (nullable) is None
         # and model_fields_set contains the field
         if self.tracking_id is None and "tracking_id" in self.model_fields_set:
             _dict['tracking_id'] = None
 
         return _dict
 
@@ -102,13 +114,15 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "description": obj.get("description"),
             "group_id": obj.get("group_id"),
+            "metadata": obj.get("metadata"),
             "name": obj.get("name"),
+            "tag_set": obj.get("tag_set"),
             "tracking_id": obj.get("tracking_id")
         })
         return _obj
```

## trieve_py_client/models/update_dataset_request.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/update_group_by_tracking_id_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,17 +24,19 @@
 from typing_extensions import Self
 
 class UpdateGroupByTrackingIDData(BaseModel):
     """
     UpdateGroupByTrackingIDData
     """ # noqa: E501
     description: Optional[StrictStr] = Field(default=None, description="Description to assign to the chunk_group. Convenience field for you to avoid having to remember what the group is for. If not provided, the description will not be updated.")
+    metadata: Optional[Any] = Field(default=None, description="Optional metadata to assign to the chunk_group. This is a JSON object that can store any additional information you want to associate with the chunks inside of the chunk_group.")
     name: Optional[StrictStr] = Field(default=None, description="Name to assign to the chunk_group. Does not need to be unique. If not provided, the name will not be updated.")
+    tag_set: Optional[List[StrictStr]] = Field(default=None, description="Optional tags to assign to the chunk_group. This is a list of strings that can be used to categorize the chunks inside the chunk_group.")
     tracking_id: StrictStr = Field(description="Tracking Id of the chunk_group to update.")
-    __properties: ClassVar[List[str]] = ["description", "name", "tracking_id"]
+    __properties: ClassVar[List[str]] = ["description", "metadata", "name", "tag_set", "tracking_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -72,31 +74,43 @@
             exclude_none=True,
         )
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
+        # set to None if metadata (nullable) is None
+        # and model_fields_set contains the field
+        if self.metadata is None and "metadata" in self.model_fields_set:
+            _dict['metadata'] = None
+
         # set to None if name (nullable) is None
         # and model_fields_set contains the field
         if self.name is None and "name" in self.model_fields_set:
             _dict['name'] = None
 
+        # set to None if tag_set (nullable) is None
+        # and model_fields_set contains the field
+        if self.tag_set is None and "tag_set" in self.model_fields_set:
+            _dict['tag_set'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of UpdateGroupByTrackingIDData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "description": obj.get("description"),
+            "metadata": obj.get("metadata"),
             "name": obj.get("name"),
+            "tag_set": obj.get("tag_set"),
             "tracking_id": obj.get("tracking_id")
         })
         return _obj
```

## trieve_py_client/models/update_organization_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/update_topic_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/update_user_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/upload_file_data.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/upload_file_result.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## trieve_py_client/models/user_organization.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## Comparing `trieve_python_client/models/reccomend_group_chunks_request.py` & `trieve_py_client/models/recommend_group_chunks_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Trieve API
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
 
-    The version of the OpenAPI document: 0.5.7
+    The version of the OpenAPI document: 0.6.0
     Contact: developers@trieve.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,31 +17,32 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from trieve_python_client.models.chunk_filter import ChunkFilter
+from trieve_py_client.models.chunk_filter import ChunkFilter
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ReccomendGroupChunksRequest(BaseModel):
+class RecommendGroupChunksRequest(BaseModel):
     """
-    ReccomendGroupChunksRequest
+    RecommendGroupChunksRequest
     """ # noqa: E501
     filters: Optional[ChunkFilter] = None
-    group_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The number of chunks to fetch for each group. This is the number of chunks which will be returned in the response for each group. The default is 10.")
+    group_size: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The number of chunks to fetch for each group. This is the number of chunks which will be returned in the response for each group. The default is 3. If this is set to a large number, we recommend setting slim_chunks to true to avoid returning the content and chunk_html of the chunks so as to reduce latency due to content download and serialization.")
     limit: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=None, description="The number of groups to return. This is the number of groups which will be returned in the response. The default is 10.")
-    negative_group_ids: Optional[List[StrictStr]] = Field(default=None, description="The  ids of the groups to be used as negative examples for the recommendation. The groups in this array will be used to filter out similar groups.")
-    negative_group_tracking_ids: Optional[List[StrictStr]] = Field(default=None, description="The  ids of the groups to be used as negative examples for the recommendation. The groups in this array will be used to filter out similar groups.")
-    positive_group_ids: Optional[List[StrictStr]] = Field(default=None, description="The  ids of the groups to be used as positive examples for the recommendation. The groups in this array will be used to find similar groups.")
-    positive_group_tracking_ids: Optional[List[StrictStr]] = Field(default=None, description="The  ids of the groups to be used as positive examples for the recommendation. The groups in this array will be used to find similar groups.")
+    negative_group_ids: Optional[List[StrictStr]] = Field(default=None, description="The ids of the groups to be used as negative examples for the recommendation. The groups in this array will be used to filter out similar groups.")
+    negative_group_tracking_ids: Optional[List[StrictStr]] = Field(default=None, description="The ids of the groups to be used as negative examples for the recommendation. The groups in this array will be used to filter out similar groups.")
+    positive_group_ids: Optional[List[StrictStr]] = Field(default=None, description="The ids of the groups to be used as positive examples for the recommendation. The groups in this array will be used to find similar groups.")
+    positive_group_tracking_ids: Optional[List[StrictStr]] = Field(default=None, description="The ids of the groups to be used as positive examples for the recommendation. The groups in this array will be used to find similar groups.")
     slim_chunks: Optional[StrictBool] = Field(default=None, description="Set slim_chunks to true to avoid returning the content and chunk_html of the chunks. This is useful for when you want to reduce amount of data over the wire for latency improvement. Default is false.")
-    __properties: ClassVar[List[str]] = ["filters", "group_size", "limit", "negative_group_ids", "negative_group_tracking_ids", "positive_group_ids", "positive_group_tracking_ids", "slim_chunks"]
+    strategy: Optional[StrictStr] = Field(default=None, description="Strategy to use for recommendations, either \"average_vector\" or \"best_score\". The default is \"average_vector\". The \"average_vector\" strategy will construct a single average vector from the positive and negative samples then use it to perform a pseudo-search. The \"best_score\" strategy is more advanced and navigates the HNSW with a heuristic of picking edges where the point is closer to the positive samples than it is the negatives.")
+    __properties: ClassVar[List[str]] = ["filters", "group_size", "limit", "negative_group_ids", "negative_group_tracking_ids", "positive_group_ids", "positive_group_tracking_ids", "slim_chunks", "strategy"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -53,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ReccomendGroupChunksRequest from a JSON string"""
+        """Create an instance of RecommendGroupChunksRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -117,31 +118,37 @@
             _dict['positive_group_tracking_ids'] = None
 
         # set to None if slim_chunks (nullable) is None
         # and model_fields_set contains the field
         if self.slim_chunks is None and "slim_chunks" in self.model_fields_set:
             _dict['slim_chunks'] = None
 
+        # set to None if strategy (nullable) is None
+        # and model_fields_set contains the field
+        if self.strategy is None and "strategy" in self.model_fields_set:
+            _dict['strategy'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ReccomendGroupChunksRequest from a dict"""
+        """Create an instance of RecommendGroupChunksRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "filters": ChunkFilter.from_dict(obj["filters"]) if obj.get("filters") is not None else None,
             "group_size": obj.get("group_size"),
             "limit": obj.get("limit"),
             "negative_group_ids": obj.get("negative_group_ids"),
             "negative_group_tracking_ids": obj.get("negative_group_tracking_ids"),
             "positive_group_ids": obj.get("positive_group_ids"),
             "positive_group_tracking_ids": obj.get("positive_group_tracking_ids"),
-            "slim_chunks": obj.get("slim_chunks")
+            "slim_chunks": obj.get("slim_chunks"),
+            "strategy": obj.get("strategy")
         })
         return _obj
```

## Comparing `trieve_py_client-0.5.7.dist-info/METADATA` & `trieve_py_client-0.6.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
-Name: trieve_py_client
-Version: 0.5.7
+Name: trieve-py-client
+Version: 0.6.0
 Summary: Trieve API
 Home-page: https://trieve.ai
 Author: Trieve Team
 Author-email: developers@trieve.ai
 License: BSL
 Keywords: OpenAPI,OpenAPI-Generator,Trieve API
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: urllib3 <2.1.0,>=1.25.3
+Requires-Dist: pydantic (>=2)
 Requires-Dist: python-dateutil
-Requires-Dist: pydantic >=2
-Requires-Dist: typing-extensions >=4.7.1
+Requires-Dist: typing-extensions (>=4.7.1)
+Requires-Dist: urllib3 (<2.1.0,>=1.25.3)
 
     Trieve OpenAPI Specification. This document describes all of the operations available through the Trieve API.
     
+
```

