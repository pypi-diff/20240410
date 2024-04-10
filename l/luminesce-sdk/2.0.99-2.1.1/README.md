# Comparing `tmp/luminesce_sdk-2.0.99.tar.gz` & `tmp/luminesce_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luminesce_sdk-2.0.99.tar", max compression
+gzip compressed data, was "luminesce_sdk-2.1.1.tar", max compression
```

## Comparing `luminesce_sdk-2.0.99.tar` & `luminesce_sdk-2.1.1.tar`

### file list

```diff
@@ -1,86 +1,95 @@
--rw-r--r--   0        0        0    20827 2024-02-24 16:21:55.042354 luminesce_sdk-2.0.99/README.md
--rw-r--r--   0        0        0     5065 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/__init__.py
--rw-r--r--   0        0        0      717 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/api/__init__.py
--rw-r--r--   0        0        0     8541 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/application_metadata_api.py
--rw-r--r--   0        0        0    11770 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/binary_downloading_api.py
--rw-r--r--   0        0        0    31266 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/certificate_management_api.py
--rw-r--r--   0        0        0    11798 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/current_table_field_catalog_api.py
--rw-r--r--   0        0        0    66228 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/historically_executed_queries_api.py
--rw-r--r--   0        0        0    38556 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/multi_query_execution_api.py
--rw-r--r--   0        0        0   238141 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/api/sql_background_execution_api.py
--rw-r--r--   0        0        0    88580 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/api/sql_design_api.py
--rw-r--r--   0        0        0   147995 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/api/sql_execution_api.py
--rw-r--r--   0        0        0    30755 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/api_client.py
--rw-r--r--   0        0        0      852 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/api_response.py
--rw-r--r--   0        0        0    14449 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/configuration.py
--rw-r--r--   0        0        0     5344 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/exceptions.py
--rw-r--r--   0        0        0      284 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/__init__.py
--rw-r--r--   0        0        0    30617 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/api_client.py
--rw-r--r--   0        0        0     9713 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8072 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/api_configuration.py
--rw-r--r--   0        0        0     6776 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12702 2024-02-24 16:21:55.039354 luminesce_sdk-2.0.99/luminesce/extensions/rest.py
--rw-r--r--   0        0        0    11568 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-02-24 16:21:55.039354 luminesce_sdk-2.0.99/luminesce/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3881 2024-02-24 16:21:55.039354 luminesce_sdk-2.0.99/luminesce/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3907 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/__init__.py
--rw-r--r--   0        0        0     3396 2024-02-24 16:21:55.034354 luminesce_sdk-2.0.99/luminesce/models/access_controlled_action.py
--rw-r--r--   0        0        0     4671 2024-02-24 16:21:55.034354 luminesce_sdk-2.0.99/luminesce/models/access_controlled_resource.py
--rw-r--r--   0        0        0     3960 2024-02-24 16:21:55.034354 luminesce_sdk-2.0.99/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py
--rw-r--r--   0        0        0     2072 2024-02-24 16:21:55.034354 luminesce_sdk-2.0.99/luminesce/models/action_id.py
--rw-r--r--   0        0        0      828 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/aggregate_function.py
--rw-r--r--   0        0        0     2315 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/aggregation.py
--rw-r--r--   0        0        0      802 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/auto_detect_type.py
--rw-r--r--   0        0        0     3204 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/available_field.py
--rw-r--r--   0        0        0     2936 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/available_parameter.py
--rw-r--r--   0        0        0     4234 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/background_multi_query_progress_response.py
--rw-r--r--   0        0        0    10650 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/background_multi_query_response.py
--rw-r--r--   0        0        0     2757 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/background_query_cancel_response.py
--rw-r--r--   0        0        0     5674 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/background_query_progress_response.py
--rw-r--r--   0        0        0     6282 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/background_query_response.py
--rw-r--r--   0        0        0     1055 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/background_query_state.py
--rw-r--r--   0        0        0      808 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/certificate_action.py
--rw-r--r--   0        0        0      778 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/certificate_file_type.py
--rw-r--r--   0        0        0     7168 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/certificate_state.py
--rw-r--r--   0        0        0      847 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/certificate_status.py
--rw-r--r--   0        0        0      716 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/certificate_type.py
--rw-r--r--   0        0        0     5105 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/column.py
--rw-r--r--   0        0        0     2856 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/column_info.py
--rw-r--r--   0        0        0      738 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/condition_attributes.py
--rw-r--r--   0        0        0     5190 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/convert_to_view_data.py
--rw-r--r--   0        0        0      789 2024-02-24 16:21:55.035354 luminesce_sdk-2.0.99/luminesce/models/data_type.py
--rw-r--r--   0        0        0     2586 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/expression_with_alias.py
--rw-r--r--   0        0        0     4092 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/feedback_event_args.py
--rw-r--r--   0        0        0      994 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/feedback_level.py
--rw-r--r--   0        0        0     4545 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/field_design.py
--rw-r--r--   0        0        0      654 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/field_type.py
--rw-r--r--   0        0        0     8352 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/file_reader_builder_def.py
--rw-r--r--   0        0        0     2207 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/filter_term_design.py
--rw-r--r--   0        0        0     3177 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/id_selector_definition.py
--rw-r--r--   0        0        0     2264 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/link.py
--rw-r--r--   0        0        0     1415 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/luminesce_binary_type.py
--rw-r--r--   0        0        0     3859 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/lusid_problem_details.py
--rw-r--r--   0        0        0     5201 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/mappable_field.py
--rw-r--r--   0        0        0      711 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/mapping_flags.py
--rw-r--r--   0        0        0     1099 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/multi_query_definition_type.py
--rw-r--r--   0        0        0     6319 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/options_csv.py
--rw-r--r--   0        0        0     5380 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/options_excel.py
--rw-r--r--   0        0        0     2310 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/options_parquet.py
--rw-r--r--   0        0        0     2216 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/options_sq_lite.py
--rw-r--r--   0        0        0     4488 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/options_xml.py
--rw-r--r--   0        0        0      707 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/order_by_direction.py
--rw-r--r--   0        0        0     2146 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/order_by_term_design.py
--rw-r--r--   0        0        0     5693 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/query_design.py
--rw-r--r--   0        0        0      884 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/query_designer_binary_operator.py
--rw-r--r--   0        0        0     4247 2024-02-24 16:21:55.036354 luminesce_sdk-2.0.99/luminesce/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     2325 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/source.py
--rw-r--r--   0        0        0      770 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/source_type.py
--rw-r--r--   0        0        0      897 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/task_status.py
--rw-r--r--   0        0        0     2988 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/view_parameter.py
--rw-r--r--   0        0        0     4491 2024-02-24 16:21:55.037354 luminesce_sdk-2.0.99/luminesce/models/writer_design.py
--rw-r--r--   0        0        0        0 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/py.typed
--rw-r--r--   0        0        0    10029 2024-02-24 16:21:55.038354 luminesce_sdk-2.0.99/luminesce/rest.py
--rw-r--r--   0        0        0      848 2024-02-24 16:21:55.042354 luminesce_sdk-2.0.99/pyproject.toml
--rw-r--r--   0        0        0    21876 1970-01-01 00:00:00.000000 luminesce_sdk-2.0.99/PKG-INFO
+-rw-r--r--   0        0        0    21799 2024-04-10 09:46:39.409819 luminesce_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     8148 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-10 09:46:39.401820 luminesce_sdk-2.1.1/luminesce/api/__init__.py
+-rw-r--r--   0        0        0     8541 2024-04-10 09:46:39.400820 luminesce_sdk-2.1.1/luminesce/api/application_metadata_api.py
+-rw-r--r--   0        0        0    12072 2024-04-10 09:46:39.400820 luminesce_sdk-2.1.1/luminesce/api/binary_downloading_api.py
+-rw-r--r--   0        0        0    31266 2024-04-10 09:46:39.400820 luminesce_sdk-2.1.1/luminesce/api/certificate_management_api.py
+-rw-r--r--   0        0        0    11798 2024-04-10 09:46:39.400820 luminesce_sdk-2.1.1/luminesce/api/current_table_field_catalog_api.py
+-rw-r--r--   0        0        0    66228 2024-04-10 09:46:39.400820 luminesce_sdk-2.1.1/luminesce/api/historically_executed_queries_api.py
+-rw-r--r--   0        0        0    38556 2024-04-10 09:46:39.401820 luminesce_sdk-2.1.1/luminesce/api/multi_query_execution_api.py
+-rw-r--r--   0        0        0   238141 2024-04-10 09:46:39.401820 luminesce_sdk-2.1.1/luminesce/api/sql_background_execution_api.py
+-rw-r--r--   0        0        0   104251 2024-04-10 09:46:39.401820 luminesce_sdk-2.1.1/luminesce/api/sql_design_api.py
+-rw-r--r--   0        0        0   147995 2024-04-10 09:46:39.401820 luminesce_sdk-2.1.1/luminesce/api/sql_execution_api.py
+-rw-r--r--   0        0        0    30755 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/api_response.py
+-rw-r--r--   0        0        0    14449 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/configuration.py
+-rw-r--r--   0        0        0     5344 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/exceptions.py
+-rw-r--r--   0        0        0      572 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/__init__.py
+-rw-r--r--   0        0        0    30617 2024-04-10 09:46:39.406819 luminesce_sdk-2.1.1/luminesce/extensions/api_client.py
+-rw-r--r--   0        0        0     9812 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8072 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6776 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12702 2024-04-10 09:46:39.406819 luminesce_sdk-2.1.1/luminesce/extensions/rest.py
+-rw-r--r--   0        0        0    11568 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 09:46:39.406819 luminesce_sdk-2.1.1/luminesce/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3881 2024-04-10 09:46:39.406819 luminesce_sdk-2.1.1/luminesce/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     6159 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/__init__.py
+-rw-r--r--   0        0        0     3396 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4671 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     3960 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py
+-rw-r--r--   0        0        0     2072 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/action_id.py
+-rw-r--r--   0        0        0      828 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/aggregate_function.py
+-rw-r--r--   0        0        0     2315 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/aggregation.py
+-rw-r--r--   0        0        0      802 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/auto_detect_type.py
+-rw-r--r--   0        0        0     3204 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/available_field.py
+-rw-r--r--   0        0        0     2936 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/available_parameter.py
+-rw-r--r--   0        0        0     4234 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/background_multi_query_progress_response.py
+-rw-r--r--   0        0        0    10650 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/background_multi_query_response.py
+-rw-r--r--   0        0        0     2757 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/background_query_cancel_response.py
+-rw-r--r--   0        0        0     5674 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/background_query_progress_response.py
+-rw-r--r--   0        0        0     6282 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/background_query_response.py
+-rw-r--r--   0        0        0     1055 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/background_query_state.py
+-rw-r--r--   0        0        0      808 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/certificate_action.py
+-rw-r--r--   0        0        0      778 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/certificate_file_type.py
+-rw-r--r--   0        0        0     7168 2024-04-10 09:46:39.402819 luminesce_sdk-2.1.1/luminesce/models/certificate_state.py
+-rw-r--r--   0        0        0      847 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/certificate_status.py
+-rw-r--r--   0        0        0      716 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/certificate_type.py
+-rw-r--r--   0        0        0     5105 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/column.py
+-rw-r--r--   0        0        0     2856 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/column_info.py
+-rw-r--r--   0        0        0      738 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/condition_attributes.py
+-rw-r--r--   0        0        0     5190 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/convert_to_view_data.py
+-rw-r--r--   0        0        0     2052 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/cursor_position.py
+-rw-r--r--   0        0        0      789 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/data_type.py
+-rw-r--r--   0        0        0     3342 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/error_highlight_item.py
+-rw-r--r--   0        0        0     2383 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/error_highlight_request.py
+-rw-r--r--   0        0        0     2699 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/error_highlight_response.py
+-rw-r--r--   0        0        0     2586 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/expression_with_alias.py
+-rw-r--r--   0        0        0     4092 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/feedback_event_args.py
+-rw-r--r--   0        0        0      994 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/feedback_level.py
+-rw-r--r--   0        0        0     4545 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/field_design.py
+-rw-r--r--   0        0        0      654 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/field_type.py
+-rw-r--r--   0        0        0     8352 2024-04-10 09:46:39.403819 luminesce_sdk-2.1.1/luminesce/models/file_reader_builder_def.py
+-rw-r--r--   0        0        0     3728 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/file_reader_builder_response.py
+-rw-r--r--   0        0        0     2207 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/filter_term_design.py
+-rw-r--r--   0        0        0     3177 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3233 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/intellisense_item.py
+-rw-r--r--   0        0        0     2402 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/intellisense_request.py
+-rw-r--r--   0        0        0     3141 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/intellisense_response.py
+-rw-r--r--   0        0        0      807 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/intellisense_type.py
+-rw-r--r--   0        0        0     2264 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/link.py
+-rw-r--r--   0        0        0     1656 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/luminesce_binary_type.py
+-rw-r--r--   0        0        0     3859 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     5201 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/mappable_field.py
+-rw-r--r--   0        0        0      711 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/mapping_flags.py
+-rw-r--r--   0        0        0     1099 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/multi_query_definition_type.py
+-rw-r--r--   0        0        0     6319 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/options_csv.py
+-rw-r--r--   0        0        0     5380 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/options_excel.py
+-rw-r--r--   0        0        0     2310 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/options_parquet.py
+-rw-r--r--   0        0        0     2216 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/options_sq_lite.py
+-rw-r--r--   0        0        0     4488 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/options_xml.py
+-rw-r--r--   0        0        0      707 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/order_by_direction.py
+-rw-r--r--   0        0        0     2146 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/order_by_term_design.py
+-rw-r--r--   0        0        0     5693 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/query_design.py
+-rw-r--r--   0        0        0      884 2024-04-10 09:46:39.404820 luminesce_sdk-2.1.1/luminesce/models/query_designer_binary_operator.py
+-rw-r--r--   0        0        0     4247 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     2325 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/source.py
+-rw-r--r--   0        0        0      770 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/source_type.py
+-rw-r--r--   0        0        0      897 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/task_status.py
+-rw-r--r--   0        0        0     2988 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/view_parameter.py
+-rw-r--r--   0        0        0     4491 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/models/writer_design.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/py.typed
+-rw-r--r--   0        0        0    10160 2024-04-10 09:46:39.405820 luminesce_sdk-2.1.1/luminesce/rest.py
+-rw-r--r--   0        0        0      847 2024-04-10 09:46:39.409819 luminesce_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    22847 1970-01-01 00:00:00.000000 luminesce_sdk-2.1.1/PKG-INFO
```

### Comparing `luminesce_sdk-2.0.99/README.md` & `luminesce_sdk-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # luminesce-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.14.571
-- Package version: 2.0.99
+- API version: 1.14.936
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -56,16 +56,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_LUMINESCE_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_LUMINESCE_API_URL,
 FBN_ACCESS_TOKEN
 ```
@@ -212,14 +211,16 @@
 *SqlBackgroundExecutionApi* | [**fetch_query_result_parquet**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_parquet) | **GET** /api/SqlBackground/{executionId}/parquet | FetchQueryResultParquet: Fetches the result from a previously started query, in Parquet format.
 *SqlBackgroundExecutionApi* | [**fetch_query_result_pipe**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_pipe) | **GET** /api/SqlBackground/{executionId}/pipe | FetchQueryResultPipe: Fetches the result from a previously started query, in pipe-delimited format.
 *SqlBackgroundExecutionApi* | [**fetch_query_result_sqlite**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_sqlite) | **GET** /api/SqlBackground/{executionId}/sqlite | FetchQueryResultSqlite: Fetches the result from a previously started query, in SqLite format.
 *SqlBackgroundExecutionApi* | [**fetch_query_result_xml**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_xml) | **GET** /api/SqlBackground/{executionId}/xml | FetchQueryResultXml: Fetches the result from a previously started query, in Xml format.
 *SqlBackgroundExecutionApi* | [**get_progress_of**](docs/SqlBackgroundExecutionApi.md#get_progress_of) | **GET** /api/SqlBackground/{executionId} | GetProgressOf: View progress information (up until this point)
 *SqlBackgroundExecutionApi* | [**start_query**](docs/SqlBackgroundExecutionApi.md#start_query) | **PUT** /api/SqlBackground | StartQuery: Starts to Execute LuminesceSql in the background.
 *SqlDesignApi* | [**put_file_read_design_to_sql**](docs/SqlDesignApi.md#put_file_read_design_to_sql) | **PUT** /api/Sql/fromfilereaddesign | [EXPERIMENTAL] PutFileReadDesignToSql: Generates file read SQL from a structured query design
+*SqlDesignApi* | [**put_intellisense**](docs/SqlDesignApi.md#put_intellisense) | **PUT** /api/Sql/intellisense | [EXPERIMENTAL] PutIntellisense: Generate a set of possible intellisense prompts given a SQL snip-it (in need not yet be valid) and cursor location
+*SqlDesignApi* | [**put_intellisense_error**](docs/SqlDesignApi.md#put_intellisense_error) | **PUT** /api/Sql/intellisenseError | [EXPERIMENTAL] PutIntellisenseError: Generate a set of error ranges, if any, in the given SQL (expressed as Lines)
 *SqlDesignApi* | [**put_query_design_to_sql**](docs/SqlDesignApi.md#put_query_design_to_sql) | **PUT** /api/Sql/fromdesign | [EXPERIMENTAL] PutQueryDesignToSql: Generates SQL from a structured query design
 *SqlDesignApi* | [**put_query_to_format**](docs/SqlDesignApi.md#put_query_to_format) | **PUT** /api/Sql/pretty | PutQueryToFormat: Formats SQL into a more readable form, a.k.a. Pretty-Print the SQL.
 *SqlDesignApi* | [**put_sql_to_file_read_design**](docs/SqlDesignApi.md#put_sql_to_file_read_design) | **PUT** /api/Sql/tofilereaddesign | [EXPERIMENTAL] PutSqlToFileReadDesign: Generates a SQL-file-read-design object from SQL string, if possible.
 *SqlDesignApi* | [**put_sql_to_query_design**](docs/SqlDesignApi.md#put_sql_to_query_design) | **PUT** /api/Sql/todesign | [EXPERIMENTAL] PutSqlToQueryDesign: Generates a SQL-design object from SQL string, if possible.
 *SqlDesignApi* | [**put_sql_to_view_design**](docs/SqlDesignApi.md#put_sql_to_view_design) | **PUT** /api/Sql/toviewdesign | [EXPERIMENTAL] PutSqlToViewDesign: Generates a structured view creation design from existing view creation SQL.
 *SqlDesignApi* | [**put_sql_to_writer_design**](docs/SqlDesignApi.md#put_sql_to_writer_design) | **PUT** /api/Sql/towriterdesign | [EXPERIMENTAL] PutSqlToWriterDesign: Generates a SQL-writer-design object from SQL string, if possible.
 *SqlDesignApi* | [**put_view_design_to_sql**](docs/SqlDesignApi.md#put_view_design_to_sql) | **PUT** /api/Sql/fromviewdesign | [EXPERIMENTAL] PutViewDesignToSql: Generates view creation sql from a structured view creation design
@@ -262,23 +263,32 @@
  - [CertificateState](docs/CertificateState.md)
  - [CertificateStatus](docs/CertificateStatus.md)
  - [CertificateType](docs/CertificateType.md)
  - [Column](docs/Column.md)
  - [ColumnInfo](docs/ColumnInfo.md)
  - [ConditionAttributes](docs/ConditionAttributes.md)
  - [ConvertToViewData](docs/ConvertToViewData.md)
+ - [CursorPosition](docs/CursorPosition.md)
  - [DataType](docs/DataType.md)
+ - [ErrorHighlightItem](docs/ErrorHighlightItem.md)
+ - [ErrorHighlightRequest](docs/ErrorHighlightRequest.md)
+ - [ErrorHighlightResponse](docs/ErrorHighlightResponse.md)
  - [ExpressionWithAlias](docs/ExpressionWithAlias.md)
  - [FeedbackEventArgs](docs/FeedbackEventArgs.md)
  - [FeedbackLevel](docs/FeedbackLevel.md)
  - [FieldDesign](docs/FieldDesign.md)
  - [FieldType](docs/FieldType.md)
  - [FileReaderBuilderDef](docs/FileReaderBuilderDef.md)
+ - [FileReaderBuilderResponse](docs/FileReaderBuilderResponse.md)
  - [FilterTermDesign](docs/FilterTermDesign.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
+ - [IntellisenseItem](docs/IntellisenseItem.md)
+ - [IntellisenseRequest](docs/IntellisenseRequest.md)
+ - [IntellisenseResponse](docs/IntellisenseResponse.md)
+ - [IntellisenseType](docs/IntellisenseType.md)
  - [Link](docs/Link.md)
  - [LuminesceBinaryType](docs/LuminesceBinaryType.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [MappableField](docs/MappableField.md)
  - [MappingFlags](docs/MappingFlags.md)
  - [MultiQueryDefinitionType](docs/MultiQueryDefinitionType.md)
  - [OptionsCsv](docs/OptionsCsv.md)
```

### Comparing `luminesce_sdk-2.0.99/luminesce/api/__init__.py` & `luminesce_sdk-2.1.1/luminesce/api/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,7 +7,19 @@
 from luminesce.api.current_table_field_catalog_api import CurrentTableFieldCatalogApi
 from luminesce.api.historically_executed_queries_api import HistoricallyExecutedQueriesApi
 from luminesce.api.multi_query_execution_api import MultiQueryExecutionApi
 from luminesce.api.sql_background_execution_api import SqlBackgroundExecutionApi
 from luminesce.api.sql_design_api import SqlDesignApi
 from luminesce.api.sql_execution_api import SqlExecutionApi
 
+
+__all__ = [
+    "ApplicationMetadataApi",
+    "BinaryDownloadingApi",
+    "CertificateManagementApi",
+    "CurrentTableFieldCatalogApi",
+    "HistoricallyExecutedQueriesApi",
+    "MultiQueryExecutionApi",
+    "SqlBackgroundExecutionApi",
+    "SqlDesignApi",
+    "SqlExecutionApi"
+]
```

### Comparing `luminesce_sdk-2.0.99/luminesce/api/application_metadata_api.py` & `luminesce_sdk-2.1.1/luminesce/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api/binary_downloading_api.py` & `luminesce_sdk-2.1.1/luminesce/api/binary_downloading_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def download_binary(self, type : Annotated[Optional[LuminesceBinaryType], Field(description="Type of binary to download (each requires separate licenses and entitlements)")] = None, version : Annotated[Optional[StrictStr], Field(description="An explicit version of the binary.  Leave blank to get the latest version (recommended)")] = None, async_req: Optional[bool]=True, **kwargs) -> bytearray:  # noqa: E501
         ...
 
     @validate_arguments
     def download_binary(self, type : Annotated[Optional[LuminesceBinaryType], Field(description="Type of binary to download (each requires separate licenses and entitlements)")] = None, version : Annotated[Optional[StrictStr], Field(description="An explicit version of the binary.  Leave blank to get the latest version (recommended)")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[bytearray, Awaitable[bytearray]]:  # noqa: E501
         """[EXPERIMENTAL] DownloadBinary: Downloads the latest version (or specific if needs be) of the specified Luminesce Binary, given the required entitlements.  # noqa: E501
 
-         Downloads the latest version (or specific if needs be) of the specified Luminesce Binary, given the required entitlements.  *NOTE:* This endpoint is an alternative to time-consuming manual distribution via Drive or Email. > it relies on as underlying datastore that is not quite as \"Highly Available\" to the degree  > that FINBOURNE services generally are.   > Thus it is not subject to the same SLAs as other API endpoints are. > *If you perceive an outage, please try again later.*  Once a file has been downloaded the following steps can be used to install it:  1. Open a terminal and cd to the directory you downloaded it to 2. Install / extract files from that package via: ``` dotnet tool install NameOfFileWithoutExtension -g --add-source \".\" ``` 3. Execute them (see documentation for specific binary)...  The installed binaries can then be found in - Windows - `%USERPROFILE%\\.dotnet\\tools\\.store\\` - Linux/macOS - `$HOME/.dotnet/tools/.store/`  The following error codes are to be anticipated with standard Problem Detail reports: - 400 BadRequest - binary file is not available for some reason (e.g. permissions or invalid version) - 401 Unauthorized   # noqa: E501
+         Downloads the latest version (or specific if needs be) of the specified Luminesce Binary, given the required entitlements.  *NOTE:* This endpoint is an alternative to time-consuming manual distribution via Drive or Email. > it relies on as underlying datastore that is not quite as \"Highly Available\" to the degree  > that FINBOURNE services generally are.   > Thus it is not subject to the same SLAs as other API endpoints are. > *If you perceive an outage, please try again later.*  Once a file has been downloaded the following steps can be used to install it (for the dotnet tools at least):  1. Open a terminal and cd to the directory you downloaded it to 2. Install / extract files from that package via: ``` dotnet tool install NameOfFileWithoutVersionNumberOrExtension -g --add-source \".\" ``` e.g. ``` dotnet tool install Finbourne.Luminesce.DbProviders.Oracle_Snowflake -g --add-source \".\" ``` 3. Execute them (see documentation for specific binary)...  The installed binaries can then be found in - Windows - `%USERPROFILE%\\.dotnet\\tools\\.store\\` - Linux/macOS - `$HOME/.dotnet/tools/.store/`  The following error codes are to be anticipated with standard Problem Detail reports: - 400 BadRequest - binary file is not available for some reason (e.g. permissions or invalid version) - 401 Unauthorized   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.download_binary(type, version, async_req=True)
         >>> result = thread.get()
 
         :param type: Type of binary to download (each requires separate licenses and entitlements)
@@ -88,15 +88,15 @@
             kwargs['async_req'] = async_req
         return self.download_binary_with_http_info(type, version, **kwargs)  # noqa: E501
 
     @validate_arguments
     def download_binary_with_http_info(self, type : Annotated[Optional[LuminesceBinaryType], Field(description="Type of binary to download (each requires separate licenses and entitlements)")] = None, version : Annotated[Optional[StrictStr], Field(description="An explicit version of the binary.  Leave blank to get the latest version (recommended)")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """[EXPERIMENTAL] DownloadBinary: Downloads the latest version (or specific if needs be) of the specified Luminesce Binary, given the required entitlements.  # noqa: E501
 
-         Downloads the latest version (or specific if needs be) of the specified Luminesce Binary, given the required entitlements.  *NOTE:* This endpoint is an alternative to time-consuming manual distribution via Drive or Email. > it relies on as underlying datastore that is not quite as \"Highly Available\" to the degree  > that FINBOURNE services generally are.   > Thus it is not subject to the same SLAs as other API endpoints are. > *If you perceive an outage, please try again later.*  Once a file has been downloaded the following steps can be used to install it:  1. Open a terminal and cd to the directory you downloaded it to 2. Install / extract files from that package via: ``` dotnet tool install NameOfFileWithoutExtension -g --add-source \".\" ``` 3. Execute them (see documentation for specific binary)...  The installed binaries can then be found in - Windows - `%USERPROFILE%\\.dotnet\\tools\\.store\\` - Linux/macOS - `$HOME/.dotnet/tools/.store/`  The following error codes are to be anticipated with standard Problem Detail reports: - 400 BadRequest - binary file is not available for some reason (e.g. permissions or invalid version) - 401 Unauthorized   # noqa: E501
+         Downloads the latest version (or specific if needs be) of the specified Luminesce Binary, given the required entitlements.  *NOTE:* This endpoint is an alternative to time-consuming manual distribution via Drive or Email. > it relies on as underlying datastore that is not quite as \"Highly Available\" to the degree  > that FINBOURNE services generally are.   > Thus it is not subject to the same SLAs as other API endpoints are. > *If you perceive an outage, please try again later.*  Once a file has been downloaded the following steps can be used to install it (for the dotnet tools at least):  1. Open a terminal and cd to the directory you downloaded it to 2. Install / extract files from that package via: ``` dotnet tool install NameOfFileWithoutVersionNumberOrExtension -g --add-source \".\" ``` e.g. ``` dotnet tool install Finbourne.Luminesce.DbProviders.Oracle_Snowflake -g --add-source \".\" ``` 3. Execute them (see documentation for specific binary)...  The installed binaries can then be found in - Windows - `%USERPROFILE%\\.dotnet\\tools\\.store\\` - Linux/macOS - `$HOME/.dotnet/tools/.store/`  The following error codes are to be anticipated with standard Problem Detail reports: - 400 BadRequest - binary file is not available for some reason (e.g. permissions or invalid version) - 401 Unauthorized   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.download_binary_with_http_info(type, version, async_req=True)
         >>> result = thread.get()
 
         :param type: Type of binary to download (each requires separate licenses and entitlements)
```

### Comparing `luminesce_sdk-2.0.99/luminesce/api/certificate_management_api.py` & `luminesce_sdk-2.1.1/luminesce/api/certificate_management_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api/current_table_field_catalog_api.py` & `luminesce_sdk-2.1.1/luminesce/api/current_table_field_catalog_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api/historically_executed_queries_api.py` & `luminesce_sdk-2.1.1/luminesce/api/historically_executed_queries_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api/multi_query_execution_api.py` & `luminesce_sdk-2.1.1/luminesce/api/multi_query_execution_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api/sql_background_execution_api.py` & `luminesce_sdk-2.1.1/luminesce/api/sql_background_execution_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api/sql_design_api.py` & `luminesce_sdk-2.1.1/luminesce/api/sql_design_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 
 from typing_extensions import Annotated
 from pydantic import Field, StrictBool, StrictInt, StrictStr
 
 from typing import Optional
 
 from luminesce.models.convert_to_view_data import ConvertToViewData
+from luminesce.models.error_highlight_request import ErrorHighlightRequest
+from luminesce.models.error_highlight_response import ErrorHighlightResponse
 from luminesce.models.file_reader_builder_def import FileReaderBuilderDef
+from luminesce.models.file_reader_builder_response import FileReaderBuilderResponse
+from luminesce.models.intellisense_request import IntellisenseRequest
+from luminesce.models.intellisense_response import IntellisenseResponse
 from luminesce.models.query_design import QueryDesign
 from luminesce.models.writer_design import WriterDesign
 
 from luminesce.api_client import ApiClient
 from luminesce.api_response import ApiResponse
 from luminesce.exceptions import (  # noqa: F401
     ApiTypeError,
@@ -46,23 +51,23 @@
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @overload
-    async def put_file_read_design_to_sql(self, file_reader_builder_def : Annotated[FileReaderBuilderDef, Field(..., description="Structured file read design object to generate SQL from")], execute_query : Annotated[Optional[StrictBool], Field(description="Should the generated query be executed to build preview data or determine errors.>")] = None, **kwargs) -> str:  # noqa: E501
+    async def put_file_read_design_to_sql(self, file_reader_builder_def : Annotated[FileReaderBuilderDef, Field(..., description="Structured file read design object to generate SQL from")], execute_query : Annotated[Optional[StrictBool], Field(description="Should the generated query be executed to build preview data or determine errors.>")] = None, **kwargs) -> FileReaderBuilderResponse:  # noqa: E501
         ...
 
     @overload
-    def put_file_read_design_to_sql(self, file_reader_builder_def : Annotated[FileReaderBuilderDef, Field(..., description="Structured file read design object to generate SQL from")], execute_query : Annotated[Optional[StrictBool], Field(description="Should the generated query be executed to build preview data or determine errors.>")] = None, async_req: Optional[bool]=True, **kwargs) -> str:  # noqa: E501
+    def put_file_read_design_to_sql(self, file_reader_builder_def : Annotated[FileReaderBuilderDef, Field(..., description="Structured file read design object to generate SQL from")], execute_query : Annotated[Optional[StrictBool], Field(description="Should the generated query be executed to build preview data or determine errors.>")] = None, async_req: Optional[bool]=True, **kwargs) -> FileReaderBuilderResponse:  # noqa: E501
         ...
 
     @validate_arguments
-    def put_file_read_design_to_sql(self, file_reader_builder_def : Annotated[FileReaderBuilderDef, Field(..., description="Structured file read design object to generate SQL from")], execute_query : Annotated[Optional[StrictBool], Field(description="Should the generated query be executed to build preview data or determine errors.>")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[str, Awaitable[str]]:  # noqa: E501
+    def put_file_read_design_to_sql(self, file_reader_builder_def : Annotated[FileReaderBuilderDef, Field(..., description="Structured file read design object to generate SQL from")], execute_query : Annotated[Optional[StrictBool], Field(description="Should the generated query be executed to build preview data or determine errors.>")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[FileReaderBuilderResponse, Awaitable[FileReaderBuilderResponse]]:  # noqa: E501
         """[EXPERIMENTAL] PutFileReadDesignToSql: Generates file read SQL from a structured query design  # noqa: E501
 
         SQL Designer specification to generate SQL from  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.put_file_read_design_to_sql(file_reader_builder_def, execute_query, async_req=True)
@@ -77,15 +82,15 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: FileReaderBuilderResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the put_file_read_design_to_sql_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
@@ -124,15 +129,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(FileReaderBuilderResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'file_reader_builder_def',
             'execute_query'
@@ -190,15 +195,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "FileReaderBuilderResponse",
             '400': "LusidProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/Sql/fromfilereaddesign', 'PUT',
             _path_params,
             _query_params,
@@ -212,14 +217,330 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
+    async def put_intellisense(self, intellisense_request : IntellisenseRequest, **kwargs) -> IntellisenseResponse:  # noqa: E501
+        ...
+
+    @overload
+    def put_intellisense(self, intellisense_request : IntellisenseRequest, async_req: Optional[bool]=True, **kwargs) -> IntellisenseResponse:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def put_intellisense(self, intellisense_request : IntellisenseRequest, async_req: Optional[bool]=None, **kwargs) -> Union[IntellisenseResponse, Awaitable[IntellisenseResponse]]:  # noqa: E501
+        """[EXPERIMENTAL] PutIntellisense: Generate a set of possible intellisense prompts given a SQL snip-it (in need not yet be valid) and cursor location  # noqa: E501
+
+        SQL and a row/colum position within it from which to determine intellisense options for the user to potentially choose from.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_intellisense(intellisense_request, async_req=True)
+        >>> result = thread.get()
+
+        :param intellisense_request: (required)
+        :type intellisense_request: IntellisenseRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: IntellisenseResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the put_intellisense_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        if async_req is not None:
+            kwargs['async_req'] = async_req
+        return self.put_intellisense_with_http_info(intellisense_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_intellisense_with_http_info(self, intellisense_request : IntellisenseRequest, **kwargs) -> ApiResponse:  # noqa: E501
+        """[EXPERIMENTAL] PutIntellisense: Generate a set of possible intellisense prompts given a SQL snip-it (in need not yet be valid) and cursor location  # noqa: E501
+
+        SQL and a row/colum position within it from which to determine intellisense options for the user to potentially choose from.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_intellisense_with_http_info(intellisense_request, async_req=True)
+        >>> result = thread.get()
+
+        :param intellisense_request: (required)
+        :type intellisense_request: IntellisenseRequest
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
+        :rtype: tuple(IntellisenseResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'intellisense_request'
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
+                    " to method put_intellisense" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
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
+        if _params['intellisense_request'] is not None:
+            _body_params = _params['intellisense_request']
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
+            '200': "IntellisenseResponse",
+            '400': "LusidProblemDetails",
+        }
+
+        return self.api_client.call_api(
+            '/api/Sql/intellisense', 'PUT',
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
+    async def put_intellisense_error(self, error_highlight_request : ErrorHighlightRequest, **kwargs) -> ErrorHighlightResponse:  # noqa: E501
+        ...
+
+    @overload
+    def put_intellisense_error(self, error_highlight_request : ErrorHighlightRequest, async_req: Optional[bool]=True, **kwargs) -> ErrorHighlightResponse:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def put_intellisense_error(self, error_highlight_request : ErrorHighlightRequest, async_req: Optional[bool]=None, **kwargs) -> Union[ErrorHighlightResponse, Awaitable[ErrorHighlightResponse]]:  # noqa: E501
+        """[EXPERIMENTAL] PutIntellisenseError: Generate a set of error ranges, if any, in the given SQL (expressed as Lines)  # noqa: E501
+
+        SQL (by line) to syntax check and return error ranges from within, if any.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_intellisense_error(error_highlight_request, async_req=True)
+        >>> result = thread.get()
+
+        :param error_highlight_request: (required)
+        :type error_highlight_request: ErrorHighlightRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ErrorHighlightResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the put_intellisense_error_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        if async_req is not None:
+            kwargs['async_req'] = async_req
+        return self.put_intellisense_error_with_http_info(error_highlight_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_intellisense_error_with_http_info(self, error_highlight_request : ErrorHighlightRequest, **kwargs) -> ApiResponse:  # noqa: E501
+        """[EXPERIMENTAL] PutIntellisenseError: Generate a set of error ranges, if any, in the given SQL (expressed as Lines)  # noqa: E501
+
+        SQL (by line) to syntax check and return error ranges from within, if any.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_intellisense_error_with_http_info(error_highlight_request, async_req=True)
+        >>> result = thread.get()
+
+        :param error_highlight_request: (required)
+        :type error_highlight_request: ErrorHighlightRequest
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
+        :rtype: tuple(ErrorHighlightResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'error_highlight_request'
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
+                    " to method put_intellisense_error" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
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
+        if _params['error_highlight_request'] is not None:
+            _body_params = _params['error_highlight_request']
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
+            '200': "ErrorHighlightResponse",
+            '400': "LusidProblemDetails",
+        }
+
+        return self.api_client.call_api(
+            '/api/Sql/intellisenseError', 'PUT',
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
     async def put_query_design_to_sql(self, query_design : Annotated[QueryDesign, Field(..., description="Structured Query design object to generate SQL from")], **kwargs) -> str:  # noqa: E501
         ...
 
     @overload
     def put_query_design_to_sql(self, query_design : Annotated[QueryDesign, Field(..., description="Structured Query design object to generate SQL from")], async_req: Optional[bool]=True, **kwargs) -> str:  # noqa: E501
         ...
 
@@ -632,23 +953,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
-    async def put_sql_to_file_read_design(self, determine_available_sources : Annotated[Optional[StrictBool], Field(description="Should the available sources be determined from `Sys.Registration`")] = None, body : Annotated[Optional[StrictStr], Field(description="SQL query to generate the file read design object from")] = None, **kwargs) -> str:  # noqa: E501
+    async def put_sql_to_file_read_design(self, determine_available_sources : Annotated[Optional[StrictBool], Field(description="Should the available sources be determined from `Sys.Registration`")] = None, body : Annotated[Optional[StrictStr], Field(description="SQL query to generate the file read design object from")] = None, **kwargs) -> FileReaderBuilderDef:  # noqa: E501
         ...
 
     @overload
-    def put_sql_to_file_read_design(self, determine_available_sources : Annotated[Optional[StrictBool], Field(description="Should the available sources be determined from `Sys.Registration`")] = None, body : Annotated[Optional[StrictStr], Field(description="SQL query to generate the file read design object from")] = None, async_req: Optional[bool]=True, **kwargs) -> str:  # noqa: E501
+    def put_sql_to_file_read_design(self, determine_available_sources : Annotated[Optional[StrictBool], Field(description="Should the available sources be determined from `Sys.Registration`")] = None, body : Annotated[Optional[StrictStr], Field(description="SQL query to generate the file read design object from")] = None, async_req: Optional[bool]=True, **kwargs) -> FileReaderBuilderDef:  # noqa: E501
         ...
 
     @validate_arguments
-    def put_sql_to_file_read_design(self, determine_available_sources : Annotated[Optional[StrictBool], Field(description="Should the available sources be determined from `Sys.Registration`")] = None, body : Annotated[Optional[StrictStr], Field(description="SQL query to generate the file read design object from")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[str, Awaitable[str]]:  # noqa: E501
+    def put_sql_to_file_read_design(self, determine_available_sources : Annotated[Optional[StrictBool], Field(description="Should the available sources be determined from `Sys.Registration`")] = None, body : Annotated[Optional[StrictStr], Field(description="SQL query to generate the file read design object from")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[FileReaderBuilderDef, Awaitable[FileReaderBuilderDef]]:  # noqa: E501
         """[EXPERIMENTAL] PutSqlToFileReadDesign: Generates a SQL-file-read-design object from SQL string, if possible.  # noqa: E501
 
         SQL to attempt to create a Design object from  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.put_sql_to_file_read_design(determine_available_sources, body, async_req=True)
@@ -663,15 +984,15 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: FileReaderBuilderDef
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the put_sql_to_file_read_design_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
@@ -710,15 +1031,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(FileReaderBuilderDef, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'determine_available_sources',
             'body'
@@ -776,15 +1097,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "FileReaderBuilderDef",
             '400': "LusidProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/Sql/tofilereaddesign', 'PUT',
             _path_params,
             _query_params,
@@ -798,23 +1119,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
-    async def put_sql_to_query_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the design object from")], validate_with_metadata : Annotated[Optional[StrictBool], Field(description="Should the table be validated against the users' view of Sys.Field to fill in DataTypes, etc.?")] = None, **kwargs) -> str:  # noqa: E501
+    async def put_sql_to_query_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the design object from")], validate_with_metadata : Annotated[Optional[StrictBool], Field(description="Should the table be validated against the users' view of Sys.Field to fill in DataTypes, etc.?")] = None, **kwargs) -> QueryDesign:  # noqa: E501
         ...
 
     @overload
-    def put_sql_to_query_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the design object from")], validate_with_metadata : Annotated[Optional[StrictBool], Field(description="Should the table be validated against the users' view of Sys.Field to fill in DataTypes, etc.?")] = None, async_req: Optional[bool]=True, **kwargs) -> str:  # noqa: E501
+    def put_sql_to_query_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the design object from")], validate_with_metadata : Annotated[Optional[StrictBool], Field(description="Should the table be validated against the users' view of Sys.Field to fill in DataTypes, etc.?")] = None, async_req: Optional[bool]=True, **kwargs) -> QueryDesign:  # noqa: E501
         ...
 
     @validate_arguments
-    def put_sql_to_query_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the design object from")], validate_with_metadata : Annotated[Optional[StrictBool], Field(description="Should the table be validated against the users' view of Sys.Field to fill in DataTypes, etc.?")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[str, Awaitable[str]]:  # noqa: E501
+    def put_sql_to_query_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the design object from")], validate_with_metadata : Annotated[Optional[StrictBool], Field(description="Should the table be validated against the users' view of Sys.Field to fill in DataTypes, etc.?")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[QueryDesign, Awaitable[QueryDesign]]:  # noqa: E501
         """[EXPERIMENTAL] PutSqlToQueryDesign: Generates a SQL-design object from SQL string, if possible.  # noqa: E501
 
         SQL to attempt to create a Design object from  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.put_sql_to_query_design(body, validate_with_metadata, async_req=True)
@@ -829,15 +1150,15 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: QueryDesign
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the put_sql_to_query_design_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
@@ -876,15 +1197,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(QueryDesign, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'body',
             'validate_with_metadata'
@@ -942,15 +1263,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "QueryDesign",
             '400': "LusidProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/Sql/todesign', 'PUT',
             _path_params,
             _query_params,
@@ -964,23 +1285,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
-    async def put_sql_to_view_design(self, body : Annotated[StrictStr, Field(..., description="SQL Query to generate the ConvertToViewData object from")], **kwargs) -> str:  # noqa: E501
+    async def put_sql_to_view_design(self, body : Annotated[StrictStr, Field(..., description="SQL Query to generate the ConvertToViewData object from")], **kwargs) -> ConvertToViewData:  # noqa: E501
         ...
 
     @overload
-    def put_sql_to_view_design(self, body : Annotated[StrictStr, Field(..., description="SQL Query to generate the ConvertToViewData object from")], async_req: Optional[bool]=True, **kwargs) -> str:  # noqa: E501
+    def put_sql_to_view_design(self, body : Annotated[StrictStr, Field(..., description="SQL Query to generate the ConvertToViewData object from")], async_req: Optional[bool]=True, **kwargs) -> ConvertToViewData:  # noqa: E501
         ...
 
     @validate_arguments
-    def put_sql_to_view_design(self, body : Annotated[StrictStr, Field(..., description="SQL Query to generate the ConvertToViewData object from")], async_req: Optional[bool]=None, **kwargs) -> Union[str, Awaitable[str]]:  # noqa: E501
+    def put_sql_to_view_design(self, body : Annotated[StrictStr, Field(..., description="SQL Query to generate the ConvertToViewData object from")], async_req: Optional[bool]=None, **kwargs) -> Union[ConvertToViewData, Awaitable[ConvertToViewData]]:  # noqa: E501
         """[EXPERIMENTAL] PutSqlToViewDesign: Generates a structured view creation design from existing view creation SQL.  # noqa: E501
 
         SQL which creates a view into a structured ConvertToViewData object  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.put_sql_to_view_design(body, async_req=True)
@@ -993,15 +1314,15 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: ConvertToViewData
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the put_sql_to_view_design_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
@@ -1038,15 +1359,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ConvertToViewData, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'body'
         ]
@@ -1100,15 +1421,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "ConvertToViewData",
             '400': "LusidProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/Sql/toviewdesign', 'PUT',
             _path_params,
             _query_params,
@@ -1122,23 +1443,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
-    async def put_sql_to_writer_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the writer design object from")], merge_additional_mapping_fields : Annotated[Optional[StrictBool], Field(description="Should `Sys.Field` be used to find additional potential fields to map from? (not always possible)")] = None, **kwargs) -> str:  # noqa: E501
+    async def put_sql_to_writer_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the writer design object from")], merge_additional_mapping_fields : Annotated[Optional[StrictBool], Field(description="Should `Sys.Field` be used to find additional potential fields to map from? (not always possible)")] = None, **kwargs) -> WriterDesign:  # noqa: E501
         ...
 
     @overload
-    def put_sql_to_writer_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the writer design object from")], merge_additional_mapping_fields : Annotated[Optional[StrictBool], Field(description="Should `Sys.Field` be used to find additional potential fields to map from? (not always possible)")] = None, async_req: Optional[bool]=True, **kwargs) -> str:  # noqa: E501
+    def put_sql_to_writer_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the writer design object from")], merge_additional_mapping_fields : Annotated[Optional[StrictBool], Field(description="Should `Sys.Field` be used to find additional potential fields to map from? (not always possible)")] = None, async_req: Optional[bool]=True, **kwargs) -> WriterDesign:  # noqa: E501
         ...
 
     @validate_arguments
-    def put_sql_to_writer_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the writer design object from")], merge_additional_mapping_fields : Annotated[Optional[StrictBool], Field(description="Should `Sys.Field` be used to find additional potential fields to map from? (not always possible)")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[str, Awaitable[str]]:  # noqa: E501
+    def put_sql_to_writer_design(self, body : Annotated[StrictStr, Field(..., description="SQL query to generate the writer design object from")], merge_additional_mapping_fields : Annotated[Optional[StrictBool], Field(description="Should `Sys.Field` be used to find additional potential fields to map from? (not always possible)")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[WriterDesign, Awaitable[WriterDesign]]:  # noqa: E501
         """[EXPERIMENTAL] PutSqlToWriterDesign: Generates a SQL-writer-design object from SQL string, if possible.  # noqa: E501
 
         SQL to attempt to create a Writer Design object from  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.put_sql_to_writer_design(body, merge_additional_mapping_fields, async_req=True)
@@ -1153,15 +1474,15 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: WriterDesign
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the put_sql_to_writer_design_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
@@ -1200,15 +1521,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(WriterDesign, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'body',
             'merge_additional_mapping_fields'
@@ -1266,15 +1587,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "WriterDesign",
             '400': "LusidProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/Sql/towriterdesign', 'PUT',
             _path_params,
             _query_params,
```

### Comparing `luminesce_sdk-2.0.99/luminesce/api/sql_execution_api.py` & `luminesce_sdk-2.1.1/luminesce/api/sql_execution_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api_client.py` & `luminesce_sdk-2.1.1/luminesce/api_client.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/api_response.py` & `luminesce_sdk-2.1.1/luminesce/api_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/configuration.py` & `luminesce_sdk-2.1.1/luminesce/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("luminesce-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.14.571\n"\
+               "Version of the API: 1.14.936\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `luminesce_sdk-2.0.99/luminesce/exceptions.py` & `luminesce_sdk-2.1.1/luminesce/exceptions.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/api_client.py` & `luminesce_sdk-2.1.1/luminesce/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/api_client_factory.py` & `luminesce_sdk-2.1.1/luminesce/extensions/api_client_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,40 +180,43 @@
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
             # dereference connector so existing session closes correctly
             rc.pool_manager._connector = None
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

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/api_configuration.py` & `luminesce_sdk-2.1.1/luminesce/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/configuration_loaders.py` & `luminesce_sdk-2.1.1/luminesce/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/proxy_config.py` & `luminesce_sdk-2.1.1/luminesce/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/refreshing_token.py` & `luminesce_sdk-2.1.1/luminesce/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/rest.py` & `luminesce_sdk-2.1.1/luminesce/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/retry.py` & `luminesce_sdk-2.1.1/luminesce/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/socket_keep_alive.py` & `luminesce_sdk-2.1.1/luminesce/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/extensions/tcp_keep_alive_connector.py` & `luminesce_sdk-2.1.1/luminesce/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/access_controlled_action.py` & `luminesce_sdk-2.1.1/luminesce/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/access_controlled_resource.py` & `luminesce_sdk-2.1.1/luminesce/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py` & `luminesce_sdk-2.1.1/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/action_id.py` & `luminesce_sdk-2.1.1/luminesce/models/action_id.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/aggregate_function.py` & `luminesce_sdk-2.1.1/luminesce/models/aggregate_function.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/aggregation.py` & `luminesce_sdk-2.1.1/luminesce/models/aggregation.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/auto_detect_type.py` & `luminesce_sdk-2.1.1/luminesce/models/auto_detect_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/available_field.py` & `luminesce_sdk-2.1.1/luminesce/models/available_field.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/available_parameter.py` & `luminesce_sdk-2.1.1/luminesce/models/available_parameter.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/background_multi_query_progress_response.py` & `luminesce_sdk-2.1.1/luminesce/models/background_multi_query_progress_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/background_multi_query_response.py` & `luminesce_sdk-2.1.1/luminesce/models/background_multi_query_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/background_query_cancel_response.py` & `luminesce_sdk-2.1.1/luminesce/models/background_query_cancel_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/background_query_progress_response.py` & `luminesce_sdk-2.1.1/luminesce/models/background_query_progress_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/background_query_response.py` & `luminesce_sdk-2.1.1/luminesce/models/background_query_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/background_query_state.py` & `luminesce_sdk-2.1.1/luminesce/models/background_query_state.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/certificate_action.py` & `luminesce_sdk-2.1.1/luminesce/models/certificate_action.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/certificate_file_type.py` & `luminesce_sdk-2.1.1/luminesce/models/certificate_file_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/certificate_state.py` & `luminesce_sdk-2.1.1/luminesce/models/certificate_state.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/certificate_status.py` & `luminesce_sdk-2.1.1/luminesce/models/certificate_status.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/certificate_type.py` & `luminesce_sdk-2.1.1/luminesce/models/certificate_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/column.py` & `luminesce_sdk-2.1.1/luminesce/models/column.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/column_info.py` & `luminesce_sdk-2.1.1/luminesce/models/column_info.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/condition_attributes.py` & `luminesce_sdk-2.1.1/luminesce/models/condition_attributes.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/convert_to_view_data.py` & `luminesce_sdk-2.1.1/luminesce/models/convert_to_view_data.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/data_type.py` & `luminesce_sdk-2.1.1/luminesce/models/data_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/expression_with_alias.py` & `luminesce_sdk-2.1.1/luminesce/models/expression_with_alias.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/feedback_event_args.py` & `luminesce_sdk-2.1.1/luminesce/models/feedback_event_args.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/feedback_level.py` & `luminesce_sdk-2.1.1/luminesce/models/feedback_level.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/field_design.py` & `luminesce_sdk-2.1.1/luminesce/models/field_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/field_type.py` & `luminesce_sdk-2.1.1/luminesce/models/field_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/file_reader_builder_def.py` & `luminesce_sdk-2.1.1/luminesce/models/file_reader_builder_def.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/filter_term_design.py` & `luminesce_sdk-2.1.1/luminesce/models/filter_term_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/id_selector_definition.py` & `luminesce_sdk-2.1.1/luminesce/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/link.py` & `luminesce_sdk-2.1.1/luminesce/models/link.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/luminesce_binary_type.py` & `luminesce_sdk-2.1.1/luminesce/models/luminesce_binary_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,21 +30,26 @@
     allowed enum values
     """
     COMMANDLINETOOL = 'CommandLineTool'
     LOCAL_FILE_SYSTEM_PROVIDERS = 'LocalFileSystem_Providers'
     EMAIL_PROVIDERS = 'Email_Providers'
     PYTHON_PROVIDERS = 'Python_Providers'
     AWS_S3_PROVIDERS = 'AwsS3_Providers'
+    AZURE_PROVIDERS = 'Azure_Providers'
     SQL_DB_PROVIDERS_DB2_LINUX = 'SqlDb_Providers_Db2Linux'
     SQL_DB_PROVIDERS_MY_SQL = 'SqlDb_Providers_MySql'
     SQL_DB_PROVIDERS_ORACLE = 'SqlDb_Providers_Oracle'
     SQL_DB_PROVIDERS_ORACLE_SNOWFLAKE = 'SqlDb_Providers_Oracle_Snowflake'
     SQL_DB_PROVIDERS_POSTGRESQL = 'SqlDb_Providers_Postgresql'
     SQL_DB_PROVIDERS_SNOWFLAKE = 'SqlDb_Providers_Snowflake'
     SQL_DB_PROVIDERS_SQL_SERVER = 'SqlDb_Providers_SqlServer'
     SQL_DB_PROVIDERS_SYBASE_ASE = 'SqlDb_Providers_SybaseAse'
+    SQL_DB_PROVIDERS_SQ_LITE = 'SqlDb_Providers_SqLite'
+    SQL_DB_PROVIDERS_DUCK_DB = 'SqlDb_Providers_DuckDb'
     JDBC_DRIVER = 'Jdbc_Driver'
+    POWER_BI_CONNECTOR = 'PowerBi_Connector'
+    ODBC_WIN64_DRIVER = 'Odbc_Win64_Driver'
 
     @classmethod
     def from_json(cls, json_str: str) -> LuminesceBinaryType:
         """Create an instance of LuminesceBinaryType from a JSON string"""
         return LuminesceBinaryType(json.loads(json_str))
```

### Comparing `luminesce_sdk-2.0.99/luminesce/models/lusid_problem_details.py` & `luminesce_sdk-2.1.1/luminesce/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/mappable_field.py` & `luminesce_sdk-2.1.1/luminesce/models/mappable_field.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/mapping_flags.py` & `luminesce_sdk-2.1.1/luminesce/models/mapping_flags.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/multi_query_definition_type.py` & `luminesce_sdk-2.1.1/luminesce/models/multi_query_definition_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/options_csv.py` & `luminesce_sdk-2.1.1/luminesce/models/options_csv.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/options_excel.py` & `luminesce_sdk-2.1.1/luminesce/models/options_excel.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/options_parquet.py` & `luminesce_sdk-2.1.1/luminesce/models/options_parquet.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/options_sq_lite.py` & `luminesce_sdk-2.1.1/luminesce/models/options_sq_lite.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/options_xml.py` & `luminesce_sdk-2.1.1/luminesce/models/options_xml.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/order_by_direction.py` & `luminesce_sdk-2.1.1/luminesce/models/order_by_direction.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/order_by_term_design.py` & `luminesce_sdk-2.1.1/luminesce/models/order_by_term_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/query_design.py` & `luminesce_sdk-2.1.1/luminesce/models/query_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/query_designer_binary_operator.py` & `luminesce_sdk-2.1.1/luminesce/models/query_designer_binary_operator.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/resource_list_of_access_controlled_resource.py` & `luminesce_sdk-2.1.1/luminesce/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/source.py` & `luminesce_sdk-2.1.1/luminesce/models/source.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/source_type.py` & `luminesce_sdk-2.1.1/luminesce/models/source_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/task_status.py` & `luminesce_sdk-2.1.1/luminesce/models/task_status.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/view_parameter.py` & `luminesce_sdk-2.1.1/luminesce/models/view_parameter.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/models/writer_design.py` & `luminesce_sdk-2.1.1/luminesce/models/writer_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.0.99/luminesce/rest.py` & `luminesce_sdk-2.1.1/luminesce/rest.py`

 * *Files 5% similar despite different names*

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

### Comparing `luminesce_sdk-2.0.99/pyproject.toml` & `luminesce_sdk-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "luminesce-sdk"
-version = "2.0.99"
+version = "2.1.1"
 description = "FINBOURNE Luminesce Web API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/luminesce-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Luminesce Web API", "luminesce-sdk"]
 packages = [
```

### Comparing `luminesce_sdk-2.0.99/PKG-INFO` & `luminesce_sdk-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luminesce-sdk
-Version: 2.0.99
+Version: 2.1.1
 Summary: FINBOURNE Luminesce Web API
 Home-page: https://github.com/finbourne/luminesce-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Luminesce Web API,luminesce-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # luminesce-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.14.571
-- Package version: 2.0.99
+- API version: 1.14.936
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -82,16 +82,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_LUMINESCE_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_LUMINESCE_API_URL,
 FBN_ACCESS_TOKEN
 ```
@@ -238,14 +237,16 @@
 *SqlBackgroundExecutionApi* | [**fetch_query_result_parquet**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_parquet) | **GET** /api/SqlBackground/{executionId}/parquet | FetchQueryResultParquet: Fetches the result from a previously started query, in Parquet format.
 *SqlBackgroundExecutionApi* | [**fetch_query_result_pipe**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_pipe) | **GET** /api/SqlBackground/{executionId}/pipe | FetchQueryResultPipe: Fetches the result from a previously started query, in pipe-delimited format.
 *SqlBackgroundExecutionApi* | [**fetch_query_result_sqlite**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_sqlite) | **GET** /api/SqlBackground/{executionId}/sqlite | FetchQueryResultSqlite: Fetches the result from a previously started query, in SqLite format.
 *SqlBackgroundExecutionApi* | [**fetch_query_result_xml**](docs/SqlBackgroundExecutionApi.md#fetch_query_result_xml) | **GET** /api/SqlBackground/{executionId}/xml | FetchQueryResultXml: Fetches the result from a previously started query, in Xml format.
 *SqlBackgroundExecutionApi* | [**get_progress_of**](docs/SqlBackgroundExecutionApi.md#get_progress_of) | **GET** /api/SqlBackground/{executionId} | GetProgressOf: View progress information (up until this point)
 *SqlBackgroundExecutionApi* | [**start_query**](docs/SqlBackgroundExecutionApi.md#start_query) | **PUT** /api/SqlBackground | StartQuery: Starts to Execute LuminesceSql in the background.
 *SqlDesignApi* | [**put_file_read_design_to_sql**](docs/SqlDesignApi.md#put_file_read_design_to_sql) | **PUT** /api/Sql/fromfilereaddesign | [EXPERIMENTAL] PutFileReadDesignToSql: Generates file read SQL from a structured query design
+*SqlDesignApi* | [**put_intellisense**](docs/SqlDesignApi.md#put_intellisense) | **PUT** /api/Sql/intellisense | [EXPERIMENTAL] PutIntellisense: Generate a set of possible intellisense prompts given a SQL snip-it (in need not yet be valid) and cursor location
+*SqlDesignApi* | [**put_intellisense_error**](docs/SqlDesignApi.md#put_intellisense_error) | **PUT** /api/Sql/intellisenseError | [EXPERIMENTAL] PutIntellisenseError: Generate a set of error ranges, if any, in the given SQL (expressed as Lines)
 *SqlDesignApi* | [**put_query_design_to_sql**](docs/SqlDesignApi.md#put_query_design_to_sql) | **PUT** /api/Sql/fromdesign | [EXPERIMENTAL] PutQueryDesignToSql: Generates SQL from a structured query design
 *SqlDesignApi* | [**put_query_to_format**](docs/SqlDesignApi.md#put_query_to_format) | **PUT** /api/Sql/pretty | PutQueryToFormat: Formats SQL into a more readable form, a.k.a. Pretty-Print the SQL.
 *SqlDesignApi* | [**put_sql_to_file_read_design**](docs/SqlDesignApi.md#put_sql_to_file_read_design) | **PUT** /api/Sql/tofilereaddesign | [EXPERIMENTAL] PutSqlToFileReadDesign: Generates a SQL-file-read-design object from SQL string, if possible.
 *SqlDesignApi* | [**put_sql_to_query_design**](docs/SqlDesignApi.md#put_sql_to_query_design) | **PUT** /api/Sql/todesign | [EXPERIMENTAL] PutSqlToQueryDesign: Generates a SQL-design object from SQL string, if possible.
 *SqlDesignApi* | [**put_sql_to_view_design**](docs/SqlDesignApi.md#put_sql_to_view_design) | **PUT** /api/Sql/toviewdesign | [EXPERIMENTAL] PutSqlToViewDesign: Generates a structured view creation design from existing view creation SQL.
 *SqlDesignApi* | [**put_sql_to_writer_design**](docs/SqlDesignApi.md#put_sql_to_writer_design) | **PUT** /api/Sql/towriterdesign | [EXPERIMENTAL] PutSqlToWriterDesign: Generates a SQL-writer-design object from SQL string, if possible.
 *SqlDesignApi* | [**put_view_design_to_sql**](docs/SqlDesignApi.md#put_view_design_to_sql) | **PUT** /api/Sql/fromviewdesign | [EXPERIMENTAL] PutViewDesignToSql: Generates view creation sql from a structured view creation design
@@ -288,23 +289,32 @@
  - [CertificateState](docs/CertificateState.md)
  - [CertificateStatus](docs/CertificateStatus.md)
  - [CertificateType](docs/CertificateType.md)
  - [Column](docs/Column.md)
  - [ColumnInfo](docs/ColumnInfo.md)
  - [ConditionAttributes](docs/ConditionAttributes.md)
  - [ConvertToViewData](docs/ConvertToViewData.md)
+ - [CursorPosition](docs/CursorPosition.md)
  - [DataType](docs/DataType.md)
+ - [ErrorHighlightItem](docs/ErrorHighlightItem.md)
+ - [ErrorHighlightRequest](docs/ErrorHighlightRequest.md)
+ - [ErrorHighlightResponse](docs/ErrorHighlightResponse.md)
  - [ExpressionWithAlias](docs/ExpressionWithAlias.md)
  - [FeedbackEventArgs](docs/FeedbackEventArgs.md)
  - [FeedbackLevel](docs/FeedbackLevel.md)
  - [FieldDesign](docs/FieldDesign.md)
  - [FieldType](docs/FieldType.md)
  - [FileReaderBuilderDef](docs/FileReaderBuilderDef.md)
+ - [FileReaderBuilderResponse](docs/FileReaderBuilderResponse.md)
  - [FilterTermDesign](docs/FilterTermDesign.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
+ - [IntellisenseItem](docs/IntellisenseItem.md)
+ - [IntellisenseRequest](docs/IntellisenseRequest.md)
+ - [IntellisenseResponse](docs/IntellisenseResponse.md)
+ - [IntellisenseType](docs/IntellisenseType.md)
  - [Link](docs/Link.md)
  - [LuminesceBinaryType](docs/LuminesceBinaryType.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [MappableField](docs/MappableField.md)
  - [MappingFlags](docs/MappingFlags.md)
  - [MultiQueryDefinitionType](docs/MultiQueryDefinitionType.md)
  - [OptionsCsv](docs/OptionsCsv.md)
```

