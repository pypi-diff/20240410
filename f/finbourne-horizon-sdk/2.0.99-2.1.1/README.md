# Comparing `tmp/finbourne_horizon_sdk-2.0.99.tar.gz` & `tmp/finbourne_horizon_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_horizon_sdk-2.0.99.tar", max compression
+gzip compressed data, was "finbourne_horizon_sdk-2.1.1.tar", max compression
```

## Comparing `finbourne_horizon_sdk-2.0.99.tar` & `finbourne_horizon_sdk-2.1.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    14292 2024-03-11 13:54:49.471807 finbourne_horizon_sdk-2.0.99/README.md
--rw-r--r--   0        0        0     4755 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/__init__.py
--rw-r--r--   0        0        0      305 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/__init__.py
--rw-r--r--   0        0        0    46616 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/instrument_api.py
--rw-r--r--   0        0        0    60678 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/integrations_api.py
--rw-r--r--   0        0        0    36418 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/process_history_api.py
--rw-r--r--   0        0        0    43381 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/vendor_api.py
--rw-r--r--   0        0        0    30805 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_client.py
--rw-r--r--   0        0        0      852 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_response.py
--rw-r--r--   0        0        0    14454 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/configuration.py
--rw-r--r--   0        0        0     5338 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/exceptions.py
--rw-r--r--   0        0        0      300 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/__init__.py
--rw-r--r--   0        0        0    30675 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client.py
--rw-r--r--   0        0        0     9793 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8112 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_configuration.py
--rw-r--r--   0        0        0     6808 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12710 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/rest.py
--rw-r--r--   0        0        0    11576 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3889 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3945 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/__init__.py
--rw-r--r--   0        0        0     1980 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/allowed_parameter_value.py
--rw-r--r--   0        0        0     4469 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_request.py
--rw-r--r--   0        0        0     2024 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_response.py
--rw-r--r--   0        0        0      745 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_status.py
--rw-r--r--   0        0        0     2132 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_details.py
--rw-r--r--   0        0        0      707 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_type.py
--rw-r--r--   0        0        0     2646 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_request.py
--rw-r--r--   0        0        0     2010 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_response.py
--rw-r--r--   0        0        0     2887 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/create_instance_request.py
--rw-r--r--   0        0        0     2599 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/enrichment_response.py
--rw-r--r--   0        0        0     2036 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/execute_instance_response.py
--rw-r--r--   0        0        0     2282 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/file_details.py
--rw-r--r--   0        0        0     1936 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/identifiers.py
--rw-r--r--   0        0        0     1918 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/instance_identifier.py
--rw-r--r--   0        0        0     2504 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_description.py
--rw-r--r--   0        0        0     3719 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_instance.py
--rw-r--r--   0        0        0     2258 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/link.py
--rw-r--r--   0        0        0     3208 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_entity.py
--rw-r--r--   0        0        0     3665 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_field.py
--rw-r--r--   0        0        0     3853 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_problem_details.py
--rw-r--r--   0        0        0     3533 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition.py
--rw-r--r--   0        0        0     2811 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides.py
--rw-r--r--   0        0        0     3938 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides_response.py
--rw-r--r--   0        0        0     3012 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py
--rw-r--r--   0        0        0     4482 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3667 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_request.py
--rw-r--r--   0        0        0     2734 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_response.py
--rw-r--r--   0        0        0     8430 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_data.py
--rw-r--r--   0        0        0      986 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_parameter_option_name.py
--rw-r--r--   0        0        0     2780 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_perm_id_result.py
--rw-r--r--   0        0        0     2887 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_search_result.py
--rw-r--r--   0        0        0      768 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/optionality.py
--rw-r--r--   0        0        0     4224 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_information.py
--rw-r--r--   0        0        0     4237 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_update_result.py
--rw-r--r--   0        0        0     4164 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_vendor_product.py
--rw-r--r--   0        0        0     3037 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/perm_id_data.py
--rw-r--r--   0        0        0     3386 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_information.py
--rw-r--r--   0        0        0     3838 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_summary.py
--rw-r--r--   0        0        0     2963 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_update_result.py
--rw-r--r--   0        0        0     2247 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_request.py
--rw-r--r--   0        0        0     2205 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_specification.py
--rw-r--r--   0        0        0     1865 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/resource_id.py
--rw-r--r--   0        0        0     3460 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/row_details.py
--rw-r--r--   0        0        0     2017 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/trigger.py
--rw-r--r--   0        0        0     2957 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/update_instance_request.py
--rw-r--r--   0        0        0     2707 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/vendor_product.py
--rw-r--r--   0        0        0        0 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/py.typed
--rw-r--r--   0        0        0    10031 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/rest.py
--rw-r--r--   0        0        0      866 2024-03-11 13:54:49.471807 finbourne_horizon_sdk-2.0.99/pyproject.toml
--rw-r--r--   0        0        0    15341 1970-01-01 00:00:00.000000 finbourne_horizon_sdk-2.0.99/PKG-INFO
+-rw-r--r--   0        0        0    14283 2024-04-10 10:43:14.074859 finbourne_horizon_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     6675 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/__init__.py
+-rw-r--r--   0        0        0    46622 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/instrument_api.py
+-rw-r--r--   0        0        0    60694 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/integrations_api.py
+-rw-r--r--   0        0        0    36424 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/process_history_api.py
+-rw-r--r--   0        0        0    43387 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/vendor_api.py
+-rw-r--r--   0        0        0    30805 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/api_response.py
+-rw-r--r--   0        0        0    14454 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/configuration.py
+-rw-r--r--   0        0        0     5338 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/exceptions.py
+-rw-r--r--   0        0        0      596 2024-04-10 10:43:14.079859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/__init__.py
+-rw-r--r--   0        0        0    30675 2024-04-10 10:43:14.079859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/api_client.py
+-rw-r--r--   0        0        0     9892 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8112 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6808 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12710 2024-04-10 10:43:14.079859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/rest.py
+-rw-r--r--   0        0        0    11576 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:43:14.079859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3889 2024-04-10 10:43:14.079859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     5217 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/__init__.py
+-rw-r--r--   0        0        0     1983 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/allowed_parameter_value.py
+-rw-r--r--   0        0        0     5006 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_complete_request.py
+-rw-r--r--   0        0        0     2027 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_complete_response.py
+-rw-r--r--   0        0        0      745 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_complete_status.py
+-rw-r--r--   0        0        0     2135 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_file_details.py
+-rw-r--r--   0        0        0      707 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_file_type.py
+-rw-r--r--   0        0        0     3183 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_update_request.py
+-rw-r--r--   0        0        0     2013 2024-04-10 10:43:14.075858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_update_response.py
+-rw-r--r--   0        0        0     2890 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/create_instance_request.py
+-rw-r--r--   0        0        0     2602 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/enrichment_response.py
+-rw-r--r--   0        0        0     2039 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/execute_instance_response.py
+-rw-r--r--   0        0        0     2285 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/file_details.py
+-rw-r--r--   0        0        0     1939 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/identifiers.py
+-rw-r--r--   0        0        0     1921 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/instance_identifier.py
+-rw-r--r--   0        0        0     2507 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/integration_description.py
+-rw-r--r--   0        0        0     3722 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/integration_instance.py
+-rw-r--r--   0        0        0     2261 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/link.py
+-rw-r--r--   0        0        0     3211 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_entity.py
+-rw-r--r--   0        0        0     3668 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_field.py
+-rw-r--r--   0        0        0     3856 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     3536 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_definition.py
+-rw-r--r--   0        0        0     2814 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_definition_overrides.py
+-rw-r--r--   0        0        0     3941 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_definition_overrides_response.py
+-rw-r--r--   0        0        0     3015 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py
+-rw-r--r--   0        0        0     4485 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3670 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/onboard_instrument_request.py
+-rw-r--r--   0        0        0     2737 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/onboard_instrument_response.py
+-rw-r--r--   0        0        0     8433 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_data.py
+-rw-r--r--   0        0        0      986 2024-04-10 10:43:14.076859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_parameter_option_name.py
+-rw-r--r--   0        0        0     2783 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_perm_id_result.py
+-rw-r--r--   0        0        0     2890 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_search_result.py
+-rw-r--r--   0        0        0      768 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/optionality.py
+-rw-r--r--   0        0        0     4227 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/paged_resource_list_of_process_information.py
+-rw-r--r--   0        0        0     4240 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/paged_resource_list_of_process_update_result.py
+-rw-r--r--   0        0        0     4167 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/paged_resource_list_of_vendor_product.py
+-rw-r--r--   0        0        0     3040 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/perm_id_data.py
+-rw-r--r--   0        0        0     3389 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/process_information.py
+-rw-r--r--   0        0        0     3841 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/process_summary.py
+-rw-r--r--   0        0        0     2966 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/process_update_result.py
+-rw-r--r--   0        0        0     2250 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/query_request.py
+-rw-r--r--   0        0        0     2208 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/query_specification.py
+-rw-r--r--   0        0        0     1868 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/resource_id.py
+-rw-r--r--   0        0        0     3463 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/row_details.py
+-rw-r--r--   0        0        0     2020 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/trigger.py
+-rw-r--r--   0        0        0     2960 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/update_instance_request.py
+-rw-r--r--   0        0        0     2710 2024-04-10 10:43:14.077859 finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/vendor_product.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/py.typed
+-rw-r--r--   0        0        0    10162 2024-04-10 10:43:14.078858 finbourne_horizon_sdk-2.1.1/finbourne_horizon/rest.py
+-rw-r--r--   0        0        0      864 2024-04-10 10:43:14.074859 finbourne_horizon_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    15330 1970-01-01 00:00:00.000000 finbourne_horizon_sdk-2.1.1/PKG-INFO
```

### Comparing `finbourne_horizon_sdk-2.0.99/README.md` & `finbourne_horizon_sdk-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-horizon-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.393
-- Package version: 2.0.99
+- API version: 0.1.438
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -56,16 +56,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_FINBOURNE_HORIZON_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_FINBOURNE_HORIZON_API_URL,
 FBN_ACCESS_TOKEN
 ```
@@ -195,15 +194,15 @@
 *InstrumentApi* | [**get_open_figi_parameter_option**](docs/InstrumentApi.md#get_open_figi_parameter_option) | **GET** /api/instrument/onboarding/search/openfigi/parameterOptions | [EARLY ACCESS] GetOpenFigiParameterOption: Get all supported market sector values for OpenFigi search
 *InstrumentApi* | [**retrieve_perm_id_result**](docs/InstrumentApi.md#retrieve_perm_id_result) | **GET** /api/instrument/onboarding/search/permid/{id} | [EARLY ACCESS] RetrievePermIdResult: Retrieve PermId results from a previous query.
 *InstrumentApi* | [**search_open_figi**](docs/InstrumentApi.md#search_open_figi) | **GET** /api/instrument/onboarding/search/openfigi | [EARLY ACCESS] SearchOpenFigi: Search OpenFigi for instruments that match the specified terms.
 *InstrumentApi* | [**vendors**](docs/InstrumentApi.md#vendors) | **GET** /api/instrument/onboarding/vendors | [EARLY ACCESS] Vendors: Gets the VendorProducts of any supported and licenced integrations for a given market sector and security type.
 *IntegrationsApi* | [**create_instance**](docs/IntegrationsApi.md#create_instance) | **POST** /api/integrations/instances | [EXPERIMENTAL] CreateInstance: Create a single integration instance.
 *IntegrationsApi* | [**delete_instance**](docs/IntegrationsApi.md#delete_instance) | **DELETE** /api/integrations/instances/{instanceId} | [EXPERIMENTAL] DeleteInstance: Delete a single integration instance.
 *IntegrationsApi* | [**execute_instance**](docs/IntegrationsApi.md#execute_instance) | **POST** /api/integrations/instances/{instanceId}/execute | [EXPERIMENTAL] ExecuteInstance: Execute an integration instance.
-*IntegrationsApi* | [**get_execution_ids_for_instance**](docs/IntegrationsApi.md#get_execution_ids_for_instance) | **GET** /api/integrations/executions/{instanceId} | [EXPERIMENTAL] GetExecutionIdsForInstance: Get integration instance execution ids.
+*IntegrationsApi* | [**get_execution_ids_for_instance**](docs/IntegrationsApi.md#get_execution_ids_for_instance) | **GET** /api/integrations/instances/{instanceId}/executions | [EXPERIMENTAL] GetExecutionIdsForInstance: Get integration instance execution ids.
 *IntegrationsApi* | [**get_schema**](docs/IntegrationsApi.md#get_schema) | **GET** /api/integrations/schema/{integration} | [EXPERIMENTAL] GetSchema: Get the JSON schema for the details section of an integration instance.
 *IntegrationsApi* | [**list_instances**](docs/IntegrationsApi.md#list_instances) | **GET** /api/integrations/instances | [EXPERIMENTAL] ListInstances: List instances across all integrations.
 *IntegrationsApi* | [**list_integrations**](docs/IntegrationsApi.md#list_integrations) | **GET** /api/integrations | [EXPERIMENTAL] ListIntegrations: List available integrations.
 *IntegrationsApi* | [**update_instance**](docs/IntegrationsApi.md#update_instance) | **PUT** /api/integrations/instances/{instanceId} | [EXPERIMENTAL] UpdateInstance: Update a single integration instance.
 *ProcessHistoryApi* | [**create_complete_event**](docs/ProcessHistoryApi.md#create_complete_event) | **POST** /api/process-history/event/complete | [EARLY ACCESS] CreateCompleteEvent: Write a completed event to the Horizon Dashboard
 *ProcessHistoryApi* | [**create_update_event**](docs/ProcessHistoryApi.md#create_update_event) | **POST** /api/process-history/event/update | [EARLY ACCESS] CreateUpdateEvent: Write an update event to the Horizon Dashboard
 *ProcessHistoryApi* | [**get_latest_runs**](docs/ProcessHistoryApi.md#get_latest_runs) | **GET** /api/process-history/$latestRuns | [EARLY ACCESS] GetLatestRuns: Get latest run for each process
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/instrument_api.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/instrument_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool, StrictInt, StrictStr
+from pydantic.v1 import Field, StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from finbourne_horizon.models.allowed_parameter_value import AllowedParameterValue
 from finbourne_horizon.models.enrichment_response import EnrichmentResponse
 from finbourne_horizon.models.identifiers import Identifiers
 from finbourne_horizon.models.onboard_instrument_request import OnboardInstrumentRequest
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/integrations_api.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/integrations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictInt, StrictStr, constr, validator
+from pydantic.v1 import Field, StrictInt, StrictStr, constr, validator
 
 from typing import List, Optional
 
 from finbourne_horizon.models.create_instance_request import CreateInstanceRequest
 from finbourne_horizon.models.execute_instance_response import ExecuteInstanceResponse
 from finbourne_horizon.models.instance_identifier import InstanceIdentifier
 from finbourne_horizon.models.integration_description import IntegrationDescription
@@ -647,15 +647,15 @@
 
         _response_types_map = {
             '200': "str",
             '404': None,
         }
 
         return self.api_client.call_api(
-            '/api/integrations/executions/{instanceId}', 'GET',
+            '/api/integrations/instances/{instanceId}/executions', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/process_history_api.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/process_history_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
-from pydantic import StrictStr
+from pydantic.v1 import StrictStr
 
 from typing import List, Optional
 
 from finbourne_horizon.models.audit_complete_request import AuditCompleteRequest
 from finbourne_horizon.models.audit_complete_response import AuditCompleteResponse
 from finbourne_horizon.models.audit_update_request import AuditUpdateRequest
 from finbourne_horizon.models.audit_update_response import AuditUpdateResponse
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/vendor_api.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/api/vendor_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
-from pydantic import StrictStr
+from pydantic.v1 import StrictStr
 
 from typing import Dict, List, Optional
 
 from finbourne_horizon.models.lusid_field import LusidField
 from finbourne_horizon.models.lusid_property_definition_overrides import LusidPropertyDefinitionOverrides
 from finbourne_horizon.models.lusid_property_definition_overrides_response import LusidPropertyDefinitionOverridesResponse
 from finbourne_horizon.models.lusid_property_to_vendor_field_mapping import LusidPropertyToVendorFieldMapping
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_client.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/configuration.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_horizon-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.393\n"\
+               "Version of the API: 0.1.438\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/exceptions.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client_factory.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/api_client_factory.py`

 * *Files 1% similar despite different names*

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

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_configuration.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/configuration_loaders.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/proxy_config.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/refreshing_token.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/rest.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/retry.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/socket_keep_alive.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/tcp_keep_alive_connector.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/allowed_parameter_value.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/allowed_parameter_value.py`

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
 
 class AllowedParameterValue(BaseModel):
     """
     An allowed parameter value for an OpenFigi Parameter Option.  # noqa: E501
     """
     allowed_value: StrictStr = Field(..., alias="allowedValue")
     __properties = ["allowedValue"]
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_request.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_complete_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
+from typing import Any, Dict, List, Optional
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist
 from finbourne_horizon.models.audit_complete_status import AuditCompleteStatus
 from finbourne_horizon.models.audit_file_details import AuditFileDetails
 
 class AuditCompleteRequest(BaseModel):
     """
     An incoming request for a Horizon Complete Event  # noqa: E501
     """
@@ -35,15 +35,16 @@
     message: StrictStr = Field(..., description="A descriptive message to accompany the status")
     status: AuditCompleteStatus = Field(...)
     rows_total: StrictInt = Field(..., alias="rowsTotal", description="The number of data rows operated on")
     rows_succeeded: StrictInt = Field(..., alias="rowsSucceeded", description="The number of data rows successfully operated on")
     rows_failed: StrictInt = Field(..., alias="rowsFailed", description="The number of data rows that failed to be operated on")
     rows_ignored: StrictInt = Field(..., alias="rowsIgnored", description="The number of data rows that had no actions taken")
     audit_files: conlist(AuditFileDetails) = Field(..., alias="auditFiles", description="A list of file details for attaching to the event")
-    __properties = ["id", "userId", "schedulerRunId", "startTime", "endTime", "message", "status", "rowsTotal", "rowsSucceeded", "rowsFailed", "rowsIgnored", "auditFiles"]
+    process_name_override: Optional[StrictStr] = Field(None, alias="processNameOverride", description="Optional Name for how the process appears in Data Feed Monitoring")
+    __properties = ["id", "userId", "schedulerRunId", "startTime", "endTime", "message", "status", "rowsTotal", "rowsSucceeded", "rowsFailed", "rowsIgnored", "auditFiles", "processNameOverride"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -68,14 +69,19 @@
         # override the default output from pydantic by calling `to_dict()` of each item in audit_files (list)
         _items = []
         if self.audit_files:
             for _item in self.audit_files:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['auditFiles'] = _items
+        # set to None if process_name_override (nullable) is None
+        # and __fields_set__ contains the field
+        if self.process_name_override is None and "process_name_override" in self.__fields_set__:
+            _dict['processNameOverride'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> AuditCompleteRequest:
         """Create an instance of AuditCompleteRequest from a dict"""
         if obj is None:
             return None
@@ -91,10 +97,11 @@
             "end_time": obj.get("endTime"),
             "message": obj.get("message"),
             "status": obj.get("status"),
             "rows_total": obj.get("rowsTotal"),
             "rows_succeeded": obj.get("rowsSucceeded"),
             "rows_failed": obj.get("rowsFailed"),
             "rows_ignored": obj.get("rowsIgnored"),
-            "audit_files": [AuditFileDetails.from_dict(_item) for _item in obj.get("auditFiles")] if obj.get("auditFiles") is not None else None
+            "audit_files": [AuditFileDetails.from_dict(_item) for _item in obj.get("auditFiles")] if obj.get("auditFiles") is not None else None,
+            "process_name_override": obj.get("processNameOverride")
         })
         return _obj
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_complete_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class AuditCompleteResponse(BaseModel):
     """
     Response type for Horizon Audit Event  # noqa: E501
     """
     process_name: StrictStr = Field(..., alias="processName", description="The name of the Process the events will be visible under")
     __properties = ["processName"]
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_status.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_complete_status.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_details.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_file_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 from finbourne_horizon.models.audit_file_type import AuditFileType
 
 class AuditFileDetails(BaseModel):
     """
     Holds information about Horizon Audit Files  # noqa: E501
     """
     file_type: AuditFileType = Field(..., alias="fileType")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_type.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_file_type.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_request.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_update_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,28 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
-class AuditUpdateRequest(BaseModel):
+class AuditUpdateResponse(BaseModel):
     """
-    An incoming request for a Horizon Update Event  # noqa: E501
+    Response type for Horizon Audit Event  # noqa: E501
     """
-    id: StrictStr = Field(..., description="A unique ID identifiying the source of the event")
-    user_id: StrictStr = Field(..., alias="userId", description="A unique ID identifiying who owns the schedule")
-    scheduler_run_id: StrictStr = Field(..., alias="schedulerRunId", description="The GUID of the schedule run")
-    start_time: datetime = Field(..., alias="startTime", description="When the run was started in UTC")
-    message: StrictStr = Field(..., description="A descriptive message to accompany the status")
-    __properties = ["id", "userId", "schedulerRunId", "startTime", "message"]
+    process_name: StrictStr = Field(..., alias="processName", description="The name of the Process the events will be visible under")
+    __properties = ["processName"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -42,36 +38,32 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AuditUpdateRequest:
-        """Create an instance of AuditUpdateRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> AuditUpdateResponse:
+        """Create an instance of AuditUpdateResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AuditUpdateRequest:
-        """Create an instance of AuditUpdateRequest from a dict"""
+    def from_dict(cls, obj: dict) -> AuditUpdateResponse:
+        """Create an instance of AuditUpdateResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return AuditUpdateRequest.parse_obj(obj)
+            return AuditUpdateResponse.parse_obj(obj)
 
-        _obj = AuditUpdateRequest.parse_obj({
-            "id": obj.get("id"),
-            "user_id": obj.get("userId"),
-            "scheduler_run_id": obj.get("schedulerRunId"),
-            "start_time": obj.get("startTime"),
-            "message": obj.get("message")
+        _obj = AuditUpdateResponse.parse_obj({
+            "process_name": obj.get("processName")
         })
         return _obj
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/link.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,23 +14,26 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from typing import Any, Dict, Optional
+from pydantic.v1 import BaseModel, Field, StrictStr
 
-class AuditUpdateResponse(BaseModel):
+class Link(BaseModel):
     """
-    Response type for Horizon Audit Event  # noqa: E501
+    Link
     """
-    process_name: StrictStr = Field(..., alias="processName", description="The name of the Process the events will be visible under")
-    __properties = ["processName"]
+    relation: StrictStr = Field(...)
+    href: StrictStr = Field(...)
+    description: Optional[StrictStr] = None
+    method: StrictStr = Field(...)
+    __properties = ["relation", "href", "description", "method"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -38,32 +41,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AuditUpdateResponse:
-        """Create an instance of AuditUpdateResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Link:
+        """Create an instance of Link from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if description (nullable) is None
+        # and __fields_set__ contains the field
+        if self.description is None and "description" in self.__fields_set__:
+            _dict['description'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AuditUpdateResponse:
-        """Create an instance of AuditUpdateResponse from a dict"""
+    def from_dict(cls, obj: dict) -> Link:
+        """Create an instance of Link from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return AuditUpdateResponse.parse_obj(obj)
+            return Link.parse_obj(obj)
 
-        _obj = AuditUpdateResponse.parse_obj({
-            "process_name": obj.get("processName")
+        _obj = Link.parse_obj({
+            "relation": obj.get("relation"),
+            "href": obj.get("href"),
+            "description": obj.get("description"),
+            "method": obj.get("method")
         })
         return _obj
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/create_instance_request.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/create_instance_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist
 from finbourne_horizon.models.trigger import Trigger
 
 class CreateInstanceRequest(BaseModel):
     """
     CreateInstanceRequest
     """
     integration_type: StrictStr = Field(..., alias="integrationType")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/enrichment_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/enrichment_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 
 class EnrichmentResponse(BaseModel):
     """
     Collated enrichment result information  # noqa: E501
     """
     enriched_instruments: conlist(StrictStr) = Field(..., alias="enrichedInstruments")
     ignored_instruments: conlist(StrictStr) = Field(..., alias="ignoredInstruments")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/execute_instance_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/execute_instance_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class ExecuteInstanceResponse(BaseModel):
     """
     Response for executing an instance.  # noqa: E501
     """
     execution_id: StrictStr = Field(..., alias="executionId", description="Identifier for the execution of the integration instance")
     __properties = ["executionId"]
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/file_details.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/file_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class FileDetails(BaseModel):
     """
     Information associated with files  # noqa: E501
     """
     file_name: StrictStr = Field(..., alias="fileName")
     file_type: Optional[StrictStr] = Field(None, alias="fileType")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/identifiers.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/identifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 
 class Identifiers(BaseModel):
     """
     A list of lusid instrument ids  # noqa: E501
     """
     lusid_instrument_ids: conlist(StrictStr) = Field(..., alias="lusidInstrumentIds")
     __properties = ["lusidInstrumentIds"]
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/instance_identifier.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/instance_identifier.py`

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
 
 class InstanceIdentifier(BaseModel):
     """
     Identifies a single instance of an integration.  # noqa: E501
     """
     id: StrictStr = Field(..., description="Instance identifier.")
     __properties = ["id"]
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_description.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/integration_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr
 
 class IntegrationDescription(BaseModel):
     """
     Response containing the description of an integration.  # noqa: E501
     """
     type: StrictStr = Field(..., description="Unique identifier of the integration e.g. \"copp-clark\".")
     name: StrictStr = Field(..., description="Readable name of the integration e.g. \"Copp Clark\".")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_instance.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/integration_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, constr, validator
 from finbourne_horizon.models.trigger import Trigger
 
 class IntegrationInstance(BaseModel):
     """
     Response containing an integration instance.  # noqa: E501
     """
     id: constr(strict=True, max_length=36, min_length=36) = Field(..., description="Identifies the instance within the integration.")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/link.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/process_update_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
-class Link(BaseModel):
+class ProcessUpdateResult(BaseModel):
     """
-    Link
+    Shows details relevant to update events for a query  # noqa: E501
     """
-    relation: StrictStr = Field(...)
-    href: StrictStr = Field(...)
-    description: Optional[StrictStr] = None
-    method: StrictStr = Field(...)
-    __properties = ["relation", "href", "description", "method"]
+    domain: StrictStr = Field(...)
+    entry_id: StrictStr = Field(..., alias="entryId")
+    process_name: StrictStr = Field(..., alias="processName")
+    run_id: StrictStr = Field(..., alias="runId")
+    entry_date: datetime = Field(..., alias="entryDate")
+    status: StrictStr = Field(...)
+    message: StrictStr = Field(...)
+    schema_version: Optional[StrictStr] = Field(None, alias="schemaVersion")
+    __properties = ["domain", "entryId", "processName", "runId", "entryDate", "status", "message", "schemaVersion"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,40 +45,44 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Link:
-        """Create an instance of Link from a JSON string"""
+    def from_json(cls, json_str: str) -> ProcessUpdateResult:
+        """Create an instance of ProcessUpdateResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if description (nullable) is None
+        # set to None if schema_version (nullable) is None
         # and __fields_set__ contains the field
-        if self.description is None and "description" in self.__fields_set__:
-            _dict['description'] = None
+        if self.schema_version is None and "schema_version" in self.__fields_set__:
+            _dict['schemaVersion'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Link:
-        """Create an instance of Link from a dict"""
+    def from_dict(cls, obj: dict) -> ProcessUpdateResult:
+        """Create an instance of ProcessUpdateResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Link.parse_obj(obj)
+            return ProcessUpdateResult.parse_obj(obj)
 
-        _obj = Link.parse_obj({
-            "relation": obj.get("relation"),
-            "href": obj.get("href"),
-            "description": obj.get("description"),
-            "method": obj.get("method")
+        _obj = ProcessUpdateResult.parse_obj({
+            "domain": obj.get("domain"),
+            "entry_id": obj.get("entryId"),
+            "process_name": obj.get("processName"),
+            "run_id": obj.get("runId"),
+            "entry_date": obj.get("entryDate"),
+            "status": obj.get("status"),
+            "message": obj.get("message"),
+            "schema_version": obj.get("schemaVersion")
         })
         return _obj
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_entity.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, constr
 
 class LusidEntity(BaseModel):
     """
     Information about the LUSID entity this data can be used with  # noqa: E501
     """
     entity_type: constr(strict=True, min_length=1) = Field(..., alias="entityType", description="The entity type")
     entity_type_display_name: constr(strict=True, min_length=1) = Field(..., alias="entityTypeDisplayName", description="The display name for the entity type.")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_field.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_field.py`

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
 
 class LusidField(BaseModel):
     """
     A field on a LUSID entity  # noqa: E501
     """
     field_name: constr(strict=True, min_length=1) = Field(..., alias="fieldName", description="The name of the LUSID field.")
     default_value: Optional[StrictStr] = Field(None, alias="defaultValue", description="The default value for the field.")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_problem_details.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_problem_details.py`

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
 
 class LusidProblemDetails(BaseModel):
     """
     LusidProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_definition.py`

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
 from finbourne_horizon.models.resource_id import ResourceId
 
 class LusidPropertyDefinition(BaseModel):
     """
     Defines the information in a LUSID Property Definition  # noqa: E501
     """
     key: StrictStr = Field(..., description="Property key associated with the mapping")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_definition_overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class LusidPropertyDefinitionOverrides(BaseModel):
     """
     Override values for property Display Name and Description  # noqa: E501
     """
     display_name_override: Optional[StrictStr] = Field(None, alias="displayNameOverride")
     description_override: Optional[StrictStr] = Field(None, alias="descriptionOverride")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_definition_overrides_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class LusidPropertyDefinitionOverridesResponse(BaseModel):
     """
     An item that has been updated as a result of setting LusidPropertyDefinitionOverrides.  # noqa: E501
     """
     action: StrictStr = Field(..., description="The action performed on this property. \"upsert\" for setting values for new and existing              properties. \"delete\" for existing properties that were removed")
     write_error: Optional[StrictStr] = Field(None, alias="writeError")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 from finbourne_horizon.models.lusid_property_definition import LusidPropertyDefinition
 from finbourne_horizon.models.optionality import Optionality
 
 class LusidPropertyToVendorFieldMapping(BaseModel):
     """
     The mapping of a LUSID Property to the Vendor Field that would populate it  # noqa: E501
     """
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_validation_problem_details.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/lusid_validation_problem_details.py`

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
 
 class LusidValidationProblemDetails(BaseModel):
     """
     LusidValidationProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_request.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/onboard_instrument_request.py`

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
 from finbourne_horizon.models.open_figi_perm_id_result import OpenFigiPermIdResult
 
 class OnboardInstrumentRequest(BaseModel):
     """
     The full structure of a instrument creation / onboarding request  # noqa: E501
     """
     data_results: conlist(OpenFigiPermIdResult) = Field(..., alias="dataResults", description="Enumerable packed OpenFigi/PermId information used to create instruments")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_response.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/onboard_instrument_response.py`

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
 
 class OnboardInstrumentResponse(BaseModel):
     """
     Simplified structure converted from the LUSID UpsertInstrumentReponse  # noqa: E501
     """
     href: Optional[StrictStr] = Field(None, description="The specific Uniform Resource Identifier (URI) for this resource at the requested effective and asAt datetime.")
     values: conlist(StrictStr) = Field(..., description="The instruments which have been successfully updated or created.")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_data.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_data.py`

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
 
 class OpenFigiData(BaseModel):
     """
     OpenFIGI data structure  # noqa: E501
     """
     figi: StrictStr = Field(..., description="FIGI assigned to the instrument.")
     name: Optional[StrictStr] = Field(None, description="Various attributes of the instrument")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_parameter_option_name.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_parameter_option_name.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_perm_id_result.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_perm_id_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_horizon.models.open_figi_data import OpenFigiData
 from finbourne_horizon.models.perm_id_data import PermIdData
 
 class OpenFigiPermIdResult(BaseModel):
     """
     A packed WebAPI OpenFigi DTO and PermId DTO  # noqa: E501
     """
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_search_result.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/open_figi_search_result.py`

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
 from finbourne_horizon.models.open_figi_data import OpenFigiData
 
 class OpenFigiSearchResult(BaseModel):
     """
     Response coming back from a search request to OpenFIGI  # noqa: E501
     """
     results: conlist(OpenFigiData) = Field(..., description="Enumerable list of OpenFIGI results")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/optionality.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/optionality.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_information.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/paged_resource_list_of_process_information.py`

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
 from finbourne_horizon.models.link import Link
 from finbourne_horizon.models.process_information import ProcessInformation
 
 class PagedResourceListOfProcessInformation(BaseModel):
     """
     PagedResourceListOfProcessInformation
     """
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_update_result.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/paged_resource_list_of_process_update_result.py`

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
 from finbourne_horizon.models.link import Link
 from finbourne_horizon.models.process_update_result import ProcessUpdateResult
 
 class PagedResourceListOfProcessUpdateResult(BaseModel):
     """
     PagedResourceListOfProcessUpdateResult
     """
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_vendor_product.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/paged_resource_list_of_vendor_product.py`

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
 from finbourne_horizon.models.link import Link
 from finbourne_horizon.models.vendor_product import VendorProduct
 
 class PagedResourceListOfVendorProduct(BaseModel):
     """
     PagedResourceListOfVendorProduct
     """
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/perm_id_data.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/perm_id_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr
 
 class PermIdData(BaseModel):
     """
     PermId Data Structure  # noqa: E501
     """
     figi: StrictStr = Field(..., description=">FIGI assigned to the instrument.")
     ticker: StrictStr = Field(..., description="Ticker assigned to the instrument")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_information.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/process_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 from finbourne_horizon.models.process_summary import ProcessSummary
 
 class ProcessInformation(BaseModel):
     """
     Required information for each process  # noqa: E501
     """
     domain: StrictStr = Field(...)
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_summary.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/process_summary.py`

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
 from finbourne_horizon.models.file_details import FileDetails
 from finbourne_horizon.models.row_details import RowDetails
 
 class ProcessSummary(BaseModel):
     """
     Completed event details  # noqa: E501
     """
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_update_result.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/audit_update_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
-class ProcessUpdateResult(BaseModel):
+class AuditUpdateRequest(BaseModel):
     """
-    Shows details relevant to update events for a query  # noqa: E501
+    An incoming request for a Horizon Update Event  # noqa: E501
     """
-    domain: StrictStr = Field(...)
-    entry_id: StrictStr = Field(..., alias="entryId")
-    process_name: StrictStr = Field(..., alias="processName")
-    run_id: StrictStr = Field(..., alias="runId")
-    entry_date: datetime = Field(..., alias="entryDate")
-    status: StrictStr = Field(...)
-    message: StrictStr = Field(...)
-    schema_version: Optional[StrictStr] = Field(None, alias="schemaVersion")
-    __properties = ["domain", "entryId", "processName", "runId", "entryDate", "status", "message", "schemaVersion"]
+    id: StrictStr = Field(..., description="A unique ID identifiying the source of the event")
+    user_id: StrictStr = Field(..., alias="userId", description="A unique ID identifiying who owns the schedule")
+    scheduler_run_id: StrictStr = Field(..., alias="schedulerRunId", description="The GUID of the schedule run")
+    start_time: datetime = Field(..., alias="startTime", description="When the run was started in UTC")
+    message: StrictStr = Field(..., description="A descriptive message to accompany the status")
+    process_name_override: Optional[StrictStr] = Field(None, alias="processNameOverride", description="Optional Name for how the process appears in Data Feed Monitoring")
+    __properties = ["id", "userId", "schedulerRunId", "startTime", "message", "processNameOverride"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -45,44 +43,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ProcessUpdateResult:
-        """Create an instance of ProcessUpdateResult from a JSON string"""
+    def from_json(cls, json_str: str) -> AuditUpdateRequest:
+        """Create an instance of AuditUpdateRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if schema_version (nullable) is None
+        # set to None if process_name_override (nullable) is None
         # and __fields_set__ contains the field
-        if self.schema_version is None and "schema_version" in self.__fields_set__:
-            _dict['schemaVersion'] = None
+        if self.process_name_override is None and "process_name_override" in self.__fields_set__:
+            _dict['processNameOverride'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ProcessUpdateResult:
-        """Create an instance of ProcessUpdateResult from a dict"""
+    def from_dict(cls, obj: dict) -> AuditUpdateRequest:
+        """Create an instance of AuditUpdateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ProcessUpdateResult.parse_obj(obj)
+            return AuditUpdateRequest.parse_obj(obj)
 
-        _obj = ProcessUpdateResult.parse_obj({
-            "domain": obj.get("domain"),
-            "entry_id": obj.get("entryId"),
-            "process_name": obj.get("processName"),
-            "run_id": obj.get("runId"),
-            "entry_date": obj.get("entryDate"),
-            "status": obj.get("status"),
+        _obj = AuditUpdateRequest.parse_obj({
+            "id": obj.get("id"),
+            "user_id": obj.get("userId"),
+            "scheduler_run_id": obj.get("schedulerRunId"),
+            "start_time": obj.get("startTime"),
             "message": obj.get("message"),
-            "schema_version": obj.get("schemaVersion")
+            "process_name_override": obj.get("processNameOverride")
         })
         return _obj
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_request.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 from finbourne_horizon.models.query_specification import QuerySpecification
 
 class QueryRequest(BaseModel):
     """
     Used to control queries, including getting \"pages\" of data  # noqa: E501
     """
     specification: Optional[QuerySpecification] = None
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_specification.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/query_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt
+from pydantic.v1 import BaseModel, Field, StrictInt
 
 class QuerySpecification(BaseModel):
     """
     Defines the information that can be used to query a set of data.  # noqa: E501
     """
     limit: Optional[StrictInt] = Field(None, description="The maximum number of results to be returned in a \"page\"")
     __properties = ["limit"]
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/resource_id.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/resource_id.py`

 * *Files 4% similar despite different names*

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

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/row_details.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/row_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt
+from pydantic.v1 import BaseModel, Field, StrictInt
 
 class RowDetails(BaseModel):
     """
     Information about the nuber of rows processed.  # noqa: E501
     """
     rows_total: Optional[StrictInt] = Field(None, alias="rowsTotal", description="The number of rows processed.")
     rows_succeeded: Optional[StrictInt] = Field(None, alias="rowsSucceeded", description="The number of rows that were successfully processed.")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/trigger.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/trigger.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class Trigger(BaseModel):
     """
     Trigger
     """
     type: StrictStr = Field(...)
     cron_expression: StrictStr = Field(..., alias="cronExpression")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/update_instance_request.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/update_instance_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist
 from finbourne_horizon.models.trigger import Trigger
 
 class UpdateInstanceRequest(BaseModel):
     """
     UpdateInstanceRequest
     """
     id: StrictStr = Field(...)
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/vendor_product.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/models/vendor_product.py`

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
 from finbourne_horizon.models.lusid_entity import LusidEntity
 
 class VendorProduct(BaseModel):
     """
     Denormalised information about vendors, the products they provide and the LUSID entity types hey can be ued to populate.  # noqa: E501
     """
     vendor_name: StrictStr = Field(..., alias="vendorName")
```

### Comparing `finbourne_horizon_sdk-2.0.99/finbourne_horizon/rest.py` & `finbourne_horizon_sdk-2.1.1/finbourne_horizon/rest.py`

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

### Comparing `finbourne_horizon_sdk-2.0.99/pyproject.toml` & `finbourne_horizon_sdk-2.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-horizon-sdk"
-version = "2.0.99"
+version = "2.1.1"
 description = "FINBOURNE Horizon API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/horizon-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Horizon API", "finbourne-horizon-sdk"]
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

### Comparing `finbourne_horizon_sdk-2.0.99/PKG-INFO` & `finbourne_horizon_sdk-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-horizon-sdk
-Version: 2.0.99
+Version: 2.1.1
 Summary: FINBOURNE Horizon API
 Home-page: https://github.com/finbourne/horizon-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Horizon API,finbourne-horizon-sdk
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
 Project-URL: Repository, https://github.com/finbourne/horizon-sdk-python
 Description-Content-Type: text/markdown
 
 # finbourne-horizon-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.393
-- Package version: 2.0.99
+- API version: 0.1.438
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -82,16 +82,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_FINBOURNE_HORIZON_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_FINBOURNE_HORIZON_API_URL,
 FBN_ACCESS_TOKEN
 ```
@@ -221,15 +220,15 @@
 *InstrumentApi* | [**get_open_figi_parameter_option**](docs/InstrumentApi.md#get_open_figi_parameter_option) | **GET** /api/instrument/onboarding/search/openfigi/parameterOptions | [EARLY ACCESS] GetOpenFigiParameterOption: Get all supported market sector values for OpenFigi search
 *InstrumentApi* | [**retrieve_perm_id_result**](docs/InstrumentApi.md#retrieve_perm_id_result) | **GET** /api/instrument/onboarding/search/permid/{id} | [EARLY ACCESS] RetrievePermIdResult: Retrieve PermId results from a previous query.
 *InstrumentApi* | [**search_open_figi**](docs/InstrumentApi.md#search_open_figi) | **GET** /api/instrument/onboarding/search/openfigi | [EARLY ACCESS] SearchOpenFigi: Search OpenFigi for instruments that match the specified terms.
 *InstrumentApi* | [**vendors**](docs/InstrumentApi.md#vendors) | **GET** /api/instrument/onboarding/vendors | [EARLY ACCESS] Vendors: Gets the VendorProducts of any supported and licenced integrations for a given market sector and security type.
 *IntegrationsApi* | [**create_instance**](docs/IntegrationsApi.md#create_instance) | **POST** /api/integrations/instances | [EXPERIMENTAL] CreateInstance: Create a single integration instance.
 *IntegrationsApi* | [**delete_instance**](docs/IntegrationsApi.md#delete_instance) | **DELETE** /api/integrations/instances/{instanceId} | [EXPERIMENTAL] DeleteInstance: Delete a single integration instance.
 *IntegrationsApi* | [**execute_instance**](docs/IntegrationsApi.md#execute_instance) | **POST** /api/integrations/instances/{instanceId}/execute | [EXPERIMENTAL] ExecuteInstance: Execute an integration instance.
-*IntegrationsApi* | [**get_execution_ids_for_instance**](docs/IntegrationsApi.md#get_execution_ids_for_instance) | **GET** /api/integrations/executions/{instanceId} | [EXPERIMENTAL] GetExecutionIdsForInstance: Get integration instance execution ids.
+*IntegrationsApi* | [**get_execution_ids_for_instance**](docs/IntegrationsApi.md#get_execution_ids_for_instance) | **GET** /api/integrations/instances/{instanceId}/executions | [EXPERIMENTAL] GetExecutionIdsForInstance: Get integration instance execution ids.
 *IntegrationsApi* | [**get_schema**](docs/IntegrationsApi.md#get_schema) | **GET** /api/integrations/schema/{integration} | [EXPERIMENTAL] GetSchema: Get the JSON schema for the details section of an integration instance.
 *IntegrationsApi* | [**list_instances**](docs/IntegrationsApi.md#list_instances) | **GET** /api/integrations/instances | [EXPERIMENTAL] ListInstances: List instances across all integrations.
 *IntegrationsApi* | [**list_integrations**](docs/IntegrationsApi.md#list_integrations) | **GET** /api/integrations | [EXPERIMENTAL] ListIntegrations: List available integrations.
 *IntegrationsApi* | [**update_instance**](docs/IntegrationsApi.md#update_instance) | **PUT** /api/integrations/instances/{instanceId} | [EXPERIMENTAL] UpdateInstance: Update a single integration instance.
 *ProcessHistoryApi* | [**create_complete_event**](docs/ProcessHistoryApi.md#create_complete_event) | **POST** /api/process-history/event/complete | [EARLY ACCESS] CreateCompleteEvent: Write a completed event to the Horizon Dashboard
 *ProcessHistoryApi* | [**create_update_event**](docs/ProcessHistoryApi.md#create_update_event) | **POST** /api/process-history/event/update | [EARLY ACCESS] CreateUpdateEvent: Write an update event to the Horizon Dashboard
 *ProcessHistoryApi* | [**get_latest_runs**](docs/ProcessHistoryApi.md#get_latest_runs) | **GET** /api/process-history/$latestRuns | [EARLY ACCESS] GetLatestRuns: Get latest run for each process
```

