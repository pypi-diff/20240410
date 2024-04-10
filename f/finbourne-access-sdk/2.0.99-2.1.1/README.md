# Comparing `tmp/finbourne_access_sdk-2.0.99.tar.gz` & `tmp/finbourne_access_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_access_sdk-2.0.99.tar", max compression
+gzip compressed data, was "finbourne_access_sdk-2.1.1.tar", max compression
```

## Comparing `finbourne_access_sdk-2.0.99.tar` & `finbourne_access_sdk-2.1.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    17797 2024-02-27 14:29:40.902362 finbourne_access_sdk-2.0.99/README.md
--rw-r--r--   0        0        0     7542 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/__init__.py
--rw-r--r--   0        0        0      373 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/__init__.py
--rw-r--r--   0        0        0     7548 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/application_metadata_api.py
--rw-r--r--   0        0        0   160681 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/policies_api.py
--rw-r--r--   0        0        0    55448 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/policy_templates_api.py
--rw-r--r--   0        0        0    68280 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/roles_api.py
--rw-r--r--   0        0        0    76095 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/user_roles_api.py
--rw-r--r--   0        0        0    30808 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api_client.py
--rw-r--r--   0        0        0      852 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/api_response.py
--rw-r--r--   0        0        0    14461 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/configuration.py
--rw-r--r--   0        0        0     5348 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/exceptions.py
--rw-r--r--   0        0        0      298 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/__init__.py
--rw-r--r--   0        0        0    30677 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client.py
--rw-r--r--   0        0        0     9783 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8107 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_configuration.py
--rw-r--r--   0        0        0     6804 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12709 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/rest.py
--rw-r--r--   0        0        0    11575 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3888 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     6672 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/__init__.py
--rw-r--r--   0        0        0     3915 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_action.py
--rw-r--r--   0        0        0     4858 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2076 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/action_id.py
--rw-r--r--   0        0        0     2702 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_collection_to_role_request.py
--rw-r--r--   0        0        0     2458 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_to_role_request.py
--rw-r--r--   0        0        0     3820 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/add_to_policy_collection_request.py
--rw-r--r--   0        0        0     2560 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_predicate_contract.py
--rw-r--r--   0        0        0     2485 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_range_for_spec.py
--rw-r--r--   0        0        0     2463 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_relative.py
--rw-r--r--   0        0        0     6885 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/attached_policy_definition_response.py
--rw-r--r--   0        0        0     1096 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/date_quality.py
--rw-r--r--   0        0        0      781 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/date_unit.py
--rw-r--r--   0        0        0     1968 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_has_quality.py
--rw-r--r--   0        0        0     2535 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_relative.py
--rw-r--r--   0        0        0     2145 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/effective_range.py
--rw-r--r--   0        0        0     2384 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/entitlement_metadata.py
--rw-r--r--   0        0        0     2622 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_request.py
--rw-r--r--   0        0        0     2470 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_response.py
--rw-r--r--   0        0        0      766 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_result.py
--rw-r--r--   0        0        0     4456 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/for_spec.py
--rw-r--r--   0        0        0     3646 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/generate_policy_from_template_request.py
--rw-r--r--   0        0        0     3728 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/generated_policy_components.py
--rw-r--r--   0        0        0      654 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/grant.py
--rw-r--r--   0        0        0     2864 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/how_spec.py
--rw-r--r--   0        0        0     3188 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/id_selector_definition.py
--rw-r--r--   0        0        0     3113 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/identifier_part_schema.py
--rw-r--r--   0        0        0     4380 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_expression.py
--rw-r--r--   0        0        0     2432 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_feature_chain_expression.py
--rw-r--r--   0        0        0     3648 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_claim_expression.py
--rw-r--r--   0        0        0     2322 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_scope_expression.py
--rw-r--r--   0        0        0     2493 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_request_header_expression.py
--rw-r--r--   0        0        0     2416 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/key_value_pair_of_string_to_string.py
--rw-r--r--   0        0        0     2268 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/link.py
--rw-r--r--   0        0        0     3863 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4699 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3112 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/match_all_selector_definition.py
--rw-r--r--   0        0        0     2445 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_expression.py
--rw-r--r--   0        0        0     3744 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_selector_definition.py
--rw-r--r--   0        0        0     2045 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/non_transitive_supervisor_role_resource.py
--rw-r--r--   0        0        0      847 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/operator.py
--rw-r--r--   0        0        0      995 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/point_in_time_specification.py
--rw-r--r--   0        0        0     6046 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_creation_request.py
--rw-r--r--   0        0        0     2942 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_id.py
--rw-r--r--   0        0        0     5202 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_response.py
--rw-r--r--   0        0        0     5464 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_update_request.py
--rw-r--r--   0        0        0     6881 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_creation_request.py
--rw-r--r--   0        0        0     2862 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id.py
--rw-r--r--   0        0        0     3543 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id_role_resource.py
--rw-r--r--   0        0        0     7548 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_response.py
--rw-r--r--   0        0        0     4489 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_selector_definition.py
--rw-r--r--   0        0        0     3683 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_creation_request.py
--rw-r--r--   0        0        0     5273 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_response.py
--rw-r--r--   0        0        0     3150 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_update_request.py
--rw-r--r--   0        0        0     2644 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_templated_selector.py
--rw-r--r--   0        0        0      697 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_type.py
--rw-r--r--   0        0        0     6361 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_update_request.py
--rw-r--r--   0        0        0      829 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/relative_to_date_time.py
--rw-r--r--   0        0        0     3863 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/remove_from_policy_collection_request.py
--rw-r--r--   0        0        0     4248 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/request_details.py
--rw-r--r--   0        0        0     3116 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/requested_action_key.py
--rw-r--r--   0        0        0     3219 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_details.py
--rw-r--r--   0        0        0     4265 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4265 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_collection_response.py
--rw-r--r--   0        0        0     4144 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_response.py
--rw-r--r--   0        0        0     4241 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_template_response.py
--rw-r--r--   0        0        0     4169 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_user_role_response.py
--rw-r--r--   0        0        0     3483 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_creation_request.py
--rw-r--r--   0        0        0     2846 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_id.py
--rw-r--r--   0        0        0     3208 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_resource_request.py
--rw-r--r--   0        0        0     4779 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_response.py
--rw-r--r--   0        0        0     3021 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_update_request.py
--rw-r--r--   0        0        0     4280 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/selector_definition.py
--rw-r--r--   0        0        0     3120 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/template_metadata.py
--rw-r--r--   0        0        0     3412 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/template_selection.py
--rw-r--r--   0        0        0     1071 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/text_operator.py
--rw-r--r--   0        0        0     2813 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_creation_request.py
--rw-r--r--   0        0        0     3271 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_response.py
--rw-r--r--   0        0        0     2259 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_update_request.py
--rw-r--r--   0        0        0     2144 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/when_spec.py
--rw-r--r--   0        0        0        0 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/py.typed
--rw-r--r--   0        0        0    10040 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/rest.py
--rw-r--r--   0        0        0      891 2024-02-27 14:29:40.902362 finbourne_access_sdk-2.0.99/pyproject.toml
--rw-r--r--   0        0        0    18882 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.0.99/PKG-INFO
+-rw-r--r--   0        0        0    17778 2024-04-10 10:43:02.041273 finbourne_access_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0    10462 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api/__init__.py
+-rw-r--r--   0        0        0     7551 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api/application_metadata_api.py
+-rw-r--r--   0        0        0   160687 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api/policies_api.py
+-rw-r--r--   0        0        0    55454 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api/policy_templates_api.py
+-rw-r--r--   0        0        0    68286 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api/roles_api.py
+-rw-r--r--   0        0        0    76101 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api/user_roles_api.py
+-rw-r--r--   0        0        0    30808 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/api_response.py
+-rw-r--r--   0        0        0    14461 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/configuration.py
+-rw-r--r--   0        0        0     5348 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/exceptions.py
+-rw-r--r--   0        0        0      593 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/__init__.py
+-rw-r--r--   0        0        0    30677 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/extensions/api_client.py
+-rw-r--r--   0        0        0     9882 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8107 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6804 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12709 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/extensions/rest.py
+-rw-r--r--   0        0        0    11575 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3888 2024-04-10 10:43:02.037274 finbourne_access_sdk-2.1.1/finbourne_access/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     8919 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/__init__.py
+-rw-r--r--   0        0        0     3918 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4861 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2079 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/action_id.py
+-rw-r--r--   0        0        0     2705 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/add_policy_collection_to_role_request.py
+-rw-r--r--   0        0        0     2461 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/add_policy_to_role_request.py
+-rw-r--r--   0        0        0     3823 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/add_to_policy_collection_request.py
+-rw-r--r--   0        0        0     2563 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/as_at_predicate_contract.py
+-rw-r--r--   0        0        0     2488 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/as_at_range_for_spec.py
+-rw-r--r--   0        0        0     2466 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/as_at_relative.py
+-rw-r--r--   0        0        0     6888 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/attached_policy_definition_response.py
+-rw-r--r--   0        0        0     1096 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/date_quality.py
+-rw-r--r--   0        0        0      781 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/date_unit.py
+-rw-r--r--   0        0        0     1971 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/effective_date_has_quality.py
+-rw-r--r--   0        0        0     2538 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/effective_date_relative.py
+-rw-r--r--   0        0        0     2148 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/effective_range.py
+-rw-r--r--   0        0        0     2387 2024-04-10 10:43:02.032273 finbourne_access_sdk-2.1.1/finbourne_access/models/entitlement_metadata.py
+-rw-r--r--   0        0        0     2625 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/evaluation_request.py
+-rw-r--r--   0        0        0     2473 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/evaluation_response.py
+-rw-r--r--   0        0        0      766 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/evaluation_result.py
+-rw-r--r--   0        0        0     4459 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/for_spec.py
+-rw-r--r--   0        0        0     3649 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/generate_policy_from_template_request.py
+-rw-r--r--   0        0        0     3731 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/generated_policy_components.py
+-rw-r--r--   0        0        0      654 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/grant.py
+-rw-r--r--   0        0        0     2867 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/how_spec.py
+-rw-r--r--   0        0        0     3191 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3116 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     4383 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/if_expression.py
+-rw-r--r--   0        0        0     2435 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/if_feature_chain_expression.py
+-rw-r--r--   0        0        0     3651 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/if_identity_claim_expression.py
+-rw-r--r--   0        0        0     2325 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/if_identity_scope_expression.py
+-rw-r--r--   0        0        0     2496 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/if_request_header_expression.py
+-rw-r--r--   0        0        0     2419 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/key_value_pair_of_string_to_string.py
+-rw-r--r--   0        0        0     2271 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/link.py
+-rw-r--r--   0        0        0     3866 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4702 2024-04-10 10:43:02.033274 finbourne_access_sdk-2.1.1/finbourne_access/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3115 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/match_all_selector_definition.py
+-rw-r--r--   0        0        0     2448 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/metadata_expression.py
+-rw-r--r--   0        0        0     3747 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/metadata_selector_definition.py
+-rw-r--r--   0        0        0     2048 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/non_transitive_supervisor_role_resource.py
+-rw-r--r--   0        0        0      847 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/operator.py
+-rw-r--r--   0        0        0      995 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/point_in_time_specification.py
+-rw-r--r--   0        0        0     6049 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_creation_request.py
+-rw-r--r--   0        0        0     2945 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_id.py
+-rw-r--r--   0        0        0     5205 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_response.py
+-rw-r--r--   0        0        0     5467 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_update_request.py
+-rw-r--r--   0        0        0     6884 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_creation_request.py
+-rw-r--r--   0        0        0     2865 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_id.py
+-rw-r--r--   0        0        0     3546 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_id_role_resource.py
+-rw-r--r--   0        0        0     7551 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_response.py
+-rw-r--r--   0        0        0     4492 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_selector_definition.py
+-rw-r--r--   0        0        0     3686 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_template_creation_request.py
+-rw-r--r--   0        0        0     5276 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_template_response.py
+-rw-r--r--   0        0        0     3153 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_template_update_request.py
+-rw-r--r--   0        0        0     2647 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_templated_selector.py
+-rw-r--r--   0        0        0      697 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_type.py
+-rw-r--r--   0        0        0     6364 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/policy_update_request.py
+-rw-r--r--   0        0        0      829 2024-04-10 10:43:02.034273 finbourne_access_sdk-2.1.1/finbourne_access/models/relative_to_date_time.py
+-rw-r--r--   0        0        0     3866 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/remove_from_policy_collection_request.py
+-rw-r--r--   0        0        0     4251 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/request_details.py
+-rw-r--r--   0        0        0     3119 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/requested_action_key.py
+-rw-r--r--   0        0        0     3222 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/resource_details.py
+-rw-r--r--   0        0        0     4268 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4268 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_policy_collection_response.py
+-rw-r--r--   0        0        0     4147 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_policy_response.py
+-rw-r--r--   0        0        0     4244 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_policy_template_response.py
+-rw-r--r--   0        0        0     4172 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_user_role_response.py
+-rw-r--r--   0        0        0     3486 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/role_creation_request.py
+-rw-r--r--   0        0        0     2849 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/role_id.py
+-rw-r--r--   0        0        0     3211 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/role_resource_request.py
+-rw-r--r--   0        0        0     4782 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/role_response.py
+-rw-r--r--   0        0        0     3024 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/role_update_request.py
+-rw-r--r--   0        0        0     4283 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/selector_definition.py
+-rw-r--r--   0        0        0     3123 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/template_metadata.py
+-rw-r--r--   0        0        0     3415 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/template_selection.py
+-rw-r--r--   0        0        0     1071 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/text_operator.py
+-rw-r--r--   0        0        0     2816 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/user_role_creation_request.py
+-rw-r--r--   0        0        0     3274 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/user_role_response.py
+-rw-r--r--   0        0        0     2262 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/user_role_update_request.py
+-rw-r--r--   0        0        0     2147 2024-04-10 10:43:02.035273 finbourne_access_sdk-2.1.1/finbourne_access/models/when_spec.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/py.typed
+-rw-r--r--   0        0        0    10171 2024-04-10 10:43:02.036273 finbourne_access_sdk-2.1.1/finbourne_access/rest.py
+-rw-r--r--   0        0        0      889 2024-04-10 10:43:02.042273 finbourne_access_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18861 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.1.1/PKG-INFO
```

### Comparing `finbourne_access_sdk-2.0.99/README.md` & `finbourne_access_sdk-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3721
-- Package version: 2.0.99
+- API version: 0.0.3767
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -56,16 +56,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_FINBOURNE_ACCESS_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_FINBOURNE_ACCESS_API_URL,
 FBN_ACCESS_TOKEN
 ```
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api/application_metadata_api.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from finbourne_access.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 from finbourne_access.api_client import ApiClient
 from finbourne_access.api_response import ApiResponse
 from finbourne_access.exceptions import (  # noqa: F401
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api/policies_api.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api/policies_api.py`

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
 
-from pydantic import Field, StrictInt, StrictStr, conint, conlist, constr, validator
+from pydantic.v1 import Field, StrictInt, StrictStr, conint, conlist, constr, validator
 
 from typing import Dict, List, Optional
 
 from finbourne_access.models.add_to_policy_collection_request import AddToPolicyCollectionRequest
 from finbourne_access.models.attached_policy_definition_response import AttachedPolicyDefinitionResponse
 from finbourne_access.models.evaluation_request import EvaluationRequest
 from finbourne_access.models.evaluation_response import EvaluationResponse
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api/policy_templates_api.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api/policy_templates_api.py`

 * *Files 1% similar despite different names*

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
 
 from finbourne_access.models.generate_policy_from_template_request import GeneratePolicyFromTemplateRequest
 from finbourne_access.models.generated_policy_components import GeneratedPolicyComponents
 from finbourne_access.models.policy_template_creation_request import PolicyTemplateCreationRequest
 from finbourne_access.models.policy_template_response import PolicyTemplateResponse
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api/roles_api.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api/roles_api.py`

 * *Files 1% similar despite different names*

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
 
-from pydantic import Field, StrictInt, StrictStr, conlist, constr, validator
+from pydantic.v1 import Field, StrictInt, StrictStr, conlist, constr, validator
 
 from typing import List, Optional
 
 from finbourne_access.models.add_policy_collection_to_role_request import AddPolicyCollectionToRoleRequest
 from finbourne_access.models.role_creation_request import RoleCreationRequest
 from finbourne_access.models.role_response import RoleResponse
 from finbourne_access.models.role_update_request import RoleUpdateRequest
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api/user_roles_api.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api/user_roles_api.py`

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
-from pydantic import Field, StrictStr, conint, constr, validator
+from pydantic.v1 import Field, StrictStr, conint, constr, validator
 
 from typing import Optional
 
 from finbourne_access.models.add_policy_collection_to_role_request import AddPolicyCollectionToRoleRequest
 from finbourne_access.models.add_policy_to_role_request import AddPolicyToRoleRequest
 from finbourne_access.models.resource_list_of_user_role_response import ResourceListOfUserRoleResponse
 from finbourne_access.models.user_role_creation_request import UserRoleCreationRequest
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api_client.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/api_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/configuration.py` & `finbourne_access_sdk-2.1.1/finbourne_access/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_access-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.3721\n"\
+               "Version of the API: 0.0.3767\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/exceptions.py` & `finbourne_access_sdk-2.1.1/finbourne_access/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client_factory.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/api_client_factory.py`

 * *Files 0% similar despite different names*

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

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_configuration.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/configuration_loaders.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/proxy_config.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/refreshing_token.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/rest.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/retry.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/socket_keep_alive.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/extensions/tcp_keep_alive_connector.py` & `finbourne_access_sdk-2.1.1/finbourne_access/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_action.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_access.models.action_id import ActionId
 from finbourne_access.models.id_selector_definition import IdSelectorDefinition
 from finbourne_access.models.link import Link
 
 class AccessControlledAction(BaseModel):
     """
     AccessControlledAction
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_resource.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/access_controlled_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_access.models.access_controlled_action import AccessControlledAction
 from finbourne_access.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_access.models.link import Link
 
 class AccessControlledResource(BaseModel):
     """
     AccessControlledResource
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/action_id.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_id.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,25 +14,41 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from typing import Any, Dict, Optional
+from pydantic.v1 import BaseModel, Field, constr, validator
 
-class ActionId(BaseModel):
+class PolicyId(BaseModel):
     """
-    ActionId
+    PolicyId
     """
-    scope: constr(strict=True, max_length=100, min_length=3) = Field(...)
-    activity: constr(strict=True, max_length=25, min_length=3) = Field(...)
-    entity: constr(strict=True, max_length=25, min_length=3) = Field(...)
-    __properties = ["scope", "activity", "entity"]
+    scope: Optional[constr(strict=True, max_length=100, min_length=3)] = None
+    code: constr(strict=True, max_length=100, min_length=3) = Field(...)
+    __properties = ["scope", "code"]
+
+    @validator('scope')
+    def scope_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if value is None:
+            return value
+
+        if not re.match(r"^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$", value):
+            raise ValueError(r"must validate the regular expression /^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$/")
+        return value
+
+    @validator('code')
+    def code_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$", value):
+            raise ValueError(r"must validate the regular expression /^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$/")
+        return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,34 +56,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ActionId:
-        """Create an instance of ActionId from a JSON string"""
+    def from_json(cls, json_str: str) -> PolicyId:
+        """Create an instance of PolicyId from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if scope (nullable) is None
+        # and __fields_set__ contains the field
+        if self.scope is None and "scope" in self.__fields_set__:
+            _dict['scope'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ActionId:
-        """Create an instance of ActionId from a dict"""
+    def from_dict(cls, obj: dict) -> PolicyId:
+        """Create an instance of PolicyId from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ActionId.parse_obj(obj)
+            return PolicyId.parse_obj(obj)
 
-        _obj = ActionId.parse_obj({
+        _obj = PolicyId.parse_obj({
             "scope": obj.get("scope"),
-            "activity": obj.get("activity"),
-            "entity": obj.get("entity")
+            "code": obj.get("code")
         })
         return _obj
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_collection_to_role_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/add_policy_collection_to_role_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 
 class AddPolicyCollectionToRoleRequest(BaseModel):
     """
     Request body used to add Policy Collections to a Role  # noqa: E501
     """
     policy_collections: conlist(PolicyCollectionId) = Field(..., alias="policyCollections", description="Identifiers of policy collections to add to a role")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_to_role_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/add_policy_to_role_request.py`

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
 from finbourne_access.models.policy_id import PolicyId
 
 class AddPolicyToRoleRequest(BaseModel):
     """
     Request body used to add Policies to a Role  # noqa: E501
     """
     policies: conlist(PolicyId) = Field(..., description="Identifiers of policies to add to a role")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/add_to_policy_collection_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/add_to_policy_collection_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 from finbourne_access.models.policy_id import PolicyId
 
 class AddToPolicyCollectionRequest(BaseModel):
     """
     Base properties to create or update a policy collection  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_predicate_contract.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/as_at_predicate_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class AsAtPredicateContract(BaseModel):
     """
     AsAtPredicateContract
     """
     value: Optional[constr(strict=True, max_length=25, min_length=5)] = None
     date_time_offset: Optional[datetime] = Field(None, alias="dateTimeOffset")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_range_for_spec.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/as_at_range_for_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.as_at_predicate_contract import AsAtPredicateContract
 
 class AsAtRangeForSpec(BaseModel):
     """
     AsAtRangeForSpec
     """
     var_from: AsAtPredicateContract = Field(..., alias="from")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_relative.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/as_at_relative.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt
+from pydantic.v1 import BaseModel, Field, StrictInt
 from finbourne_access.models.date_unit import DateUnit
 from finbourne_access.models.point_in_time_specification import PointInTimeSpecification
 from finbourne_access.models.relative_to_date_time import RelativeToDateTime
 
 class AsAtRelative(BaseModel):
     """
     AsAtRelative
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/attached_policy_definition_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/attached_policy_definition_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist
 from finbourne_access.models.for_spec import ForSpec
 from finbourne_access.models.grant import Grant
 from finbourne_access.models.how_spec import HowSpec
 from finbourne_access.models.if_expression import IfExpression
 from finbourne_access.models.policy_id import PolicyId
 from finbourne_access.models.policy_type import PolicyType
 from finbourne_access.models.role_id import RoleId
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/date_quality.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/date_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/date_unit.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/date_unit.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_has_quality.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/effective_date_has_quality.py`

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
 from finbourne_access.models.date_quality import DateQuality
 
 class EffectiveDateHasQuality(BaseModel):
     """
     EffectiveDateHasQuality
     """
     quality: Optional[DateQuality] = None
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_relative.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/effective_date_relative.py`

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
 from finbourne_access.models.date_unit import DateUnit
 from finbourne_access.models.point_in_time_specification import PointInTimeSpecification
 from finbourne_access.models.relative_to_date_time import RelativeToDateTime
 
 class EffectiveDateRelative(BaseModel):
     """
     EffectiveDateRelative
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/effective_range.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/effective_range.py`

 * *Files 6% similar despite different names*

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
 
 class EffectiveRange(BaseModel):
     """
     EffectiveRange
     """
     var_from: Optional[datetime] = Field(None, alias="from")
     to: Optional[datetime] = None
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/entitlement_metadata.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/entitlement_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic.v1 import BaseModel, StrictStr
 
 class EntitlementMetadata(BaseModel):
     """
     EntitlementMetadata
     """
     provider: Optional[StrictStr] = None
     value: Optional[StrictStr] = None
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/evaluation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.request_details import RequestDetails
 from finbourne_access.models.resource_details import ResourceDetails
 
 class EvaluationRequest(BaseModel):
     """
     Specification for a server side evaluation of entitlement.  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/evaluation_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 from finbourne_access.models.evaluation_result import EvaluationResult
 
 class EvaluationResponse(BaseModel):
     """
     The result of an evaluation request  # noqa: E501
     """
     result: EvaluationResult = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_result.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/for_spec.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/for_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.as_at_range_for_spec import AsAtRangeForSpec
 from finbourne_access.models.as_at_relative import AsAtRelative
 from finbourne_access.models.effective_date_has_quality import EffectiveDateHasQuality
 from finbourne_access.models.effective_date_relative import EffectiveDateRelative
 from finbourne_access.models.effective_range import EffectiveRange
 
 class ForSpec(BaseModel):
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/generate_policy_from_template_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/generate_policy_from_template_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.selector_definition import SelectorDefinition
 from finbourne_access.models.template_selection import TemplateSelection
 
 class GeneratePolicyFromTemplateRequest(BaseModel):
     """
     Generate policy from template  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/generated_policy_components.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/generated_policy_components.py`

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
 from finbourne_access.models.selector_definition import SelectorDefinition
 from finbourne_access.models.template_metadata import TemplateMetadata
 
 class GeneratedPolicyComponents(BaseModel):
     """
     Response object for policy generated from template  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/grant.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/grant.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/how_spec.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/how_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, StrictStr, conlist
+from pydantic.v1 import BaseModel, StrictStr, conlist
 from finbourne_access.models.key_value_pair_of_string_to_string import KeyValuePairOfStringToString
 
 class HowSpec(BaseModel):
     """
     HowSpec
     """
     type: Optional[StrictStr] = None
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/id_selector_definition.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/id_selector_definition.py`

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
 from finbourne_access.models.action_id import ActionId
 
 class IdSelectorDefinition(BaseModel):
     """
     IdSelectorDefinition
     """
     identifier: Dict[str, StrictStr] = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/identifier_part_schema.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, conlist, constr
 from finbourne_access.models.link import Link
 
 class IdentifierPartSchema(BaseModel):
     """
     IdentifierPartSchema
     """
     index: StrictInt = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/if_expression.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/if_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.if_feature_chain_expression import IfFeatureChainExpression
 from finbourne_access.models.if_identity_claim_expression import IfIdentityClaimExpression
 from finbourne_access.models.if_identity_scope_expression import IfIdentityScopeExpression
 from finbourne_access.models.if_request_header_expression import IfRequestHeaderExpression
 
 class IfExpression(BaseModel):
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/if_feature_chain_expression.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/if_feature_chain_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.selector_definition import SelectorDefinition
 
 class IfFeatureChainExpression(BaseModel):
     """
     IfFeatureChainExpression
     """
     selectors: conlist(SelectorDefinition) = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_claim_expression.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/if_identity_claim_expression.py`

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
 from finbourne_access.models.text_operator import TextOperator
 
 class IfIdentityClaimExpression(BaseModel):
     """
     IfIdentityClaimExpression
     """
     claim_type: constr(strict=True, min_length=1) = Field(..., alias="claimType")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_scope_expression.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/if_identity_scope_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class IfIdentityScopeExpression(BaseModel):
     """
     IfIdentityScopeExpression
     """
     scope_name: constr(strict=True, min_length=1) = Field(..., alias="scopeName")
     __properties = ["scopeName"]
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/if_request_header_expression.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/if_request_header_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 from finbourne_access.models.text_operator import TextOperator
 
 class IfRequestHeaderExpression(BaseModel):
     """
     IfRequestHeaderExpression
     """
     header_name: constr(strict=True, max_length=1024, min_length=1) = Field(..., alias="headerName")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/key_value_pair_of_string_to_string.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/key_value_pair_of_string_to_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic.v1 import BaseModel, StrictStr
 
 class KeyValuePairOfStringToString(BaseModel):
     """
     KeyValuePairOfStringToString
     """
     key: Optional[StrictStr] = None
     value: Optional[StrictStr] = None
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/link.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/link.py`

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

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_problem_details.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/lusid_problem_details.py`

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

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_validation_problem_details.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/lusid_validation_problem_details.py`

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

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/match_all_selector_definition.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/match_all_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_access.models.action_id import ActionId
 
 class MatchAllSelectorDefinition(BaseModel):
     """
     MatchAllSelectorDefinition
     """
     actions: conlist(ActionId, min_items=1) = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_expression.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/metadata_expression.py`

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
 from finbourne_access.models.operator import Operator
 
 class MetadataExpression(BaseModel):
     """
     MetadataExpression
     """
     metadata_key: constr(strict=True, min_length=1) = Field(..., alias="metadataKey")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_selector_definition.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/metadata_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_access.models.action_id import ActionId
 from finbourne_access.models.metadata_expression import MetadataExpression
 
 class MetadataSelectorDefinition(BaseModel):
     """
     MetadataSelectorDefinition
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/non_transitive_supervisor_role_resource.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/non_transitive_supervisor_role_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 
 class NonTransitiveSupervisorRoleResource(BaseModel):
     """
     NonTransitiveSupervisorRoleResource
     """
     roles: conlist(Dict[str, StrictStr], min_items=1) = Field(...)
     __properties = ["roles"]
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/operator.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/point_in_time_specification.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/point_in_time_specification.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_creation_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_creation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, conlist, constr, validator
 from finbourne_access.models.entitlement_metadata import EntitlementMetadata
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 from finbourne_access.models.policy_id import PolicyId
 
 class PolicyCollectionCreationRequest(BaseModel):
     """
     Create a PolicyCollection, a logical group of Policies or other PolicyCollections  # noqa: E501
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_id.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class PolicyCollectionId(BaseModel):
     """
     PolicyCollectionId
     """
     scope: Optional[constr(strict=True, max_length=100, min_length=3)] = None
     code: constr(strict=True, max_length=100, min_length=3) = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_response.py`

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
 from finbourne_access.models.link import Link
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 from finbourne_access.models.policy_id import PolicyId
 
 class PolicyCollectionResponse(BaseModel):
     """
     A PolicyCollection encapsulating one or more Policies and PolicyCollections  # noqa: E501
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_update_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_collection_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_access.models.entitlement_metadata import EntitlementMetadata
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 from finbourne_access.models.policy_id import PolicyId
 
 class PolicyCollectionUpdateRequest(BaseModel):
     """
     Update an existing PolicyCollection  # noqa: E501
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_creation_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_creation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 from finbourne_access.models.for_spec import ForSpec
 from finbourne_access.models.grant import Grant
 from finbourne_access.models.how_spec import HowSpec
 from finbourne_access.models.if_expression import IfExpression
 from finbourne_access.models.selector_definition import SelectorDefinition
 from finbourne_access.models.template_metadata import TemplateMetadata
 from finbourne_access.models.when_spec import WhenSpec
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/role_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
-class PolicyId(BaseModel):
+class RoleId(BaseModel):
     """
-    PolicyId
+    RoleId
     """
     scope: Optional[constr(strict=True, max_length=100, min_length=3)] = None
     code: constr(strict=True, max_length=100, min_length=3) = Field(...)
     __properties = ["scope", "code"]
 
     @validator('scope')
     def scope_validate_regular_expression(cls, value):
@@ -56,16 +56,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PolicyId:
-        """Create an instance of PolicyId from a JSON string"""
+    def from_json(cls, json_str: str) -> RoleId:
+        """Create an instance of RoleId from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -74,20 +74,20 @@
         # and __fields_set__ contains the field
         if self.scope is None and "scope" in self.__fields_set__:
             _dict['scope'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PolicyId:
-        """Create an instance of PolicyId from a dict"""
+    def from_dict(cls, obj: dict) -> RoleId:
+        """Create an instance of RoleId from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PolicyId.parse_obj(obj)
+            return RoleId.parse_obj(obj)
 
-        _obj = PolicyId.parse_obj({
+        _obj = RoleId.parse_obj({
             "scope": obj.get("scope"),
             "code": obj.get("code")
         })
         return _obj
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id_role_resource.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_id_role_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 from finbourne_access.models.policy_id import PolicyId
 
 class PolicyIdRoleResource(BaseModel):
     """
     PolicyIdRoleResource
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_response.py`

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
 from finbourne_access.models.for_spec import ForSpec
 from finbourne_access.models.grant import Grant
 from finbourne_access.models.how_spec import HowSpec
 from finbourne_access.models.if_expression import IfExpression
 from finbourne_access.models.link import Link
 from finbourne_access.models.policy_id import PolicyId
 from finbourne_access.models.selector_definition import SelectorDefinition
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_selector_definition.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_access.models.action_id import ActionId
 
 class PolicySelectorDefinition(BaseModel):
     """
     PolicySelectorDefinition
     """
     identity_restriction: Optional[Dict[str, StrictStr]] = Field(None, alias="identityRestriction")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_creation_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_template_creation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, conlist, constr, validator
 from finbourne_access.models.policy_templated_selector import PolicyTemplatedSelector
 
 class PolicyTemplateCreationRequest(BaseModel):
     """
     Request to create a policy template  # noqa: E501
     """
     code: constr(strict=True, max_length=100, min_length=3) = Field(..., description="The Code of the policy template being created")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_template_response.py`

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
 from finbourne_access.models.policy_templated_selector import PolicyTemplatedSelector
 
 class PolicyTemplateResponse(BaseModel):
     """
     Response object for a policy template  # noqa: E501
     """
     display_name: Optional[StrictStr] = Field(None, alias="displayName", description="Display name of the policy template being created")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_update_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_template_update_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_access.models.policy_templated_selector import PolicyTemplatedSelector
 
 class PolicyTemplateUpdateRequest(BaseModel):
     """
     Update policy template request  # noqa: E501
     """
     display_name: constr(strict=True, max_length=512, min_length=1) = Field(..., alias="displayName", description="The display name of the policy template being created")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_templated_selector.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_templated_selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 from finbourne_access.models.selector_definition import SelectorDefinition
 
 class PolicyTemplatedSelector(BaseModel):
     """
     Templated selector for a policy template  # noqa: E501
     """
     application: constr(strict=True, min_length=1) = Field(..., description="The application that this selector definition applies to")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_type.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_type.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_update_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/policy_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_access.models.for_spec import ForSpec
 from finbourne_access.models.grant import Grant
 from finbourne_access.models.how_spec import HowSpec
 from finbourne_access.models.if_expression import IfExpression
 from finbourne_access.models.selector_definition import SelectorDefinition
 from finbourne_access.models.template_metadata import TemplateMetadata
 from finbourne_access.models.when_spec import WhenSpec
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/relative_to_date_time.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/relative_to_date_time.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/remove_from_policy_collection_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/remove_from_policy_collection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.policy_collection_id import PolicyCollectionId
 from finbourne_access.models.policy_id import PolicyId
 
 class RemoveFromPolicyCollectionRequest(BaseModel):
     """
     Base properties to create or update a policy collection  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/request_details.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/request_details.py`

 * *Files 2% similar despite different names*

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
 from finbourne_access.models.requested_action_key import RequestedActionKey
 
 class RequestDetails(BaseModel):
     """
     The details of the requested evaluation  # noqa: E501
     """
     action: RequestedActionKey = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/requested_action_key.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/requested_action_key.py`

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
 
 class RequestedActionKey(BaseModel):
     """
     A fully qualified action identifier  # noqa: E501
     """
     entity_code: constr(strict=True, max_length=100, min_length=3) = Field(..., alias="entityCode", description="The type of the resource on which the activity would be performed")
     scope: constr(strict=True, max_length=100, min_length=3) = Field(..., description="The scope/provider/vendor of the activity")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_details.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/resource_details.py`

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
 from finbourne_access.models.entitlement_metadata import EntitlementMetadata
 
 class ResourceDetails(BaseModel):
     """
     Details about the resource being requested that may be pertinent to the entitlement evaluation  # noqa: E501
     """
     id: Dict[str, StrictStr] = Field(..., description="The identifier of the resource being evaluated")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_access_controlled_resource.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_access_controlled_resource.py`

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
 from finbourne_access.models.access_controlled_resource import AccessControlledResource
 from finbourne_access.models.link import Link
 
 class ResourceListOfAccessControlledResource(BaseModel):
     """
     ResourceListOfAccessControlledResource
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_collection_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_policy_collection_response.py`

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
 from finbourne_access.models.link import Link
 from finbourne_access.models.policy_collection_response import PolicyCollectionResponse
 
 class ResourceListOfPolicyCollectionResponse(BaseModel):
     """
     ResourceListOfPolicyCollectionResponse
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_policy_response.py`

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
 from finbourne_access.models.link import Link
 from finbourne_access.models.policy_response import PolicyResponse
 
 class ResourceListOfPolicyResponse(BaseModel):
     """
     ResourceListOfPolicyResponse
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_template_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_policy_template_response.py`

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
 from finbourne_access.models.link import Link
 from finbourne_access.models.policy_template_response import PolicyTemplateResponse
 
 class ResourceListOfPolicyTemplateResponse(BaseModel):
     """
     ResourceListOfPolicyTemplateResponse
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_user_role_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/resource_list_of_user_role_response.py`

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
 from finbourne_access.models.link import Link
 from finbourne_access.models.user_role_response import UserRoleResponse
 
 class ResourceListOfUserRoleResponse(BaseModel):
     """
     ResourceListOfUserRoleResponse
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/role_creation_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/role_creation_request.py`

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
 from finbourne_access.models.role_resource_request import RoleResourceRequest
 from finbourne_access.models.when_spec import WhenSpec
 
 class RoleCreationRequest(BaseModel):
     """
     Request to create a role  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/role_id.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/template_selection.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,31 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from typing import Any, Dict, List, Optional
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 
-class RoleId(BaseModel):
+class TemplateSelection(BaseModel):
     """
-    RoleId
+    A template selection, identifying a policy template to use for generation  # noqa: E501
     """
-    scope: Optional[constr(strict=True, max_length=100, min_length=3)] = None
-    code: constr(strict=True, max_length=100, min_length=3) = Field(...)
-    __properties = ["scope", "code"]
+    scope: constr(strict=True, max_length=100, min_length=3) = Field(..., description="Scope identifying policy template to use for generation")
+    code: constr(strict=True, max_length=100, min_length=3) = Field(..., description="Code identifying policy template to use for generation")
+    selector_tags: Optional[conlist(StrictStr)] = Field(None, alias="selectorTags", description="List of selector tags to optionally filter in the template generation   (Eg: Feature, Data, etc)")
+    __properties = ["scope", "code", "selectorTags"]
 
     @validator('scope')
     def scope_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if value is None:
-            return value
-
         if not re.match(r"^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$", value):
             raise ValueError(r"must validate the regular expression /^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$/")
         return value
 
     @validator('code')
     def code_validate_regular_expression(cls, value):
         """Validates the regular expression"""
@@ -56,38 +54,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> RoleId:
-        """Create an instance of RoleId from a JSON string"""
+    def from_json(cls, json_str: str) -> TemplateSelection:
+        """Create an instance of TemplateSelection from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if scope (nullable) is None
+        # set to None if selector_tags (nullable) is None
         # and __fields_set__ contains the field
-        if self.scope is None and "scope" in self.__fields_set__:
-            _dict['scope'] = None
+        if self.selector_tags is None and "selector_tags" in self.__fields_set__:
+            _dict['selectorTags'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> RoleId:
-        """Create an instance of RoleId from a dict"""
+    def from_dict(cls, obj: dict) -> TemplateSelection:
+        """Create an instance of TemplateSelection from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return RoleId.parse_obj(obj)
+            return TemplateSelection.parse_obj(obj)
 
-        _obj = RoleId.parse_obj({
+        _obj = TemplateSelection.parse_obj({
             "scope": obj.get("scope"),
-            "code": obj.get("code")
+            "code": obj.get("code"),
+            "selector_tags": obj.get("selectorTags")
         })
         return _obj
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/role_resource_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/role_resource_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.non_transitive_supervisor_role_resource import NonTransitiveSupervisorRoleResource
 from finbourne_access.models.policy_id_role_resource import PolicyIdRoleResource
 
 class RoleResourceRequest(BaseModel):
     """
     RoleResourceRequest  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/role_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/role_response.py`

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
 from finbourne_access.models.link import Link
 from finbourne_access.models.role_id import RoleId
 from finbourne_access.models.role_resource_request import RoleResourceRequest
 from finbourne_access.models.when_spec import WhenSpec
 
 class RoleResponse(BaseModel):
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/role_update_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/role_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 from finbourne_access.models.role_resource_request import RoleResourceRequest
 from finbourne_access.models.when_spec import WhenSpec
 
 class RoleUpdateRequest(BaseModel):
     """
     Role update does not allow the changing of the id  # noqa: E501
     """
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/selector_definition.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/selector_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.id_selector_definition import IdSelectorDefinition
 from finbourne_access.models.match_all_selector_definition import MatchAllSelectorDefinition
 from finbourne_access.models.metadata_selector_definition import MetadataSelectorDefinition
 
 class SelectorDefinition(BaseModel):
     """
     SelectorDefinition
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/template_metadata.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/template_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.template_selection import TemplateSelection
 
 class TemplateMetadata(BaseModel):
     """
     Extra policy template metadata information, used during a generation request  # noqa: E501
     """
     template_selection: Optional[conlist(TemplateSelection)] = Field(None, alias="templateSelection", description="List of policy templates used for a generation request")
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/template_selection.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/user_role_creation_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,35 +14,28 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field, constr, validator
+from finbourne_access.models.policy_id_role_resource import PolicyIdRoleResource
 
-class TemplateSelection(BaseModel):
+class UserRoleCreationRequest(BaseModel):
     """
-    A template selection, identifying a policy template to use for generation  # noqa: E501
+    Dto used to request creating a user's role  # noqa: E501
     """
-    scope: constr(strict=True, max_length=100, min_length=3) = Field(..., description="Scope identifying policy template to use for generation")
-    code: constr(strict=True, max_length=100, min_length=3) = Field(..., description="Code identifying policy template to use for generation")
-    selector_tags: Optional[conlist(StrictStr)] = Field(None, alias="selectorTags", description="List of selector tags to optionally filter in the template generation   (Eg: Feature, Data, etc)")
-    __properties = ["scope", "code", "selectorTags"]
+    user_id: constr(strict=True, min_length=1) = Field(..., alias="userId", description="The Id of the user for whom to create the role.")
+    resource: PolicyIdRoleResource = Field(...)
+    __properties = ["userId", "resource"]
 
-    @validator('scope')
-    def scope_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$", value):
-            raise ValueError(r"must validate the regular expression /^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$/")
-        return value
-
-    @validator('code')
-    def code_validate_regular_expression(cls, value):
+    @validator('user_id')
+    def user_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$", value):
             raise ValueError(r"must validate the regular expression /^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$/")
         return value
 
     class Config:
         """Pydantic configuration"""
@@ -54,39 +47,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TemplateSelection:
-        """Create an instance of TemplateSelection from a JSON string"""
+    def from_json(cls, json_str: str) -> UserRoleCreationRequest:
+        """Create an instance of UserRoleCreationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if selector_tags (nullable) is None
-        # and __fields_set__ contains the field
-        if self.selector_tags is None and "selector_tags" in self.__fields_set__:
-            _dict['selectorTags'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of resource
+        if self.resource:
+            _dict['resource'] = self.resource.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TemplateSelection:
-        """Create an instance of TemplateSelection from a dict"""
+    def from_dict(cls, obj: dict) -> UserRoleCreationRequest:
+        """Create an instance of UserRoleCreationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return TemplateSelection.parse_obj(obj)
+            return UserRoleCreationRequest.parse_obj(obj)
 
-        _obj = TemplateSelection.parse_obj({
-            "scope": obj.get("scope"),
-            "code": obj.get("code"),
-            "selector_tags": obj.get("selectorTags")
+        _obj = UserRoleCreationRequest.parse_obj({
+            "user_id": obj.get("userId"),
+            "resource": PolicyIdRoleResource.from_dict(obj.get("resource")) if obj.get("resource") is not None else None
         })
         return _obj
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/text_operator.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/text_operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_creation_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/action_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,31 +15,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
-from finbourne_access.models.policy_id_role_resource import PolicyIdRoleResource
+from pydantic.v1 import BaseModel, Field, constr
 
-class UserRoleCreationRequest(BaseModel):
+class ActionId(BaseModel):
     """
-    Dto used to request creating a user's role  # noqa: E501
+    ActionId
     """
-    user_id: constr(strict=True, min_length=1) = Field(..., alias="userId", description="The Id of the user for whom to create the role.")
-    resource: PolicyIdRoleResource = Field(...)
-    __properties = ["userId", "resource"]
-
-    @validator('user_id')
-    def user_id_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$", value):
-            raise ValueError(r"must validate the regular expression /^(?=.*[a-zA-Z])[\w][\w +-]{2,100}$/")
-        return value
+    scope: constr(strict=True, max_length=100, min_length=3) = Field(...)
+    activity: constr(strict=True, max_length=25, min_length=3) = Field(...)
+    entity: constr(strict=True, max_length=25, min_length=3) = Field(...)
+    __properties = ["scope", "activity", "entity"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -47,36 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserRoleCreationRequest:
-        """Create an instance of UserRoleCreationRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> ActionId:
+        """Create an instance of ActionId from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of resource
-        if self.resource:
-            _dict['resource'] = self.resource.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserRoleCreationRequest:
-        """Create an instance of UserRoleCreationRequest from a dict"""
+    def from_dict(cls, obj: dict) -> ActionId:
+        """Create an instance of ActionId from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UserRoleCreationRequest.parse_obj(obj)
+            return ActionId.parse_obj(obj)
 
-        _obj = UserRoleCreationRequest.parse_obj({
-            "user_id": obj.get("userId"),
-            "resource": PolicyIdRoleResource.from_dict(obj.get("resource")) if obj.get("resource") is not None else None
+        _obj = ActionId.parse_obj({
+            "scope": obj.get("scope"),
+            "activity": obj.get("activity"),
+            "entity": obj.get("entity")
         })
         return _obj
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_response.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/user_role_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_access.models.link import Link
 from finbourne_access.models.role_id import RoleId
 from finbourne_access.models.role_resource_request import RoleResourceRequest
 
 class UserRoleResponse(BaseModel):
     """
     Response object from the user role API  # noqa: E501
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_update_request.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/user_role_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_access.models.policy_id_role_resource import PolicyIdRoleResource
 
 class UserRoleUpdateRequest(BaseModel):
     """
     Dto used to request updating a user's role  # noqa: E501
     """
     resource: PolicyIdRoleResource = Field(...)
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/models/when_spec.py` & `finbourne_access_sdk-2.1.1/finbourne_access/models/when_spec.py`

 * *Files 2% similar despite different names*

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
 
 class WhenSpec(BaseModel):
     """
     WhenSpec
     """
     activate: datetime = Field(...)
     deactivate: Optional[datetime] = None
```

### Comparing `finbourne_access_sdk-2.0.99/finbourne_access/rest.py` & `finbourne_access_sdk-2.1.1/finbourne_access/rest.py`

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

### Comparing `finbourne_access_sdk-2.0.99/pyproject.toml` & `finbourne_access_sdk-2.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-access-sdk"
-version = "2.0.99"
+version = "2.1.1"
 description = "FINBOURNE Access Management API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-access-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Access Management API", "finbourne-access-sdk"]
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

### Comparing `finbourne_access_sdk-2.0.99/PKG-INFO` & `finbourne_access_sdk-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-access-sdk
-Version: 2.0.99
+Version: 2.1.1
 Summary: FINBOURNE Access Management API
 Home-page: https://github.com/finbourne/finbourne-access-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Access Management API,finbourne-access-sdk
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
 Project-URL: Repository, https://github.com/finbourne/finbourne-access-sdk-python
 Description-Content-Type: text/markdown
 
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3721
-- Package version: 2.0.99
+- API version: 0.0.3767
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -82,16 +82,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_FINBOURNE_ACCESS_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_FINBOURNE_ACCESS_API_URL,
 FBN_ACCESS_TOKEN
 ```
```

