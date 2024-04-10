# Comparing `tmp/trycourier-6.0.0b0.tar.gz` & `tmp/trycourier-6.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-6.0.0b0.tar", max compression
+gzip compressed data, was "trycourier-6.0.0b1.tar", max compression
```

## Comparing `trycourier-6.0.0b0.tar` & `trycourier-6.0.0b1.tar`

### file list

```diff
@@ -1,341 +1,351 @@
--rw-r--r--   0        0        0     1063 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/LICENSE
--rw-r--r--   0        0        0     5512 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/README.md
--rw-r--r--   0        0        0      406 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/pyproject.toml
--rw-r--r--   0        0        0    12519 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/__init__.py
--rw-r--r--   0        0        0     9148 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/client.py
--rw-r--r--   0        0        0      519 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/core/__init__.py
--rw-r--r--   0        0        0      426 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/core/api_error.py
--rw-r--r--   0        0        0     1649 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      159 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/environment.py
--rw-r--r--   0        0        0        0 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/py.typed
--rw-r--r--   0        0        0    12702 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/__init__.py
--rw-r--r--   0        0        0      751 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/__init__.py
--rw-r--r--   0        0        0    12869 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/client.py
--rw-r--r--   0        0        0     1100 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/audience.py
--rw-r--r--   0        0        0      991 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_list_response.py
--rw-r--r--   0        0        0      959 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_member.py
--rw-r--r--   0        0        0     1037 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_member_get_response.py
--rw-r--r--   0        0        0     1016 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_member_list_response.py
--rw-r--r--   0        0        0      921 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_update_response.py
--rw-r--r--   0        0        0      981 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/base_filter_config.py
--rw-r--r--   0        0        0     2042 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/comparison_operator.py
--rw-r--r--   0        0        0      249 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/filter.py
--rw-r--r--   0        0        0      255 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/filter_config.py
--rw-r--r--   0        0        0      438 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/logical_operator.py
--rw-r--r--   0        0        0     1069 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/nested_filter_config.py
--rw-r--r--   0        0        0      240 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/operator.py
--rw-r--r--   0        0        0     1236 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audiences/types/single_filter_config.py
--rw-r--r--   0        0        0      299 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/__init__.py
--rw-r--r--   0        0        0     4722 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/client.py
--rw-r--r--   0        0        0      453 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/__init__.py
--rw-r--r--   0        0        0      911 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/actor.py
--rw-r--r--   0        0        0     1135 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/audit_event.py
--rw-r--r--   0        0        0      973 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/get_audit_event_params.py
--rw-r--r--   0        0        0      899 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/list_audit_events_params.py
--rw-r--r--   0        0        0     1003 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/list_audit_events_response.py
--rw-r--r--   0        0        0      912 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/audit_events/types/target.py
--rw-r--r--   0        0        0      137 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/auth_tokens/__init__.py
--rw-r--r--   0        0        0     3818 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/auth_tokens/client.py
--rw-r--r--   0        0        0      152 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/auth_tokens/types/__init__.py
--rw-r--r--   0        0        0      895 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/auth_tokens/types/issue_token_response.py
--rw-r--r--   0        0        0     1063 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/__init__.py
--rw-r--r--   0        0        0     7746 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/client.py
--rw-r--r--   0        0        0     1593 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/__init__.py
--rw-r--r--   0        0        0     1001 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation.py
--rw-r--r--   0        0        0      932 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_ad_hoc_invoke_params.py
--rw-r--r--   0        0        0      956 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_cancel_step.py
--rw-r--r--   0        0        0      942 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_delay_step.py
--rw-r--r--   0        0        0     1093 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_params.py
--rw-r--r--   0        0        0      963 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_response.py
--rw-r--r--   0        0        0      930 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_step.py
--rw-r--r--   0        0        0     1044 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_template_params.py
--rw-r--r--   0        0        0     1073 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_run_context.py
--rw-r--r--   0        0        0     1114 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_send_list_step.py
--rw-r--r--   0        0        0     1168 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_send_step.py
--rw-r--r--   0        0        0      994 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_step.py
--rw-r--r--   0        0        0     1135 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_step_action.py
--rw-r--r--   0        0        0      723 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_step_option.py
--rw-r--r--   0        0        0     1096 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_update_profile_step.py
--rw-r--r--   0        0        0      973 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/automation_v_2_send_step.py
--rw-r--r--   0        0        0      805 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/merge_algorithm.py
--rw-r--r--   0        0        0      101 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/automations/types/profile.py
--rw-r--r--   0        0        0      419 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/__init__.py
--rw-r--r--   0        0        0    13748 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/client.py
--rw-r--r--   0        0        0      579 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/__init__.py
--rw-r--r--   0        0        0     1694 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand.py
--rw-r--r--   0        0        0      961 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand_colors.py
--rw-r--r--   0        0        0      983 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand_get_all_response.py
--rw-r--r--   0        0        0     1115 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand_parameters.py
--rw-r--r--   0        0        0     1051 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand_settings.py
--rw-r--r--   0        0        0      964 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand_snippet.py
--rw-r--r--   0        0        0      935 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brand_snippets.py
--rw-r--r--   0        0        0      978 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/brands/types/brands_response.py
--rw-r--r--   0        0        0     1059 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/__init__.py
--rw-r--r--   0        0        0    14009 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/client.py
--rw-r--r--   0        0        0     1603 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/__init__.py
--rw-r--r--   0        0        0      960 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_create_job_response.py
--rw-r--r--   0        0        0      955 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_params.py
--rw-r--r--   0        0        0      919 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_response.py
--rw-r--r--   0        0        0      993 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_users_params.py
--rw-r--r--   0        0        0     1042 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_users_response.py
--rw-r--r--   0        0        0      903 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_ingest_error.py
--rw-r--r--   0        0        0      975 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_ingest_users_params.py
--rw-r--r--   0        0        0      988 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_ingest_users_response.py
--rw-r--r--   0        0        0      805 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_job_status.py
--rw-r--r--   0        0        0      658 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_job_user_status.py
--rw-r--r--   0        0        0     1135 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_message_user_response.py
--rw-r--r--   0        0        0     1545 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_content_message.py
--rw-r--r--   0        0        0      967 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message.py
--rw-r--r--   0        0        0     1203 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message_user.py
--rw-r--r--   0        0        0     1766 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message_v_1.py
--rw-r--r--   0        0        0      310 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message_v_2.py
--rw-r--r--   0        0        0     1198 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_template_message.py
--rw-r--r--   0        0        0     1066 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/bulk/types/job_details.py
--rw-r--r--   0        0        0     1071 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/__init__.py
--rw-r--r--   0        0        0      527 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      290 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/already_exists_error.py
--rw-r--r--   0        0        0      278 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      269 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/conflict_error.py
--rw-r--r--   0        0        0      299 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/message_not_found_error.py
--rw-r--r--   0        0        0      270 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      298 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/errors/payment_required_error.py
--rw-r--r--   0        0        0     1119 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      903 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/already_exists.py
--rw-r--r--   0        0        0      900 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/bad_request.py
--rw-r--r--   0        0        0      949 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/base_error.py
--rw-r--r--   0        0        0     1112 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/channel_classification.py
--rw-r--r--   0        0        0      955 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/channel_preference.py
--rw-r--r--   0        0        0      898 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/conflict.py
--rw-r--r--   0        0        0      896 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/email.py
--rw-r--r--   0        0        0      905 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/message_not_found.py
--rw-r--r--   0        0        0      898 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/not_found.py
--rw-r--r--   0        0        0     1143 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/notification_preference_details.py
--rw-r--r--   0        0        0      230 2024-01-26 17:35:08.308188 trycourier-6.0.0b0/src/courier/resources/commons/types/notification_preferences.py
--rw-r--r--   0        0        0      899 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/commons/types/paging.py
--rw-r--r--   0        0        0      903 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/commons/types/payment_required.py
--rw-r--r--   0        0        0      679 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/commons/types/preference_status.py
--rw-r--r--   0        0        0     1044 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/commons/types/recipient_preferences.py
--rw-r--r--   0        0        0      896 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/commons/types/rule.py
--rw-r--r--   0        0        0      739 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/__init__.py
--rw-r--r--   0        0        0    26745 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/client.py
--rw-r--r--   0        0        0     1086 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/__init__.py
--rw-r--r--   0        0        0      943 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list.py
--rw-r--r--   0        0        0      905 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_find_by_recipient_id_params.py
--rw-r--r--   0        0        0      990 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_find_by_recipient_id_response.py
--rw-r--r--   0        0        0      928 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_all_params.py
--rw-r--r--   0        0        0      977 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_all_response.py
--rw-r--r--   0        0        0      904 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_subscriptions_params.py
--rw-r--r--   0        0        0     1052 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_subscriptions_response.py
--rw-r--r--   0        0        0      999 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_put_params.py
--rw-r--r--   0        0        0     1137 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/list_subscription_recipient.py
--rw-r--r--   0        0        0     1103 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/put_subscriptions_recipient.py
--rw-r--r--   0        0        0      991 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/lists/types/recipient_subscriptions_response.py
--rw-r--r--   0        0        0      527 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/__init__.py
--rw-r--r--   0        0        0    20617 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/client.py
--rw-r--r--   0        0        0      747 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/__init__.py
--rw-r--r--   0        0        0     1156 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/list_messages_response.py
--rw-r--r--   0        0        0     2788 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/message_details.py
--rw-r--r--   0        0        0      952 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/message_history_response.py
--rw-r--r--   0        0        0     2661 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/message_status.py
--rw-r--r--   0        0        0     1689 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/reason.py
--rw-r--r--   0        0        0     1222 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/render_output.py
--rw-r--r--   0        0        0     1046 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/render_output_response.py
--rw-r--r--   0        0        0     1049 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/rendered_message_block.py
--rw-r--r--   0        0        0     1454 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/messages/types/rendered_message_content.py
--rw-r--r--   0        0        0      985 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/__init__.py
--rw-r--r--   0        0        0    17458 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/client.py
--rw-r--r--   0        0        0     1463 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/__init__.py
--rw-r--r--   0        0        0     1000 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/base_check.py
--rw-r--r--   0        0        0     1420 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/block_type.py
--rw-r--r--   0        0        0      825 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/check.py
--rw-r--r--   0        0        0      639 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/check_status.py
--rw-r--r--   0        0        0     1147 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/message_routing.py
--rw-r--r--   0        0        0      183 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/message_routing_channel.py
--rw-r--r--   0        0        0      469 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/message_routing_method.py
--rw-r--r--   0        0        0      961 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification.py
--rw-r--r--   0        0        0     1201 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_block.py
--rw-r--r--   0        0        0     1143 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_channel.py
--rw-r--r--   0        0        0      937 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_channel_content.py
--rw-r--r--   0        0        0      224 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_content.py
--rw-r--r--   0        0        0      941 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_content_hierarchy.py
--rw-r--r--   0        0        0     1138 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_get_content_response.py
--rw-r--r--   0        0        0     1009 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_list_response.py
--rw-r--r--   0        0        0      928 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/submission_checks_get_response.py
--rw-r--r--   0        0        0      932 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/notifications/types/submission_checks_replace_response.py
--rw-r--r--   0        0        0     1415 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/__init__.py
--rw-r--r--   0        0        0    20924 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/client.py
--rw-r--r--   0        0        0     2155 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/__init__.py
--rw-r--r--   0        0        0      967 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/address.py
--rw-r--r--   0        0        0     1035 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/airship_profile.py
--rw-r--r--   0        0        0      887 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/airship_profile_audience.py
--rw-r--r--   0        0        0      950 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/delete_list_subscription_response.py
--rw-r--r--   0        0        0      104 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/device_type.py
--rw-r--r--   0        0        0      232 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/discord.py
--rw-r--r--   0        0        0      193 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/expo.py
--rw-r--r--   0        0        0     1356 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/get_list_subscriptions_list.py
--rw-r--r--   0        0        0     1102 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/get_list_subscriptions_response.py
--rw-r--r--   0        0        0     1024 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/intercom.py
--rw-r--r--   0        0        0      875 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/intercome_recipient.py
--rw-r--r--   0        0        0      940 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/merge_profile_response.py
--rw-r--r--   0        0        0      257 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/ms_teams.py
--rw-r--r--   0        0        0      915 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/multiple_tokens.py
--rw-r--r--   0        0        0      971 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/profile_get_parameters.py
--rw-r--r--   0        0        0     1032 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/profile_get_response.py
--rw-r--r--   0        0        0      942 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/replace_profile_response.py
--rw-r--r--   0        0        0      879 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/send_direct_message.py
--rw-r--r--   0        0        0      878 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/send_to_channel.py
--rw-r--r--   0        0        0      930 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/send_to_ms_teams_channel.py
--rw-r--r--   0        0        0      919 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/send_to_ms_teams_user.py
--rw-r--r--   0        0        0      955 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/snooze_rule.py
--rw-r--r--   0        0        0      335 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/snooze_rule_type.py
--rw-r--r--   0        0        0     1012 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/subscribe_to_lists_request.py
--rw-r--r--   0        0        0     1101 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/subscribe_to_lists_request_list_object.py
--rw-r--r--   0        0        0      944 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/subscribe_to_lists_response.py
--rw-r--r--   0        0        0      865 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/token.py
--rw-r--r--   0        0        0     1969 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/profiles/types/user_profile.py
--rw-r--r--   0        0        0     3925 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/__init__.py
--rw-r--r--   0        0        0     5870 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/__init__.py
--rw-r--r--   0        0        0      122 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/attachment.py
--rw-r--r--   0        0        0     1102 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/audience_filter.py
--rw-r--r--   0        0        0     1210 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/audience_recipient.py
--rw-r--r--   0        0        0     2974 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/base_message.py
--rw-r--r--   0        0        0      876 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/base_social_presence.py
--rw-r--r--   0        0        0     1302 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/brand_settings_email.py
--rw-r--r--   0        0        0     1564 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/brand_settings_in_app.py
--rw-r--r--   0        0        0     1303 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/brand_settings_social_presence.py
--rw-r--r--   0        0        0     1234 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/brand_template.py
--rw-r--r--   0        0        0     1158 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/brand_template_override.py
--rw-r--r--   0        0        0     2459 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/channel.py
--rw-r--r--   0        0        0      911 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/channel_metadata.py
--rw-r--r--   0        0        0      667 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/channel_source.py
--rw-r--r--   0        0        0      252 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/content.py
--rw-r--r--   0        0        0     1666 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/content_message.py
--rw-r--r--   0        0        0      800 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/criteria.py
--rw-r--r--   0        0        0      943 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/delay.py
--rw-r--r--   0        0        0     2040 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_action_node.py
--rw-r--r--   0        0        0     1076 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_base_node.py
--rw-r--r--   0        0        0     2603 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_channel_node.py
--rw-r--r--   0        0        0     1058 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_content.py
--rw-r--r--   0        0        0     1193 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_content_sugar.py
--rw-r--r--   0        0        0     1161 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_divider_node.py
--rw-r--r--   0        0        0     1430 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_group_node.py
--rw-r--r--   0        0        0     1592 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_image_node.py
--rw-r--r--   0        0        0     1367 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_meta_node.py
--rw-r--r--   0        0        0     2827 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_node.py
--rw-r--r--   0        0        0     1649 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_quote_node.py
--rw-r--r--   0        0        0     2391 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/elemental_text_node.py
--rw-r--r--   0        0        0     1027 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/email_footer.py
--rw-r--r--   0        0        0     1001 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/email_head.py
--rw-r--r--   0        0        0     1095 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/email_header.py
--rw-r--r--   0        0        0      119 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/expires_in_type.py
--rw-r--r--   0        0        0     1272 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/expiry.py
--rw-r--r--   0        0        0      468 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/i_action_button_style.py
--rw-r--r--   0        0        0      730 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/i_alignment.py
--rw-r--r--   0        0        0      160 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/i_preferences.py
--rw-r--r--   0        0        0     1103 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/i_profile_preferences.py
--rw-r--r--   0        0        0      915 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/icons.py
--rw-r--r--   0        0        0      745 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/in_app_placement.py
--rw-r--r--   0        0        0      906 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/invalid_list_pattern_recipient.py
--rw-r--r--   0        0        0      904 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/invalid_list_recipient.py
--rw-r--r--   0        0        0      904 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/invalid_user_recipient.py
--rw-r--r--   0        0        0     1098 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/list_filter.py
--rw-r--r--   0        0        0      986 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/list_pattern_recipient.py
--rw-r--r--   0        0        0      868 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/list_pattern_recipient_type.py
--rw-r--r--   0        0        0     1042 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/list_recipient.py
--rw-r--r--   0        0        0      861 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/list_recipient_type.py
--rw-r--r--   0        0        0      868 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/locale.py
--rw-r--r--   0        0        0      160 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/locales.py
--rw-r--r--   0        0        0      912 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/logo.py
--rw-r--r--   0        0        0      227 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message.py
--rw-r--r--   0        0        0     1417 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_channel_email_override.py
--rw-r--r--   0        0        0      154 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_channels.py
--rw-r--r--   0        0        0     1173 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_context.py
--rw-r--r--   0        0        0      123 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_data.py
--rw-r--r--   0        0        0     1708 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_metadata.py
--rw-r--r--   0        0        0      196 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_providers.py
--rw-r--r--   0        0        0     1478 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_providers_type.py
--rw-r--r--   0        0        0      181 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/message_recipient.py
--rw-r--r--   0        0        0      904 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/metadata.py
--rw-r--r--   0        0        0      708 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/override.py
--rw-r--r--   0        0        0     1257 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/preference.py
--rw-r--r--   0        0        0      975 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/preferences.py
--rw-r--r--   0        0        0      368 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/recipient.py
--rw-r--r--   0        0        0     1536 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/routing.py
--rw-r--r--   0        0        0      289 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/routing_channel.py
--rw-r--r--   0        0        0      448 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/routing_method.py
--rw-r--r--   0        0        0     1229 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/routing_strategy_channel.py
--rw-r--r--   0        0        0     1099 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/routing_strategy_provider.py
--rw-r--r--   0        0        0      677 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/rule_type.py
--rw-r--r--   0        0        0     1332 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/template_message.py
--rw-r--r--   0        0        0      601 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/text_align.py
--rw-r--r--   0        0        0      713 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/text_style.py
--rw-r--r--   0        0        0     1099 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/timeout.py
--rw-r--r--   0        0        0      922 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/timeouts.py
--rw-r--r--   0        0        0      876 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/tracking_override.py
--rw-r--r--   0        0        0     1966 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/user_recipient.py
--rw-r--r--   0        0        0      861 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/user_recipient_type.py
--rw-r--r--   0        0        0     1014 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/utm.py
--rw-r--r--   0        0        0     1055 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/send/types/widget_background.py
--rw-r--r--   0        0        0      411 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/__init__.py
--rw-r--r--   0        0        0     2821 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/client.py
--rw-r--r--   0        0        0      564 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/__init__.py
--rw-r--r--   0        0        0       89 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/channel_identifier.py
--rw-r--r--   0        0        0     1101 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/list_templates_response.py
--rw-r--r--   0        0        0     1764 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/notification_templates.py
--rw-r--r--   0        0        0     1378 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/routing_strategy.py
--rw-r--r--   0        0        0      472 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/routing_strategy_method.py
--rw-r--r--   0        0        0      909 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/tag.py
--rw-r--r--   0        0        0      991 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/templates/types/tag_data.py
--rw-r--r--   0        0        0      383 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/__init__.py
--rw-r--r--   0        0        0    11221 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/client.py
--rw-r--r--   0        0        0      519 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/__init__.py
--rw-r--r--   0        0        0      955 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/default_preferences.py
--rw-r--r--   0        0        0     1014 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/subscription_topic.py
--rw-r--r--   0        0        0      707 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/subscription_topic_status.py
--rw-r--r--   0        0        0      110 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/template_property.py
--rw-r--r--   0        0        0     1844 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/tenant.py
--rw-r--r--   0        0        0     1744 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/tenants/types/tenant_list_response.py
--rw-r--r--   0        0        0       65 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/translations/__init__.py
--rw-r--r--   0        0        0     5527 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/translations/client.py
--rw-r--r--   0        0        0     1315 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/__init__.py
--rw-r--r--   0        0        0     1098 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/client.py
--rw-r--r--   0        0        0     1350 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/__init__.py
--rw-r--r--   0        0        0      353 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/__init__.py
--rw-r--r--   0        0        0    10433 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/client.py
--rw-r--r--   0        0        0      473 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/__init__.py
--rw-r--r--   0        0        0     1351 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/topic_preference.py
--rw-r--r--   0        0        0      946 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/user_preferences_get_response.py
--rw-r--r--   0        0        0     1101 2024-01-26 17:35:08.312188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/user_preferences_list_response.py
--rw-r--r--   0        0        0      893 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/user_preferences_update_response.py
--rw-r--r--   0        0        0      277 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/__init__.py
--rw-r--r--   0        0        0    10718 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/client.py
--rw-r--r--   0        0        0      392 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/__init__.py
--rw-r--r--   0        0        0     1279 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/add_user_to_single_tenants_params_profile.py
--rw-r--r--   0        0        0     1766 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/list_tenants_for_user_response.py
--rw-r--r--   0        0        0     1004 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/user_tenant_association.py
--rw-r--r--   0        0        0      765 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/__init__.py
--rw-r--r--   0        0        0    12257 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/client.py
--rw-r--r--   0        0        0     1135 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/__init__.py
--rw-r--r--   0        0        0      898 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/delete_user_token_opts.py
--rw-r--r--   0        0        0     1459 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/device.py
--rw-r--r--   0        0        0      117 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/expiry_date.py
--rw-r--r--   0        0        0      161 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_all_tokens_response.py
--rw-r--r--   0        0        0      895 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_user_token_opts.py
--rw-r--r--   0        0        0     1122 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_user_token_response.py
--rw-r--r--   0        0        0      881 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_user_tokens_opts.py
--rw-r--r--   0        0        0      964 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/patch_op.py
--rw-r--r--   0        0        0     1134 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/patch_operation.py
--rw-r--r--   0        0        0      948 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/patch_user_token_opts.py
--rw-r--r--   0        0        0      780 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/provider_key.py
--rw-r--r--   0        0        0      935 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/put_user_token_opts.py
--rw-r--r--   0        0        0      950 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/put_user_tokens_opts.py
--rw-r--r--   0        0        0      770 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/token_status.py
--rw-r--r--   0        0        0     1223 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/tracking.py
--rw-r--r--   0        0        0     1752 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/user_token.py
--rw-r--r--   0        0        0      155 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/types/__init__.py
--rw-r--r--   0        0        0     1669 2024-01-26 17:35:08.316188 trycourier-6.0.0b0/src/courier/types/send_message_response.py
--rw-r--r--   0        0        0     6021 1970-01-01 00:00:00.000000 trycourier-6.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/LICENSE
+-rw-r--r--   0        0        0     5507 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/README.md
+-rw-r--r--   0        0        0      406 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0    13103 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/__init__.py
+-rw-r--r--   0        0        0     9148 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/client.py
+-rw-r--r--   0        0        0      519 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/api_error.py
+-rw-r--r--   0        0        0     1649 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      159 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/environment.py
+-rw-r--r--   0        0        0        0 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/py.typed
+-rw-r--r--   0        0        0    13286 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/__init__.py
+-rw-r--r--   0        0        0      751 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/__init__.py
+-rw-r--r--   0        0        0    12869 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/client.py
+-rw-r--r--   0        0        0     1100 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/__init__.py
+-rw-r--r--   0        0        0     1186 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience.py
+-rw-r--r--   0        0        0      991 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_list_response.py
+-rw-r--r--   0        0        0      959 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member.py
+-rw-r--r--   0        0        0     1037 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_get_response.py
+-rw-r--r--   0        0        0     1016 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_list_response.py
+-rw-r--r--   0        0        0      921 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_update_response.py
+-rw-r--r--   0        0        0      981 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/base_filter_config.py
+-rw-r--r--   0        0        0     2042 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/comparison_operator.py
+-rw-r--r--   0        0        0      249 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/filter.py
+-rw-r--r--   0        0        0      255 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/filter_config.py
+-rw-r--r--   0        0        0      438 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/logical_operator.py
+-rw-r--r--   0        0        0     1069 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/nested_filter_config.py
+-rw-r--r--   0        0        0      240 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/operator.py
+-rw-r--r--   0        0        0     1236 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/single_filter_config.py
+-rw-r--r--   0        0        0      299 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/__init__.py
+-rw-r--r--   0        0        0     4722 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/client.py
+-rw-r--r--   0        0        0      453 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/__init__.py
+-rw-r--r--   0        0        0      911 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/actor.py
+-rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/audit_event.py
+-rw-r--r--   0        0        0      973 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/get_audit_event_params.py
+-rw-r--r--   0        0        0      899 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_params.py
+-rw-r--r--   0        0        0     1003 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_response.py
+-rw-r--r--   0        0        0      912 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/target.py
+-rw-r--r--   0        0        0      137 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/__init__.py
+-rw-r--r--   0        0        0     3818 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/client.py
+-rw-r--r--   0        0        0      152 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/types/__init__.py
+-rw-r--r--   0        0        0      895 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/types/issue_token_response.py
+-rw-r--r--   0        0        0     1063 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/__init__.py
+-rw-r--r--   0        0        0     7746 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/client.py
+-rw-r--r--   0        0        0     1593 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/__init__.py
+-rw-r--r--   0        0        0     1001 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation.py
+-rw-r--r--   0        0        0      932 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_ad_hoc_invoke_params.py
+-rw-r--r--   0        0        0      956 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_cancel_step.py
+-rw-r--r--   0        0        0      942 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_delay_step.py
+-rw-r--r--   0        0        0     1093 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_params.py
+-rw-r--r--   0        0        0      963 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_response.py
+-rw-r--r--   0        0        0      930 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_step.py
+-rw-r--r--   0        0        0     1044 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_template_params.py
+-rw-r--r--   0        0        0     1073 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_run_context.py
+-rw-r--r--   0        0        0     1114 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_list_step.py
+-rw-r--r--   0        0        0     1168 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_step.py
+-rw-r--r--   0        0        0      994 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step.py
+-rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_action.py
+-rw-r--r--   0        0        0      723 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_option.py
+-rw-r--r--   0        0        0     1096 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_update_profile_step.py
+-rw-r--r--   0        0        0      973 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_v_2_send_step.py
+-rw-r--r--   0        0        0      805 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/merge_algorithm.py
+-rw-r--r--   0        0        0      101 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/profile.py
+-rw-r--r--   0        0        0      419 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/__init__.py
+-rw-r--r--   0        0        0    13748 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/client.py
+-rw-r--r--   0        0        0      579 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/__init__.py
+-rw-r--r--   0        0        0     1694 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand.py
+-rw-r--r--   0        0        0      961 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_colors.py
+-rw-r--r--   0        0        0      983 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_get_all_response.py
+-rw-r--r--   0        0        0     1115 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_parameters.py
+-rw-r--r--   0        0        0     1051 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_settings.py
+-rw-r--r--   0        0        0      964 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippet.py
+-rw-r--r--   0        0        0      935 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippets.py
+-rw-r--r--   0        0        0      978 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brands_response.py
+-rw-r--r--   0        0        0     1059 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/__init__.py
+-rw-r--r--   0        0        0    14009 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/client.py
+-rw-r--r--   0        0        0     1603 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/__init__.py
+-rw-r--r--   0        0        0      960 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_create_job_response.py
+-rw-r--r--   0        0        0      955 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_params.py
+-rw-r--r--   0        0        0      919 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_response.py
+-rw-r--r--   0        0        0      993 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_params.py
+-rw-r--r--   0        0        0     1042 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_response.py
+-rw-r--r--   0        0        0      903 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_error.py
+-rw-r--r--   0        0        0      975 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_params.py
+-rw-r--r--   0        0        0      988 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_response.py
+-rw-r--r--   0        0        0      805 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_job_status.py
+-rw-r--r--   0        0        0      658 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_job_user_status.py
+-rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_message_user_response.py
+-rw-r--r--   0        0        0     1545 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_content_message.py
+-rw-r--r--   0        0        0      967 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message.py
+-rw-r--r--   0        0        0     1203 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_user.py
+-rw-r--r--   0        0        0     1766 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_v_1.py
+-rw-r--r--   0        0        0      310 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_v_2.py
+-rw-r--r--   0        0        0     1198 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_template_message.py
+-rw-r--r--   0        0        0     1066 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/job_details.py
+-rw-r--r--   0        0        0     1127 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/__init__.py
+-rw-r--r--   0        0        0      527 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      290 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/already_exists_error.py
+-rw-r--r--   0        0        0      278 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      269 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/conflict_error.py
+-rw-r--r--   0        0        0      299 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/message_not_found_error.py
+-rw-r--r--   0        0        0      270 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      298 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/payment_required_error.py
+-rw-r--r--   0        0        0     1207 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      903 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/already_exists.py
+-rw-r--r--   0        0        0      900 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/bad_request.py
+-rw-r--r--   0        0        0      949 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/base_error.py
+-rw-r--r--   0        0        0     1112 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/channel_classification.py
+-rw-r--r--   0        0        0      955 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/channel_preference.py
+-rw-r--r--   0        0        0      898 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/conflict.py
+-rw-r--r--   0        0        0      896 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/email.py
+-rw-r--r--   0        0        0      905 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/message_not_found.py
+-rw-r--r--   0        0        0      898 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/not_found.py
+-rw-r--r--   0        0        0     1143 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/notification_preference_details.py
+-rw-r--r--   0        0        0      230 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/notification_preferences.py
+-rw-r--r--   0        0        0      899 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/paging.py
+-rw-r--r--   0        0        0      903 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/payment_required.py
+-rw-r--r--   0        0        0      679 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/preference_status.py
+-rw-r--r--   0        0        0     1044 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/recipient_preferences.py
+-rw-r--r--   0        0        0      896 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/rule.py
+-rw-r--r--   0        0        0     1182 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/user_tenant_association.py
+-rw-r--r--   0        0        0      739 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/__init__.py
+-rw-r--r--   0        0        0    26745 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/client.py
+-rw-r--r--   0        0        0     1086 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/__init__.py
+-rw-r--r--   0        0        0      943 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list.py
+-rw-r--r--   0        0        0      905 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_params.py
+-rw-r--r--   0        0        0      990 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_response.py
+-rw-r--r--   0        0        0      928 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_params.py
+-rw-r--r--   0        0        0      977 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_response.py
+-rw-r--r--   0        0        0      904 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_params.py
+-rw-r--r--   0        0        0     1052 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_response.py
+-rw-r--r--   0        0        0      999 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_put_params.py
+-rw-r--r--   0        0        0     1137 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_subscription_recipient.py
+-rw-r--r--   0        0        0     1103 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/put_subscriptions_recipient.py
+-rw-r--r--   0        0        0      991 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/recipient_subscriptions_response.py
+-rw-r--r--   0        0        0      527 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/__init__.py
+-rw-r--r--   0        0        0    20617 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/client.py
+-rw-r--r--   0        0        0      747 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/__init__.py
+-rw-r--r--   0        0        0     1156 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/list_messages_response.py
+-rw-r--r--   0        0        0     2788 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/message_details.py
+-rw-r--r--   0        0        0      952 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/message_history_response.py
+-rw-r--r--   0        0        0     2661 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/message_status.py
+-rw-r--r--   0        0        0     1689 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/reason.py
+-rw-r--r--   0        0        0     1222 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/render_output.py
+-rw-r--r--   0        0        0     1046 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/render_output_response.py
+-rw-r--r--   0        0        0     1049 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_block.py
+-rw-r--r--   0        0        0     1454 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_content.py
+-rw-r--r--   0        0        0      985 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/__init__.py
+-rw-r--r--   0        0        0    17458 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/client.py
+-rw-r--r--   0        0        0     1463 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/__init__.py
+-rw-r--r--   0        0        0     1000 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/base_check.py
+-rw-r--r--   0        0        0     1420 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/block_type.py
+-rw-r--r--   0        0        0      825 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/check.py
+-rw-r--r--   0        0        0      639 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/check_status.py
+-rw-r--r--   0        0        0     1147 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing.py
+-rw-r--r--   0        0        0      183 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing_channel.py
+-rw-r--r--   0        0        0      469 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing_method.py
+-rw-r--r--   0        0        0      961 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification.py
+-rw-r--r--   0        0        0     1201 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_block.py
+-rw-r--r--   0        0        0     1143 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel.py
+-rw-r--r--   0        0        0      937 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel_content.py
+-rw-r--r--   0        0        0      224 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_content.py
+-rw-r--r--   0        0        0      941 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_content_hierarchy.py
+-rw-r--r--   0        0        0     1138 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_get_content_response.py
+-rw-r--r--   0        0        0     1009 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_list_response.py
+-rw-r--r--   0        0        0      928 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_get_response.py
+-rw-r--r--   0        0        0      932 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_replace_response.py
+-rw-r--r--   0        0        0     1877 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/__init__.py
+-rw-r--r--   0        0        0    20924 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/client.py
+-rw-r--r--   0        0        0     2897 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/__init__.py
+-rw-r--r--   0        0        0      967 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/address.py
+-rw-r--r--   0        0        0     1035 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile.py
+-rw-r--r--   0        0        0      887 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile_audience.py
+-rw-r--r--   0        0        0      950 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/delete_list_subscription_response.py
+-rw-r--r--   0        0        0      104 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/device_type.py
+-rw-r--r--   0        0        0      232 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/discord.py
+-rw-r--r--   0        0        0      193 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/expo.py
+-rw-r--r--   0        0        0     1356 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_list.py
+-rw-r--r--   0        0        0     1102 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1021 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom.py
+-rw-r--r--   0        0        0      874 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom_recipient.py
+-rw-r--r--   0        0        0      940 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/merge_profile_response.py
+-rw-r--r--   0        0        0      566 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams.py
+-rw-r--r--   0        0        0      906 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams_base_properties.py
+-rw-r--r--   0        0        0      915 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/multiple_tokens.py
+-rw-r--r--   0        0        0      971 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_parameters.py
+-rw-r--r--   0        0        0     1032 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_response.py
+-rw-r--r--   0        0        0      942 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/replace_profile_response.py
+-rw-r--r--   0        0        0      879 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_direct_message.py
+-rw-r--r--   0        0        0      878 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_channel.py
+-rw-r--r--   0        0        0      883 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_channel_id.py
+-rw-r--r--   0        0        0      904 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_channel_name.py
+-rw-r--r--   0        0        0      893 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_conversation_id.py
+-rw-r--r--   0        0        0      874 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_email.py
+-rw-r--r--   0        0        0      877 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_user_id.py
+-rw-r--r--   0        0        0      869 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_channel.py
+-rw-r--r--   0        0        0      865 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_email.py
+-rw-r--r--   0        0        0      868 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_user_id.py
+-rw-r--r--   0        0        0      316 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/slack.py
+-rw-r--r--   0        0        0      886 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/slack_base_properties.py
+-rw-r--r--   0        0        0      955 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/snooze_rule.py
+-rw-r--r--   0        0        0      335 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/snooze_rule_type.py
+-rw-r--r--   0        0        0     1012 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request.py
+-rw-r--r--   0        0        0     1101 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request_list_object.py
+-rw-r--r--   0        0        0      944 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_response.py
+-rw-r--r--   0        0        0      865 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/token.py
+-rw-r--r--   0        0        0     2011 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/user_profile.py
+-rw-r--r--   0        0        0     3925 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/__init__.py
+-rw-r--r--   0        0        0     5870 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/__init__.py
+-rw-r--r--   0        0        0      122 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/attachment.py
+-rw-r--r--   0        0        0     1102 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/audience_filter.py
+-rw-r--r--   0        0        0     1210 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/audience_recipient.py
+-rw-r--r--   0        0        0     2974 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/base_message.py
+-rw-r--r--   0        0        0      876 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/base_social_presence.py
+-rw-r--r--   0        0        0     1302 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_email.py
+-rw-r--r--   0        0        0     1564 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_in_app.py
+-rw-r--r--   0        0        0     1303 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_social_presence.py
+-rw-r--r--   0        0        0     1234 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_template.py
+-rw-r--r--   0        0        0     1158 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_template_override.py
+-rw-r--r--   0        0        0     2459 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/channel.py
+-rw-r--r--   0        0        0      911 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/channel_metadata.py
+-rw-r--r--   0        0        0      667 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/channel_source.py
+-rw-r--r--   0        0        0      252 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/content.py
+-rw-r--r--   0        0        0     1666 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/content_message.py
+-rw-r--r--   0        0        0      800 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/criteria.py
+-rw-r--r--   0        0        0      943 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/delay.py
+-rw-r--r--   0        0        0     2040 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_action_node.py
+-rw-r--r--   0        0        0     1076 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_base_node.py
+-rw-r--r--   0        0        0     2603 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_channel_node.py
+-rw-r--r--   0        0        0     1058 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content.py
+-rw-r--r--   0        0        0     1193 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content_sugar.py
+-rw-r--r--   0        0        0     1161 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_divider_node.py
+-rw-r--r--   0        0        0     1430 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_group_node.py
+-rw-r--r--   0        0        0     1592 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_image_node.py
+-rw-r--r--   0        0        0     1367 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_meta_node.py
+-rw-r--r--   0        0        0     2827 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_node.py
+-rw-r--r--   0        0        0     1649 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_quote_node.py
+-rw-r--r--   0        0        0     2391 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_text_node.py
+-rw-r--r--   0        0        0     1027 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/email_footer.py
+-rw-r--r--   0        0        0     1001 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/email_head.py
+-rw-r--r--   0        0        0     1095 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/email_header.py
+-rw-r--r--   0        0        0      119 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/expires_in_type.py
+-rw-r--r--   0        0        0     1272 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/expiry.py
+-rw-r--r--   0        0        0      468 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_action_button_style.py
+-rw-r--r--   0        0        0      730 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_alignment.py
+-rw-r--r--   0        0        0      160 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_preferences.py
+-rw-r--r--   0        0        0     1103 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_profile_preferences.py
+-rw-r--r--   0        0        0      915 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/icons.py
+-rw-r--r--   0        0        0      745 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/in_app_placement.py
+-rw-r--r--   0        0        0      906 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_pattern_recipient.py
+-rw-r--r--   0        0        0      904 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_recipient.py
+-rw-r--r--   0        0        0      904 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/invalid_user_recipient.py
+-rw-r--r--   0        0        0     1098 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_filter.py
+-rw-r--r--   0        0        0      986 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient.py
+-rw-r--r--   0        0        0      868 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient_type.py
+-rw-r--r--   0        0        0     1042 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient.py
+-rw-r--r--   0        0        0      861 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient_type.py
+-rw-r--r--   0        0        0      868 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/locale.py
+-rw-r--r--   0        0        0      160 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/locales.py
+-rw-r--r--   0        0        0      912 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/logo.py
+-rw-r--r--   0        0        0      227 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message.py
+-rw-r--r--   0        0        0     1417 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_channel_email_override.py
+-rw-r--r--   0        0        0      154 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_channels.py
+-rw-r--r--   0        0        0     1173 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_context.py
+-rw-r--r--   0        0        0      123 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_data.py
+-rw-r--r--   0        0        0     1708 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_metadata.py
+-rw-r--r--   0        0        0      196 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_providers.py
+-rw-r--r--   0        0        0     1478 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_providers_type.py
+-rw-r--r--   0        0        0      181 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_recipient.py
+-rw-r--r--   0        0        0      904 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/metadata.py
+-rw-r--r--   0        0        0      708 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/override.py
+-rw-r--r--   0        0        0     1257 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/preference.py
+-rw-r--r--   0        0        0      975 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/preferences.py
+-rw-r--r--   0        0        0      473 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/recipient.py
+-rw-r--r--   0        0        0     1536 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing.py
+-rw-r--r--   0        0        0      289 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_channel.py
+-rw-r--r--   0        0        0      448 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_method.py
+-rw-r--r--   0        0        0     1229 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_channel.py
+-rw-r--r--   0        0        0     1099 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_provider.py
+-rw-r--r--   0        0        0      677 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/rule_type.py
+-rw-r--r--   0        0        0     1332 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/template_message.py
+-rw-r--r--   0        0        0      601 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/text_align.py
+-rw-r--r--   0        0        0      713 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/text_style.py
+-rw-r--r--   0        0        0     1099 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/timeout.py
+-rw-r--r--   0        0        0      922 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/timeouts.py
+-rw-r--r--   0        0        0      876 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/tracking_override.py
+-rw-r--r--   0        0        0     1966 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient.py
+-rw-r--r--   0        0        0      861 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient_type.py
+-rw-r--r--   0        0        0     1014 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/utm.py
+-rw-r--r--   0        0        0     1055 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/widget_background.py
+-rw-r--r--   0        0        0      411 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/__init__.py
+-rw-r--r--   0        0        0     2821 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/client.py
+-rw-r--r--   0        0        0      564 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/__init__.py
+-rw-r--r--   0        0        0       89 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/channel_identifier.py
+-rw-r--r--   0        0        0     1101 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/list_templates_response.py
+-rw-r--r--   0        0        0     1764 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/notification_templates.py
+-rw-r--r--   0        0        0     1378 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/routing_strategy.py
+-rw-r--r--   0        0        0      472 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/routing_strategy_method.py
+-rw-r--r--   0        0        0      909 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/tag.py
+-rw-r--r--   0        0        0      991 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/tag_data.py
+-rw-r--r--   0        0        0      449 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/__init__.py
+-rw-r--r--   0        0        0    13350 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/client.py
+-rw-r--r--   0        0        0      624 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/__init__.py
+-rw-r--r--   0        0        0      955 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/default_preferences.py
+-rw-r--r--   0        0        0     1780 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/list_users_for_tenant_response.py
+-rw-r--r--   0        0        0     1014 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic.py
+-rw-r--r--   0        0        0      707 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic_status.py
+-rw-r--r--   0        0        0      110 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/template_property.py
+-rw-r--r--   0        0        0     1844 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/tenant.py
+-rw-r--r--   0        0        0     1746 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/tenant_list_response.py
+-rw-r--r--   0        0        0       65 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/translations/__init__.py
+-rw-r--r--   0        0        0     5527 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/translations/client.py
+-rw-r--r--   0        0        0     1259 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/__init__.py
+-rw-r--r--   0        0        0     1098 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/client.py
+-rw-r--r--   0        0        0     1298 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/__init__.py
+-rw-r--r--   0        0        0      353 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/__init__.py
+-rw-r--r--   0        0        0    10433 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/client.py
+-rw-r--r--   0        0        0      473 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/__init__.py
+-rw-r--r--   0        0        0     1351 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/topic_preference.py
+-rw-r--r--   0        0        0      946 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_get_response.py
+-rw-r--r--   0        0        0     1101 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_list_response.py
+-rw-r--r--   0        0        0      893 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_update_response.py
+-rw-r--r--   0        0        0      229 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/__init__.py
+-rw-r--r--   0        0        0    10729 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/client.py
+-rw-r--r--   0        0        0      308 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/__init__.py
+-rw-r--r--   0        0        0     1279 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/add_user_to_single_tenants_params_profile.py
+-rw-r--r--   0        0        0     1784 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/list_tenants_for_user_response.py
+-rw-r--r--   0        0        0      765 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/__init__.py
+-rw-r--r--   0        0        0    12257 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/client.py
+-rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/__init__.py
+-rw-r--r--   0        0        0      898 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/delete_user_token_opts.py
+-rw-r--r--   0        0        0     1459 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/device.py
+-rw-r--r--   0        0        0      117 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/expiry_date.py
+-rw-r--r--   0        0        0      161 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_all_tokens_response.py
+-rw-r--r--   0        0        0      895 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_opts.py
+-rw-r--r--   0        0        0     1122 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_response.py
+-rw-r--r--   0        0        0      881 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_tokens_opts.py
+-rw-r--r--   0        0        0      964 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_op.py
+-rw-r--r--   0        0        0     1134 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_operation.py
+-rw-r--r--   0        0        0      948 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_user_token_opts.py
+-rw-r--r--   0        0        0      780 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/provider_key.py
+-rw-r--r--   0        0        0      935 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_token_opts.py
+-rw-r--r--   0        0        0      950 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_tokens_opts.py
+-rw-r--r--   0        0        0      770 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/token_status.py
+-rw-r--r--   0        0        0     1223 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/tracking.py
+-rw-r--r--   0        0        0     1752 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/user_token.py
+-rw-r--r--   0        0        0      155 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/types/__init__.py
+-rw-r--r--   0        0        0     1669 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/types/send_message_response.py
+-rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 trycourier-6.0.0b1/PKG-INFO
```

### Comparing `trycourier-6.0.0b0/LICENSE` & `trycourier-6.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/README.md` & `trycourier-6.0.0b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 import os
 import courier
 import asyncio
 
 from courier.client import AsyncCourier
 
 client = AsyncCourier(
-  authorization_token="YOUR_TOKENY" # Defaults to COURIER_AUTH_TOKEN
+  authorization_token="YOUR_TOKEN" # Defaults to COURIER_AUTH_TOKEN
 )
 
 async def main() -> None: 
-  response = client.send(
+  response = await client.send(
     message=courier.ContentMessage(
       to=courier.UserRecipient(
         email="marty_mcfly@email.com",
         data={
           name: "Marty",
         }
       ),
@@ -140,15 +140,15 @@
 
 ```python
 import courier
 
 from courier import Courier
 
 client = Courier(
-  authorization_token="YOUR_AUTH_TOKEN")
+  authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.TemplateMessage(
       template="my-template",
       to=courier.UserRecipient(email="foo@bar.com")
     )
 )
@@ -159,15 +159,15 @@
 
 ```python
 import courier
 
 from courier import Courier
 
 client = Courier(
-  authorization_token="YOUR_AUTH_TOKEN")
+  authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.ContentMessage(
       content=courier.ElementalContent(
         version='2020-01-01',
         elements=[
           courier.ElementalNode_Action(
```

### Comparing `trycourier-6.0.0b0/src/courier/__init__.py` & `trycourier-6.0.0b1/src/courier/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     InboundBulkContentMessage,
     InboundBulkMessage,
     InboundBulkMessageUser,
     InboundBulkMessageV1,
     InboundBulkMessageV2,
     InboundBulkTemplateMessage,
     Intercom,
-    IntercomeRecipient,
+    IntercomRecipient,
     InvalidListPatternRecipient,
     InvalidListRecipient,
     InvalidUserRecipient,
     IssueTokenResponse,
     JobDetails,
     List,
     ListAuditEventsParams,
@@ -150,14 +150,15 @@
     ListPatternRecipient,
     ListPatternRecipientType,
     ListPutParams,
     ListRecipient,
     ListRecipientType,
     ListSubscriptionRecipient,
     ListTemplatesResponse,
+    ListUsersForTenantResponse,
     Locale,
     Locales,
     LogicalOperator,
     Logo,
     MergeAlgorithm,
     MergeProfileResponse,
     Message,
@@ -175,14 +176,15 @@
     MessageRecipient,
     MessageRouting,
     MessageRoutingChannel,
     MessageRoutingMethod,
     MessageStatus,
     Metadata,
     MsTeams,
+    MsTeamsBaseProperties,
     MultipleTokens,
     NestedFilterConfig,
     NotFound,
     NotFoundError,
     Notification,
     NotificationBlock,
     NotificationChannel,
@@ -222,17 +224,25 @@
     RoutingStrategyChannel,
     RoutingStrategyMethod,
     RoutingStrategyProvider,
     Rule,
     RuleType,
     SendDirectMessage,
     SendToChannel,
-    SendToMsTeamsChannel,
-    SendToMsTeamsUser,
+    SendToMsTeamsChannelId,
+    SendToMsTeamsChannelName,
+    SendToMsTeamsConversationId,
+    SendToMsTeamsEmail,
+    SendToMsTeamsUserId,
+    SendToSlackChannel,
+    SendToSlackEmail,
+    SendToSlackUserId,
     SingleFilterConfig,
+    Slack,
+    SlackBaseProperties,
     SnoozeRule,
     SnoozeRuleType,
     SubmissionChecksGetResponse,
     SubmissionChecksReplaceResponse,
     SubscribeToListsRequest,
     SubscribeToListsRequestListObject,
     SubscribeToListsResponse,
@@ -250,14 +260,15 @@
     Timeout,
     Timeouts,
     Token,
     TrackingOverride,
     UserProfile,
     UserRecipient,
     UserRecipientType,
+    UserTenantAssociation,
     Utm,
     WidgetBackground,
     audiences,
     audit_events,
     auth_tokens,
     automations,
     brands,
@@ -401,15 +412,15 @@
     "InboundBulkContentMessage",
     "InboundBulkMessage",
     "InboundBulkMessageUser",
     "InboundBulkMessageV1",
     "InboundBulkMessageV2",
     "InboundBulkTemplateMessage",
     "Intercom",
-    "IntercomeRecipient",
+    "IntercomRecipient",
     "InvalidListPatternRecipient",
     "InvalidListRecipient",
     "InvalidUserRecipient",
     "IssueTokenResponse",
     "JobDetails",
     "List",
     "ListAuditEventsParams",
@@ -425,14 +436,15 @@
     "ListPatternRecipient",
     "ListPatternRecipientType",
     "ListPutParams",
     "ListRecipient",
     "ListRecipientType",
     "ListSubscriptionRecipient",
     "ListTemplatesResponse",
+    "ListUsersForTenantResponse",
     "Locale",
     "Locales",
     "LogicalOperator",
     "Logo",
     "MergeAlgorithm",
     "MergeProfileResponse",
     "Message",
@@ -450,14 +462,15 @@
     "MessageRecipient",
     "MessageRouting",
     "MessageRoutingChannel",
     "MessageRoutingMethod",
     "MessageStatus",
     "Metadata",
     "MsTeams",
+    "MsTeamsBaseProperties",
     "MultipleTokens",
     "NestedFilterConfig",
     "NotFound",
     "NotFoundError",
     "Notification",
     "NotificationBlock",
     "NotificationChannel",
@@ -498,17 +511,25 @@
     "RoutingStrategyMethod",
     "RoutingStrategyProvider",
     "Rule",
     "RuleType",
     "SendDirectMessage",
     "SendMessageResponse",
     "SendToChannel",
-    "SendToMsTeamsChannel",
-    "SendToMsTeamsUser",
+    "SendToMsTeamsChannelId",
+    "SendToMsTeamsChannelName",
+    "SendToMsTeamsConversationId",
+    "SendToMsTeamsEmail",
+    "SendToMsTeamsUserId",
+    "SendToSlackChannel",
+    "SendToSlackEmail",
+    "SendToSlackUserId",
     "SingleFilterConfig",
+    "Slack",
+    "SlackBaseProperties",
     "SnoozeRule",
     "SnoozeRuleType",
     "SubmissionChecksGetResponse",
     "SubmissionChecksReplaceResponse",
     "SubscribeToListsRequest",
     "SubscribeToListsRequestListObject",
     "SubscribeToListsResponse",
@@ -526,14 +547,15 @@
     "Timeout",
     "Timeouts",
     "Token",
     "TrackingOverride",
     "UserProfile",
     "UserRecipient",
     "UserRecipientType",
+    "UserTenantAssociation",
     "Utm",
     "WidgetBackground",
     "audiences",
     "audit_events",
     "auth_tokens",
     "automations",
     "brands",
```

### Comparing `trycourier-6.0.0b0/src/courier/client.py` & `trycourier-6.0.0b1/src/courier/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/core/__init__.py` & `trycourier-6.0.0b1/src/courier/core/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/core/client_wrapper.py` & `trycourier-6.0.0b1/src/courier/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._authorization_token = authorization_token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "trycourier",
-            "X-Fern-SDK-Version": "v6.0.0b0",
+            "X-Fern-SDK-Version": "v6.0.0b1",
         }
         headers["Authorization"] = f"Bearer {self._get_authorization_token()}"
         return headers
 
     def _get_authorization_token(self) -> str:
         if isinstance(self._authorization_token, str):
             return self._authorization_token
```

### Comparing `trycourier-6.0.0b0/src/courier/core/datetime_utils.py` & `trycourier-6.0.0b1/src/courier/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/core/jsonable_encoder.py` & `trycourier-6.0.0b1/src/courier/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     NotificationPreferences,
     Paging,
     PaymentRequired,
     PaymentRequiredError,
     PreferenceStatus,
     RecipientPreferences,
     Rule,
+    UserTenantAssociation,
 )
 from .lists import (
     List,
     ListFindByRecipientIdParams,
     ListFindByRecipientIdResponse,
     ListGetAllParams,
     ListGetAllResponse,
@@ -160,25 +161,34 @@
     DeleteListSubscriptionResponse,
     DeviceType,
     Discord,
     Expo,
     GetListSubscriptionsList,
     GetListSubscriptionsResponse,
     Intercom,
-    IntercomeRecipient,
+    IntercomRecipient,
     MergeProfileResponse,
     MsTeams,
+    MsTeamsBaseProperties,
     MultipleTokens,
     ProfileGetParameters,
     ProfileGetResponse,
     ReplaceProfileResponse,
     SendDirectMessage,
     SendToChannel,
-    SendToMsTeamsChannel,
-    SendToMsTeamsUser,
+    SendToMsTeamsChannelId,
+    SendToMsTeamsChannelName,
+    SendToMsTeamsConversationId,
+    SendToMsTeamsEmail,
+    SendToMsTeamsUserId,
+    SendToSlackChannel,
+    SendToSlackEmail,
+    SendToSlackUserId,
+    Slack,
+    SlackBaseProperties,
     SnoozeRule,
     SnoozeRuleType,
     SubscribeToListsRequest,
     SubscribeToListsRequestListObject,
     SubscribeToListsResponse,
     Token,
     UserProfile,
@@ -281,14 +291,15 @@
     RoutingStrategy,
     RoutingStrategyMethod,
     Tag,
     TagData,
 )
 from .tenants import (
     DefaultPreferences,
+    ListUsersForTenantResponse,
     SubscriptionTopic,
     SubscriptionTopicStatus,
     TemplateProperty,
     Tenant,
     TenantListResponse,
 )
 
@@ -417,15 +428,15 @@
     "InboundBulkContentMessage",
     "InboundBulkMessage",
     "InboundBulkMessageUser",
     "InboundBulkMessageV1",
     "InboundBulkMessageV2",
     "InboundBulkTemplateMessage",
     "Intercom",
-    "IntercomeRecipient",
+    "IntercomRecipient",
     "InvalidListPatternRecipient",
     "InvalidListRecipient",
     "InvalidUserRecipient",
     "IssueTokenResponse",
     "JobDetails",
     "List",
     "ListAuditEventsParams",
@@ -441,14 +452,15 @@
     "ListPatternRecipient",
     "ListPatternRecipientType",
     "ListPutParams",
     "ListRecipient",
     "ListRecipientType",
     "ListSubscriptionRecipient",
     "ListTemplatesResponse",
+    "ListUsersForTenantResponse",
     "Locale",
     "Locales",
     "LogicalOperator",
     "Logo",
     "MergeAlgorithm",
     "MergeProfileResponse",
     "Message",
@@ -466,14 +478,15 @@
     "MessageRecipient",
     "MessageRouting",
     "MessageRoutingChannel",
     "MessageRoutingMethod",
     "MessageStatus",
     "Metadata",
     "MsTeams",
+    "MsTeamsBaseProperties",
     "MultipleTokens",
     "NestedFilterConfig",
     "NotFound",
     "NotFoundError",
     "Notification",
     "NotificationBlock",
     "NotificationChannel",
@@ -513,17 +526,25 @@
     "RoutingStrategyChannel",
     "RoutingStrategyMethod",
     "RoutingStrategyProvider",
     "Rule",
     "RuleType",
     "SendDirectMessage",
     "SendToChannel",
-    "SendToMsTeamsChannel",
-    "SendToMsTeamsUser",
+    "SendToMsTeamsChannelId",
+    "SendToMsTeamsChannelName",
+    "SendToMsTeamsConversationId",
+    "SendToMsTeamsEmail",
+    "SendToMsTeamsUserId",
+    "SendToSlackChannel",
+    "SendToSlackEmail",
+    "SendToSlackUserId",
     "SingleFilterConfig",
+    "Slack",
+    "SlackBaseProperties",
     "SnoozeRule",
     "SnoozeRuleType",
     "SubmissionChecksGetResponse",
     "SubmissionChecksReplaceResponse",
     "SubscribeToListsRequest",
     "SubscribeToListsRequestListObject",
     "SubscribeToListsResponse",
@@ -541,14 +562,15 @@
     "Timeout",
     "Timeouts",
     "Token",
     "TrackingOverride",
     "UserProfile",
     "UserRecipient",
     "UserRecipientType",
+    "UserTenantAssociation",
     "Utm",
     "WidgetBackground",
     "audiences",
     "audit_events",
     "auth_tokens",
     "automations",
     "brands",
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/client.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/audience.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_list_response.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_member.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_member_get_response.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_member_list_response.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/audience_update_response.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_update_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/base_filter_config.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/base_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/comparison_operator.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/comparison_operator.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/nested_filter_config.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/nested_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audiences/types/single_filter_config.py` & `trycourier-6.0.0b1/src/courier/resources/audiences/types/single_filter_config.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/client.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/types/actor.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/types/actor.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/types/audit_event.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/types/audit_event.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/types/get_audit_event_params.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/types/get_audit_event_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/types/list_audit_events_params.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/types/list_audit_events_response.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/audit_events/types/target.py` & `trycourier-6.0.0b1/src/courier/resources/audit_events/types/target.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/auth_tokens/client.py` & `trycourier-6.0.0b1/src/courier/resources/auth_tokens/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/auth_tokens/types/issue_token_response.py` & `trycourier-6.0.0b1/src/courier/resources/auth_tokens/types/issue_token_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/client.py` & `trycourier-6.0.0b1/src/courier/resources/automations/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_ad_hoc_invoke_params.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_ad_hoc_invoke_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_cancel_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_cancel_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_delay_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_delay_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_params.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_response.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_invoke_template_params.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_template_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_run_context.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_run_context.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_send_list_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_list_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_send_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_step_action.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_action.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_step_option.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_option.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_update_profile_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_update_profile_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/automation_v_2_send_step.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_v_2_send_step.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/automations/types/merge_algorithm.py` & `trycourier-6.0.0b1/src/courier/resources/automations/types/merge_algorithm.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/client.py` & `trycourier-6.0.0b1/src/courier/resources/brands/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand_colors.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_colors.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand_get_all_response.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_get_all_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand_parameters.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_parameters.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand_settings.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_settings.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand_snippet.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippet.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brand_snippets.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippets.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/brands/types/brands_response.py` & `trycourier-6.0.0b1/src/courier/resources/brands/types/brands_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/client.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_create_job_response.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_create_job_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_params.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_response.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_users_params.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_get_job_users_response.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_ingest_error.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_error.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_ingest_users_params.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_ingest_users_response.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_job_status.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_job_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_job_user_status.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_job_user_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/bulk_message_user_response.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_message_user_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_content_message.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_content_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message_user.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_user.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_message_v_1.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_v_1.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/inbound_bulk_template_message.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_template_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/bulk/types/job_details.py` & `trycourier-6.0.0b1/src/courier/resources/bulk/types/job_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/commons/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     NotificationPreferenceDetails,
     NotificationPreferences,
     Paging,
     PaymentRequired,
     PreferenceStatus,
     RecipientPreferences,
     Rule,
+    UserTenantAssociation,
 )
 from .errors import (
     AlreadyExistsError,
     BadRequestError,
     ConflictError,
     MessageNotFoundError,
     NotFoundError,
@@ -46,8 +47,9 @@
     "NotificationPreferences",
     "Paging",
     "PaymentRequired",
     "PaymentRequiredError",
     "PreferenceStatus",
     "RecipientPreferences",
     "Rule",
+    "UserTenantAssociation",
 ]
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/errors/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/commons/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .notification_preference_details import NotificationPreferenceDetails
 from .notification_preferences import NotificationPreferences
 from .paging import Paging
 from .payment_required import PaymentRequired
 from .preference_status import PreferenceStatus
 from .recipient_preferences import RecipientPreferences
 from .rule import Rule
+from .user_tenant_association import UserTenantAssociation
 
 __all__ = [
     "AlreadyExists",
     "BadRequest",
     "BaseError",
     "ChannelClassification",
     "ChannelPreference",
@@ -30,8 +31,9 @@
     "NotificationPreferenceDetails",
     "NotificationPreferences",
     "Paging",
     "PaymentRequired",
     "PreferenceStatus",
     "RecipientPreferences",
     "Rule",
+    "UserTenantAssociation",
 ]
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/already_exists.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/already_exists.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/bad_request.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/bad_request.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/base_error.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/base_error.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/channel_classification.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/channel_classification.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/channel_preference.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/channel_preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/conflict.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/conflict.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/email.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/message_not_found.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/message_not_found.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/not_found.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/not_found.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/notification_preference_details.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/notification_preference_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/paging.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/paging.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/payment_required.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/payment_required.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/preference_status.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/preference_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/recipient_preferences.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/recipient_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/commons/types/rule.py` & `trycourier-6.0.0b1/src/courier/resources/commons/types/rule.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/client.py` & `trycourier-6.0.0b1/src/courier/resources/lists/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_find_by_recipient_id_params.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_find_by_recipient_id_response.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_all_params.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_all_response.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_subscriptions_params.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_get_subscriptions_response.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_put_params.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_put_params.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/list_subscription_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/list_subscription_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/put_subscriptions_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/put_subscriptions_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/lists/types/recipient_subscriptions_response.py` & `trycourier-6.0.0b1/src/courier/resources/lists/types/recipient_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/client.py` & `trycourier-6.0.0b1/src/courier/resources/messages/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/list_messages_response.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/list_messages_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/message_details.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/message_details.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/message_history_response.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/message_history_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/message_status.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/message_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/reason.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/reason.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/render_output.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/render_output.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/render_output_response.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/render_output_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/rendered_message_block.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_block.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/messages/types/rendered_message_content.py` & `trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/client.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/base_check.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/base_check.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/block_type.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/block_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/check.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/check.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/check_status.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/check_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/message_routing.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_block.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_block.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_channel.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_channel_content.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_content_hierarchy.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_content_hierarchy.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_get_content_response.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_get_content_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/notification_list_response.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/submission_checks_get_response.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/notifications/types/submission_checks_replace_response.py` & `trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_replace_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/client.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,34 @@
 from .delete_list_subscription_response import DeleteListSubscriptionResponse
 from .device_type import DeviceType
 from .discord import Discord
 from .expo import Expo
 from .get_list_subscriptions_list import GetListSubscriptionsList
 from .get_list_subscriptions_response import GetListSubscriptionsResponse
 from .intercom import Intercom
-from .intercome_recipient import IntercomeRecipient
+from .intercom_recipient import IntercomRecipient
 from .merge_profile_response import MergeProfileResponse
 from .ms_teams import MsTeams
+from .ms_teams_base_properties import MsTeamsBaseProperties
 from .multiple_tokens import MultipleTokens
 from .profile_get_parameters import ProfileGetParameters
 from .profile_get_response import ProfileGetResponse
 from .replace_profile_response import ReplaceProfileResponse
 from .send_direct_message import SendDirectMessage
 from .send_to_channel import SendToChannel
-from .send_to_ms_teams_channel import SendToMsTeamsChannel
-from .send_to_ms_teams_user import SendToMsTeamsUser
+from .send_to_ms_teams_channel_id import SendToMsTeamsChannelId
+from .send_to_ms_teams_channel_name import SendToMsTeamsChannelName
+from .send_to_ms_teams_conversation_id import SendToMsTeamsConversationId
+from .send_to_ms_teams_email import SendToMsTeamsEmail
+from .send_to_ms_teams_user_id import SendToMsTeamsUserId
+from .send_to_slack_channel import SendToSlackChannel
+from .send_to_slack_email import SendToSlackEmail
+from .send_to_slack_user_id import SendToSlackUserId
+from .slack import Slack
+from .slack_base_properties import SlackBaseProperties
 from .snooze_rule import SnoozeRule
 from .snooze_rule_type import SnoozeRuleType
 from .subscribe_to_lists_request import SubscribeToListsRequest
 from .subscribe_to_lists_request_list_object import SubscribeToListsRequestListObject
 from .subscribe_to_lists_response import SubscribeToListsResponse
 from .token import Token
 from .user_profile import UserProfile
@@ -36,25 +45,34 @@
     "DeleteListSubscriptionResponse",
     "DeviceType",
     "Discord",
     "Expo",
     "GetListSubscriptionsList",
     "GetListSubscriptionsResponse",
     "Intercom",
-    "IntercomeRecipient",
+    "IntercomRecipient",
     "MergeProfileResponse",
     "MsTeams",
+    "MsTeamsBaseProperties",
     "MultipleTokens",
     "ProfileGetParameters",
     "ProfileGetResponse",
     "ReplaceProfileResponse",
     "SendDirectMessage",
     "SendToChannel",
-    "SendToMsTeamsChannel",
-    "SendToMsTeamsUser",
+    "SendToMsTeamsChannelId",
+    "SendToMsTeamsChannelName",
+    "SendToMsTeamsConversationId",
+    "SendToMsTeamsEmail",
+    "SendToMsTeamsUserId",
+    "SendToSlackChannel",
+    "SendToSlackEmail",
+    "SendToSlackUserId",
+    "Slack",
+    "SlackBaseProperties",
     "SnoozeRule",
     "SnoozeRuleType",
     "SubscribeToListsRequest",
     "SubscribeToListsRequestListObject",
     "SubscribeToListsResponse",
     "Token",
     "UserProfile",
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/address.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/address.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/airship_profile.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/airship_profile_audience.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile_audience.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/delete_list_subscription_response.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/delete_list_subscription_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/get_list_subscriptions_list.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_list.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/get_list_subscriptions_response.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/intercom.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .intercome_recipient import IntercomeRecipient
+from .intercom_recipient import IntercomRecipient
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class Intercom(pydantic.BaseModel):
     from_: str = pydantic.Field(alias="from")
-    to: IntercomeRecipient
+    to: IntercomRecipient
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/intercome_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom_recipient.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class IntercomeRecipient(pydantic.BaseModel):
+class IntercomRecipient(pydantic.BaseModel):
     id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/merge_profile_response.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/merge_profile_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/multiple_tokens.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/multiple_tokens.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/profile_get_parameters.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_parameters.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/profile_get_response.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/replace_profile_response.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/replace_profile_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/send_direct_message.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_direct_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/send_to_channel.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/send_to_ms_teams_channel.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_token_opts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ......core.datetime_utils import serialize_datetime
+from .user_token import UserToken
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SendToMsTeamsChannel(pydantic.BaseModel):
-    conversation_id: str
-    tenant_id: str
-    service_url: str
+class PutUserTokenOpts(pydantic.BaseModel):
+    user_id: str
+    token: UserToken
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/send_to_ms_teams_user.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams_base_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SendToMsTeamsUser(pydantic.BaseModel):
-    user_id: str
+class MsTeamsBaseProperties(pydantic.BaseModel):
     tenant_id: str
     service_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/snooze_rule.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/snooze_rule.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/subscribe_to_lists_request.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/subscribe_to_lists_request_list_object.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request_list_object.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/subscribe_to_lists_response.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/token.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/token.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/profiles/types/user_profile.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/user_profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ....core.datetime_utils import serialize_datetime
 from .address import Address
 from .airship_profile import AirshipProfile
 from .discord import Discord
 from .expo import Expo
 from .intercom import Intercom
 from .ms_teams import MsTeams
+from .slack import Slack
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
@@ -45,14 +46,15 @@
     apn: str
     target_arn: str
     discord: Discord
     expo: Expo
     facebook_psid: str = pydantic.Field(alias="facebookPSID")
     firebase_token: str = pydantic.Field(alias="firebaseToken")
     intercom: Intercom
+    slack: Slack
     ms_teams: MsTeams
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/send/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/audience_filter.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/audience_filter.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/audience_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/audience_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/base_message.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/base_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/base_social_presence.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/base_social_presence.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/brand_settings_email.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_email.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/brand_settings_in_app.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_in_app.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/brand_settings_social_presence.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_social_presence.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/brand_template.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/brand_template.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/brand_template_override.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/brand_template_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/channel.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/channel_metadata.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/channel_metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/channel_source.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/channel_source.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/content_message.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/content_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/criteria.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/criteria.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/delay.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/delay.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_action_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_action_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_base_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_base_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_channel_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_channel_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_content.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_content_sugar.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content_sugar.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_divider_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_divider_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_group_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_group_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_image_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_image_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_meta_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_meta_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_quote_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_quote_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/elemental_text_node.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_text_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/email_footer.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/email_footer.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/email_head.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/email_head.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/email_header.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/email_header.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/expiry.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/expiry.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/i_alignment.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/i_alignment.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/i_profile_preferences.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/i_profile_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/icons.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/icons.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/in_app_placement.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/in_app_placement.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/invalid_list_pattern_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_pattern_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/invalid_list_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/invalid_user_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/invalid_user_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/list_filter.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/list_filter.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/list_pattern_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/list_pattern_recipient_type.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/list_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/list_recipient_type.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/locale.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/locale.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/logo.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/logo.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/message_channel_email_override.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/message_channel_email_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/message_context.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/message_context.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/message_metadata.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/message_metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/message_providers_type.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/message_providers_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/metadata.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/metadata.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/override.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/preference.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/preferences.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/routing.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/routing.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/routing_strategy_channel.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_channel.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/routing_strategy_provider.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_provider.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/rule_type.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/rule_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/template_message.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/template_message.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/text_align.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/text_align.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/text_style.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/text_style.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/timeout.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/timeout.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/timeouts.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/timeouts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/tracking_override.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/tracking_override.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/user_recipient.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/user_recipient_type.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient_type.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/utm.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/utm.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/send/types/widget_background.py` & `trycourier-6.0.0b1/src/courier/resources/send/types/widget_background.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/client.py` & `trycourier-6.0.0b1/src/courier/resources/templates/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/templates/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/types/list_templates_response.py` & `trycourier-6.0.0b1/src/courier/resources/templates/types/list_templates_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/types/notification_templates.py` & `trycourier-6.0.0b1/src/courier/resources/templates/types/notification_templates.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/types/routing_strategy.py` & `trycourier-6.0.0b1/src/courier/resources/templates/types/routing_strategy.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/types/tag.py` & `trycourier-6.0.0b1/src/courier/resources/templates/types/tag.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/templates/types/tag_data.py` & `trycourier-6.0.0b1/src/courier/resources/templates/types/tag_data.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/client.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.types.bad_request import BadRequest
 from .types.default_preferences import DefaultPreferences
+from .types.list_users_for_tenant_response import ListUsersForTenantResponse
 from .types.template_property import TemplateProperty
 from .types.tenant import Tenant
 from .types.tenant_list_response import TenantListResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
@@ -133,14 +134,35 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_users_by_tenant(self, tenant_id: str) -> ListUsersForTenantResponse:
+        """
+        Parameters:
+            - tenant_id: str. Id of the tenant for user membership.
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{tenant_id}/users"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncTenantsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create_or_replace(
         self,
@@ -247,7 +269,28 @@
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_users_by_tenant(self, tenant_id: str) -> ListUsersForTenantResponse:
+        """
+        Parameters:
+            - tenant_id: str. Id of the tenant for user membership.
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"tenants/{tenant_id}/users"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .default_preferences import DefaultPreferences
+from .list_users_for_tenant_response import ListUsersForTenantResponse
 from .subscription_topic import SubscriptionTopic
 from .subscription_topic_status import SubscriptionTopicStatus
 from .template_property import TemplateProperty
 from .tenant import Tenant
 from .tenant_list_response import TenantListResponse
 
 __all__ = [
     "DefaultPreferences",
+    "ListUsersForTenantResponse",
     "SubscriptionTopic",
     "SubscriptionTopicStatus",
     "TemplateProperty",
     "Tenant",
     "TenantListResponse",
 ]
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/types/default_preferences.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/types/default_preferences.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/types/subscription_topic.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/types/subscription_topic_status.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/types/tenant.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/types/tenant.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/tenants/types/tenant_list_response.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/list_tenants_for_user_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import typing_extensions
 
-from ....core.datetime_utils import serialize_datetime
-from .tenant import Tenant
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.user_tenant_association import UserTenantAssociation
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TenantListResponse(pydantic.BaseModel):
-    cursor: typing.Optional[str] = pydantic.Field(
-        description="A pointer to the next page of results. Defined only whenhas_more is set to true."
-    )
+class ListTenantsForUserResponse(pydantic.BaseModel):
+    items: typing.Optional[UserTenantAssociation]
     has_more: bool = pydantic.Field(description="Set to true when there are more pages that can be retrieved.")
-    items: typing.List[Tenant] = pydantic.Field(description="An array of Tenants")
+    url: str = pydantic.Field(description="A url that may be used to generate these results.")
     next_url: typing.Optional[str] = pydantic.Field(
         description=(
             "A url that may be used to generate fetch the next set of results.\n"
-            "Defined only whenhas_more is set to true\n"
+            "Defined only when `has_more` is set to true\n"
         )
     )
-    url: str = pydantic.Field(description="A url that may be used to generate these results.")
+    cursor: typing.Optional[str] = pydantic.Field(
+        description=("A pointer to the next page of results. Defined\n" "only when `has_more` is set to true\n")
+    )
     type: typing_extensions.Literal["list"] = pydantic.Field(
-        description='Always set to "list". Represents the type of this object.'
+        description="Always set to `list`. Represents the type of this object."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/translations/client.py` & `trycourier-6.0.0b1/src/courier/resources/translations/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .resources import (
-    AddUserToSingleTenantsParamsProfile,
+from . import preferences, tenants, tokens
+from .preferences import (
+    TopicPreference,
+    UserPreferencesGetResponse,
+    UserPreferencesListResponse,
+    UserPreferencesUpdateResponse,
+)
+from .tenants import AddUserToSingleTenantsParamsProfile, ListTenantsForUserResponse
+from .tokens import (
     DeleteUserTokenOpts,
     Device,
     ExpiryDate,
     GetAllTokensResponse,
     GetUserTokenOpts,
     GetUserTokenResponse,
     GetUserTokensOpts,
-    ListTenantsForUserResponse,
     PatchOp,
     PatchOperation,
     PatchUserTokenOpts,
     ProviderKey,
     PutUserTokenOpts,
     PutUserTokensOpts,
     TokenStatus,
-    TopicPreference,
     Tracking,
-    UserPreferencesGetResponse,
-    UserPreferencesListResponse,
-    UserPreferencesUpdateResponse,
-    UserTenantAssociation,
     UserToken,
-    preferences,
-    tenants,
-    tokens,
 )
 
 __all__ = [
     "AddUserToSingleTenantsParamsProfile",
     "DeleteUserTokenOpts",
     "Device",
     "ExpiryDate",
@@ -47,13 +45,12 @@
     "PutUserTokensOpts",
     "TokenStatus",
     "TopicPreference",
     "Tracking",
     "UserPreferencesGetResponse",
     "UserPreferencesListResponse",
     "UserPreferencesUpdateResponse",
-    "UserTenantAssociation",
     "UserToken",
     "preferences",
     "tenants",
     "tokens",
 ]
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/client.py` & `trycourier-6.0.0b1/src/courier/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/users/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import preferences, tenants, tokens
-from .preferences import (
-    TopicPreference,
-    UserPreferencesGetResponse,
-    UserPreferencesListResponse,
-    UserPreferencesUpdateResponse,
-)
-from .tenants import AddUserToSingleTenantsParamsProfile, ListTenantsForUserResponse, UserTenantAssociation
-from .tokens import (
+from .resources import (
+    AddUserToSingleTenantsParamsProfile,
     DeleteUserTokenOpts,
     Device,
     ExpiryDate,
     GetAllTokensResponse,
     GetUserTokenOpts,
     GetUserTokenResponse,
     GetUserTokensOpts,
+    ListTenantsForUserResponse,
     PatchOp,
     PatchOperation,
     PatchUserTokenOpts,
     ProviderKey,
     PutUserTokenOpts,
     PutUserTokensOpts,
     TokenStatus,
+    TopicPreference,
     Tracking,
+    UserPreferencesGetResponse,
+    UserPreferencesListResponse,
+    UserPreferencesUpdateResponse,
     UserToken,
+    preferences,
+    tenants,
+    tokens,
 )
 
 __all__ = [
     "AddUserToSingleTenantsParamsProfile",
     "DeleteUserTokenOpts",
     "Device",
     "ExpiryDate",
@@ -45,13 +46,12 @@
     "PutUserTokensOpts",
     "TokenStatus",
     "TopicPreference",
     "Tracking",
     "UserPreferencesGetResponse",
     "UserPreferencesListResponse",
     "UserPreferencesUpdateResponse",
-    "UserTenantAssociation",
     "UserToken",
     "preferences",
     "tenants",
     "tokens",
 ]
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/client.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/topic_preference.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/topic_preference.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/user_preferences_get_response.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_get_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/user_preferences_list_response.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_list_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/preferences/types/user_preferences_update_response.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_update_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/client.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
+from ....commons.types.user_tenant_association import UserTenantAssociation
 from .types.add_user_to_single_tenants_params_profile import AddUserToSingleTenantsParamsProfile
 from .types.list_tenants_for_user_response import ListTenantsForUserResponse
-from .types.user_tenant_association import UserTenantAssociation
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/add_user_to_single_tenants_params_profile.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/add_user_to_single_tenants_params_profile.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/list_tenants_for_user_response.py` & `trycourier-6.0.0b1/src/courier/resources/tenants/types/list_users_for_tenant_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import typing_extensions
 
-from ......core.datetime_utils import serialize_datetime
-from .user_tenant_association import UserTenantAssociation
+from ....core.datetime_utils import serialize_datetime
+from ...commons.types.user_tenant_association import UserTenantAssociation
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ListTenantsForUserResponse(pydantic.BaseModel):
+class ListUsersForTenantResponse(pydantic.BaseModel):
     items: typing.Optional[UserTenantAssociation]
     has_more: bool = pydantic.Field(description="Set to true when there are more pages that can be retrieved.")
     url: str = pydantic.Field(description="A url that may be used to generate these results.")
     next_url: typing.Optional[str] = pydantic.Field(
         description=(
             "A url that may be used to generate fetch the next set of results.\n"
             "Defined only when `has_more` is set to true\n"
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tenants/types/user_tenant_association.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_tokens_opts.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UserTenantAssociation(pydantic.BaseModel):
-    tenant_id: str = pydantic.Field(description="Tenant ID the user association is tied to.")
-    profile: typing.Dict[str, typing.Any]
+class GetUserTokensOpts(pydantic.BaseModel):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/client.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/__init__.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/delete_user_token_opts.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/delete_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/device.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/device.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_user_token_opts.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_user_token_response.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/get_user_tokens_opts.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/slack_base_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
+from ....core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetUserTokensOpts(pydantic.BaseModel):
-    user_id: str
+class SlackBaseProperties(pydantic.BaseModel):
+    access_token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/patch_op.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_op.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/patch_operation.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_operation.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/patch_user_token_opts.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_user_token_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/provider_key.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/provider_key.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/put_user_token_opts.py` & `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_user_id.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .user_token import UserToken
+from ....core.datetime_utils import serialize_datetime
+from .slack_base_properties import SlackBaseProperties
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PutUserTokenOpts(pydantic.BaseModel):
+class SendToSlackUserId(SlackBaseProperties):
     user_id: str
-    token: UserToken
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/put_user_tokens_opts.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_tokens_opts.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/token_status.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/token_status.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/tracking.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/tracking.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/resources/users/resources/tokens/types/user_token.py` & `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/user_token.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/src/courier/types/send_message_response.py` & `trycourier-6.0.0b1/src/courier/types/send_message_response.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b0/PKG-INFO` & `trycourier-6.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 6.0.0b0
+Version: 6.0.0b1
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -74,19 +74,19 @@
 import os
 import courier
 import asyncio
 
 from courier.client import AsyncCourier
 
 client = AsyncCourier(
-  authorization_token="YOUR_TOKENY" # Defaults to COURIER_AUTH_TOKEN
+  authorization_token="YOUR_TOKEN" # Defaults to COURIER_AUTH_TOKEN
 )
 
 async def main() -> None: 
-  response = client.send(
+  response = await client.send(
     message=courier.ContentMessage(
       to=courier.UserRecipient(
         email="marty_mcfly@email.com",
         data={
           name: "Marty",
         }
       ),
@@ -155,15 +155,15 @@
 
 ```python
 import courier
 
 from courier import Courier
 
 client = Courier(
-  authorization_token="YOUR_AUTH_TOKEN")
+  authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.TemplateMessage(
       template="my-template",
       to=courier.UserRecipient(email="foo@bar.com")
     )
 )
@@ -174,15 +174,15 @@
 
 ```python
 import courier
 
 from courier import Courier
 
 client = Courier(
-  authorization_token="YOUR_AUTH_TOKEN")
+  authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.ContentMessage(
       content=courier.ElementalContent(
         version='2020-01-01',
         elements=[
           courier.ElementalNode_Action(
```

