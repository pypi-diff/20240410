# Comparing `tmp/lusid_workflow_sdk-2.0.9.tar.gz` & `tmp/lusid_workflow_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_workflow_sdk-2.0.9.tar", max compression
+gzip compressed data, was "lusid_workflow_sdk-2.1.1.tar", max compression
```

## Comparing `lusid_workflow_sdk-2.0.9.tar` & `lusid_workflow_sdk-2.1.1.tar`

### file list

```diff
@@ -1,85 +1,93 @@
--rw-r--r--   0        0        0    11754 2023-12-18 10:59:03.578883 lusid_workflow_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     5331 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/__init__.py
--rw-r--r--   0        0        0      223 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/__init__.py
--rw-r--r--   0        0        0    57591 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0        0        0    44649 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/tasks_api.py
--rw-r--r--   0        0        0    44961 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/workers_api.py
--rw-r--r--   0        0        0    30535 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api_client.py
--rw-r--r--   0        0        0      852 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api_response.py
--rw-r--r--   0        0        0    14451 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/configuration.py
--rw-r--r--   0        0        0     5339 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/exceptions.py
--rw-r--r--   0        0        0      294 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/__init__.py
--rw-r--r--   0        0        0    30488 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client.py
--rw-r--r--   0        0        0     9644 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8012 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_configuration.py
--rw-r--r--   0        0        0     6868 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12707 2023-12-18 10:59:03.575883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/rest.py
--rw-r--r--   0        0        0    11573 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/retry.py
--rw-r--r--   0        0        0     1653 2023-12-18 10:59:03.575883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3886 2023-12-18 10:59:03.575883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     4627 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/__init__.py
--rw-r--r--   0        0        0     2711 2023-12-18 10:59:03.570883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition.py
--rw-r--r--   0        0        0     2708 2023-12-18 10:59:03.570883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0        0        0     6172 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details.py
--rw-r--r--   0        0        0     6643 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details_response.py
--rw-r--r--   0        0        0     5403 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0        0        0     3162 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0        0        0     3763 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0        0        0     7465 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0        0        0     4142 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_request.py
--rw-r--r--   0        0        0     3969 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0        0        0     3456 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0        0        0     2158 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail.py
--rw-r--r--   0        0        0     2470 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail_response.py
--rw-r--r--   0        0        0     2875 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/field_mapping.py
--rw-r--r--   0        0        0     2604 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0        0        0     2338 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check.py
--rw-r--r--   0        0        0     2811 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check_response.py
--rw-r--r--   0        0        0     2720 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/initial_state.py
--rw-r--r--   0        0        0     2259 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/link.py
--rw-r--r--   0        0        0     2604 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0        0        0     2808 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0        0        0     3854 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4690 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4050 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0        0        0     4171 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0        0        0     4074 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0        0        0     3314 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter.py
--rw-r--r--   0        0        0     2580 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter_value.py
--rw-r--r--   0        0        0     1866 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_id.py
--rw-r--r--   0        0        0     4010 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0        0        0     2790 2023-12-18 10:59:03.570883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_field.py
--rw-r--r--   0        0        0     2290 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0        0        0     5710 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0        0        0     5910 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0        0        0     6224 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0        0        0     2425 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0        0        0     2357 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0        0        0     2113 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep.py
--rw-r--r--   0        0        0     2169 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep_response.py
--rw-r--r--   0        0        0     4394 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/stack.py
--rw-r--r--   0        0        0     8350 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task.py
--rw-r--r--   0        0        0     7861 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition.py
--rw-r--r--   0        0        0     2087 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0        0        0     2480 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0        0        0     2543 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0        0        0     2276 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0        0        0     3412 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_summary.py
--rw-r--r--   0        0        0     4803 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0        0        0     2725 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0        0        0     2713 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0        0        0     2907 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0        0        0     1948 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0        0        0     7127 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0        0        0     3585 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_request.py
--rw-r--r--   0        0        0     5121 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/version_info.py
--rw-r--r--   0        0        0     6134 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker.py
--rw-r--r--   0        0        0     6354 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0        0        0     6935 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0        0        0     4201 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0        0        0        0 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/py.typed
--rw-r--r--   0        0        0    10029 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/rest.py
--rw-r--r--   0        0        0      856 2023-12-18 10:59:03.578883 lusid_workflow_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    12800 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    13185 2024-04-10 10:42:19.477844 lusid_workflow_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     8289 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/__init__.py
+-rw-r--r--   0        0        0     8588 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/event_handlers_api.py
+-rw-r--r--   0        0        0    57597 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0        0        0    44655 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0        0        0    61860 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/workers_api.py
+-rw-r--r--   0        0        0    30785 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/api_response.py
+-rw-r--r--   0        0        0    14451 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/configuration.py
+-rw-r--r--   0        0        0     5339 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/exceptions.py
+-rw-r--r--   0        0        0      587 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/__init__.py
+-rw-r--r--   0        0        0    30652 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client.py
+-rw-r--r--   0        0        0     9862 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8097 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6796 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12707 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/rest.py
+-rw-r--r--   0        0        0    11573 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3886 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     6872 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/__init__.py
+-rw-r--r--   0        0        0     3649 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition.py
+-rw-r--r--   0        0        0     3233 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0        0        0     6172 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details.py
+-rw-r--r--   0        0        0     6643 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0        0        0     5406 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0        0        0     3165 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0        0        0     3766 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0        0        0     5424 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_event_handler_request.py
+-rw-r--r--   0        0        0     7468 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0        0        0     4145 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0        0        0     3972 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0        0        0     3459 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     5704 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_handler.py
+-rw-r--r--   0        0        0     2554 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_handler_mapping.py
+-rw-r--r--   0        0        0     2951 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_matching_pattern.py
+-rw-r--r--   0        0        0     2193 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail.py
+-rw-r--r--   0        0        0     2505 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail_response.py
+-rw-r--r--   0        0        0     2878 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0        0        0     2607 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0        0        0     2341 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check.py
+-rw-r--r--   0        0        0     2814 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0        0        0     2723 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/initial_state.py
+-rw-r--r--   0        0        0     2262 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/link.py
+-rw-r--r--   0        0        0     2607 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0        0        0     2811 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0        0        0     3857 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4053 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0        0        0     4174 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0        0        0     4077 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0        0        0     3317 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter.py
+-rw-r--r--   0        0        0     2583 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0        0        0     1869 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_id.py
+-rw-r--r--   0        0        0     4013 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0        0        0     2793 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_field.py
+-rw-r--r--   0        0        0     2293 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0        0        0     5713 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0        0        0     5913 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0        0        0     6227 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0        0        0     2428 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0        0        0     2360 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0        0        0     2541 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0        0        0     2864 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0        0        0     2116 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep.py
+-rw-r--r--   0        0        0     2172 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0        0        0     4397 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/stack.py
+-rw-r--r--   0        0        0     8353 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task.py
+-rw-r--r--   0        0        0     7864 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition.py
+-rw-r--r--   0        0        0     2090 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0        0        0     2483 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0        0        0     2546 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0        0        0     2279 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0        0        0     3415 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_summary.py
+-rw-r--r--   0        0        0     4806 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0        0        0     2728 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0        0        0     2716 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0        0        0     2910 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0        0        0     1951 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0        0        0     7130 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0        0        0     3588 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0        0        0     3579 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0        0        0     5124 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/version_info.py
+-rw-r--r--   0        0        0     6137 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker.py
+-rw-r--r--   0        0        0     7051 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0        0        0     7753 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0        0        0     4204 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/py.typed
+-rw-r--r--   0        0        0    10160 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/rest.py
+-rw-r--r--   0        0        0      855 2024-04-10 10:42:19.477844 lusid_workflow_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14230 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.1/PKG-INFO
```

### Comparing `lusid_workflow_sdk-2.0.9/README.md` & `lusid_workflow_sdk-2.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.674
-- Package version: 2.0.9
+- API version: 0.1.878
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -43,29 +43,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_workflow application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_WORKFLOW_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_WORKFLOW_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_workflow via a proxy, by setting `FBN_PROXY_ADDRESS`. 
+If your proxy has basic auth enabled, you must akso supply `FBN_PROXY_USERNAME` and `FBN_PROXY_PASSWORD`
+
+### Secrets file
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set in a `secrets.json` file in the same folder as your script.
+
+``` 
+{
+    "api":
+    {
+        "tokenUrl":"<your-token-url>",
+        "lusid_workflowUrl":"<FINBOURNE-application-url>",
+        "username":"<your-username>",
+        "password":"<your-password>",
+        "clientId":"<your-client-id>",
+        "clientSecret":"<your-client-secret>",
+    }
+}
+```
+
+To use a long lived Personal Access Token, you must provide a `secrets.json` with the following variables:
+``` 
+{
+    "api":
+    {
+        "lusid_workflowUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_workflow via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_workflowUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    },
+    "proxy":
+    {
+        "address":"<your-proxy-address>",
+        "username":"<your-proxy-username>",
+        "password":"<your-proxy-password>"
+    }
+}
+```
+
+### Using the SDK
+
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
 import lusid_workflow
-from lusid_workflow.rest import ApiException
+from lusid_workflow.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_workflow import (
-	  ApiClientFactory,
-	  ApplicationMetadataApi,
-	  EnvironmentVariablesConfigurationLoader,
-	  SecretsFileConfigurationLoader,
-	  ArgsConfigurationLoader
+    ApiClientFactory,
+    EventHandlersApi,
+    EnvironmentVariablesConfigurationLoader,
+    SecretsFileConfigurationLoader,
+    ArgsConfigurationLoader
 )
 
 # Use the lusid_workflow ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -90,64 +166,71 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_workflow.TaskDefinitionsApi(api_client)
-    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
+    api_instance = api_client_factory.build(EventHandlersApi)
+    create_event_handler_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example Event Handler","description":"Test","status":"Active","eventMatchingPattern":{"eventType":"PortfolioCreated","filter":"body.scope eq 'TestScope'"},"runAsUserId":{"setTo":"ExampleUserId"},"taskDefinitionId":{"scope":"A1","code":"YYY"},"taskDefinitionAsAt":"9999-12-31T23:59:59.9999999+00:00","taskActivity":{"InitialTrigger":"InitialTrigger","Type":"CreateNewTask","CorrelationIds":[],"TaskFields":{}}} # CreateEventHandlerRequest | The data to create an Event Handler
 
     try:
-        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
-        api_response = await api_instance.create_task_definition(create_task_definition_request)
-        print("The response of TaskDefinitionsApi->create_task_definition:\n")
+        # [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
+        api_response = await api_instance.create_event_handler(create_event_handler_request)
+        print("The response of EventHandlersApi->create_event_handler:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
+        print("Exception when calling EventHandlersApi->create_event_handler: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*EventHandlersApi* | [**create_event_handler**](docs/EventHandlersApi.md#create_event_handler) | **POST** /api/eventhandlers | [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
 *TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
 *TasksApi* | [**delete_task**](docs/TasksApi.md#delete_task) | **DELETE** /api/tasks/{id} | [EXPERIMENTAL] DeleteTask: Delete a Task
 *TasksApi* | [**get_task**](docs/TasksApi.md#get_task) | **GET** /api/tasks/{id} | [EXPERIMENTAL] GetTask: Get a Task
 *TasksApi* | [**list_tasks**](docs/TasksApi.md#list_tasks) | **GET** /api/tasks | [EXPERIMENTAL] ListTasks: List Tasks
 *TasksApi* | [**update_task**](docs/TasksApi.md#update_task) | **POST** /api/tasks/{id} | [EXPERIMENTAL] UpdateTask: Update a Task
 *WorkersApi* | [**create_worker**](docs/WorkersApi.md#create_worker) | **POST** /api/workers | [EXPERIMENTAL] CreateWorker: Create a new Worker
+*WorkersApi* | [**delete_worker**](docs/WorkersApi.md#delete_worker) | **DELETE** /api/workers/{scope}/{code} | [EXPERIMENTAL] DeleteWorker: Delete a Worker
 *WorkersApi* | [**get_worker**](docs/WorkersApi.md#get_worker) | **GET** /api/workers/{scope}/{code} | [EXPERIMENTAL] GetWorker: Get a Worker
 *WorkersApi* | [**get_worker_result**](docs/WorkersApi.md#get_worker_result) | **GET** /api/workers/{runId}/$result | [EXPERIMENTAL] GetWorkerResult: Get the status of a specific run of a worker with any relevant results
 *WorkersApi* | [**list_workers**](docs/WorkersApi.md#list_workers) | **GET** /api/workers | [EXPERIMENTAL] ListWorkers: List Workers
 *WorkersApi* | [**run_worker**](docs/WorkersApi.md#run_worker) | **POST** /api/workers/{scope}/{code}/$run | [EXPERIMENTAL] RunWorker: Run a Worker
+*WorkersApi* | [**update_worker**](docs/WorkersApi.md#update_worker) | **PUT** /api/workers/{scope}/{code} | [EXPERIMENTAL] UpdateWorker: Update a Worker
 
 
 ## Documentation For Models
 
  - [ActionDefinition](docs/ActionDefinition.md)
  - [ActionDefinitionResponse](docs/ActionDefinitionResponse.md)
  - [ActionDetails](docs/ActionDetails.md)
  - [ActionDetailsResponse](docs/ActionDetailsResponse.md)
  - [CreateChildTaskConfiguration](docs/CreateChildTaskConfiguration.md)
  - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateChildTasksActionResponse](docs/CreateChildTasksActionResponse.md)
+ - [CreateEventHandlerRequest](docs/CreateEventHandlerRequest.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
+ - [EventHandler](docs/EventHandler.md)
+ - [EventHandlerMapping](docs/EventHandlerMapping.md)
+ - [EventMatchingPattern](docs/EventMatchingPattern.md)
  - [Fail](docs/Fail.md)
  - [FailResponse](docs/FailResponse.md)
  - [FieldMapping](docs/FieldMapping.md)
  - [GetWorkerResultResponse](docs/GetWorkerResultResponse.md)
  - [HealthCheck](docs/HealthCheck.md)
  - [HealthCheckResponse](docs/HealthCheckResponse.md)
  - [InitialState](docs/InitialState.md)
@@ -166,14 +249,16 @@
  - [ResultField](docs/ResultField.md)
  - [ResultMatchingPattern](docs/ResultMatchingPattern.md)
  - [ResultantChildTaskConfiguration](docs/ResultantChildTaskConfiguration.md)
  - [RunWorkerAction](docs/RunWorkerAction.md)
  - [RunWorkerActionResponse](docs/RunWorkerActionResponse.md)
  - [RunWorkerRequest](docs/RunWorkerRequest.md)
  - [RunWorkerResponse](docs/RunWorkerResponse.md)
+ - [SchedulerJob](docs/SchedulerJob.md)
+ - [SchedulerJobResponse](docs/SchedulerJobResponse.md)
  - [Sleep](docs/Sleep.md)
  - [SleepResponse](docs/SleepResponse.md)
  - [Stack](docs/Stack.md)
  - [Task](docs/Task.md)
  - [TaskDefinition](docs/TaskDefinition.md)
  - [TaskDefinitionVersion](docs/TaskDefinitionVersion.md)
  - [TaskFieldDefinition](docs/TaskFieldDefinition.md)
@@ -183,14 +268,15 @@
  - [TaskTransitionDefinition](docs/TaskTransitionDefinition.md)
  - [TransitionTriggerDefinition](docs/TransitionTriggerDefinition.md)
  - [TriggerParentTaskAction](docs/TriggerParentTaskAction.md)
  - [TriggerParentTaskActionResponse](docs/TriggerParentTaskActionResponse.md)
  - [TriggerSchema](docs/TriggerSchema.md)
  - [UpdateTaskDefinitionRequest](docs/UpdateTaskDefinitionRequest.md)
  - [UpdateTaskRequest](docs/UpdateTaskRequest.md)
+ - [UpdateWorkerRequest](docs/UpdateWorkerRequest.md)
  - [VersionInfo](docs/VersionInfo.md)
  - [Worker](docs/Worker.md)
  - [WorkerConfiguration](docs/WorkerConfiguration.md)
  - [WorkerConfigurationResponse](docs/WorkerConfigurationResponse.md)
  - [WorkerStatusTriggers](docs/WorkerStatusTriggers.md)
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/api/task_definitions_api.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/api/task_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, StrictInt, constr, validator
+from pydantic.v1 import Field, StrictInt, constr, validator
 
 from typing import Optional
 
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
 from lusid_workflow.models.resource_list_of_task import ResourceListOfTask
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/api/tasks_api.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, StrictInt, constr, validator
+from pydantic.v1 import Field, StrictInt, constr, validator
 
 from typing import Optional
 
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
 from lusid_workflow.models.task import Task
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/api/workers_api.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/api/workers_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, StrictInt, constr, validator
+from pydantic.v1 import Field, StrictInt, constr, validator
 
 from typing import Optional
 
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
+from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
 from lusid_workflow.models.run_worker_request import RunWorkerRequest
 from lusid_workflow.models.run_worker_response import RunWorkerResponse
+from lusid_workflow.models.update_worker_request import UpdateWorkerRequest
 from lusid_workflow.models.worker import Worker
 
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.api_response import ApiResponse
 from lusid_workflow.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
@@ -208,14 +210,174 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
+    async def delete_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be deleted")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be deleted")], **kwargs) -> DeletedEntityResponse:  # noqa: E501
+        ...
+
+    @overload
+    def delete_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be deleted")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be deleted")], async_req: Optional[bool]=True, **kwargs) -> DeletedEntityResponse:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def delete_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be deleted")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be deleted")], async_req: Optional[bool]=None, **kwargs) -> Union[DeletedEntityResponse, Awaitable[DeletedEntityResponse]]:  # noqa: E501
+        """[EXPERIMENTAL] DeleteWorker: Delete a Worker  # noqa: E501
+
+        If the Worker does not exist a failure will be returned  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_worker(scope, code, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: Scope of the worker to be deleted (required)
+        :type scope: str
+        :param code: Code of the worker to be deleted (required)
+        :type code: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: DeletedEntityResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the delete_worker_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        if async_req is not None:
+            kwargs['async_req'] = async_req
+        return self.delete_worker_with_http_info(scope, code, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_worker_with_http_info(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be deleted")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be deleted")], **kwargs) -> ApiResponse:  # noqa: E501
+        """[EXPERIMENTAL] DeleteWorker: Delete a Worker  # noqa: E501
+
+        If the Worker does not exist a failure will be returned  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_worker_with_http_info(scope, code, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: Scope of the worker to be deleted (required)
+        :type scope: str
+        :param code: Code of the worker to be deleted (required)
+        :type code: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(DeletedEntityResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'scope',
+            'code'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_worker" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['scope']:
+            _path_params['scope'] = _params['scope']
+
+        if _params['code']:
+            _path_params['code'] = _params['code']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['oauth2']  # noqa: E501
+
+        _response_types_map = {
+            '200': "DeletedEntityResponse",
+            '400': "LusidValidationProblemDetails",
+            '404': "str",
+        }
+
+        return self.api_client.call_api(
+            '/api/workers/{scope}/{code}', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @overload
     async def get_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker")], as_at : Annotated[Optional[datetime], Field(description="The asAt datetime at which to retrieve the Worker. Defaults to returning the latest version of the Worker if not specified.")] = None, **kwargs) -> Worker:  # noqa: E501
         ...
 
     @overload
     def get_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker")], as_at : Annotated[Optional[datetime], Field(description="The asAt datetime at which to retrieve the Worker. Defaults to returning the latest version of the Worker if not specified.")] = None, async_req: Optional[bool]=True, **kwargs) -> Worker:  # noqa: E501
         ...
 
@@ -673,15 +835,15 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '201': "PagedResourceListOfWorker",
+            '200': "PagedResourceListOfWorker",
             '400': "LusidValidationProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/workers', 'GET',
             _path_params,
             _query_params,
@@ -869,14 +1031,189 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @overload
+    async def update_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be updated")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be updated")], update_worker_request : Annotated[UpdateWorkerRequest, Field(..., description="State of the updated worker")], **kwargs) -> Worker:  # noqa: E501
+        ...
+
+    @overload
+    def update_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be updated")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be updated")], update_worker_request : Annotated[UpdateWorkerRequest, Field(..., description="State of the updated worker")], async_req: Optional[bool]=True, **kwargs) -> Worker:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def update_worker(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be updated")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be updated")], update_worker_request : Annotated[UpdateWorkerRequest, Field(..., description="State of the updated worker")], async_req: Optional[bool]=None, **kwargs) -> Union[Worker, Awaitable[Worker]]:  # noqa: E501
+        """[EXPERIMENTAL] UpdateWorker: Update a Worker  # noqa: E501
+
+        If the Worker does not exist a failure will be returned  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_worker(scope, code, update_worker_request, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: Scope of the worker to be updated (required)
+        :type scope: str
+        :param code: Code of the worker to be updated (required)
+        :type code: str
+        :param update_worker_request: State of the updated worker (required)
+        :type update_worker_request: UpdateWorkerRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Worker
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the update_worker_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        if async_req is not None:
+            kwargs['async_req'] = async_req
+        return self.update_worker_with_http_info(scope, code, update_worker_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def update_worker_with_http_info(self, scope : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Scope of the worker to be updated")], code : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="Code of the worker to be updated")], update_worker_request : Annotated[UpdateWorkerRequest, Field(..., description="State of the updated worker")], **kwargs) -> ApiResponse:  # noqa: E501
+        """[EXPERIMENTAL] UpdateWorker: Update a Worker  # noqa: E501
+
+        If the Worker does not exist a failure will be returned  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_worker_with_http_info(scope, code, update_worker_request, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: Scope of the worker to be updated (required)
+        :type scope: str
+        :param code: Code of the worker to be updated (required)
+        :type code: str
+        :param update_worker_request: State of the updated worker (required)
+        :type update_worker_request: UpdateWorkerRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(Worker, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'scope',
+            'code',
+            'update_worker_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_worker" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['scope']:
+            _path_params['scope'] = _params['scope']
+
+        if _params['code']:
+            _path_params['code'] = _params['code']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['update_worker_request'] is not None:
+            _body_params = _params['update_worker_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['oauth2']  # noqa: E501
+
+        _response_types_map = {
+            '200': "Worker",
+            '400': "LusidValidationProblemDetails",
+            '404': "str",
+        }
+
+        return self.api_client.call_api(
+            '/api/workers/{scope}/{code}', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/api_client.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
+            # if returning http_data_only then we need to deserialise response.
+            _preload_content = True if _return_http_data_only else _preload_content
             # perform request and return response
             response_data = await self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
@@ -256,16 +258,16 @@
               return_data = None
 
         if _return_http_data_only:
             return return_data
         else:
             return ApiResponse(status_code = response_data.status,
                            data = return_data,
-                           headers = response_data.getheaders(),
-                           raw_data = response_data.data)
+                           headers = response_data.getheaders() if _preload_content else response_data.headers,
+                           raw_data = response_data.data if _preload_content else response_data)
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/api_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/configuration.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_workflow-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.674\n"\
+               "Version of the API: 0.1.878\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/exceptions.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,16 @@
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
+            # if returning http_data_only then we need to deserialise response.
+            _preload_content = True if _return_http_data_only else _preload_content
             # perform request and return response
             response_data = self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client_factory.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,38 +180,43 @@
         An aiohttp.ClientSession, pass this to re-use 
         connections across different ApiFactories,
         by default None
         trace_configs: Optional[List[TraceConfig]], optional
         A list of aiohttp TraceConfigs, used to set up request tracing.
         by default None
         """
+        is_owner = True
         api_config = get_api_configuration(config_loaders=config_loaders)
         api_client_config = api_config.build_api_client_config(
             tcp_keep_alive=tcp_keep_alive,
             socket_options=socket_options,
             id_provider_response_handler=id_provider_response_handler
         )
         self.__api_client = ApiClient(
             configuration=api_client_config,
         )
         rc = self.__api_client.rest_client
         try:
             if client_session is not None:
                 connector = client_session.connector
+                is_owner = False
                 # by default take explicitly passed trace_config param
                 # otherwise copy from session.
                 trace_configs = trace_configs or client_session.trace_configs
             else:
                 connector = rc.pool_manager.connector
             if tcp_keep_alive:
                 connector = TcpKeepAliveConnector(connector=connector, socket_options=socket_options)
+            # dereference connector so existing session closes correctly
+            rc.pool_manager._connector = None
             rc.pool_manager = ClientSession(
                 connector=connector,
                 trust_env=True,
-                trace_configs=trace_configs
+                trace_configs=trace_configs,
+                connector_owner=is_owner
             )
         except AttributeError:
             logger.exception("client_session must be an aiohttp.ClientSession"
                              " object with an initialised TCP Connector")
         rest_client_wrapper = RetryingRestWrapperAsync
         wrapped_rest_client = rest_client_wrapper(rc)
         self.__api_client.rest_client = wrapped_rest_client
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_configuration.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import logging
 from typing import Optional, Union, Tuple, Any, Callable
 from lusid_workflow.configuration import Configuration
 from lusid_workflow.extensions.refreshing_token import RefreshingToken
 from lusid_workflow.extensions.socket_keep_alive import keep_alive_socket_options
+from lusid_workflow.extensions.proxy_config import ProxyConfig
 from requests import Response
 logger = logging.getLogger(__name__)
 
 
 class ApiConfiguration:
     def __init__(
         self,
@@ -15,15 +16,15 @@
         api_url=None,
         username=None,
         password=None,
         client_id=None,
         client_secret=None,
         app_name=None,
         certificate_filename=None,
-        proxy_config=None,
+        proxy_config:Optional[ProxyConfig]=None,
         access_token=None,
     ):
         """
         The configuration required to access LUSID, read more at https://support.finbourne.com/getting-started-with-apis-sdks
 
         :param str token_url: The token URL of the identity provider
         :param str api_url: The API URL for the LUSID client
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/configuration_loaders.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/configuration_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,15 @@
             if value is not None
         }
         config.update(loaded_config)
     proxy_address = config.pop("proxy_address", None)
     proxy_username = config.pop("proxy_username", None)
     proxy_password = config.pop("proxy_password", None)
     # If the proxy address is missing ensure that no proxy is used in the ApiConfiguration
-    if all(
-        (item is not None for item in (proxy_address, proxy_password, proxy_username))
-    ):
+    if proxy_address is not None:
         config["proxy_config"] = ProxyConfig(
             address=proxy_address, username=proxy_username, password=proxy_password
         )
     else:
         config["proxy_config"] = None
     # Create and return the ApiConfiguration
     return ApiConfiguration(**config)
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/proxy_config.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/proxy_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib3 import make_headers
-from typing import Any
+from typing import Dict
 
 
 class ProxyConfig:
     """
     This class is used to hold the proxy configuration details
     """
 
@@ -52,18 +52,21 @@
             index = self.address.index("://")
 
             proxy_url = f"{self.address[0:index + 3]}{self.username}:{self.password}@{self.address[index + 3:]}"
 
         return {"http": proxy_url, "https": proxy_url}
 
     @property
-    def headers(self) -> Any:
+    def headers(self) -> Dict[str, str]:
         """Return Proxy auth headers
 
         Returns
         -------
         Any
             Proxy auth headers
         """
-        return make_headers(
-            proxy_basic_auth=f"{self.__username}:{self.__password}"
-        )
+        if self.__username is not None and self.__password is not None:
+            return make_headers(
+                proxy_basic_auth=f"{self.__username}:{self.__password}"
+            )
+        else:
+            return {}
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/refreshing_token.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/rest.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/retry.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/socket_keep_alive.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/tcp_keep_alive_connector.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,32 +14,26 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
-from lusid_workflow.models.action_details import ActionDetails
+from typing import Any, Dict, Optional
+from pydantic.v1 import BaseModel, Field, StrictStr
+from lusid_workflow.models.action_details_response import ActionDetailsResponse
 
-class ActionDefinition(BaseModel):
+class ActionDefinitionResponse(BaseModel):
     """
-    Defines the Actions for a Task  # noqa: E501
+    Defines the Actions for a Task in a read-only form  # noqa: E501
     """
-    name: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The Name of this Action")
-    action_details: ActionDetails = Field(..., alias="actionDetails")
-    __properties = ["name", "actionDetails"]
-
-    @validator('name')
-    def name_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^[a-zA-Z0-9\-_]+$", value):
-            raise ValueError(r"must validate the regular expression /^[a-zA-Z0-9\-_]+$/")
-        return value
+    name: Optional[StrictStr] = Field(None, description="The Name of this Action")
+    run_as_user_id: Optional[StrictStr] = Field(None, alias="runAsUserId", description="The ID of the user that this action will be performed by. If not specified, the actions will be performed by the \"current user\".")
+    action_details: Optional[ActionDetailsResponse] = Field(None, alias="actionDetails")
+    __properties = ["name", "runAsUserId", "actionDetails"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -47,36 +41,47 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ActionDefinition:
-        """Create an instance of ActionDefinition from a JSON string"""
+    def from_json(cls, json_str: str) -> ActionDefinitionResponse:
+        """Create an instance of ActionDefinitionResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of action_details
         if self.action_details:
             _dict['actionDetails'] = self.action_details.to_dict()
+        # set to None if name (nullable) is None
+        # and __fields_set__ contains the field
+        if self.name is None and "name" in self.__fields_set__:
+            _dict['name'] = None
+
+        # set to None if run_as_user_id (nullable) is None
+        # and __fields_set__ contains the field
+        if self.run_as_user_id is None and "run_as_user_id" in self.__fields_set__:
+            _dict['runAsUserId'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ActionDefinition:
-        """Create an instance of ActionDefinition from a dict"""
+    def from_dict(cls, obj: dict) -> ActionDefinitionResponse:
+        """Create an instance of ActionDefinitionResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ActionDefinition.parse_obj(obj)
+            return ActionDefinitionResponse.parse_obj(obj)
 
-        _obj = ActionDefinition.parse_obj({
+        _obj = ActionDefinitionResponse.parse_obj({
             "name": obj.get("name"),
-            "action_details": ActionDetails.from_dict(obj.get("actionDetails")) if obj.get("actionDetails") is not None else None
+            "run_as_user_id": obj.get("runAsUserId"),
+            "action_details": ActionDetailsResponse.from_dict(obj.get("actionDetails")) if obj.get("actionDetails") is not None else None
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,24 +15,34 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
-from lusid_workflow.models.action_details_response import ActionDetailsResponse
+from pydantic.v1 import BaseModel, Field, StrictStr, validator
+from lusid_workflow.models.resource_id import ResourceId
 
-class ActionDefinitionResponse(BaseModel):
+class SchedulerJobResponse(BaseModel):
     """
-    Defines the Actions for a Task in a read-only form  # noqa: E501
+    Readonly configuration for a Worker that calls a Scheduler job  # noqa: E501
     """
-    name: Optional[StrictStr] = Field(None, description="The Name of this Action")
-    action_details: Optional[ActionDetailsResponse] = Field(None, alias="actionDetails")
-    __properties = ["name", "actionDetails"]
+    type: Optional[StrictStr] = Field(None, description="The type of worker")
+    job_id: Optional[ResourceId] = Field(None, alias="jobId")
+    __properties = ["type", "jobId"]
+
+    @validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('SchedulerJob'):
+            raise ValueError("must be one of enum values ('SchedulerJob')")
+        return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,41 +50,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ActionDefinitionResponse:
-        """Create an instance of ActionDefinitionResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> SchedulerJobResponse:
+        """Create an instance of SchedulerJobResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of action_details
-        if self.action_details:
-            _dict['actionDetails'] = self.action_details.to_dict()
-        # set to None if name (nullable) is None
+        # override the default output from pydantic by calling `to_dict()` of job_id
+        if self.job_id:
+            _dict['jobId'] = self.job_id.to_dict()
+        # set to None if type (nullable) is None
         # and __fields_set__ contains the field
-        if self.name is None and "name" in self.__fields_set__:
-            _dict['name'] = None
+        if self.type is None and "type" in self.__fields_set__:
+            _dict['type'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ActionDefinitionResponse:
-        """Create an instance of ActionDefinitionResponse from a dict"""
+    def from_dict(cls, obj: dict) -> SchedulerJobResponse:
+        """Create an instance of SchedulerJobResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ActionDefinitionResponse.parse_obj(obj)
+            return SchedulerJobResponse.parse_obj(obj)
 
-        _obj = ActionDefinitionResponse.parse_obj({
-            "name": obj.get("name"),
-            "action_details": ActionDetailsResponse.from_dict(obj.get("actionDetails")) if obj.get("actionDetails") is not None else None
+        _obj = SchedulerJobResponse.parse_obj({
+            "type": obj.get("type"),
+            "job_id": ResourceId.from_dict(obj.get("jobId")) if obj.get("jobId") is not None else None
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_task_configuration.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_task_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.resource_id import ResourceId
 
 class CreateChildTaskConfiguration(BaseModel):
     """
     Create Child Task Configuration  # noqa: E501
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, conlist, constr, validator
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 
 class CreateChildTasksAction(BaseModel):
     """
     Defines a Create Child Tasks Action  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="Type name for this Action")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 
 class CreateChildTasksActionResponse(BaseModel):
     """
     Defines a read-only Create Child Tasks Action  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="Type name for this Action")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_definition_request.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.task_field_definition import TaskFieldDefinition
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_request.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.task_instance_field import TaskInstanceField
 
 class CreateTaskRequest(BaseModel):
     """
     Contains required info to create a new Task  # noqa: E501
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_worker_request.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_worker_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
 
 class CreateWorkerRequest(BaseModel):
     """
     Request to Create a new worker  # noqa: E501
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/deleted_entity_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/deleted_entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.link import Link
 
 class DeletedEntityResponse(BaseModel):
     """
     DeletedEntityResponse
     """
     href: Optional[StrictStr] = Field(None, description="The Uri related to this Entity")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class Fail(BaseModel):
     """
     Configuration for a Worker that always Fails  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of worker")
     __properties = ["type"]
 
     @validator('type')
     def type_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in ('Fail', 'HealthCheck', 'LuminesceView', 'Sleep'):
-            raise ValueError("must be one of enum values ('Fail', 'HealthCheck', 'LuminesceView', 'Sleep')")
+        if value not in ('Fail', 'HealthCheck', 'LuminesceView', 'SchedulerJob', 'Sleep'):
+            raise ValueError("must be one of enum values ('Fail', 'HealthCheck', 'LuminesceView', 'SchedulerJob', 'Sleep')")
         return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, validator
 
 class FailResponse(BaseModel):
     """
     Readonly configuration for a Worker that always Fails  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of worker")
     __properties = ["type"]
 
     @validator('type')
     def type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Fail', 'HealthCheck', 'LuminesceView', 'Sleep'):
-            raise ValueError("must be one of enum values ('Fail', 'HealthCheck', 'LuminesceView', 'Sleep')")
+        if value not in ('Fail', 'HealthCheck', 'LuminesceView', 'SchedulerJob', 'Sleep'):
+            raise ValueError("must be one of enum values ('Fail', 'HealthCheck', 'LuminesceView', 'SchedulerJob', 'Sleep')")
         return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/field_mapping.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/field_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class FieldMapping(BaseModel):
     """
     Defines a single Field map  # noqa: E501
     """
     map_from: Optional[constr(strict=True, max_length=1024, min_length=1)] = Field(None, alias="mapFrom", description="The field to map from")
     set_to: Optional[Any] = Field(None, alias="setTo", description="The (constant) value to set")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/get_worker_result_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/get_worker_result_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 
 class GetWorkerResultResponse(BaseModel):
     """
     The RunWorker response  # noqa: E501
     """
     worker_status: constr(strict=True, min_length=1) = Field(..., alias="workerStatus", description="The final status of the Worker")
     results: conlist(Dict[str, Any]) = Field(..., description="Results")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class HealthCheck(BaseModel):
     """
     Configuration for a Worker that performs a GET against a given Url.  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of worker")
     url: constr(strict=True, max_length=2048, min_length=1) = Field(..., description="The URL to check, eg: https://www.google.com/")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, validator
 
 class HealthCheckResponse(BaseModel):
     """
     Readonly configuration for a Worker that performs a GET against a given Url.  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of worker")
     url: Optional[StrictStr] = Field(None, description="The URL to check, eg: https://www.google.com/")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/initial_state.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/initial_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 
 class InitialState(BaseModel):
     """
     Defines the Initial State of the Task  # noqa: E501
     """
     name: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The Initial State of the Task")
     required_fields: Optional[conlist(StrictStr)] = Field(None, alias="requiredFields", description="Required input Fields for the Initial State")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/link.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class Link(BaseModel):
     """
     Link
     """
     relation: StrictStr = Field(...)
     href: StrictStr = Field(...)
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class LuminesceView(BaseModel):
     """
     Configuration for a Worker that calls a Luminesce view  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of worker")
     name: constr(strict=True, max_length=512, min_length=1) = Field(..., description="Name of the view in Luminesce")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, validator
 
 class LuminesceViewResponse(BaseModel):
     """
     Readonly configuration for a Worker that calls a Luminesce view  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of worker")
     name: Optional[StrictStr] = Field(None, description="Name of the view in Luminesce")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_problem_details.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr
 
 class LusidProblemDetails(BaseModel):
     """
     LusidProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr
 
 class LusidValidationProblemDetails(BaseModel):
     """
     LusidValidationProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.task import Task
 
 class PagedResourceListOfTask(BaseModel):
     """
     PagedResourceListOfTask
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.task_definition import TaskDefinition
 
 class PagedResourceListOfTaskDefinition(BaseModel):
     """
     PagedResourceListOfTaskDefinition
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.worker import Worker
 
 class PagedResourceListOfWorker(BaseModel):
     """
     PagedResourceListOfWorker
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, constr
 
 class Parameter(BaseModel):
     """
     Defines a Worker Parameter  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of this Parameter")
     name: constr(strict=True, min_length=1) = Field(..., description="Name")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter_value.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class ParameterValue(BaseModel):
     """
     Defines a Parameter Value  # noqa: E501
     """
     name: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="Name")
     value: Optional[Any] = Field(None, description="Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_id.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class ResourceId(BaseModel):
     """
     ResourceId
     """
     scope: StrictStr = Field(...)
     code: StrictStr = Field(...)
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_list_of_task.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_list_of_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.task import Task
 
 class ResourceListOfTask(BaseModel):
     """
     ResourceListOfTask
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_field.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, constr
 
 class ResultField(BaseModel):
     """
     Defines a Worker Result Field  # noqa: E501
     """
     name: constr(strict=True, min_length=1) = Field(..., description="Name")
     type: constr(strict=True, min_length=1) = Field(..., description="The type of this Parameter")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_matching_pattern.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class ResultMatchingPattern(BaseModel):
     """
     Standard Finbourne filter to match against Run Worker results  # noqa: E501
     """
     filter: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="Filter string")
     __properties = ["filter"]
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
 
 class ResultantChildTaskConfiguration(BaseModel):
     """
     Child Task Configuration  # noqa: E501
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, conlist, constr, validator
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
 
 class RunWorkerAction(BaseModel):
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
 
 class RunWorkerActionResponse(BaseModel):
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_request.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from lusid_workflow.models.parameter_value import ParameterValue
 
 class RunWorkerRequest(BaseModel):
     """
     Request to Create a new worker  # noqa: E501
     """
     parameters: conlist(ParameterValue) = Field(..., description="The Parameter and their values.")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr
 
 class RunWorkerResponse(BaseModel):
     """
     The RunWorker response  # noqa: E501
     """
     run_id: StrictInt = Field(..., alias="runId", description="Identifies a Worker run")
     status_detail: Optional[StrictStr] = Field(None, alias="statusDetail", description="Detail on the final status")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class Sleep(BaseModel):
     """
     Configuration for a Worker that Sleeps for a user-defined amount of time  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of worker")
     __properties = ["type"]
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class SleepResponse(BaseModel):
     """
     Configuration for a Worker that Sleeps for a user-defined amount of time  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of worker")
     __properties = ["type"]
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/stack.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr
 
 class Stack(BaseModel):
     """
     Information pertaining to the Tasks Stack if one is present  # noqa: E501
     """
     member_added_as_at: Optional[datetime] = Field(None, alias="memberAddedAsAt", description="When the Task was added to the Stack")
     stack_opened_as_at: Optional[datetime] = Field(None, alias="stackOpenedAsAt", description="When the Stack was opened")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, constr
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.stack import Stack
 from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
 from lusid_workflow.models.task_instance_field import TaskInstanceField
 from lusid_workflow.models.task_summary import TaskSummary
 from lusid_workflow.models.version_info import VersionInfo
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.task_field_definition import TaskFieldDefinition
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition_version.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 
 class TaskDefinitionVersion(BaseModel):
     """
     The version of the Task Definition used by this Task  # noqa: E501
     """
     as_at_modified: Optional[datetime] = Field(None, alias="asAtModified", description="The asAt datetime of the Task Definition used by this Task")
     __properties = ["asAtModified"]
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_field_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class TaskFieldDefinition(BaseModel):
     """
     Defines a Task Definition Field  # noqa: E501
     """
     name: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The name of this Field")
     type: constr(strict=True, min_length=1) = Field(..., description="The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_instance_field.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_instance_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class TaskInstanceField(BaseModel):
     """
     Defines a Field on a Task  # noqa: E501
     """
     name: constr(strict=True) = Field(..., description="The name of this Field")
     value: Optional[Any] = Field(None, description="The value of this Field")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_state_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_state_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class TaskStateDefinition(BaseModel):
     """
     A Task Definition/Task has a given set of States  # noqa: E501
     """
     name: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The Name of this State")
     __properties = ["name"]
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_summary.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, constr
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
 
 class TaskSummary(BaseModel):
     """
     Summary of a Task created based on a Task Definition  # noqa: E501
     """
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_transition_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_transition_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class TaskTransitionDefinition(BaseModel):
     """
     Defines a State change  # noqa: E501
     """
     from_state: constr(strict=True, max_length=1024, min_length=1) = Field(..., alias="fromState", description="The State this Transition if coming From")
     to_state: constr(strict=True, max_length=1024, min_length=1) = Field(..., alias="toState", description="The State this Transition is going To")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/transition_trigger_definition.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 from lusid_workflow.models.trigger_schema import TriggerSchema
 
 class TransitionTriggerDefinition(BaseModel):
     """
     State changes happen in response to Triggers  # noqa: E501
     """
     name: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The key/Name of this Trigger")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class TriggerParentTaskAction(BaseModel):
     """
     Defines a Trigger Parent Task Action  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="Type name for this Action")
     trigger: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="Trigger on parent task to be invoked")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, validator
 
 class TriggerParentTaskActionResponse(BaseModel):
     """
     Defines a read-only Trigger Parent Task Action  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="Type name for this Action")
     trigger: Optional[StrictStr] = Field(None, description="Trigger on parent task to be invoked")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_schema.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class TriggerSchema(BaseModel):
     """
     Triggers can operate in response to different stimuli  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of Trigger; available value(s): External")
     __properties = ["type"]
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_definition_request.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.task_field_definition import TaskFieldDefinition
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_request.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_workflow.models.task_instance_field import TaskInstanceField
 
 class UpdateTaskRequest(BaseModel):
     """
     A request to update a Task  # noqa: E501
     """
     correlation_ids: Optional[conlist(StrictStr)] = Field(None, alias="correlationIds", description="A set of guid identifiers that allow correlation across the application tier")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/version_info.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/version_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr
 
 class VersionInfo(BaseModel):
     """
     The version metadata.  # noqa: E501
     """
     as_at_created: Optional[datetime] = Field(None, alias="asAtCreated", description="The asAt datetime at which this entity was first created.")
     user_id_created: Optional[StrictStr] = Field(None, alias="userIdCreated", description="The unique id of the user who created this entity.")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.parameter import Parameter
 from lusid_workflow.models.resource_id import ResourceId
 from lusid_workflow.models.result_field import ResultField
 from lusid_workflow.models.version_info import VersionInfo
 from lusid_workflow.models.worker_configuration_response import WorkerConfigurationResponse
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,34 +19,37 @@
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.luminesce_view import LuminesceView
+from lusid_workflow.models.scheduler_job import SchedulerJob
 from lusid_workflow.models.sleep import Sleep
 from typing import Union, Any, List, TYPE_CHECKING
 from pydantic import StrictStr, Field
 
-WORKERCONFIGURATION_ONE_OF_SCHEMAS = ["Fail", "HealthCheck", "LuminesceView", "Sleep"]
+WORKERCONFIGURATION_ONE_OF_SCHEMAS = ["Fail", "HealthCheck", "LuminesceView", "SchedulerJob", "Sleep"]
 
 class WorkerConfiguration(BaseModel):
     """
     Information about how the worker should be executed
     """
     # data type: Fail
     oneof_schema_1_validator: Optional[Fail] = None
     # data type: HealthCheck
     oneof_schema_2_validator: Optional[HealthCheck] = None
     # data type: LuminesceView
     oneof_schema_3_validator: Optional[LuminesceView] = None
+    # data type: SchedulerJob
+    oneof_schema_4_validator: Optional[SchedulerJob] = None
     # data type: Sleep
-    oneof_schema_4_validator: Optional[Sleep] = None
+    oneof_schema_5_validator: Optional[Sleep] = None
     if TYPE_CHECKING:
-        actual_instance: Union[Fail, HealthCheck, LuminesceView, Sleep]
+        actual_instance: Union[Fail, HealthCheck, LuminesceView, SchedulerJob, Sleep]
     else:
         actual_instance: Any
     one_of_schemas: List[str] = Field(WORKERCONFIGURATION_ONE_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
@@ -76,25 +79,30 @@
         else:
             match += 1
         # validate data type: LuminesceView
         if not isinstance(v, LuminesceView):
             error_messages.append(f"Error! Input type `{type(v)}` is not `LuminesceView`")
         else:
             match += 1
+        # validate data type: SchedulerJob
+        if not isinstance(v, SchedulerJob):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `SchedulerJob`")
+        else:
+            match += 1
         # validate data type: Sleep
         if not isinstance(v, Sleep):
             error_messages.append(f"Error! Input type `{type(v)}` is not `Sleep`")
         else:
             match += 1
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, Sleep. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, SchedulerJob, Sleep. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, Sleep. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, SchedulerJob, Sleep. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> WorkerConfiguration:
         return cls.from_json(json.dumps(obj))
 
@@ -119,27 +127,33 @@
             error_messages.append(str(e))
         # deserialize data into LuminesceView
         try:
             instance.actual_instance = LuminesceView.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # deserialize data into SchedulerJob
+        try:
+            instance.actual_instance = SchedulerJob.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # deserialize data into Sleep
         try:
             instance.actual_instance = Sleep.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, Sleep. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, SchedulerJob, Sleep. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, Sleep. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into WorkerConfiguration with oneOf schemas: Fail, HealthCheck, LuminesceView, SchedulerJob, Sleep. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration_response.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,34 +19,37 @@
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.health_check_response import HealthCheckResponse
 from lusid_workflow.models.luminesce_view_response import LuminesceViewResponse
+from lusid_workflow.models.scheduler_job_response import SchedulerJobResponse
 from lusid_workflow.models.sleep_response import SleepResponse
 from typing import Union, Any, List, TYPE_CHECKING
 from pydantic import StrictStr, Field
 
-WORKERCONFIGURATIONRESPONSE_ONE_OF_SCHEMAS = ["FailResponse", "HealthCheckResponse", "LuminesceViewResponse", "SleepResponse"]
+WORKERCONFIGURATIONRESPONSE_ONE_OF_SCHEMAS = ["FailResponse", "HealthCheckResponse", "LuminesceViewResponse", "SchedulerJobResponse", "SleepResponse"]
 
 class WorkerConfigurationResponse(BaseModel):
     """
     Readonly information about how the worker should be executed
     """
     # data type: FailResponse
     oneof_schema_1_validator: Optional[FailResponse] = None
     # data type: HealthCheckResponse
     oneof_schema_2_validator: Optional[HealthCheckResponse] = None
     # data type: LuminesceViewResponse
     oneof_schema_3_validator: Optional[LuminesceViewResponse] = None
+    # data type: SchedulerJobResponse
+    oneof_schema_4_validator: Optional[SchedulerJobResponse] = None
     # data type: SleepResponse
-    oneof_schema_4_validator: Optional[SleepResponse] = None
+    oneof_schema_5_validator: Optional[SleepResponse] = None
     if TYPE_CHECKING:
-        actual_instance: Union[FailResponse, HealthCheckResponse, LuminesceViewResponse, SleepResponse]
+        actual_instance: Union[FailResponse, HealthCheckResponse, LuminesceViewResponse, SchedulerJobResponse, SleepResponse]
     else:
         actual_instance: Any
     one_of_schemas: List[str] = Field(WORKERCONFIGURATIONRESPONSE_ONE_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
@@ -76,25 +79,30 @@
         else:
             match += 1
         # validate data type: LuminesceViewResponse
         if not isinstance(v, LuminesceViewResponse):
             error_messages.append(f"Error! Input type `{type(v)}` is not `LuminesceViewResponse`")
         else:
             match += 1
+        # validate data type: SchedulerJobResponse
+        if not isinstance(v, SchedulerJobResponse):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `SchedulerJobResponse`")
+        else:
+            match += 1
         # validate data type: SleepResponse
         if not isinstance(v, SleepResponse):
             error_messages.append(f"Error! Input type `{type(v)}` is not `SleepResponse`")
         else:
             match += 1
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SleepResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SchedulerJobResponse, SleepResponse. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SleepResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SchedulerJobResponse, SleepResponse. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> WorkerConfigurationResponse:
         return cls.from_json(json.dumps(obj))
 
@@ -119,27 +127,33 @@
             error_messages.append(str(e))
         # deserialize data into LuminesceViewResponse
         try:
             instance.actual_instance = LuminesceViewResponse.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # deserialize data into SchedulerJobResponse
+        try:
+            instance.actual_instance = SchedulerJobResponse.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # deserialize data into SleepResponse
         try:
             instance.actual_instance = SleepResponse.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SleepResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SchedulerJobResponse, SleepResponse. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SleepResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into WorkerConfigurationResponse with oneOf schemas: FailResponse, HealthCheckResponse, LuminesceViewResponse, SchedulerJobResponse, SleepResponse. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_status_triggers.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_status_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class WorkerStatusTriggers(BaseModel):
     """
     Defines triggers that will be invoked per Worker outcome  # noqa: E501
     """
     started: Optional[StrictStr] = Field(None, description="Trigger to invoke when the Worker has Started")
     completed_with_results: Optional[StrictStr] = Field(None, alias="completedWithResults", description="Trigger to invoke when the Worker has Completed (with results)")
```

### Comparing `lusid_workflow_sdk-2.0.9/lusid_workflow/rest.py` & `lusid_workflow_sdk-2.1.1/lusid_workflow/rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,15 +112,18 @@
         # url already contains the URL query string
         # so reset query_params to empty dict
         query_params = {}
         timeout = _request_timeout or 5 * 60
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/json'
-
+        
+        for content in headers:
+            headers[content] = str(headers[content])
+            
         args = {
             "method": method,
             "url": url,
             "timeout": timeout,
             "headers": headers
         }
 
@@ -155,15 +158,15 @@
                     else:
                         data.add_field(k, v)
                 args["data"] = data
 
             # Pass a `bytes` parameter directly in the body to support
             # other content types than Json when `body` argument is provided
             # in serialized form
-            elif isinstance(body, bytes):
+            elif isinstance(body, str) or isinstance(body, bytes):
                 args["data"] = body
             else:
                 # Cannot generate the request from given parameters
                 msg = """Cannot prepare a request message for provided
                          arguments. Please check that your arguments match
                          declared content type."""
                 raise ApiException(status=0, reason=msg)
```

### Comparing `lusid_workflow_sdk-2.0.9/pyproject.toml` & `lusid_workflow_sdk-2.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-workflow-sdk"
-version = "2.0.9"
+version = "2.1.1"
 description = "FINBOURNE Workflow API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/workflow-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Workflow API", "lusid-workflow-sdk"]
 packages = [
@@ -15,15 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 urllib3 = "^1.25.3"
 python-dateutil = "^2.8.2"
 requests = "^2"
 aiohttp = "^3.8.4"
-pydantic = "^1.10.5"
+pydantic = "^2.6.3"
 aenum = "^3.1.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0"
 flake8 = "^4.0.0"
 black = "^23.9.1"
```

### Comparing `lusid_workflow_sdk-2.0.9/PKG-INFO` & `lusid_workflow_sdk-2.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-workflow-sdk
-Version: 2.0.9
+Version: 2.1.1
 Summary: FINBOURNE Workflow API
 Home-page: https://github.com/finbourne/workflow-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Workflow API,lusid-workflow-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
 Project-URL: Repository, https://github.com/finbourne/workflow-sdk-python
 Description-Content-Type: text/markdown
 
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.674
-- Package version: 2.0.9
+- API version: 0.1.878
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -69,29 +69,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_workflow application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_WORKFLOW_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_WORKFLOW_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_workflow via a proxy, by setting `FBN_PROXY_ADDRESS`. 
+If your proxy has basic auth enabled, you must akso supply `FBN_PROXY_USERNAME` and `FBN_PROXY_PASSWORD`
+
+### Secrets file
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set in a `secrets.json` file in the same folder as your script.
+
+``` 
+{
+    "api":
+    {
+        "tokenUrl":"<your-token-url>",
+        "lusid_workflowUrl":"<FINBOURNE-application-url>",
+        "username":"<your-username>",
+        "password":"<your-password>",
+        "clientId":"<your-client-id>",
+        "clientSecret":"<your-client-secret>",
+    }
+}
+```
+
+To use a long lived Personal Access Token, you must provide a `secrets.json` with the following variables:
+``` 
+{
+    "api":
+    {
+        "lusid_workflowUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_workflow via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_workflowUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    },
+    "proxy":
+    {
+        "address":"<your-proxy-address>",
+        "username":"<your-proxy-username>",
+        "password":"<your-proxy-password>"
+    }
+}
+```
+
+### Using the SDK
+
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
 import lusid_workflow
-from lusid_workflow.rest import ApiException
+from lusid_workflow.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_workflow import (
-	  ApiClientFactory,
-	  ApplicationMetadataApi,
-	  EnvironmentVariablesConfigurationLoader,
-	  SecretsFileConfigurationLoader,
-	  ArgsConfigurationLoader
+    ApiClientFactory,
+    EventHandlersApi,
+    EnvironmentVariablesConfigurationLoader,
+    SecretsFileConfigurationLoader,
+    ArgsConfigurationLoader
 )
 
 # Use the lusid_workflow ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -116,64 +192,71 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_workflow.TaskDefinitionsApi(api_client)
-    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
+    api_instance = api_client_factory.build(EventHandlersApi)
+    create_event_handler_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example Event Handler","description":"Test","status":"Active","eventMatchingPattern":{"eventType":"PortfolioCreated","filter":"body.scope eq 'TestScope'"},"runAsUserId":{"setTo":"ExampleUserId"},"taskDefinitionId":{"scope":"A1","code":"YYY"},"taskDefinitionAsAt":"9999-12-31T23:59:59.9999999+00:00","taskActivity":{"InitialTrigger":"InitialTrigger","Type":"CreateNewTask","CorrelationIds":[],"TaskFields":{}}} # CreateEventHandlerRequest | The data to create an Event Handler
 
     try:
-        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
-        api_response = await api_instance.create_task_definition(create_task_definition_request)
-        print("The response of TaskDefinitionsApi->create_task_definition:\n")
+        # [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
+        api_response = await api_instance.create_event_handler(create_event_handler_request)
+        print("The response of EventHandlersApi->create_event_handler:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
+        print("Exception when calling EventHandlersApi->create_event_handler: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*EventHandlersApi* | [**create_event_handler**](docs/EventHandlersApi.md#create_event_handler) | **POST** /api/eventhandlers | [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
 *TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
 *TasksApi* | [**delete_task**](docs/TasksApi.md#delete_task) | **DELETE** /api/tasks/{id} | [EXPERIMENTAL] DeleteTask: Delete a Task
 *TasksApi* | [**get_task**](docs/TasksApi.md#get_task) | **GET** /api/tasks/{id} | [EXPERIMENTAL] GetTask: Get a Task
 *TasksApi* | [**list_tasks**](docs/TasksApi.md#list_tasks) | **GET** /api/tasks | [EXPERIMENTAL] ListTasks: List Tasks
 *TasksApi* | [**update_task**](docs/TasksApi.md#update_task) | **POST** /api/tasks/{id} | [EXPERIMENTAL] UpdateTask: Update a Task
 *WorkersApi* | [**create_worker**](docs/WorkersApi.md#create_worker) | **POST** /api/workers | [EXPERIMENTAL] CreateWorker: Create a new Worker
+*WorkersApi* | [**delete_worker**](docs/WorkersApi.md#delete_worker) | **DELETE** /api/workers/{scope}/{code} | [EXPERIMENTAL] DeleteWorker: Delete a Worker
 *WorkersApi* | [**get_worker**](docs/WorkersApi.md#get_worker) | **GET** /api/workers/{scope}/{code} | [EXPERIMENTAL] GetWorker: Get a Worker
 *WorkersApi* | [**get_worker_result**](docs/WorkersApi.md#get_worker_result) | **GET** /api/workers/{runId}/$result | [EXPERIMENTAL] GetWorkerResult: Get the status of a specific run of a worker with any relevant results
 *WorkersApi* | [**list_workers**](docs/WorkersApi.md#list_workers) | **GET** /api/workers | [EXPERIMENTAL] ListWorkers: List Workers
 *WorkersApi* | [**run_worker**](docs/WorkersApi.md#run_worker) | **POST** /api/workers/{scope}/{code}/$run | [EXPERIMENTAL] RunWorker: Run a Worker
+*WorkersApi* | [**update_worker**](docs/WorkersApi.md#update_worker) | **PUT** /api/workers/{scope}/{code} | [EXPERIMENTAL] UpdateWorker: Update a Worker
 
 
 ## Documentation For Models
 
  - [ActionDefinition](docs/ActionDefinition.md)
  - [ActionDefinitionResponse](docs/ActionDefinitionResponse.md)
  - [ActionDetails](docs/ActionDetails.md)
  - [ActionDetailsResponse](docs/ActionDetailsResponse.md)
  - [CreateChildTaskConfiguration](docs/CreateChildTaskConfiguration.md)
  - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateChildTasksActionResponse](docs/CreateChildTasksActionResponse.md)
+ - [CreateEventHandlerRequest](docs/CreateEventHandlerRequest.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
+ - [EventHandler](docs/EventHandler.md)
+ - [EventHandlerMapping](docs/EventHandlerMapping.md)
+ - [EventMatchingPattern](docs/EventMatchingPattern.md)
  - [Fail](docs/Fail.md)
  - [FailResponse](docs/FailResponse.md)
  - [FieldMapping](docs/FieldMapping.md)
  - [GetWorkerResultResponse](docs/GetWorkerResultResponse.md)
  - [HealthCheck](docs/HealthCheck.md)
  - [HealthCheckResponse](docs/HealthCheckResponse.md)
  - [InitialState](docs/InitialState.md)
@@ -192,14 +275,16 @@
  - [ResultField](docs/ResultField.md)
  - [ResultMatchingPattern](docs/ResultMatchingPattern.md)
  - [ResultantChildTaskConfiguration](docs/ResultantChildTaskConfiguration.md)
  - [RunWorkerAction](docs/RunWorkerAction.md)
  - [RunWorkerActionResponse](docs/RunWorkerActionResponse.md)
  - [RunWorkerRequest](docs/RunWorkerRequest.md)
  - [RunWorkerResponse](docs/RunWorkerResponse.md)
+ - [SchedulerJob](docs/SchedulerJob.md)
+ - [SchedulerJobResponse](docs/SchedulerJobResponse.md)
  - [Sleep](docs/Sleep.md)
  - [SleepResponse](docs/SleepResponse.md)
  - [Stack](docs/Stack.md)
  - [Task](docs/Task.md)
  - [TaskDefinition](docs/TaskDefinition.md)
  - [TaskDefinitionVersion](docs/TaskDefinitionVersion.md)
  - [TaskFieldDefinition](docs/TaskFieldDefinition.md)
@@ -209,14 +294,15 @@
  - [TaskTransitionDefinition](docs/TaskTransitionDefinition.md)
  - [TransitionTriggerDefinition](docs/TransitionTriggerDefinition.md)
  - [TriggerParentTaskAction](docs/TriggerParentTaskAction.md)
  - [TriggerParentTaskActionResponse](docs/TriggerParentTaskActionResponse.md)
  - [TriggerSchema](docs/TriggerSchema.md)
  - [UpdateTaskDefinitionRequest](docs/UpdateTaskDefinitionRequest.md)
  - [UpdateTaskRequest](docs/UpdateTaskRequest.md)
+ - [UpdateWorkerRequest](docs/UpdateWorkerRequest.md)
  - [VersionInfo](docs/VersionInfo.md)
  - [Worker](docs/Worker.md)
  - [WorkerConfiguration](docs/WorkerConfiguration.md)
  - [WorkerConfigurationResponse](docs/WorkerConfigurationResponse.md)
  - [WorkerStatusTriggers](docs/WorkerStatusTriggers.md)
```

