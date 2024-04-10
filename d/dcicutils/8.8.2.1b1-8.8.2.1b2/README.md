# Comparing `tmp/dcicutils-8.8.2.1b1.tar.gz` & `tmp/dcicutils-8.8.2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.2.1b1.tar", max compression
+gzip compressed data, was "dcicutils-8.8.2.1b2.tar", max compression
```

## Comparing `dcicutils-8.8.2.1b1.tar` & `dcicutils-8.8.2.1b2.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/README.rst
--rw-r--r--   0        0        0        0 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     2522 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    68891 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-07 14:58:08.046705 dcicutils-8.8.2.1b1/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/log_utils.py
--rw-r--r--   0        0        0   102210 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30260 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    31250 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-07 14:58:08.050705 dcicutils-8.8.2.1b1/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    58458 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-04-07 14:58:08.054705 dcicutils-8.8.2.1b1/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.2.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     2522 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    68891 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-09 18:57:31.438430 dcicutils-8.8.2.1b2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   102210 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30260 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    13384 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-09 18:57:31.442431 dcicutils-8.8.2.1b2/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58458 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-04-09 18:57:31.446431 dcicutils-8.8.2.1b2/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.2.1b2/PKG-INFO
```

### Comparing `dcicutils-8.8.2.1b1/LICENSE.txt` & `dcicutils-8.8.2.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/README.rst` & `dcicutils-8.8.2.1b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/base.py` & `dcicutils-8.8.2.1b2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/bundle_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/captured_output.py` & `dcicutils-8.8.2.1b2/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/codebuild_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/command_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/common.py` & `dcicutils-8.8.2.1b2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/contribution_scripts.py` & `dcicutils-8.8.2.1b2/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/contribution_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/creds_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/data_readers.py` & `dcicutils-8.8.2.1b2/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/data_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/datetime_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/deployment_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/diff_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/docker_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/ecr_scripts.py` & `dcicutils-8.8.2.1b2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/ecr_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/ecs_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/env_base.py` & `dcicutils-8.8.2.1b2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/env_manager.py` & `dcicutils-8.8.2.1b2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/env_scripts.py` & `dcicutils-8.8.2.1b2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/env_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.2.1b2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/es_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/exceptions.py` & `dcicutils-8.8.2.1b2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/ff_mocks.py` & `dcicutils-8.8.2.1b2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/ff_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/file_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.2.1b2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/glacier_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/jh_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.2.1b2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/kibana/readme.md` & `dcicutils-8.8.2.1b2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/lang_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.2.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/license_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/log_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/misc_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/opensearch_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/portal_object_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/portal_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/project_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/qa_checkers.py` & `dcicutils-8.8.2.1b2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/qa_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/redis_tools.py` & `dcicutils-8.8.2.1b2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/redis_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/s3_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/schema_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.2.1b2/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.2.1b2/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.2.1b2/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/secrets_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/sheet_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/snapshot_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/structured_data.py` & `dcicutils-8.8.2.1b2/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.2.1b2/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.2.1b2/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/task_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/trace_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/validation_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/variant_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/dcicutils/zip_utils.py` & `dcicutils-8.8.2.1b2/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b1/pyproject.toml` & `dcicutils-8.8.2.1b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.2.1b1"  # TODO: To become 8.8.3
+version = "8.8.2.1b2"  # TODO: To become 8.8.3
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.2.1b1/PKG-INFO` & `dcicutils-8.8.2.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.2.1b1
+Version: 8.8.2.1b2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```
