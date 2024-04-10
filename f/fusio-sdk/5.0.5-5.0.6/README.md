# Comparing `tmp/fusio-sdk-5.0.5.tar.gz` & `tmp/fusio-sdk-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusio-sdk-5.0.5.tar", last modified: Sun Apr  7 10:33:59 2024, max compression
+gzip compressed data, was "fusio-sdk-5.0.6.tar", last modified: Wed Apr 10 21:20:59 2024, max compression
```

## Comparing `fusio-sdk-5.0.5.tar` & `fusio-sdk-5.0.6.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:33:59.005769 fusio-sdk-5.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-07 10:33:59.005769 fusio-sdk-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:33:59.005769 fusio-sdk-5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:33:58.957769 fusio-sdk-5.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:33:59.005769 fusio-sdk-5.0.5/src/fusio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-07 10:33:58.000000 fusio-sdk-5.0.5/src/fusio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-07 10:33:58.000000 fusio-sdk-5.0.5/src/fusio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:33:58.000000 fusio-sdk-5.0.5/src/fusio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 10:33:58.000000 fusio-sdk-5.0.5/src/fusio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 10:33:58.000000 fusio-sdk-5.0.5/src/fusio_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:33:59.005769 fusio-sdk-5.0.5/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/authorization_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_account_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_execute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_execute_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_execute_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_execute_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_execute_response_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_action_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_audit_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_audit_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_audit_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_backup_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_backup_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_backup_import_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_backup_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_category_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_category_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_category_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_category_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_config_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_config_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_config_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_introspection_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_introspection_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_introspection_entity_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_connection_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_cronjob.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_cronjob_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_cronjob_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_cronjob_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_cronjob_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_cronjob_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_dashboard_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_event_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_event_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_generator_index_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_generator_index_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_generator_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_generator_provider_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_generator_provider_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_generator_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_identity_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_log_error_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_collection_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_local_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_remote_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_marketplace_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_throws.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_operation_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_page_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_page_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_rate_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_rate_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_rate_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_rate_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_rate_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_preview_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_category_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_scope_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_sdk_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_sdk_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_sdk_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_sdk_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_statistic_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_statistic_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_statistic_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_statistic_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_tenant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_trash_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_trash_data_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_trash_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_trash_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_trash_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_user_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/backend_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_element_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_element_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_element_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_form_element_text_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_message_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_authorize_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_authorize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_authorize_response_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_grant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_grant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_payment_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_payment_checkout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_payment_portal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_payment_portal_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_token_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_password_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_user_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/consumer_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/passthru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_about.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_about_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_about_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_o_auth_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_route.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_route_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_route_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_schema_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 10:33:55.000000 fusio-sdk-5.0.5/src/sdk/system_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 21:20:56.000000 fusio-sdk-5.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.732830 fusio-sdk-5.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/authorization_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_account_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entity_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_index_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_index_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_provider_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_error_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_collection_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_local_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_throws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_preview_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_category_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_tenant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_text_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_response_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_grant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_grant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_portal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_portal_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_password_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/passthru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_about_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_about_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_o_auth_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_route_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_route_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_schema_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_tag.py
```

### Comparing `fusio-sdk-5.0.5/LICENSE` & `fusio-sdk-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/PKG-INFO` & `fusio-sdk-5.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.5
+Version: 5.0.6
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sdkgen-client==0.1.0
+Requires-Dist: sdkgen-client>=0.2.1
 
 
 # Fusio Python SDK
 
 This is the official Fusio Java CSharp, it helps to talk to the Fusio REST API.
 Fusio is an open source API management system, more information at:
 https://www.fusio-project.org
```

### Comparing `fusio-sdk-5.0.5/README.md` & `fusio-sdk-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/pyproject.toml` & `fusio-sdk-5.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "fusio-sdk"
-version = "5.0.5"
+version = "5.0.6"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDK to talk to the Fusio REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Code Generators",
 ]
 dependencies = [
-    "sdkgen-client == 0.1.0",
+    "sdkgen-client >= 0.2.1",
 ]
 
 [project.urls]
 Homepage = "https://github.com/apioo/fusio-sdk-python"
 Issues = "https://github.com/apioo/fusio-sdk-sdkgen-python/issues"
 
 [build-system]
```

### Comparing `fusio-sdk-5.0.5/src/fusio_sdk.egg-info/PKG-INFO` & `fusio-sdk-5.0.6/src/fusio_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.5
+Version: 5.0.6
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sdkgen-client==0.1.0
+Requires-Dist: sdkgen-client>=0.2.1
 
 
 # Fusio Python SDK
 
 This is the official Fusio Java CSharp, it helps to talk to the Fusio REST API.
 Fusio is an open source API management system, more information at:
 https://www.fusio-project.org
```

### Comparing `fusio-sdk-5.0.5/src/fusio_sdk.egg-info/SOURCES.txt` & `fusio-sdk-5.0.6/src/fusio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/authorization_tag.py` & `fusio-sdk-5.0.6/src/sdk/authorization_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_account_change_password.py` & `fusio-sdk-5.0.6/src/sdk/backend_account_change_password.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_account_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_account_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_action.py` & `fusio-sdk-5.0.6/src/sdk/backend_action.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_action_execute_request.py` & `fusio-sdk-5.0.6/src/sdk/backend_action_execute_request.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_action_execute_response.py` & `fusio-sdk-5.0.6/src/sdk/backend_action_execute_response.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_action_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_action_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_app.py` & `fusio-sdk-5.0.6/src/sdk/backend_app.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_app_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_app_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_audit.py` & `fusio-sdk-5.0.6/src/sdk/backend_audit.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_audit_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_audit_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_backup_import_result.py` & `fusio-sdk-5.0.6/src/sdk/backend_backup_import_result.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_backup_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_backup_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_category_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_category_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_config.py` & `fusio-sdk-5.0.6/src/sdk/backend_config.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_config_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_config_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_connection.py` & `fusio-sdk-5.0.6/src/sdk/backend_connection.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_connection_introspection_entity.py` & `fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entity.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_connection_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_connection_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_cronjob.py` & `fusio-sdk-5.0.6/src/sdk/backend_cronjob.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_cronjob_error.py` & `fusio-sdk-5.0.6/src/sdk/backend_cronjob_error.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_cronjob_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_cronjob_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_dashboard.py` & `fusio-sdk-5.0.6/src/sdk/backend_dashboard.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_dashboard_request.py` & `fusio-sdk-5.0.6/src/sdk/backend_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_dashboard_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_dashboard_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_dashboard_transaction.py` & `fusio-sdk-5.0.6/src/sdk/backend_dashboard_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_dashboard_user.py` & `fusio-sdk-5.0.6/src/sdk/backend_dashboard_user.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_event.py` & `fusio-sdk-5.0.6/src/sdk/backend_event.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_event_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_event_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_generator_provider.py` & `fusio-sdk-5.0.6/src/sdk/backend_generator_provider.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_generator_provider_changelog.py` & `fusio-sdk-5.0.6/src/sdk/backend_generator_provider_changelog.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_generator_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_generator_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,16 @@
             headers["Content-Type"] = "application/json"
 
             response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
 
             if response.status_code >= 200 and response.status_code < 300:
                 return BackendGeneratorProviderChangelog.from_json(response.content)
 
+            if response.status_code == 400:
+                raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
@@ -67,14 +69,16 @@
             headers["Content-Type"] = "application/json"
 
             response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
 
             if response.status_code >= 200 and response.status_code < 300:
                 return CommonMessage.from_json(response.content)
 
+            if response.status_code == 400:
+                raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
@@ -96,14 +100,16 @@
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return CommonFormContainer.from_json(response.content)
 
+            if response.status_code == 400:
+                raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
```

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_identity.py` & `fusio-sdk-5.0.6/src/sdk/backend_identity.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_identity_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_identity_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_log.py` & `fusio-sdk-5.0.6/src/sdk/backend_log.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_log_error.py` & `fusio-sdk-5.0.6/src/sdk/backend_log_error.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_log_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_log_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_marketplace_app.py` & `fusio-sdk-5.0.6/src/sdk/backend_marketplace_app.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_marketplace_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_marketplace_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_operation.py` & `fusio-sdk-5.0.6/src/sdk/backend_operation.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_operation_schema.py` & `fusio-sdk-5.0.6/src/sdk/backend_operation_schema.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_operation_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_operation_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_page.py` & `fusio-sdk-5.0.6/src/sdk/backend_page.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_page_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_page_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_plan.py` & `fusio-sdk-5.0.6/src/sdk/backend_plan.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_plan_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_plan_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_rate.py` & `fusio-sdk-5.0.6/src/sdk/backend_rate.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_rate_allocation.py` & `fusio-sdk-5.0.6/src/sdk/backend_rate_allocation.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_rate_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_rate_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_role.py` & `fusio-sdk-5.0.6/src/sdk/backend_role.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_role_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_schema.py` & `fusio-sdk-5.0.6/src/sdk/backend_schema.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_schema_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_schema_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_scope.py` & `fusio-sdk-5.0.6/src/sdk/backend_scope.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_scope_category.py` & `fusio-sdk-5.0.6/src/sdk/backend_scope_category.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_scope_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_scope_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_sdk_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_sdk_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_statistic_chart.py` & `fusio-sdk-5.0.6/src/sdk/backend_statistic_chart.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_statistic_count.py` & `fusio-sdk-5.0.6/src/sdk/backend_statistic_count.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_statistic_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_statistic_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_tenant_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_tenant_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_token.py` & `fusio-sdk-5.0.6/src/sdk/backend_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_token_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_token_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_transaction.py` & `fusio-sdk-5.0.6/src/sdk/backend_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_transaction_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_transaction_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_trash_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_trash_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_user.py` & `fusio-sdk-5.0.6/src/sdk/backend_user.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_user_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_user_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_webhook.py` & `fusio-sdk-5.0.6/src/sdk/backend_webhook.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_webhook_response.py` & `fusio-sdk-5.0.6/src/sdk/backend_webhook_response.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/backend_webhook_tag.py` & `fusio-sdk-5.0.6/src/sdk/backend_webhook_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/client.py` & `fusio-sdk-5.0.6/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/common_collection.py` & `fusio-sdk-5.0.6/src/sdk/common_collection.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/common_form_container.py` & `fusio-sdk-5.0.6/src/sdk/common_form_container.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/common_form_element.py` & `fusio-sdk-5.0.6/src/sdk/common_form_element.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/common_form_element_select.py` & `fusio-sdk-5.0.6/src/sdk/common_form_element_select.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_account_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_account_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_app.py` & `fusio-sdk-5.0.6/src/sdk/consumer_app.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_app_create.py` & `fusio-sdk-5.0.6/src/sdk/consumer_app_create.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_app_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_app_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_app_update.py` & `fusio-sdk-5.0.6/src/sdk/consumer_app_update.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_authorize_meta.py` & `fusio-sdk-5.0.6/src/sdk/consumer_authorize_meta.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_authorize_request.py` & `fusio-sdk-5.0.6/src/sdk/consumer_authorize_request.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_authorize_response.py` & `fusio-sdk-5.0.6/src/sdk/consumer_authorize_response.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_authorize_response_token.py` & `fusio-sdk-5.0.6/src/sdk/consumer_authorize_response_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_event.py` & `fusio-sdk-5.0.6/src/sdk/consumer_event.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_event_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_event_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_grant.py` & `fusio-sdk-5.0.6/src/sdk/consumer_grant.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_grant_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_grant_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_identity.py` & `fusio-sdk-5.0.6/src/sdk/consumer_identity.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_identity_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_identity_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_log.py` & `fusio-sdk-5.0.6/src/sdk/consumer_log.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_log_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_log_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_page.py` & `fusio-sdk-5.0.6/src/sdk/consumer_page.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_page_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_page_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_payment_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_payment_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_plan.py` & `fusio-sdk-5.0.6/src/sdk/consumer_plan.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_plan_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_plan_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_scope.py` & `fusio-sdk-5.0.6/src/sdk/consumer_scope.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_scope_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_scope_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_token.py` & `fusio-sdk-5.0.6/src/sdk/consumer_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_token_access_token.py` & `fusio-sdk-5.0.6/src/sdk/consumer_token_access_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_token_create.py` & `fusio-sdk-5.0.6/src/sdk/consumer_token_create.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_token_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_token_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_transaction.py` & `fusio-sdk-5.0.6/src/sdk/consumer_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_transaction_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_transaction_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_user_account.py` & `fusio-sdk-5.0.6/src/sdk/consumer_user_account.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_user_jwt.py` & `fusio-sdk-5.0.6/src/sdk/consumer_user_jwt.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_user_login.py` & `fusio-sdk-5.0.6/src/sdk/consumer_user_login.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_user_plan.py` & `fusio-sdk-5.0.6/src/sdk/consumer_user_plan.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_user_register.py` & `fusio-sdk-5.0.6/src/sdk/consumer_user_register.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_webhook.py` & `fusio-sdk-5.0.6/src/sdk/consumer_webhook.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_webhook_response.py` & `fusio-sdk-5.0.6/src/sdk/consumer_webhook_response.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/consumer_webhook_tag.py` & `fusio-sdk-5.0.6/src/sdk/consumer_webhook_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_about.py` & `fusio-sdk-5.0.6/src/sdk/system_about.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_connection_tag.py` & `fusio-sdk-5.0.6/src/sdk/system_connection_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_meta_tag.py` & `fusio-sdk-5.0.6/src/sdk/system_meta_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_o_auth_configuration.py` & `fusio-sdk-5.0.6/src/sdk/system_o_auth_configuration.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_payment_tag.py` & `fusio-sdk-5.0.6/src/sdk/system_payment_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_schema.py` & `fusio-sdk-5.0.6/src/sdk/system_schema.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.5/src/sdk/system_tag.py` & `fusio-sdk-5.0.6/src/sdk/system_tag.py`

 * *Files identical despite different names*

