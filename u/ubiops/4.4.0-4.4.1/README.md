# Comparing `tmp/ubiops-4.4.0.tar.gz` & `tmp/ubiops-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiops-4.4.0.tar", last modified: Tue Apr  9 07:52:46 2024, max compression
+gzip compressed data, was "ubiops-4.4.1.tar", last modified: Wed Apr 10 12:43:21 2024, max compression
```

## Comparing `ubiops-4.4.0.tar` & `ubiops-4.4.1.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 07:52:36.000000 ubiops-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 07:52:46.221026 ubiops-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48602 2024-04-09 07:52:36.000000 ubiops-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 07:52:46.221026 ubiops-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 07:52:36.000000 ubiops-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.189026 ubiops-4.4.0/ubiops/
--rw-r--r--   0 runner    (1001) docker     (127)    11925 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.197026 ubiops-4.4.0/ubiops/api/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/blobs.py
--rw-r--r--   0 runner    (1001) docker     (127)   286653 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    90527 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/deployment_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)   139344 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    68268 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    53403 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    43724 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/imports_and_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    45097 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    85253 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/pipeline_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    56252 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/request_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)    38898 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    24173 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/service_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    28746 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23968 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.217026 ubiops-4.4.0/ubiops/models/
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachment_fields_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachment_sources_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachments_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachments_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/audit_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/blob_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/build_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_input_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_output_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_batch_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_batch_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_single_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    33911 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    30739 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    21760 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/direct_pipeline_request_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/direct_pipeline_request_operator_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/direct_pipeline_request_pipeline_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_build_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_build_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_build_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    20218 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_revision_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_revision_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_variable_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_variable_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_variable_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/export_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/export_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/export_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/expression_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/expression_evaluate_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/expression_input_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_complete_multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/import_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/import_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/import_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/inherited_environment_variable_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_field_widget_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_field_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_field_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_field_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_widget_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/logs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/metric_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/metric_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/metric_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    14399 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/operator_request_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_project_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/output_field_widget_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/output_value_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/permission_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_input_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_output_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_batch_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18204 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_operator_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_pipeline_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    20488 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_single_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    17386 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_object_configuration_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_object_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_object_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_deployment_version_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_resource_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_user_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/quota_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/requests_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/resource_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/revision_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/revision_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_assignment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_detail_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/schedule_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/schedule_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_token_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_token_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/template_deployment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_point_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_point_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/user_pending_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/user_pending_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/voucher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_test_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/training/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    39257 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/metrics/metric_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/metrics/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/run_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/utils/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validators/validate_requirements_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validators/validate_yaml_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    33908 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/wait_for.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.193026 ubiops-4.4.0/ubiops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-09 07:52:46.000000 ubiops-4.4.0/ubiops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.532792 ubiops-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 12:43:05.000000 ubiops-4.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-10 12:43:21.532792 ubiops-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48602 2024-04-10 12:43:05.000000 ubiops-4.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 12:43:21.532792 ubiops-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-10 12:43:05.000000 ubiops-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.500792 ubiops-4.4.1/ubiops/
+-rw-r--r--   0 runner    (1001) docker     (127)    11925 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.508792 ubiops-4.4.1/ubiops/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/blobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286653 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90527 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/deployment_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139344 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68268 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53403 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43724 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/imports_and_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45097 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85253 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/pipeline_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56252 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/request_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38898 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24173 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/service_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28746 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23968 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.528792 ubiops-4.4.1/ubiops/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/attachment_fields_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/attachment_sources_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/attachments_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/attachments_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/audit_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/blob_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/bucket_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/bucket_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/bucket_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/bucket_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/build_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_input_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_output_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_batch_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_batch_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_single_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_request_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_version_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33911 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_version_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30739 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_version_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21760 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/deployment_version_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/direct_pipeline_request_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/direct_pipeline_request_operator_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/direct_pipeline_request_pipeline_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_build_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_build_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_build_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20218 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_revision_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_revision_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_variable_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_variable_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/environment_variable_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/export_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/export_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/export_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/expression_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/expression_evaluate_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/expression_input_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/file_complete_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/file_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/file_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/file_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/file_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/import_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/import_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/import_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/inherited_environment_variable_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/input_field_widget_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/input_output_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/input_output_field_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/input_output_field_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/input_output_widget_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/logs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/metric_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/metric_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/metric_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/notification_group_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/notification_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/notification_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/notification_group_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14399 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/operator_request_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/organization_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/output_field_widget_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/output_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/permission_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_input_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_output_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_batch_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18204 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_operator_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_pipeline_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20488 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_request_single_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17386 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_object_configuration_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_object_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_object_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/pipeline_version_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_deployment_version_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_resource_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/project_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/quota_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/requests_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/resource_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/revision_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/revision_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/role_assignment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/role_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/role_detail_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/role_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/schedule_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/schedule_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/service_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/service_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/service_user_token_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/service_user_token_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/template_deployment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/time_series_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/time_series_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/time_series_data_point_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/time_series_data_point_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/time_series_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/user_pending_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/user_pending_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/voucher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/webhook_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/webhook_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/webhook_test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/webhook_test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/models/webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.528792 ubiops-4.4.1/ubiops/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_run_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_run_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_run_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_run_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_run_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/experiment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39257 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/training/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.532792 ubiops-4.4.1/ubiops/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.532792 ubiops-4.4.1/ubiops/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/metrics/metric_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/metrics/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/run_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.532792 ubiops-4.4.1/ubiops/utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/validators/validate_requirements_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/validators/validate_yaml_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33908 2024-04-10 12:43:05.000000 ubiops-4.4.1/ubiops/utils/wait_for.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:43:21.500792 ubiops-4.4.1/ubiops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-10 12:43:20.000000 ubiops-4.4.1/ubiops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-10 12:43:21.000000 ubiops-4.4.1/ubiops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:43:20.000000 ubiops-4.4.1/ubiops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 12:43:20.000000 ubiops-4.4.1/ubiops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 12:43:20.000000 ubiops-4.4.1/ubiops.egg-info/top_level.txt
```

### Comparing `ubiops-4.4.0/LICENSE` & `ubiops-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/PKG-INFO` & `ubiops-4.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiops
-Version: 4.4.0
+Version: 4.4.1
 Summary: UbiOps
 Home-page: https://github.com/UbiOps/client-library-python.git
 Author: UbiOps
 License: Apache 2.0
 Description: # ubiops
         Client Library to interact with the [UbiOps](https://ubiops.com) API (v2.1).
```

### Comparing `ubiops-4.4.0/README.md` & `ubiops-4.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [www.ubiops.com](https://ubiops.com)
 
 Client Library to interact with the UbiOps API.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v2.1
-- Package version: 4.4.0
+- Package version: 4.4.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://ubiops.com/docs](https://ubiops.com/docs)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `ubiops-4.4.0/setup.py` & `ubiops-4.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ubiops"
-VERSION = "4.4.0"
+VERSION = "4.4.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ubiops-4.4.0/ubiops/__init__.py` & `ubiops-4.4.1/ubiops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v2.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 
 # import CoreApi
 from ubiops.api.core_api import CoreApi
 
 # import Training
 from ubiops.training.training import Training
 from ubiops.training.experiment_create import ExperimentCreate
```

### Comparing `ubiops-4.4.0/ubiops/api/blobs.py` & `ubiops-4.4.1/ubiops/api/blobs.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/core_api.py` & `ubiops-4.4.1/ubiops/api/core_api.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/deployment_requests.py` & `ubiops-4.4.1/ubiops/api/deployment_requests.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/deployments.py` & `ubiops-4.4.1/ubiops/api/deployments.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/environments.py` & `ubiops-4.4.1/ubiops/api/environments.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/files.py` & `ubiops-4.4.1/ubiops/api/files.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/imports_and_exports.py` & `ubiops-4.4.1/ubiops/api/imports_and_exports.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/metrics.py` & `ubiops-4.4.1/ubiops/api/metrics.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/monitoring.py` & `ubiops-4.4.1/ubiops/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/organizations.py` & `ubiops-4.4.1/ubiops/api/organizations.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/pipeline_requests.py` & `ubiops-4.4.1/ubiops/api/pipeline_requests.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/pipelines.py` & `ubiops-4.4.1/ubiops/api/pipelines.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/projects.py` & `ubiops-4.4.1/ubiops/api/projects.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/request_schedules.py` & `ubiops-4.4.1/ubiops/api/request_schedules.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/roles.py` & `ubiops-4.4.1/ubiops/api/roles.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/service_users.py` & `ubiops-4.4.1/ubiops/api/service_users.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/status.py` & `ubiops-4.4.1/ubiops/api/status.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/user.py` & `ubiops-4.4.1/ubiops/api/user.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api/webhooks.py` & `ubiops-4.4.1/ubiops/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/api_client.py` & `ubiops-4.4.1/ubiops/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
 
         self.cookie = cookie
-        self.user_agent = "UbiOps/python/4.4.0"
+        self.user_agent = "UbiOps/python/4.4.1"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ubiops-4.4.0/ubiops/configuration.py` & `ubiops-4.4.1/ubiops/configuration.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/exceptions.py` & `ubiops-4.4.1/ubiops/exceptions.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/__init__.py` & `ubiops-4.4.1/ubiops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/attachment_fields_list.py` & `ubiops-4.4.1/ubiops/models/attachment_fields_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/attachment_sources_list.py` & `ubiops-4.4.1/ubiops/models/attachment_sources_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/attachments_create.py` & `ubiops-4.4.1/ubiops/models/attachments_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/attachments_list.py` & `ubiops-4.4.1/ubiops/models/attachments_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/audit_list.py` & `ubiops-4.4.1/ubiops/models/audit_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/blob_list.py` & `ubiops-4.4.1/ubiops/models/blob_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/bucket_create.py` & `ubiops-4.4.1/ubiops/models/bucket_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/bucket_detail.py` & `ubiops-4.4.1/ubiops/models/bucket_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/bucket_list.py` & `ubiops-4.4.1/ubiops/models/bucket_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/bucket_update.py` & `ubiops-4.4.1/ubiops/models/bucket_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/build_list.py` & `ubiops-4.4.1/ubiops/models/build_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_create.py` & `ubiops-4.4.1/ubiops/models/deployment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_create_response.py` & `ubiops-4.4.1/ubiops/models/deployment_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_detail.py` & `ubiops-4.4.1/ubiops/models/deployment_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_input_field_create.py` & `ubiops-4.4.1/ubiops/models/deployment_input_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_instance_type.py` & `ubiops-4.4.1/ubiops/models/deployment_instance_type.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_list.py` & `ubiops-4.4.1/ubiops/models/deployment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_output_field_create.py` & `ubiops-4.4.1/ubiops/models/deployment_output_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_batch_create_response.py` & `ubiops-4.4.1/ubiops/models/deployment_request_batch_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_batch_detail.py` & `ubiops-4.4.1/ubiops/models/deployment_request_batch_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_create_response.py` & `ubiops-4.4.1/ubiops/models/deployment_request_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_list.py` & `ubiops-4.4.1/ubiops/models/deployment_request_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_single_detail.py` & `ubiops-4.4.1/ubiops/models/deployment_request_single_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_update.py` & `ubiops-4.4.1/ubiops/models/deployment_request_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_request_update_response.py` & `ubiops-4.4.1/ubiops/models/deployment_request_update_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_update.py` & `ubiops-4.4.1/ubiops/models/deployment_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_version_create.py` & `ubiops-4.4.1/ubiops/models/deployment_version_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_version_detail.py` & `ubiops-4.4.1/ubiops/models/deployment_version_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_version_list.py` & `ubiops-4.4.1/ubiops/models/deployment_version_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_version_port.py` & `ubiops-4.4.1/ubiops/models/deployment_version_port.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/deployment_version_update.py` & `ubiops-4.4.1/ubiops/models/deployment_version_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/direct_pipeline_request_deployment_request.py` & `ubiops-4.4.1/ubiops/models/direct_pipeline_request_deployment_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/direct_pipeline_request_operator_request.py` & `ubiops-4.4.1/ubiops/models/direct_pipeline_request_operator_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/direct_pipeline_request_pipeline_request.py` & `ubiops-4.4.1/ubiops/models/direct_pipeline_request_pipeline_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_build_dependency.py` & `ubiops-4.4.1/ubiops/models/environment_build_dependency.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_build_list.py` & `ubiops-4.4.1/ubiops/models/environment_build_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_build_update.py` & `ubiops-4.4.1/ubiops/models/environment_build_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_create.py` & `ubiops-4.4.1/ubiops/models/environment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_detail.py` & `ubiops-4.4.1/ubiops/models/environment_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_list.py` & `ubiops-4.4.1/ubiops/models/environment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_revision_create.py` & `ubiops-4.4.1/ubiops/models/environment_revision_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_revision_detail.py` & `ubiops-4.4.1/ubiops/models/environment_revision_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_update.py` & `ubiops-4.4.1/ubiops/models/environment_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_usage.py` & `ubiops-4.4.1/ubiops/models/environment_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_variable_copy.py` & `ubiops-4.4.1/ubiops/models/environment_variable_copy.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_variable_create.py` & `ubiops-4.4.1/ubiops/models/environment_variable_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/environment_variable_list.py` & `ubiops-4.4.1/ubiops/models/environment_variable_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/export_create.py` & `ubiops-4.4.1/ubiops/models/export_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/export_detail.py` & `ubiops-4.4.1/ubiops/models/export_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/export_list.py` & `ubiops-4.4.1/ubiops/models/export_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/expression_evaluate.py` & `ubiops-4.4.1/ubiops/models/expression_evaluate.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/expression_evaluate_response.py` & `ubiops-4.4.1/ubiops/models/expression_evaluate_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/expression_input_field_create.py` & `ubiops-4.4.1/ubiops/models/expression_input_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/file_complete_multipart_upload.py` & `ubiops-4.4.1/ubiops/models/file_complete_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/file_detail.py` & `ubiops-4.4.1/ubiops/models/file_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/file_item.py` & `ubiops-4.4.1/ubiops/models/file_item.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/file_multipart_upload.py` & `ubiops-4.4.1/ubiops/models/file_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/file_upload_response.py` & `ubiops-4.4.1/ubiops/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/import_detail.py` & `ubiops-4.4.1/ubiops/models/import_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/import_list.py` & `ubiops-4.4.1/ubiops/models/import_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/import_update.py` & `ubiops-4.4.1/ubiops/models/import_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/inherited_environment_variable_list.py` & `ubiops-4.4.1/ubiops/models/inherited_environment_variable_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/input_field_widget_create.py` & `ubiops-4.4.1/ubiops/models/input_field_widget_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/input_output_field_base.py` & `ubiops-4.4.1/ubiops/models/input_output_field_base.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/input_output_field_detail.py` & `ubiops-4.4.1/ubiops/models/input_output_field_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/input_output_field_list.py` & `ubiops-4.4.1/ubiops/models/input_output_field_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/input_output_widget_list.py` & `ubiops-4.4.1/ubiops/models/input_output_widget_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/logs.py` & `ubiops-4.4.1/ubiops/models/logs.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/logs_create.py` & `ubiops-4.4.1/ubiops/models/logs_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/metric_create.py` & `ubiops-4.4.1/ubiops/models/metric_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/metric_detail.py` & `ubiops-4.4.1/ubiops/models/metric_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/metric_update.py` & `ubiops-4.4.1/ubiops/models/metric_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/notification_group_contact.py` & `ubiops-4.4.1/ubiops/models/notification_group_contact.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/notification_group_create.py` & `ubiops-4.4.1/ubiops/models/notification_group_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/notification_group_list.py` & `ubiops-4.4.1/ubiops/models/notification_group_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/notification_group_update.py` & `ubiops-4.4.1/ubiops/models/notification_group_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/operator_request_detail.py` & `ubiops-4.4.1/ubiops/models/operator_request_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_create.py` & `ubiops-4.4.1/ubiops/models/organization_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_detail.py` & `ubiops-4.4.1/ubiops/models/organization_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_list.py` & `ubiops-4.4.1/ubiops/models/organization_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_project_usage.py` & `ubiops-4.4.1/ubiops/models/organization_project_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_update.py` & `ubiops-4.4.1/ubiops/models/organization_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_usage.py` & `ubiops-4.4.1/ubiops/models/organization_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_user_create.py` & `ubiops-4.4.1/ubiops/models/organization_user_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_user_detail.py` & `ubiops-4.4.1/ubiops/models/organization_user_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/organization_user_update.py` & `ubiops-4.4.1/ubiops/models/organization_user_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/output_field_widget_create.py` & `ubiops-4.4.1/ubiops/models/output_field_widget_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/output_value_list.py` & `ubiops-4.4.1/ubiops/models/output_value_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/permission_list.py` & `ubiops-4.4.1/ubiops/models/permission_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_create.py` & `ubiops-4.4.1/ubiops/models/pipeline_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_create_response.py` & `ubiops-4.4.1/ubiops/models/pipeline_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_detail.py` & `ubiops-4.4.1/ubiops/models/pipeline_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_input_field_create.py` & `ubiops-4.4.1/ubiops/models/pipeline_input_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_list.py` & `ubiops-4.4.1/ubiops/models/pipeline_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_output_field_create.py` & `ubiops-4.4.1/ubiops/models/pipeline_output_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_batch_create_response.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_batch_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_create_response.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_deployment_request.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_deployment_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_detail.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_list.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_operator_request.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_operator_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_pipeline_request.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_pipeline_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_request_single_detail.py` & `ubiops-4.4.1/ubiops/models/pipeline_request_single_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_update.py` & `ubiops-4.4.1/ubiops/models/pipeline_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_create.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_detail.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_list.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_object_configuration_list.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_object_configuration_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_object_create.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_object_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_object_list.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_object_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/pipeline_version_update.py` & `ubiops-4.4.1/ubiops/models/pipeline_version_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_create.py` & `ubiops-4.4.1/ubiops/models/project_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_deployment_version_usage.py` & `ubiops-4.4.1/ubiops/models/project_deployment_version_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_detail.py` & `ubiops-4.4.1/ubiops/models/project_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_list.py` & `ubiops-4.4.1/ubiops/models/project_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_resource_usage.py` & `ubiops-4.4.1/ubiops/models/project_resource_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_update.py` & `ubiops-4.4.1/ubiops/models/project_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_usage.py` & `ubiops-4.4.1/ubiops/models/project_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_user_create.py` & `ubiops-4.4.1/ubiops/models/project_user_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/project_user_list.py` & `ubiops-4.4.1/ubiops/models/project_user_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/quota_detail.py` & `ubiops-4.4.1/ubiops/models/quota_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/requests_overview.py` & `ubiops-4.4.1/ubiops/models/requests_overview.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/resource_usage.py` & `ubiops-4.4.1/ubiops/models/resource_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/revision_create.py` & `ubiops-4.4.1/ubiops/models/revision_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/revision_list.py` & `ubiops-4.4.1/ubiops/models/revision_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/role_assignment_create.py` & `ubiops-4.4.1/ubiops/models/role_assignment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/role_assignment_list.py` & `ubiops-4.4.1/ubiops/models/role_assignment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/role_create.py` & `ubiops-4.4.1/ubiops/models/role_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/role_detail_list.py` & `ubiops-4.4.1/ubiops/models/role_detail_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/role_list.py` & `ubiops-4.4.1/ubiops/models/role_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/role_update.py` & `ubiops-4.4.1/ubiops/models/role_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/schedule_create.py` & `ubiops-4.4.1/ubiops/models/schedule_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/schedule_list.py` & `ubiops-4.4.1/ubiops/models/schedule_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/schedule_update.py` & `ubiops-4.4.1/ubiops/models/schedule_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/service_user_create.py` & `ubiops-4.4.1/ubiops/models/service_user_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/service_user_list.py` & `ubiops-4.4.1/ubiops/models/service_user_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/service_user_token_detail.py` & `ubiops-4.4.1/ubiops/models/service_user_token_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/service_user_token_list.py` & `ubiops-4.4.1/ubiops/models/service_user_token_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/status.py` & `ubiops-4.4.1/ubiops/models/status.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/template_deployment_list.py` & `ubiops-4.4.1/ubiops/models/template_deployment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/time_series_data_create.py` & `ubiops-4.4.1/ubiops/models/time_series_data_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/time_series_data_list.py` & `ubiops-4.4.1/ubiops/models/time_series_data_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/time_series_data_point_create.py` & `ubiops-4.4.1/ubiops/models/time_series_data_point_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/time_series_data_point_list.py` & `ubiops-4.4.1/ubiops/models/time_series_data_point_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/time_series_search.py` & `ubiops-4.4.1/ubiops/models/time_series_search.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/user_pending_create.py` & `ubiops-4.4.1/ubiops/models/user_pending_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/user_pending_detail.py` & `ubiops-4.4.1/ubiops/models/user_pending_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/voucher.py` & `ubiops-4.4.1/ubiops/models/voucher.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/webhook_create.py` & `ubiops-4.4.1/ubiops/models/webhook_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/webhook_detail.py` & `ubiops-4.4.1/ubiops/models/webhook_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/webhook_header.py` & `ubiops-4.4.1/ubiops/models/webhook_header.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/webhook_test_create.py` & `ubiops-4.4.1/ubiops/models/webhook_test_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/webhook_test_detail.py` & `ubiops-4.4.1/ubiops/models/webhook_test_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/models/webhook_update.py` & `ubiops-4.4.1/ubiops/models/webhook_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/rest.py` & `ubiops-4.4.1/ubiops/rest.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/__init__.py` & `ubiops-4.4.1/ubiops/training/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_create.py` & `ubiops-4.4.1/ubiops/training/experiment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_detail.py` & `ubiops-4.4.1/ubiops/training/experiment_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_list.py` & `ubiops-4.4.1/ubiops/training/experiment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_run_create.py` & `ubiops-4.4.1/ubiops/training/experiment_run_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_run_create_response.py` & `ubiops-4.4.1/ubiops/training/experiment_run_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_run_detail.py` & `ubiops-4.4.1/ubiops/training/experiment_run_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_run_list.py` & `ubiops-4.4.1/ubiops/training/experiment_run_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_run_update_response.py` & `ubiops-4.4.1/ubiops/training/experiment_run_update_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/experiment_update.py` & `ubiops-4.4.1/ubiops/training/experiment_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/training/training.py` & `ubiops-4.4.1/ubiops/training/training.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/__init__.py` & `ubiops-4.4.1/ubiops/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/file_operations.py` & `ubiops-4.4.1/ubiops/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/metrics/metric_client.py` & `ubiops-4.4.1/ubiops/utils/metrics/metric_client.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/metrics/metric_utils.py` & `ubiops-4.4.1/ubiops/utils/metrics/metric_utils.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/run_local.py` & `ubiops-4.4.1/ubiops/utils/run_local.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/validate.py` & `ubiops-4.4.1/ubiops/utils/validate.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/validators/validate_requirements_file.py` & `ubiops-4.4.1/ubiops/utils/validators/validate_requirements_file.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/validators/validate_yaml_file.py` & `ubiops-4.4.1/ubiops/utils/validators/validate_yaml_file.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops/utils/wait_for.py` & `ubiops-4.4.1/ubiops/utils/wait_for.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.4.0/ubiops.egg-info/PKG-INFO` & `ubiops-4.4.1/ubiops.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiops
-Version: 4.4.0
+Version: 4.4.1
 Summary: UbiOps
 Home-page: https://github.com/UbiOps/client-library-python.git
 Author: UbiOps
 License: Apache 2.0
 Description: # ubiops
         Client Library to interact with the [UbiOps](https://ubiops.com) API (v2.1).
```

### Comparing `ubiops-4.4.0/ubiops.egg-info/SOURCES.txt` & `ubiops-4.4.1/ubiops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

