# Comparing `tmp/lusid_notifications_sdk-2.0.9.tar.gz` & `tmp/lusid_notifications_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_notifications_sdk-2.0.9.tar", max compression
+gzip compressed data, was "lusid_notifications_sdk-2.1.1.tar", max compression
```

## Comparing `lusid_notifications_sdk-2.0.9.tar` & `lusid_notifications_sdk-2.1.1.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0     9297 2024-01-16 10:29:34.453622 lusid_notifications_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     4665 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/__init__.py
--rw-r--r--   0        0        0      473 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/__init__.py
--rw-r--r--   0        0        0     7556 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0        0        0    13216 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0        0        0    14128 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/event_types_api.py
--rw-r--r--   0        0        0     8478 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/manual_event_api.py
--rw-r--r--   0        0        0    45083 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/notifications_api.py
--rw-r--r--   0        0        0    44721 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0        0        0    30825 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api_client.py
--rw-r--r--   0        0        0      852 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api_response.py
--rw-r--r--   0        0        0    14474 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/configuration.py
--rw-r--r--   0        0        0     5344 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/exceptions.py
--rw-r--r--   0        0        0      304 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/__init__.py
--rw-r--r--   0        0        0    30697 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client.py
--rw-r--r--   0        0        0     9813 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8032 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_configuration.py
--rw-r--r--   0        0        0     6888 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12712 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/rest.py
--rw-r--r--   0        0        0    11578 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3891 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3671 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/__init__.py
--rw-r--r--   0        0        0     3920 2024-01-16 10:29:34.444623 lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0        0        0     4863 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2072 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/action_id.py
--rw-r--r--   0        0        0     3443 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type.py
--rw-r--r--   0        0        0     3922 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type_response.py
--rw-r--r--   0        0        0     2519 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt.py
--rw-r--r--   0        0        0     2412 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt_status.py
--rw-r--r--   0        0        0     4248 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_notification_request.py
--rw-r--r--   0        0        0     5201 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_subscription.py
--rw-r--r--   0        0        0     3813 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/delivery.py
--rw-r--r--   0        0        0     5205 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type.py
--rw-r--r--   0        0        0     4817 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type_response.py
--rw-r--r--   0        0        0     2459 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_field_definition.py
--rw-r--r--   0        0        0     5524 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0        0        0     3187 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0        0        0     3112 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2264 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/link.py
--rw-r--r--   0        0        0     3859 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4695 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2530 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event.py
--rw-r--r--   0        0        0     3129 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_body.py
--rw-r--r--   0        0        0     3196 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_header.py
--rw-r--r--   0        0        0     2188 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_request.py
--rw-r--r--   0        0        0     3241 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0        0        0     5023 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification.py
--rw-r--r--   0        0        0     2404 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_status.py
--rw-r--r--   0        0        0     7237 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type.py
--rw-r--r--   0        0        0     7796 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type_response.py
--rw-r--r--   0        0        0     2079 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_id.py
--rw-r--r--   0        0        0     4267 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4073 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0        0        0     4159 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0        0        0     4121 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0        0        0     4121 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0        0        0     2911 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type.py
--rw-r--r--   0        0        0     3004 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type_response.py
--rw-r--r--   0        0        0     4770 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/subscription.py
--rw-r--r--   0        0        0     3701 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_notification_request.py
--rw-r--r--   0        0        0     4862 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_subscription.py
--rw-r--r--   0        0        0     5542 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type.py
--rw-r--r--   0        0        0     5672 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type_response.py
--rw-r--r--   0        0        0        0 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/py.typed
--rw-r--r--   0        0        0    10039 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/rest.py
--rw-r--r--   0        0        0      891 2024-01-16 10:29:34.453622 lusid_notifications_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    10373 1970-01-01 00:00:00.000000 lusid_notifications_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11699 2024-04-10 10:43:04.950297 lusid_notifications_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     6885 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/__init__.py
+-rw-r--r--   0        0        0      629 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/__init__.py
+-rw-r--r--   0        0        0     7559 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0        0        0    13222 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0        0        0    14134 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0        0        0     8484 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/manual_event_api.py
+-rw-r--r--   0        0        0    45089 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0        0        0    44727 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0        0        0    30825 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api_response.py
+-rw-r--r--   0        0        0    14474 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/configuration.py
+-rw-r--r--   0        0        0     5344 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/exceptions.py
+-rw-r--r--   0        0        0      602 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/__init__.py
+-rw-r--r--   0        0        0    30697 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client.py
+-rw-r--r--   0        0        0     9912 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8122 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6816 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12712 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/rest.py
+-rw-r--r--   0        0        0    11578 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3891 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     5187 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4866 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2075 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/action_id.py
+-rw-r--r--   0        0        0     3498 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type.py
+-rw-r--r--   0        0        0     3925 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0        0        0     3109 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_principal_auth_notification_type.py
+-rw-r--r--   0        0        0     3188 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_principal_auth_notification_type_response.py
+-rw-r--r--   0        0        0     2522 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt.py
+-rw-r--r--   0        0        0     2415 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0        0        0     4251 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_notification_request.py
+-rw-r--r--   0        0        0     5204 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0        0        0     3816 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/delivery.py
+-rw-r--r--   0        0        0     5208 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type.py
+-rw-r--r--   0        0        0     4820 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type_response.py
+-rw-r--r--   0        0        0     2462 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_field_definition.py
+-rw-r--r--   0        0        0     5527 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0        0        0     3190 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3115 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2267 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/link.py
+-rw-r--r--   0        0        0     3862 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4698 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2533 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event.py
+-rw-r--r--   0        0        0     3132 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_body.py
+-rw-r--r--   0        0        0     3199 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_header.py
+-rw-r--r--   0        0        0     2191 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_request.py
+-rw-r--r--   0        0        0     3244 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0        0        0     5026 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification.py
+-rw-r--r--   0        0        0     2407 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_status.py
+-rw-r--r--   0        0        0     8333 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type.py
+-rw-r--r--   0        0        0     9013 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type_response.py
+-rw-r--r--   0        0        0     2082 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_id.py
+-rw-r--r--   0        0        0     4270 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4076 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0        0        0     4162 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0        0        0     4124 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0        0        0     4124 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0        0        0     2914 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type.py
+-rw-r--r--   0        0        0     3007 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type_response.py
+-rw-r--r--   0        0        0     4773 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/subscription.py
+-rw-r--r--   0        0        0     3704 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_notification_request.py
+-rw-r--r--   0        0        0     4865 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0        0        0     5545 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type.py
+-rw-r--r--   0        0        0     5675 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type_response.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/py.typed
+-rw-r--r--   0        0        0    10170 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/rest.py
+-rw-r--r--   0        0        0      890 2024-04-10 10:43:04.951297 lusid_notifications_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12774 1970-01-01 00:00:00.000000 lusid_notifications_sdk-2.1.1/PKG-INFO
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/__init__.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,30 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
     Contact: info@finbourne.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-from __future__ import absolute_import
-
-# import apis into sdk package
-from lusid_notifications.api.application_metadata_api import ApplicationMetadataApi
-from lusid_notifications.api.deliveries_api import DeliveriesApi
-from lusid_notifications.api.event_types_api import EventTypesApi
-from lusid_notifications.api.manual_event_api import ManualEventApi
-from lusid_notifications.api.notifications_api import NotificationsApi
-from lusid_notifications.api.subscriptions_api import SubscriptionsApi
-
-# import ApiClient
-from lusid_notifications.api_client import ApiClient
-from lusid_notifications.configuration import Configuration
-from lusid_notifications.exceptions import OpenApiException
-from lusid_notifications.exceptions import ApiTypeError
-from lusid_notifications.exceptions import ApiValueError
-from lusid_notifications.exceptions import ApiKeyError
-from lusid_notifications.exceptions import ApiException
-# import models into sdk package
+# import models into model package
 from lusid_notifications.models.access_controlled_action import AccessControlledAction
 from lusid_notifications.models.access_controlled_resource import AccessControlledResource
 from lusid_notifications.models.action_id import ActionId
 from lusid_notifications.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notifications.models.amazon_sqs_notification_type_response import AmazonSqsNotificationTypeResponse
+from lusid_notifications.models.amazon_sqs_principal_auth_notification_type import AmazonSqsPrincipalAuthNotificationType
+from lusid_notifications.models.amazon_sqs_principal_auth_notification_type_response import AmazonSqsPrincipalAuthNotificationTypeResponse
 from lusid_notifications.models.attempt import Attempt
 from lusid_notifications.models.attempt_status import AttemptStatus
 from lusid_notifications.models.create_notification_request import CreateNotificationRequest
 from lusid_notifications.models.create_subscription import CreateSubscription
 from lusid_notifications.models.delivery import Delivery
 from lusid_notifications.models.email_notification_type import EmailNotificationType
 from lusid_notifications.models.email_notification_type_response import EmailNotificationTypeResponse
@@ -71,9 +54,53 @@
 from lusid_notifications.models.sms_notification_type_response import SmsNotificationTypeResponse
 from lusid_notifications.models.subscription import Subscription
 from lusid_notifications.models.update_notification_request import UpdateNotificationRequest
 from lusid_notifications.models.update_subscription import UpdateSubscription
 from lusid_notifications.models.webhook_notification_type import WebhookNotificationType
 from lusid_notifications.models.webhook_notification_type_response import WebhookNotificationTypeResponse
 
-# import extensions into sdk package
-from lusid_notifications.extensions import *
+
+__all__ = [
+    "AccessControlledAction",
+    "AccessControlledResource",
+    "ActionId",
+    "AmazonSqsNotificationType",
+    "AmazonSqsNotificationTypeResponse",
+    "AmazonSqsPrincipalAuthNotificationType",
+    "AmazonSqsPrincipalAuthNotificationTypeResponse",
+    "Attempt",
+    "AttemptStatus",
+    "CreateNotificationRequest",
+    "CreateSubscription",
+    "Delivery",
+    "EmailNotificationType",
+    "EmailNotificationTypeResponse",
+    "EventFieldDefinition",
+    "EventTypeSchema",
+    "IdSelectorDefinition",
+    "IdentifierPartSchema",
+    "Link",
+    "LusidProblemDetails",
+    "LusidValidationProblemDetails",
+    "ManualEvent",
+    "ManualEventBody",
+    "ManualEventHeader",
+    "ManualEventRequest",
+    "MatchingPattern",
+    "Notification",
+    "NotificationStatus",
+    "NotificationType",
+    "NotificationTypeResponse",
+    "ResourceId",
+    "ResourceListOfAccessControlledResource",
+    "ResourceListOfDelivery",
+    "ResourceListOfEventTypeSchema",
+    "ResourceListOfNotification",
+    "ResourceListOfSubscription",
+    "SmsNotificationType",
+    "SmsNotificationTypeResponse",
+    "Subscription",
+    "UpdateNotificationRequest",
+    "UpdateSubscription",
+    "WebhookNotificationType",
+    "WebhookNotificationTypeResponse"
+]
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api/application_metadata_api.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from lusid_notifications.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 from lusid_notifications.api_client import ApiClient
 from lusid_notifications.api_response import ApiResponse
 from lusid_notifications.exceptions import (  # noqa: F401
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api/deliveries_api.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api/deliveries_api.py`

 * *Files 1% similar despite different names*

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
-from pydantic import Field, StrictInt, constr, validator
+from pydantic.v1 import Field, StrictInt, constr, validator
 
 from typing import Optional
 
 from lusid_notifications.models.resource_list_of_delivery import ResourceListOfDelivery
 
 from lusid_notifications.api_client import ApiClient
 from lusid_notifications.api_response import ApiResponse
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api/event_types_api.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api/event_types_api.py`

 * *Files 1% similar despite different names*

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
-from pydantic import Field, constr, validator
+from pydantic.v1 import Field, constr, validator
 
 from lusid_notifications.models.event_type_schema import EventTypeSchema
 from lusid_notifications.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 
 from lusid_notifications.api_client import ApiClient
 from lusid_notifications.api_response import ApiResponse
 from lusid_notifications.exceptions import (  # noqa: F401
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api/manual_event_api.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api/manual_event_api.py`

 * *Files 2% similar despite different names*

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
-from pydantic import Field
+from pydantic.v1 import Field
 
 from lusid_notifications.models.manual_event import ManualEvent
 from lusid_notifications.models.manual_event_request import ManualEventRequest
 
 from lusid_notifications.api_client import ApiClient
 from lusid_notifications.api_response import ApiResponse
 from lusid_notifications.exceptions import (  # noqa: F401
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api/notifications_api.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api/notifications_api.py`

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
-from pydantic import Field, StrictStr, constr, validator
+from pydantic.v1 import Field, StrictStr, constr, validator
 
 from lusid_notifications.models.create_notification_request import CreateNotificationRequest
 from lusid_notifications.models.notification import Notification
 from lusid_notifications.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notifications.models.update_notification_request import UpdateNotificationRequest
 
 from lusid_notifications.api_client import ApiClient
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api/subscriptions_api.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api/subscriptions_api.py`

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
-from pydantic import Field, conint, constr, validator
+from pydantic.v1 import Field, conint, constr, validator
 
 from typing import Optional
 
 from lusid_notifications.models.create_subscription import CreateSubscription
 from lusid_notifications.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notifications.models.subscription import Subscription
 from lusid_notifications.models.update_subscription import UpdateSubscription
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api_client.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/api_response.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/configuration.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_notifications-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.906\n"\
+               "Version of the API: 0.1.929\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/exceptions.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client_factory.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client_factory.py`

 * *Files 2% similar despite different names*

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

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_configuration.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import logging
 from typing import Optional, Union, Tuple, Any, Callable
 from lusid_notifications.configuration import Configuration
 from lusid_notifications.extensions.refreshing_token import RefreshingToken
 from lusid_notifications.extensions.socket_keep_alive import keep_alive_socket_options
+from lusid_notifications.extensions.proxy_config import ProxyConfig
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

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/configuration_loaders.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/configuration_loaders.py`

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

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/proxy_config.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/proxy_config.py`

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

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/refreshing_token.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/rest.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/retry.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/socket_keep_alive.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/tcp_keep_alive_connector.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_action.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_action.py`

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
 from lusid_notifications.models.action_id import ActionId
 from lusid_notifications.models.id_selector_definition import IdSelectorDefinition
 from lusid_notifications.models.link import Link
 
 class AccessControlledAction(BaseModel):
     """
     AccessControlledAction
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_resource.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_resource.py`

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
 from lusid_notifications.models.access_controlled_action import AccessControlledAction
 from lusid_notifications.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notifications.models.link import Link
 
 class AccessControlledResource(BaseModel):
     """
     AccessControlledResource
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/action_id.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/action_id.py`

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
 
 class ActionId(BaseModel):
     """
     ActionId
     """
     scope: constr(strict=True, max_length=100, min_length=3) = Field(...)
     activity: constr(strict=True, max_length=25, min_length=3) = Field(...)
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type.py`

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
 
 class AmazonSqsNotificationType(BaseModel):
     """
     The information required to create or update an AWS SQS notification  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of delivery mechanism for this notification")
     api_key_ref: constr(strict=True, min_length=1) = Field(..., alias="apiKeyRef", description="Reference to API key from Configuration Store")
@@ -31,16 +31,16 @@
     body: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The body of the Amazon Queue Message")
     queue_url_ref: constr(strict=True, min_length=1) = Field(..., alias="queueUrlRef", description="Reference to queue url from Configuration Store")
     __properties = ["type", "apiKeyRef", "apiSecretRef", "body", "queueUrlRef"]
 
     @validator('type')
     def type_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in ('AmazonSqs', 'Email', 'Sms', 'Webhook'):
-            raise ValueError("must be one of enum values ('AmazonSqs', 'Email', 'Sms', 'Webhook')")
+        if value not in ('AmazonSqs', 'AmazonSqsPrincipalAuth', 'Email', 'Sms', 'Webhook'):
+            raise ValueError("must be one of enum values ('AmazonSqs', 'AmazonSqsPrincipalAuth', 'Email', 'Sms', 'Webhook')")
         return value
 
     @validator('body')
     def body_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[\s\S]*$", value):
             raise ValueError(r"must validate the regular expression /^[\s\S]*$/")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type_response.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type_response.py`

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
 
 class AmazonSqsNotificationTypeResponse(BaseModel):
     """
     Holds readonly information about an AWS SQS notification  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of delivery mechanism for this notification")
     api_key_ref: Optional[StrictStr] = Field(None, alias="apiKeyRef", description="Reference to API key from Configuration Store")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict
-from pydantic import BaseModel, Field, StrictInt
+from pydantic.v1 import BaseModel, Field, StrictInt
 from lusid_notifications.models.attempt_status import AttemptStatus
 
 class Attempt(BaseModel):
     """
     Details of an attempt of delivery.  # noqa: E501
     """
     attempt_number: StrictInt = Field(..., alias="attemptNumber", description="The attempt number of the delivery.")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt_status.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt_status.py`

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
 
 class AttemptStatus(BaseModel):
     """
     Status of the delivery attempt.  # noqa: E501
     """
     result: constr(strict=True, min_length=1) = Field(..., description="Result of the delivery.")
     detailed_message: Optional[StrictStr] = Field(None, alias="detailedMessage", description="The detailed message from attempting to deliver the message.")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_notification_request.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_notification_request.py`

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
 from lusid_notifications.models.notification_type import NotificationType
 
 class CreateNotificationRequest(BaseModel):
     """
     The information required to create a notification  # noqa: E501
     """
     notification_id: constr(strict=True, max_length=100, min_length=1) = Field(..., alias="notificationId", description="The identifier of the notification.")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_subscription.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_subscription.py`

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
 from lusid_notifications.models.matching_pattern import MatchingPattern
 from lusid_notifications.models.resource_id import ResourceId
 
 class CreateSubscription(BaseModel):
     """
     The information required to create a subscription  # noqa: E501
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/delivery.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_notifications.models.attempt import Attempt
 from lusid_notifications.models.resource_id import ResourceId
 
 class Delivery(BaseModel):
     """
     Delivery
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 
 class EmailNotificationType(BaseModel):
     """
     The information required to create or update an Email notification  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of delivery mechanism for this notification")
     subject: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The subject of the email")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type_response.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type_response.py`

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
 
 class EmailNotificationTypeResponse(BaseModel):
     """
     Holds readonly information about an Email notification  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of delivery mechanism for this notification")
     subject: Optional[StrictStr] = Field(None, description="The subject of the email")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_field_definition.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_field_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class EventFieldDefinition(BaseModel):
     """
     An EventFieldDefinition object  # noqa: E501
     """
     name: Optional[StrictStr] = Field(None, description="Name of the field")
     type: Optional[StrictStr] = Field(None, description="Type of the field")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_type_schema.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_type_schema.py`

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
 from lusid_notifications.models.event_field_definition import EventFieldDefinition
 
 class EventTypeSchema(BaseModel):
     """
     An EventType object  # noqa: E501
     """
     id: Optional[StrictStr] = Field(None, description="The identifier of the event type")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/id_selector_definition.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/id_selector_definition.py`

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
 from lusid_notifications.models.action_id import ActionId
 
 class IdSelectorDefinition(BaseModel):
     """
     IdSelectorDefinition
     """
     identifier: Dict[str, StrictStr] = Field(...)
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/identifier_part_schema.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/identifier_part_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, conlist, constr
 from lusid_notifications.models.link import Link
 
 class IdentifierPartSchema(BaseModel):
     """
     IdentifierPartSchema
     """
     index: StrictInt = Field(...)
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/link.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/link.py`

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
 
 class Link(BaseModel):
     """
     Link
     """
     relation: StrictStr = Field(...)
     href: StrictStr = Field(...)
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_problem_details.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_problem_details.py`

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

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_validation_problem_details.py`

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

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event.py`

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
 from lusid_notifications.models.manual_event_body import ManualEventBody
 from lusid_notifications.models.manual_event_header import ManualEventHeader
 
 class ManualEvent(BaseModel):
     """
     Details of a manually triggered event  # noqa: E501
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_body.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_body.py`

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
 
 class ManualEventBody(BaseModel):
     """
     The body of the manual event  # noqa: E501
     """
     subject: constr(strict=True, max_length=256, min_length=1) = Field(..., description="The subject of the manual event")
     message: constr(strict=True, max_length=2147483647, min_length=1) = Field(..., description="The message of the manual event")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_header.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_header.py`

 * *Files 1% similar despite different names*

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
 
 class ManualEventHeader(BaseModel):
     """
     The header of the manual event  # noqa: E501
     """
     event_type: Optional[StrictStr] = Field(None, alias="eventType", description="The event type of the manual event")
     timestamp: Optional[datetime] = Field(None, description="The timestamp of the manual event")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_request.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_request.py`

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
 from lusid_notifications.models.manual_event_body import ManualEventBody
 
 class ManualEventRequest(BaseModel):
     """
     The information required to trigger a manual event  # noqa: E501
     """
     body: ManualEventBody = Field(...)
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/matching_pattern.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/matching_pattern.py`

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
 
 class MatchingPattern(BaseModel):
     """
     A matching pattern object  # noqa: E501
     """
     event_type: constr(strict=True, max_length=512, min_length=0) = Field(..., alias="eventType", description="The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint.")
     filter: Optional[constr(strict=True, max_length=16384, min_length=0)] = Field(None, description="A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification.py`

 * *Files 0% similar despite different names*

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
 from lusid_notifications.models.notification_type_response import NotificationTypeResponse
 
 class Notification(BaseModel):
     """
     A notification object  # noqa: E501
     """
     notification_id: constr(strict=True, min_length=1) = Field(..., alias="notificationId", description="The identifier of the notification")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_status.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_status.py`

 * *Files 1% similar despite different names*

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
 
 class NotificationStatus(BaseModel):
     """
     The status object of a notification  # noqa: E501
     """
     result: Optional[StrictStr] = Field(None, description="The status of the notification")
     last_updated: Optional[datetime] = Field(None, alias="lastUpdated", description="The time at which the notification status was last updated")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,36 +17,39 @@
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_notifications.models.amazon_sqs_notification_type import AmazonSqsNotificationType
+from lusid_notifications.models.amazon_sqs_principal_auth_notification_type import AmazonSqsPrincipalAuthNotificationType
 from lusid_notifications.models.email_notification_type import EmailNotificationType
 from lusid_notifications.models.sms_notification_type import SmsNotificationType
 from lusid_notifications.models.webhook_notification_type import WebhookNotificationType
 from typing import Union, Any, List, TYPE_CHECKING
 from pydantic import StrictStr, Field
 
-NOTIFICATIONTYPE_ONE_OF_SCHEMAS = ["AmazonSqsNotificationType", "EmailNotificationType", "SmsNotificationType", "WebhookNotificationType"]
+NOTIFICATIONTYPE_ONE_OF_SCHEMAS = ["AmazonSqsNotificationType", "AmazonSqsPrincipalAuthNotificationType", "EmailNotificationType", "SmsNotificationType", "WebhookNotificationType"]
 
 class NotificationType(BaseModel):
     """
     Holds information about a Finbourne.Notifications.WebApi.Dtos.Notifications.Notification that is being created
     """
     # data type: AmazonSqsNotificationType
     oneof_schema_1_validator: Optional[AmazonSqsNotificationType] = None
+    # data type: AmazonSqsPrincipalAuthNotificationType
+    oneof_schema_2_validator: Optional[AmazonSqsPrincipalAuthNotificationType] = None
     # data type: EmailNotificationType
-    oneof_schema_2_validator: Optional[EmailNotificationType] = None
+    oneof_schema_3_validator: Optional[EmailNotificationType] = None
     # data type: SmsNotificationType
-    oneof_schema_3_validator: Optional[SmsNotificationType] = None
+    oneof_schema_4_validator: Optional[SmsNotificationType] = None
     # data type: WebhookNotificationType
-    oneof_schema_4_validator: Optional[WebhookNotificationType] = None
+    oneof_schema_5_validator: Optional[WebhookNotificationType] = None
     if TYPE_CHECKING:
-        actual_instance: Union[AmazonSqsNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType]
+        actual_instance: Union[AmazonSqsNotificationType, AmazonSqsPrincipalAuthNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType]
     else:
         actual_instance: Any
     one_of_schemas: List[str] = Field(NOTIFICATIONTYPE_ONE_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
@@ -66,14 +69,19 @@
         error_messages = []
         match = 0
         # validate data type: AmazonSqsNotificationType
         if not isinstance(v, AmazonSqsNotificationType):
             error_messages.append(f"Error! Input type `{type(v)}` is not `AmazonSqsNotificationType`")
         else:
             match += 1
+        # validate data type: AmazonSqsPrincipalAuthNotificationType
+        if not isinstance(v, AmazonSqsPrincipalAuthNotificationType):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `AmazonSqsPrincipalAuthNotificationType`")
+        else:
+            match += 1
         # validate data type: EmailNotificationType
         if not isinstance(v, EmailNotificationType):
             error_messages.append(f"Error! Input type `{type(v)}` is not `EmailNotificationType`")
         else:
             match += 1
         # validate data type: SmsNotificationType
         if not isinstance(v, SmsNotificationType):
@@ -83,18 +91,18 @@
         # validate data type: WebhookNotificationType
         if not isinstance(v, WebhookNotificationType):
             error_messages.append(f"Error! Input type `{type(v)}` is not `WebhookNotificationType`")
         else:
             match += 1
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in NotificationType with oneOf schemas: AmazonSqsNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in NotificationType with oneOf schemas: AmazonSqsNotificationType, AmazonSqsPrincipalAuthNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in NotificationType with oneOf schemas: AmazonSqsNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in NotificationType with oneOf schemas: AmazonSqsNotificationType, AmazonSqsPrincipalAuthNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> NotificationType:
         return cls.from_json(json.dumps(obj))
 
@@ -107,14 +115,20 @@
 
         # deserialize data into AmazonSqsNotificationType
         try:
             instance.actual_instance = AmazonSqsNotificationType.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # deserialize data into AmazonSqsPrincipalAuthNotificationType
+        try:
+            instance.actual_instance = AmazonSqsPrincipalAuthNotificationType.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # deserialize data into EmailNotificationType
         try:
             instance.actual_instance = EmailNotificationType.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into SmsNotificationType
@@ -128,18 +142,18 @@
             instance.actual_instance = WebhookNotificationType.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into NotificationType with oneOf schemas: AmazonSqsNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into NotificationType with oneOf schemas: AmazonSqsNotificationType, AmazonSqsPrincipalAuthNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into NotificationType with oneOf schemas: AmazonSqsNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into NotificationType with oneOf schemas: AmazonSqsNotificationType, AmazonSqsPrincipalAuthNotificationType, EmailNotificationType, SmsNotificationType, WebhookNotificationType. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type_response.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,36 +17,39 @@
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_notifications.models.amazon_sqs_notification_type_response import AmazonSqsNotificationTypeResponse
+from lusid_notifications.models.amazon_sqs_principal_auth_notification_type_response import AmazonSqsPrincipalAuthNotificationTypeResponse
 from lusid_notifications.models.email_notification_type_response import EmailNotificationTypeResponse
 from lusid_notifications.models.sms_notification_type_response import SmsNotificationTypeResponse
 from lusid_notifications.models.webhook_notification_type_response import WebhookNotificationTypeResponse
 from typing import Union, Any, List, TYPE_CHECKING
 from pydantic import StrictStr, Field
 
-NOTIFICATIONTYPERESPONSE_ONE_OF_SCHEMAS = ["AmazonSqsNotificationTypeResponse", "EmailNotificationTypeResponse", "SmsNotificationTypeResponse", "WebhookNotificationTypeResponse"]
+NOTIFICATIONTYPERESPONSE_ONE_OF_SCHEMAS = ["AmazonSqsNotificationTypeResponse", "AmazonSqsPrincipalAuthNotificationTypeResponse", "EmailNotificationTypeResponse", "SmsNotificationTypeResponse", "WebhookNotificationTypeResponse"]
 
 class NotificationTypeResponse(BaseModel):
     """
     Holds readonly information about a Finbourne.Notifications.WebApi.Dtos.Notifications.Notification
     """
     # data type: AmazonSqsNotificationTypeResponse
     oneof_schema_1_validator: Optional[AmazonSqsNotificationTypeResponse] = None
+    # data type: AmazonSqsPrincipalAuthNotificationTypeResponse
+    oneof_schema_2_validator: Optional[AmazonSqsPrincipalAuthNotificationTypeResponse] = None
     # data type: EmailNotificationTypeResponse
-    oneof_schema_2_validator: Optional[EmailNotificationTypeResponse] = None
+    oneof_schema_3_validator: Optional[EmailNotificationTypeResponse] = None
     # data type: SmsNotificationTypeResponse
-    oneof_schema_3_validator: Optional[SmsNotificationTypeResponse] = None
+    oneof_schema_4_validator: Optional[SmsNotificationTypeResponse] = None
     # data type: WebhookNotificationTypeResponse
-    oneof_schema_4_validator: Optional[WebhookNotificationTypeResponse] = None
+    oneof_schema_5_validator: Optional[WebhookNotificationTypeResponse] = None
     if TYPE_CHECKING:
-        actual_instance: Union[AmazonSqsNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse]
+        actual_instance: Union[AmazonSqsNotificationTypeResponse, AmazonSqsPrincipalAuthNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse]
     else:
         actual_instance: Any
     one_of_schemas: List[str] = Field(NOTIFICATIONTYPERESPONSE_ONE_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
@@ -66,14 +69,19 @@
         error_messages = []
         match = 0
         # validate data type: AmazonSqsNotificationTypeResponse
         if not isinstance(v, AmazonSqsNotificationTypeResponse):
             error_messages.append(f"Error! Input type `{type(v)}` is not `AmazonSqsNotificationTypeResponse`")
         else:
             match += 1
+        # validate data type: AmazonSqsPrincipalAuthNotificationTypeResponse
+        if not isinstance(v, AmazonSqsPrincipalAuthNotificationTypeResponse):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `AmazonSqsPrincipalAuthNotificationTypeResponse`")
+        else:
+            match += 1
         # validate data type: EmailNotificationTypeResponse
         if not isinstance(v, EmailNotificationTypeResponse):
             error_messages.append(f"Error! Input type `{type(v)}` is not `EmailNotificationTypeResponse`")
         else:
             match += 1
         # validate data type: SmsNotificationTypeResponse
         if not isinstance(v, SmsNotificationTypeResponse):
@@ -83,18 +91,18 @@
         # validate data type: WebhookNotificationTypeResponse
         if not isinstance(v, WebhookNotificationTypeResponse):
             error_messages.append(f"Error! Input type `{type(v)}` is not `WebhookNotificationTypeResponse`")
         else:
             match += 1
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, AmazonSqsPrincipalAuthNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, AmazonSqsPrincipalAuthNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> NotificationTypeResponse:
         return cls.from_json(json.dumps(obj))
 
@@ -107,14 +115,20 @@
 
         # deserialize data into AmazonSqsNotificationTypeResponse
         try:
             instance.actual_instance = AmazonSqsNotificationTypeResponse.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # deserialize data into AmazonSqsPrincipalAuthNotificationTypeResponse
+        try:
+            instance.actual_instance = AmazonSqsPrincipalAuthNotificationTypeResponse.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # deserialize data into EmailNotificationTypeResponse
         try:
             instance.actual_instance = EmailNotificationTypeResponse.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into SmsNotificationTypeResponse
@@ -128,18 +142,18 @@
             instance.actual_instance = WebhookNotificationTypeResponse.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, AmazonSqsPrincipalAuthNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into NotificationTypeResponse with oneOf schemas: AmazonSqsNotificationTypeResponse, AmazonSqsPrincipalAuthNotificationTypeResponse, EmailNotificationTypeResponse, SmsNotificationTypeResponse, WebhookNotificationTypeResponse. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_id.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_id.py`

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
 
 class ResourceId(BaseModel):
     """
     Identifiers of an entity  # noqa: E501
     """
     scope: constr(strict=True, max_length=512, min_length=1) = Field(..., description="The scope used to identify an entity")
     code: constr(strict=True, max_length=512, min_length=1) = Field(..., description="The code used to identify an entity")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

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
 from lusid_notifications.models.access_controlled_resource import AccessControlledResource
 from lusid_notifications.models.link import Link
 
 class ResourceListOfAccessControlledResource(BaseModel):
     """
     ResourceListOfAccessControlledResource
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_delivery.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_delivery.py`

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
 from lusid_notifications.models.delivery import Delivery
 from lusid_notifications.models.link import Link
 
 class ResourceListOfDelivery(BaseModel):
     """
     ResourceListOfDelivery
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_event_type_schema.py`

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
 from lusid_notifications.models.event_type_schema import EventTypeSchema
 from lusid_notifications.models.link import Link
 
 class ResourceListOfEventTypeSchema(BaseModel):
     """
     ResourceListOfEventTypeSchema
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_notification.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_notification.py`

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
 from lusid_notifications.models.link import Link
 from lusid_notifications.models.notification import Notification
 
 class ResourceListOfNotification(BaseModel):
     """
     ResourceListOfNotification
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_subscription.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_subscription.py`

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
 from lusid_notifications.models.link import Link
 from lusid_notifications.models.subscription import Subscription
 
 class ResourceListOfSubscription(BaseModel):
     """
     ResourceListOfSubscription
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 
 class SmsNotificationType(BaseModel):
     """
     The information required to create or update an SMS notification  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of delivery mechanism for this notification")
     body: constr(strict=True, max_length=1024, min_length=1) = Field(..., description="The body of the SMS")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type_response.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type_response.py`

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
 
 class SmsNotificationTypeResponse(BaseModel):
     """
     Holds readonly information about an SMS notification  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of delivery mechanism for this notification")
     body: Optional[StrictStr] = Field(None, description="The body of the SMS")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/subscription.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, constr
 from lusid_notifications.models.matching_pattern import MatchingPattern
 from lusid_notifications.models.resource_id import ResourceId
 
 class Subscription(BaseModel):
     """
     A subscription object  # noqa: E501
     """
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_notification_request.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_notification_request.py`

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
 from lusid_notifications.models.notification_type import NotificationType
 
 class UpdateNotificationRequest(BaseModel):
     """
     The information required to update a notification  # noqa: E501
     """
     display_name: constr(strict=True, max_length=64, min_length=0) = Field(..., alias="displayName", description="The name of the notification")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_subscription.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_subscription.py`

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
 from lusid_notifications.models.matching_pattern import MatchingPattern
 
 class UpdateSubscription(BaseModel):
     """
     The information required to update a subscription  # noqa: E501
     """
     display_name: constr(strict=True, max_length=64, min_length=1) = Field(..., alias="displayName", description="The name of the subscription")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
 
 class WebhookNotificationType(BaseModel):
     """
     The information required to create or update a Webhook notification  # noqa: E501
     """
     type: constr(strict=True, min_length=1) = Field(..., description="The type of delivery mechanism for this notification")
     http_method: constr(strict=True, min_length=1) = Field(..., alias="httpMethod", description="The HTTP method such as GET, POST, etc. to use on the request")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type_response.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type_response.py`

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
 
 class WebhookNotificationTypeResponse(BaseModel):
     """
     Holds readonly information about a Webhook notification  # noqa: E501
     """
     type: Optional[StrictStr] = Field(None, description="The type of delivery mechanism for this notification")
     http_method: Optional[StrictStr] = Field(None, alias="httpMethod", description="The HTTP method such as GET, POST, etc. to use on the request")
```

### Comparing `lusid_notifications_sdk-2.0.9/lusid_notifications/rest.py` & `lusid_notifications_sdk-2.1.1/lusid_notifications/rest.py`

 * *Files 2% similar despite different names*

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

### Comparing `lusid_notifications_sdk-2.0.9/pyproject.toml` & `lusid_notifications_sdk-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-notifications-sdk"
-version = "2.0.9"
+version = "2.1.1"
 description = "FINBOURNE Notifications API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/notifications-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Notifications API", "lusid-notifications-sdk"]
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

### Comparing `lusid_notifications_sdk-2.0.9/PKG-INFO` & `lusid_notifications_sdk-2.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,14 @@
-Metadata-Version: 2.1
-Name: lusid-notifications-sdk
-Version: 2.0.9
-Summary: FINBOURNE Notifications API
-Home-page: https://github.com/finbourne/notifications-sdk-python
-License: MIT
-Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Notifications API,lusid-notifications-sdk
-Author: FINBOURNE Technology
-Author-email: info@finbourne.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aenum (>=3.1.11,<4.0.0)
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2,<3)
-Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
-Project-URL: Repository, https://github.com/finbourne/notifications-sdk-python
-Description-Content-Type: text/markdown
-
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.906
-- Package version: 2.0.9
+- API version: 0.1.929
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -69,29 +43,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_notifications application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_NOTIFICATIONS_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_NOTIFICATIONS_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_notifications via a proxy, by setting `FBN_PROXY_ADDRESS`. 
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
+        "lusid_notificationsUrl":"<FINBOURNE-application-url>",
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
+        "lusid_notificationsUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_notifications via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_notificationsUrl":"<FINBOURNE-application-url>",
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
 import lusid_notifications
-from lusid_notifications.rest import ApiException
+from lusid_notifications.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_notifications import (
-	  ApiClientFactory,
-	  ApplicationMetadataApi,
-	  EnvironmentVariablesConfigurationLoader,
-	  SecretsFileConfigurationLoader,
-	  ArgsConfigurationLoader
+    ApiClientFactory,
+    ApplicationMetadataApi,
+    EnvironmentVariablesConfigurationLoader,
+    SecretsFileConfigurationLoader,
+    ArgsConfigurationLoader
 )
 
 # Use the lusid_notifications ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -116,15 +166,15 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_notifications.ApplicationMetadataApi(api_client)
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
         # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
@@ -158,14 +208,16 @@
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
  - [AmazonSqsNotificationTypeResponse](docs/AmazonSqsNotificationTypeResponse.md)
+ - [AmazonSqsPrincipalAuthNotificationType](docs/AmazonSqsPrincipalAuthNotificationType.md)
+ - [AmazonSqsPrincipalAuthNotificationTypeResponse](docs/AmazonSqsPrincipalAuthNotificationTypeResponse.md)
  - [Attempt](docs/Attempt.md)
  - [AttemptStatus](docs/AttemptStatus.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [Delivery](docs/Delivery.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
  - [EmailNotificationTypeResponse](docs/EmailNotificationTypeResponse.md)
@@ -215,8 +267,7 @@
 
 
 ## Author
 
 info@finbourne.com
 
 
-
```

