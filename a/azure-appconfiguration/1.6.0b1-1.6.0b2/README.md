# Comparing `tmp/azure-appconfiguration-1.6.0b1.tar.gz` & `tmp/azure-appconfiguration-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-appconfiguration-1.6.0b1.tar", last modified: Fri Mar 15 03:15:32 2024, max compression
+gzip compressed data, was "azure-appconfiguration-1.6.0b2.tar", last modified: Fri Mar 22 01:00:58 2024, max compression
```

## Comparing `azure-appconfiguration-1.6.0b1.tar` & `azure-appconfiguration-1.6.0b2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.873201 azure-appconfiguration-1.6.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5619 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      188 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    24485 2024-03-15 03:15:32.873201 azure-appconfiguration-1.6.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17863 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4294 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/TROUBLESHOOTING.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.857201 azure-appconfiguration-1.6.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.857201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1328 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37452 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      530 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3297 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      441 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_constants.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.861201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      850 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4866 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3349 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3312 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79269 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1323 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.861201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      850 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4971 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3359 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3389 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1063 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.861201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    98556 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7187 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.861201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1983 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2180 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22032 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.861201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   128461 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7396 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24948 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4941 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_sync_token.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3209 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      172 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.861201 azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      595 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38349 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4196 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/_sync_token_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/azure/appconfiguration/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.873201 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    24485 2024-03-15 03:15:32.000000 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3265 2024-03-15 03:15:32.000000 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-15 03:15:32.000000 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-15 03:15:32.000000 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       34 2024-03-15 03:15:32.000000 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-15 03:15:32.000000 azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       39 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.869202 azure-appconfiguration-1.6.0b1/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4498 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2356 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/conditional_operation_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2512 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/conditional_operation_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2725 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/hello_world_advanced_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2635 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/hello_world_advanced_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1885 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/hello_world_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1953 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/hello_world_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1661 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/list_revision_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1769 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/list_revision_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1954 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/read_only_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2062 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/read_only_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1225 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/send_request_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1287 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/send_request_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2953 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/snapshot_samples.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3127 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/snapshot_samples_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/sync_token_samples.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1597 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/sync_token_samples_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1309 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/samples/util.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-15 03:15:32.873201 azure-appconfiguration-1.6.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2509 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.869202 azure-appconfiguration-1.6.0b1/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1364 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/async_preparers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2207 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/asynctestcase.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2029 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      863 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/consts.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:15:32.873201 azure-appconfiguration-1.6.0b1/tests/perfstress_tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/perfstress_tests/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1613 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/perfstress_tests/get.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1685 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/perfstress_tests/set.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2283 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/preparers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    52831 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34112 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client_aad.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38873 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client_aad_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    57758 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5735 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/test_consistency.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4662 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/test_sync_token_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4404 2024-03-15 03:14:06.000000 azure-appconfiguration-1.6.0b1/tests/testcase.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.909104 azure-appconfiguration-1.6.0b2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5925 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      188 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    24791 2024-03-22 01:00:58.909104 azure-appconfiguration-1.6.0b2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17863 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4294 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/TROUBLESHOOTING.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.893104 azure-appconfiguration-1.6.0b2/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.893104 azure-appconfiguration-1.6.0b2/azure/appconfiguration/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1328 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37152 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_azure_appconfiguration_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      530 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_azure_appconfiguration_error.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3297 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_azure_appconfiguration_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      441 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_constants.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.897104 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      850 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4866 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_azure_app_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3349 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3312 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79269 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1323 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.897104 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      850 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4971 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3359 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3389 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1063 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.897104 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    98556 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7187 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.897104 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1983 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2180 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22032 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.901105 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   128461 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7396 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/py.typed
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25008 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4941 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_sync_token.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3209 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      172 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.901105 azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      595 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38049 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4196 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/_sync_token_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/azure/appconfiguration/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.909104 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    24791 2024-03-22 01:00:58.000000 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3265 2024-03-22 01:00:58.000000 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-22 01:00:58.000000 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-22 01:00:58.000000 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       34 2024-03-22 01:00:58.000000 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-22 01:00:58.000000 azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       39 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.905104 azure-appconfiguration-1.6.0b2/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4498 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2356 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/conditional_operation_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2512 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/conditional_operation_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2725 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/hello_world_advanced_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2635 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/hello_world_advanced_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1885 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/hello_world_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1953 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/hello_world_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1661 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/list_revision_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1769 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/list_revision_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1954 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/read_only_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2062 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/read_only_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1225 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/send_request_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1287 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/send_request_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2953 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/snapshot_samples.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3127 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/snapshot_samples_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/sync_token_samples.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1597 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/sync_token_samples_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1309 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/samples/util.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-22 01:00:58.909104 azure-appconfiguration-1.6.0b2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2509 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.905104 azure-appconfiguration-1.6.0b2/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1364 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/async_preparers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2207 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/asynctestcase.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2029 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      863 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/consts.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 01:00:58.909104 azure-appconfiguration-1.6.0b2/tests/perfstress_tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/perfstress_tests/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1613 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/perfstress_tests/get.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1685 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/perfstress_tests/set.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2283 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/preparers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    54325 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34115 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client_aad.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38876 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client_aad_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    59401 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5736 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/test_consistency.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4662 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/test_sync_token_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4510 2024-03-22 00:59:36.000000 azure-appconfiguration-1.6.0b2/tests/testcase.py
```

### Comparing `azure-appconfiguration-1.6.0b1/CHANGELOG.md` & `azure-appconfiguration-1.6.0b2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 1.6.0b2 (2024-03-21)
+
+### Bugs Fixed
+- Changed invalid default value `None` to `False` for property `enabled` in `FeatureFlagConfigurationSetting`.
+- Fixed the issue that `description`, `display_name` and other customer fields are missing when de/serializing `FeatureFlagConfigurationSetting` objects.
+
 ## 1.6.0b1 (2024-03-14)
 
 ### Features Added
 - Exposed `send_request()` method in each client to send custom requests using the client's existing pipeline.
 - Supported to get page ETag while iterating `list_configuration_setting()` result by page.
 
 ### Bugs Fixed
```

### Comparing `azure-appconfiguration-1.6.0b1/LICENSE` & `azure-appconfiguration-1.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/PKG-INFO` & `azure-appconfiguration-1.6.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-appconfiguration
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Microsoft App Configuration Data Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -487,14 +487,20 @@
 [coc_contact]: mailto:opencode@microsoft.com
 [troubleshooting_guide]: https://aka.ms/azsdk/python/appconfiguration/troubleshoot
 [label_concept]: https://docs.microsoft.com/azure/azure-app-configuration/concept-key-value#label-keys
 
 
 # Release History
 
+## 1.6.0b2 (2024-03-21)
+
+### Bugs Fixed
+- Changed invalid default value `None` to `False` for property `enabled` in `FeatureFlagConfigurationSetting`.
+- Fixed the issue that `description`, `display_name` and other customer fields are missing when de/serializing `FeatureFlagConfigurationSetting` objects.
+
 ## 1.6.0b1 (2024-03-14)
 
 ### Features Added
 - Exposed `send_request()` method in each client to send custom requests using the client's existing pipeline.
 - Supported to get page ETag while iterating `list_configuration_setting()` result by page.
 
 ### Bugs Fixed
```

### Comparing `azure-appconfiguration-1.6.0b1/README.md` & `azure-appconfiguration-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/TROUBLESHOOTING.md` & `azure-appconfiguration-1.6.0b2/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_azure_appconfiguration_client.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_azure_appconfiguration_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import binascii
 import functools
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Optional, Union, cast, overload
+from typing import Any, Dict, List, Optional, Union, cast, overload
 from typing_extensions import Literal
 from azure.core import MatchConditions
 from azure.core.paging import ItemPaged
 from azure.core.credentials import TokenCredential, AzureKeyCredential
 from azure.core.pipeline.policies import BearerTokenCredentialPolicy
 from azure.core.polling import LROPoller
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.exceptions import (
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceModifiedError,
     ResourceNotModifiedError,
 )
 from azure.core.rest import HttpRequest, HttpResponse
-from azure.core.utils import CaseInsensitiveDict
 from ._azure_appconfiguration_error import ResourceReadOnlyError
 from ._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
 from ._generated import AzureAppConfiguration
 from ._generated.models import SnapshotUpdateParameters, SnapshotStatus
 from ._models import (
     ConfigurationSetting,
     ConfigurationSettingsFilter,
@@ -317,24 +316,23 @@
                 value="my value",
                 content_type="my content type",
                 tags={"my tag": "my tag value"}
             )
             added_config_setting = client.add_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
-        custom_headers: Mapping[str, Any] = CaseInsensitiveDict(kwargs.get("headers"))
         error_map = {412: ResourceExistsError}
         try:
             key_value_added = self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_none_match="*",
-                headers=custom_headers,
                 error_map=error_map,
+                **kwargs,
             )
             return ConfigurationSetting._from_generated(key_value_added)
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def set_configuration_setting(
@@ -354,17 +352,17 @@
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param match_condition: The match condition to use upon the etag
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: check if the ConfigurationSetting is changed. \
             Will use the value from param configuration_setting if not set.
         :return: The ConfigurationSetting returned from the service
         :rtype: ~azure.appconfiguration.ConfigurationSetting
-        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+        :raises: :class:`~azure.appconfiguration.ResourceReadOnlyError`, \
+            :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
-            :class:`~azure.core.exceptions.ResourceReadOnlyError`, \
             :class:`~azure.core.exceptions.ResourceModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
@@ -376,15 +374,14 @@
                 value="my set value",
                 content_type="my set content type",
                 tags={"my set tag": "my set tag value"}
             )
             returned_config_setting = client.set_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
-        custom_headers: Mapping[str, Any] = CaseInsensitiveDict(kwargs.get("headers"))
         error_map: Dict[int, Any] = {409: ResourceReadOnlyError}
         if match_condition == MatchConditions.IfNotModified:
             error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
             error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
             error_map.update({412: ResourceNotFoundError})
@@ -394,59 +391,58 @@
         try:
             key_value_set = self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_match=prep_if_match(configuration_setting.etag, match_condition),
                 if_none_match=prep_if_none_match(etag or configuration_setting.etag, match_condition),
-                headers=custom_headers,
                 error_map=error_map,
+                **kwargs,
             )
             return ConfigurationSetting._from_generated(key_value_set)
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def delete_configuration_setting(  # pylint:disable=delete-operation-wrong-return-type
         self,
         key: str,
         label: Optional[str] = None,
         *,
         etag: Optional[str] = None,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         **kwargs,
-    ) -> ConfigurationSetting:
+    ) -> Union[None, ConfigurationSetting]:
         """Delete a ConfigurationSetting if it exists
 
         :param key: key used to identify the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :keyword match_condition: The match condition to use upon the etag
         :paramtype match_condition: ~azure.core.MatchConditions
         :return: The deleted ConfigurationSetting returned from the service, or None if it doesn't exist.
         :rtype: ~azure.appconfiguration.ConfigurationSetting
-        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+        :raises: :class:`~azure.appconfiguration.ResourceReadOnlyError`, \
+            :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
-            :class:`~azure.core.exceptions.ResourceReadOnlyError`, \
             :class:`~azure.core.exceptions.ResourceModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
             deleted_config_setting = client.delete_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
-        custom_headers: Mapping[str, Any] = CaseInsensitiveDict(kwargs.get("headers"))
         error_map: Dict[int, Any] = {409: ResourceReadOnlyError}
         if match_condition == MatchConditions.IfNotModified:
             error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
             error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
             error_map.update({412: ResourceNotFoundError})
@@ -454,18 +450,20 @@
             error_map.update({412: ResourceExistsError})
 
         try:
             key_value_deleted = self._impl.delete_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
-                headers=custom_headers,
                 error_map=error_map,
+                **kwargs,
             )
-            return ConfigurationSetting._from_generated(key_value_deleted)  # type: ignore
+            if key_value_deleted:
+                return ConfigurationSetting._from_generated(key_value_deleted)
+            return None
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def list_revisions(
         self,
         key_filter: Optional[str] = None,
```

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_azure_appconfiguration_error.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_azure_appconfiguration_error.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_azure_appconfiguration_requests.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_azure_app_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_configuration.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_patch.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_serialization.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/_vendor.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_azure_app_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_configuration.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_patch.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/_vendor.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/_models_py3.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/models/_patch.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_generated/operations/_patch.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_models.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
 from ._generated.models import (
     KeyValue,
     KeyValueFilter,
     Snapshot as GeneratedConfigurationSnapshot,
     SnapshotStatus,
 )
 
-PolymorphicConfigurationSetting = Union[
-    "ConfigurationSetting", "SecretReferenceConfigurationSetting", "FeatureFlagConfigurationSetting"
-]
-
 
 class ConfigurationSetting(Model):
     """A setting, defined by a unique combination of a key and label."""
 
     value: str
     """The value of the configuration setting."""
     etag: str
@@ -66,33 +62,31 @@
         self.etag = kwargs.get("etag", None)
         self.content_type = kwargs.get("content_type", None)
         self.last_modified = kwargs.get("last_modified", None)
         self.read_only = kwargs.get("read_only", None)
         self.tags = kwargs.get("tags", {})
 
     @classmethod
-    def _from_generated(cls, key_value: KeyValue) -> PolymorphicConfigurationSetting:
-        if key_value is None:
-            return key_value
+    def _from_generated(cls, key_value: KeyValue) -> "ConfigurationSetting":
+        # pylint:disable=protected-access
         if key_value.content_type is not None:
             try:
                 if key_value.content_type.startswith(
-                    FeatureFlagConfigurationSetting._feature_flag_content_type  # pylint:disable=protected-access
+                    FeatureFlagConfigurationSetting._feature_flag_content_type
                 ) and key_value.key.startswith(  # type: ignore
-                    FeatureFlagConfigurationSetting._key_prefix  # pylint: disable=protected-access
+                    FeatureFlagConfigurationSetting._key_prefix
                 ):
-                    return FeatureFlagConfigurationSetting._from_generated(  # pylint: disable=protected-access
-                        key_value
-                    )
+                    config_setting = FeatureFlagConfigurationSetting._from_generated(key_value)
+                    if key_value.value:
+                        config_setting.value = key_value.value
+                    return config_setting
                 if key_value.content_type.startswith(
-                    SecretReferenceConfigurationSetting._secret_reference_content_type  # pylint:disable=protected-access
+                    SecretReferenceConfigurationSetting._secret_reference_content_type
                 ):
-                    return SecretReferenceConfigurationSetting._from_generated(  # pylint: disable=protected-access
-                        key_value
-                    )
+                    return SecretReferenceConfigurationSetting._from_generated(key_value)
             except (KeyError, AttributeError):
                 pass
 
         return cls(
             key=key_value.key,
             label=key_value.label,
             value=key_value.value,
@@ -121,15 +115,15 @@
 
     etag: str
     """A value representing the current state of the resource."""
     feature_id: str
     """The identity of the configuration setting."""
     key: str
     """The key of the configuration setting."""
-    enabled: Optional[bool]
+    enabled: bool
     """The value indicating whether the feature flag is enabled. A feature is OFF if enabled is false.
         If enabled is true, then the feature is ON if there are no conditions or if all conditions are satisfied."""
     filters: Optional[List[Dict[str, Any]]]
     """Filters that must run on the client and be evaluated as true for the feature
         to be considered enabled."""
     label: str
     """The label used to group this configuration setting with others."""
@@ -160,25 +154,25 @@
     _feature_flag_content_type = "application/vnd.microsoft.appconfig.ff+json;charset=utf-8"
     kind = "FeatureFlag"
 
     def __init__(  # pylint: disable=super-init-not-called
         self,
         feature_id: str,
         *,
-        enabled: Optional[bool] = None,
+        enabled: bool = False,
         filters: Optional[List[Dict[str, Any]]] = None,
         **kwargs: Any,
     ) -> None:
         """
         :param feature_id: The identity of the configuration setting.
         :type feature_id: str
         :keyword enabled: The value indicating whether the feature flag is enabled.
             A feature is OFF if enabled is false. If enabled is true, then the feature is ON
-            if there are no conditions or if all conditions are satisfied.
-        :paramtype enabled: bool or None
+            if there are no conditions or if all conditions are satisfied. Default value of this property is False.
+        :paramtype enabled: bool
         :keyword filters: Filters that must run on the client and be evaluated as true for the feature
             to be considered enabled.
         :paramtype filters: list[dict[str, Any]] or None
         """
         if "key" in kwargs or "value" in kwargs:
             raise TypeError("Unexpected keyword argument, do not provide 'key' or 'value' as a keyword-arg")
         self.feature_id = feature_id
@@ -203,48 +197,54 @@
 
         :rtype: str
         """
         try:
             temp = json.loads(self._value)
             temp["id"] = self.feature_id
             temp["enabled"] = self.enabled
+            temp["display_name"] = self.display_name
+            temp["description"] = self.description
             if "conditions" not in temp.keys():
                 temp["conditions"] = {}
             temp["conditions"]["client_filters"] = self.filters
             self._value = json.dumps(temp)
             return self._value
         except (json.JSONDecodeError, ValueError):
             return self._value
 
     @value.setter
     def value(self, new_value: str) -> None:
         try:
             temp = json.loads(new_value)
             temp["id"] = self.feature_id
             self._value = json.dumps(temp)
-            self.enabled = temp.get("enabled", None)
+            self.enabled = temp.get("enabled", False)
+            self.display_name = temp.get("display_name", None)
+            self.description = temp.get("description", None)
             self.filters = None
             conditions = temp.get("conditions", None)
             if conditions:
                 self.filters = conditions.get("client_filters", None)
         except (json.JSONDecodeError, ValueError):
             self._value = new_value
-            self.enabled = None
+            self.enabled = False
             self.filters = None
 
     @classmethod
-    def _from_generated(cls, key_value: KeyValue) -> Union["FeatureFlagConfigurationSetting", ConfigurationSetting]:
-        if key_value is None:
-            return key_value
-        enabled = None
+    def _from_generated(cls, key_value: KeyValue) -> "FeatureFlagConfigurationSetting":
+        enabled = False
         filters = None
+        display_name = None
+        description = None
         try:
             temp = json.loads(key_value.value)  # type: ignore
             if isinstance(temp, dict):
-                enabled = temp.get("enabled")
+                enabled = temp.get("enabled", False)
+                display_name = temp.get("display_name")
+                description = temp.get("description")
                 if "conditions" in temp.keys():
                     filters = temp["conditions"].get("client_filters")
         except (ValueError, json.JSONDecodeError):
             pass
 
         return cls(
             feature_id=key_value.key.lstrip(".appconfig.featureflag").lstrip("/"),  # type: ignore
@@ -252,14 +252,16 @@
             content_type=key_value.content_type,
             last_modified=key_value.last_modified,
             tags=key_value.tags,
             read_only=key_value.locked,
             etag=key_value.etag,
             enabled=enabled,
             filters=filters,
+            display_name=display_name,
+            description=description,
         )
 
     def _to_generated(self) -> KeyValue:
         return KeyValue(
             key=self.key,
             label=self.label,
             value=self.value,
@@ -345,16 +347,14 @@
             self.secret_id = temp.get("uri")
         except (json.JSONDecodeError, ValueError):
             self._value = new_value
             self.secret_id = None
 
     @classmethod
     def _from_generated(cls, key_value: KeyValue) -> "SecretReferenceConfigurationSetting":
-        if key_value is None:
-            return key_value
         secret_uri = None
         try:
             temp = json.loads(key_value.value)  # type: ignore
             secret_uri = temp.get("uri")
             if not secret_uri:
                 secret_uri = temp.get("secret_uri")
         except (ValueError, json.JSONDecodeError):
```

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_sync_token.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_sync_token.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/_utils.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/__init__.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import binascii
 import functools
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Optional, Union, cast, overload
+from typing import Any, Dict, List, Optional, Union, cast, overload
 from typing_extensions import Literal
 from azure.core import MatchConditions
 from azure.core.async_paging import AsyncItemPaged
 from azure.core.credentials import AzureKeyCredential
 from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.pipeline.policies import AsyncBearerTokenCredentialPolicy
 from azure.core.polling import AsyncLROPoller
@@ -19,15 +19,14 @@
 from azure.core.exceptions import (
     ResourceExistsError,
     ResourceModifiedError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
 )
 from azure.core.rest import AsyncHttpResponse, HttpRequest
-from azure.core.utils import CaseInsensitiveDict
 from ._sync_token_async import AsyncSyncTokenPolicy
 from .._azure_appconfiguration_error import ResourceReadOnlyError
 from .._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
 from .._generated.aio import AzureAppConfiguration
 from .._generated.models import SnapshotUpdateParameters, SnapshotStatus
 from .._models import (
     ConfigurationSetting,
@@ -330,25 +329,24 @@
                 value="my value",
                 content_type="my content type",
                 tags={"my tag": "my tag value"}
             )
             added_config_setting = await async_client.add_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
-        custom_headers: Mapping[str, Any] = CaseInsensitiveDict(kwargs.get("headers"))
         error_map = {412: ResourceExistsError}
 
         try:
             key_value_added = await self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_none_match="*",
-                headers=custom_headers,
                 error_map=error_map,
+                **kwargs,
             )
             return ConfigurationSetting._from_generated(key_value_added)
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace_async
     async def set_configuration_setting(
@@ -369,17 +367,17 @@
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param match_condition: The match condition to use upon the etag
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: check if the ConfigurationSetting is changed. \
             Will use the value from param configuration_setting if not set.
         :return: The ConfigurationSetting returned from the service
         :rtype: ~azure.appconfiguration.ConfigurationSetting
-        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+        :raises: :class:`~azure.appconfiguration.ResourceReadOnlyError`, \
+            :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
-            :class:`~azure.core.exceptions.ResourceReadOnlyError`, \
             :class:`~azure.core.exceptions.ResourceModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
@@ -392,15 +390,14 @@
                 value="my set value",
                 content_type="my set content type",
                 tags={"my set tag": "my set tag value"}
             )
             returned_config_setting = await async_client.set_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
-        custom_headers: Mapping[str, Any] = CaseInsensitiveDict(kwargs.get("headers"))
         error_map: Dict[int, Any] = {409: ResourceReadOnlyError}
         if match_condition == MatchConditions.IfNotModified:
             error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
             error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
             error_map.update({412: ResourceNotFoundError})
@@ -410,60 +407,59 @@
         try:
             key_value_set = await self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_match=prep_if_match(configuration_setting.etag, match_condition),
                 if_none_match=prep_if_none_match(etag or configuration_setting.etag, match_condition),
-                headers=custom_headers,
                 error_map=error_map,
+                **kwargs,
             )
             return ConfigurationSetting._from_generated(key_value_set)
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace_async
     async def delete_configuration_setting(
         self,
         key: str,
         label: Optional[str] = None,
         *,
         etag: Optional[str] = None,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         **kwargs,
-    ) -> ConfigurationSetting:
+    ) -> Union[None, ConfigurationSetting]:
         """Delete a ConfigurationSetting if it exists
 
         :param key: key used to identify the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :keyword match_condition: The match condition to use upon the etag
         :paramtype match_condition: ~azure.core.MatchConditions
         :return: The deleted ConfigurationSetting returned from the service, or None if it doesn't exist.
         :rtype: ~azure.appconfiguration.ConfigurationSetting
-        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+        :raises: :class:`~azure.appconfiguration.ResourceReadOnlyError`, \
+            :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
-            :class:`~azure.core.exceptions.ResourceReadOnlyError`, \
             :class:`~azure.core.exceptions.ResourceModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotModifiedError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
             # in async function
             deleted_config_setting = await async_client.delete_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
-        custom_headers: Mapping[str, Any] = CaseInsensitiveDict(kwargs.get("headers"))
         error_map: Dict[int, Any] = {409: ResourceReadOnlyError}
         if match_condition == MatchConditions.IfNotModified:
             error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
             error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
             error_map.update({412: ResourceNotFoundError})
@@ -471,18 +467,20 @@
             error_map.update({412: ResourceExistsError})
 
         try:
             key_value_deleted = await self._impl.delete_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
-                headers=custom_headers,
                 error_map=error_map,
+                **kwargs,
             )
-            return ConfigurationSetting._from_generated(key_value_deleted)  # type: ignore
+            if key_value_deleted:
+                return ConfigurationSetting._from_generated(key_value_deleted)
+            return None
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def list_revisions(
         self,
         key_filter: Optional[str] = None,
```

### Comparing `azure-appconfiguration-1.6.0b1/azure/appconfiguration/aio/_sync_token_async.py` & `azure-appconfiguration-1.6.0b2/azure/appconfiguration/aio/_sync_token_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/PKG-INFO` & `azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-appconfiguration
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Microsoft App Configuration Data Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -487,14 +487,20 @@
 [coc_contact]: mailto:opencode@microsoft.com
 [troubleshooting_guide]: https://aka.ms/azsdk/python/appconfiguration/troubleshoot
 [label_concept]: https://docs.microsoft.com/azure/azure-app-configuration/concept-key-value#label-keys
 
 
 # Release History
 
+## 1.6.0b2 (2024-03-21)
+
+### Bugs Fixed
+- Changed invalid default value `None` to `False` for property `enabled` in `FeatureFlagConfigurationSetting`.
+- Fixed the issue that `description`, `display_name` and other customer fields are missing when de/serializing `FeatureFlagConfigurationSetting` objects.
+
 ## 1.6.0b1 (2024-03-14)
 
 ### Features Added
 - Exposed `send_request()` method in each client to send custom requests using the client's existing pipeline.
 - Supported to get page ETag while iterating `list_configuration_setting()` result by page.
 
 ### Bugs Fixed
```

### Comparing `azure-appconfiguration-1.6.0b1/azure_appconfiguration.egg-info/SOURCES.txt` & `azure-appconfiguration-1.6.0b2/azure_appconfiguration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/README.md` & `azure-appconfiguration-1.6.0b2/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/conditional_operation_sample.py` & `azure-appconfiguration-1.6.0b2/samples/conditional_operation_sample.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/conditional_operation_sample_async.py` & `azure-appconfiguration-1.6.0b2/samples/conditional_operation_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/hello_world_advanced_sample.py` & `azure-appconfiguration-1.6.0b2/samples/hello_world_advanced_sample.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/hello_world_advanced_sample_async.py` & `azure-appconfiguration-1.6.0b2/samples/hello_world_advanced_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/hello_world_sample.py` & `azure-appconfiguration-1.6.0b2/samples/hello_world_sample.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/hello_world_sample_async.py` & `azure-appconfiguration-1.6.0b2/samples/hello_world_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/list_revision_sample.py` & `azure-appconfiguration-1.6.0b2/samples/list_revision_sample.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/list_revision_sample_async.py` & `azure-appconfiguration-1.6.0b2/samples/list_revision_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/read_only_sample.py` & `azure-appconfiguration-1.6.0b2/samples/read_only_sample.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/read_only_sample_async.py` & `azure-appconfiguration-1.6.0b2/samples/read_only_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/send_request_sample.py` & `azure-appconfiguration-1.6.0b2/samples/send_request_sample.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/send_request_sample_async.py` & `azure-appconfiguration-1.6.0b2/samples/send_request_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/snapshot_samples.py` & `azure-appconfiguration-1.6.0b2/samples/snapshot_samples.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/snapshot_samples_async.py` & `azure-appconfiguration-1.6.0b2/samples/snapshot_samples_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/sync_token_samples.py` & `azure-appconfiguration-1.6.0b2/samples/sync_token_samples.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/sync_token_samples_async.py` & `azure-appconfiguration-1.6.0b2/samples/sync_token_samples_async.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/samples/util.py` & `azure-appconfiguration-1.6.0b2/samples/util.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/setup.py` & `azure-appconfiguration-1.6.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/async_preparers.py` & `azure-appconfiguration-1.6.0b2/tests/async_preparers.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/asynctestcase.py` & `azure-appconfiguration-1.6.0b2/tests/asynctestcase.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/conftest.py` & `azure-appconfiguration-1.6.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/consts.py` & `azure-appconfiguration-1.6.0b2/tests/consts.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/perfstress_tests/get.py` & `azure-appconfiguration-1.6.0b2/tests/perfstress_tests/get.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/perfstress_tests/set.py` & `azure-appconfiguration-1.6.0b2/tests/perfstress_tests/set.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/preparers.py` & `azure-appconfiguration-1.6.0b2/tests/preparers.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client.py` & `azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,23 +625,23 @@
         assert changed_flag.enabled == True
         temp = json.loads(changed_flag.value)
         assert temp["id"] == set_flag_value["id"]
         assert temp["enabled"] == True
         assert temp["conditions"] == set_flag_value["conditions"]
 
         changed_flag.value = json.dumps({})
-        assert changed_flag.enabled == None
+        assert changed_flag.enabled == False
         temp = json.loads(changed_flag.value)
         assert temp["id"] == set_flag_value["id"]
-        assert temp["enabled"] == None
+        assert temp["enabled"] == False
         assert temp["conditions"] != None
         assert temp["conditions"]["client_filters"] == None
 
         set_flag.value = "bad_value"
-        assert set_flag.enabled == None
+        assert set_flag.enabled == False
         assert set_flag.filters == None
         assert set_flag.value == "bad_value"
 
         client.delete_configuration_setting(changed_flag.key)
 
     @app_config_decorator
     @recorded_by_proxy
@@ -809,14 +809,42 @@
         assert new_sent.filters[1]["parameters"]["Start"] == "Wed, 10 Mar 2021 08:00:00 GMT"
         assert new_sent.filters[2]["parameters"]["Audience"]["DefaultRolloutPercentage"] == 100
 
         client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator
     @recorded_by_proxy
+    def test_feature_custom_fields(self, appconfiguration_connection_string):
+        client = self.create_client(appconfiguration_connection_string)
+        custom_fields = {
+            "variants": [
+                {"name": "Off", "configuration_value": "Off", "status_override": "Enabled"},
+                {"name": "On", "configuration_value": "On", "status_override": "Disabled"},
+            ],
+            "allocation": {
+                "percentile": [{"variant": "Off", "from": 0, "to": 100}],
+                "user": [{"variant": "Off", "users": ["Adam"]}],
+                "seed": "adfsasdfzsd",
+                "default_when_enabled": "Off",
+                "default_when_disabled": "Off",
+            },
+        }
+        new = FeatureFlagConfigurationSetting(
+            "Beta",
+            description="Matt's variant FF",
+            enabled=True,
+        )
+        new.value = json.dumps(custom_fields)
+        sent = client.set_configuration_setting(new)
+        self._assert_same_keys(sent, new)
+
+        client.delete_configuration_setting(new.key)
+
+    @app_config_decorator
+    @recorded_by_proxy
     def test_breaking_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
             "breaking1",
             enabled=True,
             filters=[
                 {
@@ -826,14 +854,15 @@
                         "End": "Fri, 02 Apr 2021 04:00:00 GMT",
                     },
                 },
             ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
             "breaking2",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TIME_WINDOW,
@@ -842,14 +871,15 @@
                         "End": "not even trying to be a date",
                     },
                 },
             ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         # This will show up as a Custom filter
         new = FeatureFlagConfigurationSetting(
             "breaking3",
             enabled=True,
             filters=[
                 {
@@ -859,48 +889,52 @@
                         "End": "not even trying to be a date",
                     },
                 },
             ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
             "breaking4",
             enabled=True,
             filters=[
                 {"name": FILTER_TIME_WINDOW, "parameters": "stringystring"},
             ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
             "breaking5",
             enabled=True,
             filters=[{"name": FILTER_TARGETING, "parameters": {"Audience": {"Users": "123"}}}],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
             "breaking6", enabled=True, filters=[{"name": FILTER_TARGETING, "parameters": "invalidformat"}]
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting("breaking7", enabled=True, filters=[{"abc": "def"}])
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
+        client.delete_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting("breaking8", enabled=True, filters=[{"abc": "def"}])
         new.feature_flag_content_type = "fakeyfakey"  # cspell:disable-line
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
-
         client.delete_configuration_setting(new.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_breaking_with_secret_reference_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = SecretReferenceConfigurationSetting("aref", "notaurl")  # cspell:disable-line
```

### Comparing `azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client_aad.py` & `azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client_aad.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,23 +571,23 @@
         assert changed_flag.enabled == True
         temp = json.loads(changed_flag.value)
         assert temp["id"] == set_flag_value["id"]
         assert temp["enabled"] == True
         assert temp["conditions"] == set_flag_value["conditions"]
 
         changed_flag.value = json.dumps({})
-        assert changed_flag.enabled == None
+        assert changed_flag.enabled == False
         temp = json.loads(changed_flag.value)
         assert temp["id"] == set_flag_value["id"]
-        assert temp["enabled"] == None
+        assert temp["enabled"] == False
         assert temp["conditions"] != None
         assert temp["conditions"]["client_filters"] == None
 
         set_flag.value = "bad_value"
-        assert set_flag.enabled == None
+        assert set_flag.enabled == False
         assert set_flag.filters == None
         assert set_flag.value == "bad_value"
 
         client.delete_configuration_setting(changed_flag.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
```

### Comparing `azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client_aad_async.py` & `azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client_aad_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,23 +597,23 @@
             assert changed_flag.enabled == True
             temp = json.loads(changed_flag.value)
             assert temp["id"] == set_flag_value["id"]
             assert temp["enabled"] == True
             assert temp["conditions"] == set_flag_value["conditions"]
 
             changed_flag.value = json.dumps({})
-            assert changed_flag.enabled == None
+            assert changed_flag.enabled == False
             temp = json.loads(changed_flag.value)
             assert temp["id"] == set_flag_value["id"]
-            assert temp["enabled"] == None
+            assert temp["enabled"] == False
             assert temp["conditions"] != None
             assert temp["conditions"]["client_filters"] == None
 
             set_flag.value = "bad_value"
-            assert set_flag.enabled == None
+            assert set_flag.enabled == False
             assert set_flag.filters == None
             assert set_flag.value == "bad_value"
 
             await client.delete_configuration_setting(changed_flag.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
```

### Comparing `azure-appconfiguration-1.6.0b1/tests/test_azure_appconfiguration_client_async.py` & `azure-appconfiguration-1.6.0b2/tests/test_azure_appconfiguration_client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -635,23 +635,23 @@
             assert changed_flag.enabled == True
             temp = json.loads(changed_flag.value)
             assert temp["id"] == set_flag_value["id"]
             assert temp["enabled"] == True
             assert temp["conditions"] == set_flag_value["conditions"]
 
             changed_flag.value = json.dumps({})
-            assert changed_flag.enabled == None
+            assert changed_flag.enabled == False
             temp = json.loads(changed_flag.value)
             assert temp["id"] == set_flag_value["id"]
-            assert temp["enabled"] == None
+            assert temp["enabled"] == False
             assert temp["conditions"] != None
             assert temp["conditions"]["client_filters"] == None
 
             set_flag.value = "bad_value"
-            assert set_flag.enabled == None
+            assert set_flag.enabled == False
             assert set_flag.filters == None
             assert set_flag.value == "bad_value"
 
             await client.delete_configuration_setting(changed_flag.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
@@ -832,14 +832,42 @@
             assert new_sent.filters[1]["parameters"]["Start"] == "Wed, 10 Mar 2021 08:00:00 GMT"
             assert new_sent.filters[2]["parameters"]["Audience"]["DefaultRolloutPercentage"] == 100
 
             await client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
+    async def test_feature_custom_fields(self, appconfiguration_connection_string):
+        custom_fields = {
+            "variants": [
+                {"name": "Off", "configuration_value": "Off", "status_override": "Enabled"},
+                {"name": "On", "configuration_value": "On", "status_override": "Disabled"},
+            ],
+            "allocation": {
+                "percentile": [{"variant": "Off", "from": 0, "to": 100}],
+                "user": [{"variant": "Off", "users": ["Adam"]}],
+                "seed": "adfsasdfzsd",
+                "default_when_enabled": "Off",
+                "default_when_disabled": "Off",
+            },
+        }
+        async with self.create_client(appconfiguration_connection_string) as client:
+            new = FeatureFlagConfigurationSetting(
+                "Beta",
+                description="Matt's variant FF",
+                enabled=True,
+            )
+            new.value = json.dumps(custom_fields)
+            sent = await client.set_configuration_setting(new)
+            self._assert_same_keys(sent, new)
+
+            await client.delete_configuration_setting(new.key)
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
     async def test_breaking_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = FeatureFlagConfigurationSetting(
                 "breaking1",
                 enabled=True,
                 filters=[
                     {
@@ -849,14 +877,15 @@
                             "End": "Fri, 02 Apr 2021 04:00:00 GMT",
                         },
                     },
                 ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
                 "breaking2",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TIME_WINDOW,
@@ -865,14 +894,15 @@
                             "End": "not even trying to be a date",
                         },
                     },
                 ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             # This will show up as a Custom filter
             new = FeatureFlagConfigurationSetting(
                 "breaking3",
                 enabled=True,
                 filters=[
                     {
@@ -882,48 +912,52 @@
                             "End": "not even trying to be a date",
                         },
                     },
                 ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
                 "breaking4",
                 enabled=True,
                 filters=[
                     {"name": FILTER_TIME_WINDOW, "parameters": "stringystring"},
                 ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
                 "breaking5",
                 enabled=True,
                 filters=[{"name": FILTER_TARGETING, "parameters": {"Audience": {"Users": "123"}}}],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
                 "breaking6", enabled=True, filters=[{"name": FILTER_TARGETING, "parameters": "invalidformat"}]
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting("breaking7", enabled=True, filters=[{"abc": "def"}])
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
+            await client.delete_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting("breaking8", enabled=True, filters=[{"abc": "def"}])
             new.feature_flag_content_type = "fakeyfakey"  # cspell:disable-line
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
-
             await client.delete_configuration_setting(new.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_breaking_with_secret_reference_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = SecretReferenceConfigurationSetting("aref", "notaurl")  # cspell:disable-line
```

### Comparing `azure-appconfiguration-1.6.0b1/tests/test_consistency.py` & `azure-appconfiguration-1.6.0b2/tests/test_consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         set_custom_default_matcher(compare_bodies=False, excluded_headers="x-ms-content-sha256,x-ms-date")
         client = self.create_client(appconfiguration_connection_string)
         key = self.get_resource_name("key")
         feature_flag = FeatureFlagConfigurationSetting(key, enabled=True)
         set_flag = client.set_configuration_setting(feature_flag)
 
         set_flag.value = "hello world"
-        assert set_flag.enabled == None
+        assert set_flag.enabled == False
         assert set_flag.filters == None
         client.delete_configuration_setting(feature_flag)
 
 
 class TestAppConfigurationConsistencyUnitTest(AppConfigTestCase):
     def test_feature_flag_set_value(self):
         key = self.get_resource_name("key")
```

### Comparing `azure-appconfiguration-1.6.0b1/tests/test_sync_token_policy.py` & `azure-appconfiguration-1.6.0b2/tests/test_sync_token_policy.py`

 * *Files identical despite different names*

### Comparing `azure-appconfiguration-1.6.0b1/tests/testcase.py` & `azure-appconfiguration-1.6.0b2/tests/testcase.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,17 @@
         assert key1.label == key2.label
         assert key1.content_type == key2.content_type
         assert key1.tags == key2.tags
         assert key1.etag != key2.etag
         assert key1.value == key2.value
         if isinstance(key1, FeatureFlagConfigurationSetting):
             assert key1.enabled == key2.enabled
-            assert len(key1.filters) == len(key2.filters)
+            if key1.filters and key2.filters:
+                assert len(key1.filters) == len(key2.filters)
+            assert key1.description == key2.description
         elif isinstance(key1, SecretReferenceConfigurationSetting):
             assert key1.secret_id == key2.secret_id
 
     def _assert_snapshots(self, snapshot: ConfigurationSnapshot, expected_snapshot: ConfigurationSnapshot):
         assert snapshot.composition_type == expected_snapshot.composition_type
         assert snapshot.created == expected_snapshot.created
         assert snapshot.etag == expected_snapshot.etag
```

