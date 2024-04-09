# Comparing `tmp/rox-5.1.2.tar.gz` & `tmp/rox-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rox-python/rox-python/dist/.tmp-wti42k22/rox-5.1.2.tar", last modified: Tue Mar  5 04:22:04 2024, max compression
+gzip compressed data, was "/home/runner/work/rox-python/rox-python/dist/.tmp-rqlnbgrt/rox-5.1.3.tar", last modified: Tue Apr  9 22:36:02 2024, max compression
```

## Comparing `rox-5.1.2.tar` & `rox-5.1.3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-05 04:21:44.000000 rox-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-05 04:21:44.000000 rox-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-05 04:22:04.000000 rox-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-05 04:21:44.000000 rox-5.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/analytics-test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/analytics-test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-05 04:21:44.000000 rox-5.1.2/analytics-test/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/e2e-server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/e2e-server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-03-05 04:21:44.000000 rox-5.1.2/e2e-server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-05 04:22:02.000000 rox-5.1.2/rox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/client_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/analytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/client/buid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/client/device_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/client/dynamic_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/client/internal_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/client/sdk_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/configuration_fetched_invoker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/configuration_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/configuration/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/models/experiment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/configuration/models/target_group_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/consts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/consts/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/consts/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/consts/property_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/context/merged_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/custom_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/custom_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/custom_properties/custom_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/custom_properties/custom_property_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/custom_properties/device_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/default_flag_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/flag_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/rox_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/rox_double.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/rox_int.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/entities/rox_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/error_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/error_handling/exception_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/error_handling/userspace_handler_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/error_handling/userspace_unhandled_error_invoker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/impression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/impression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/impression/impression_invoker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/impression/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/impression/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/impression/models/reporting_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/logging/no_op_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/configuration_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/configuration_fetcher_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/configuration_fetcher_roxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/configuration_fetcher_self_managed.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/configuration_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/network/state_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/notifications/notification_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/register/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/register/registerer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/reporting/error_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/custom_property_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/experiment_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/flag_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/repositories/roxx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/roxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/roxx/experiments_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/roxx/properties_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/repositories/target_group_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/roxx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/basic_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/core_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/evaluation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/regular_expression_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/string_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/token_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/tokenized_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/roxx/value_compare_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/security/signature_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/security/signature_verifier_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/aggregate_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/http_status_code_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/md5_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/numeric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/periodic_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-05 04:21:44.000000 rox-5.1.2/rox/core/utils/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/server/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/client/sdk_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/client/server_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/server/flags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/flags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/flags/flag_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/flags/normalize_flag_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/flags/rox_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/flags/server_entities_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox/server/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/logging/server_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/rox_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/rox_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-05 04:21:44.000000 rox-5.1.2/rox/server/rox_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:22:04.000000 rox-5.1.2/rox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-05 04:22:04.000000 rox-5.1.2/rox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-05 04:22:04.000000 rox-5.1.2/rox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 04:22:04.000000 rox-5.1.2/rox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-05 04:22:04.000000 rox-5.1.2/rox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-05 04:22:04.000000 rox-5.1.2/rox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 04:22:04.000000 rox-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-05 04:21:44.000000 rox-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-09 22:35:44.000000 rox-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 22:35:44.000000 rox-5.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-09 22:36:02.000000 rox-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 22:35:44.000000 rox-5.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/analytics-test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/analytics-test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-09 22:35:44.000000 rox-5.1.3/analytics-test/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/e2e-server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/e2e-server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-04-09 22:35:44.000000 rox-5.1.3/e2e-server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 22:36:00.000000 rox-5.1.3/rox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/client_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/analytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/client/buid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/client/device_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/client/dynamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/client/internal_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/client/sdk_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/configuration_fetched_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/configuration_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/configuration/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/models/experiment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/configuration/models/target_group_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/consts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/consts/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/consts/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/consts/property_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/context/merged_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/custom_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/custom_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/custom_properties/custom_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/custom_properties/custom_property_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/custom_properties/device_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/default_flag_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/flag_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/rox_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/rox_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/rox_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/entities/rox_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/error_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/error_handling/exception_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/error_handling/userspace_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/error_handling/userspace_unhandled_error_invoker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/impression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/impression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/impression/impression_invoker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/impression/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/impression/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/impression/models/reporting_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/logging/no_op_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/configuration_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/configuration_fetcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/configuration_fetcher_roxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/configuration_fetcher_self_managed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/configuration_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/network/state_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/notifications/notification_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/register/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/register/registerer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/reporting/error_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/custom_property_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/experiment_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/flag_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/repositories/roxx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/roxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/roxx/experiments_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/roxx/properties_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/repositories/target_group_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/roxx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/basic_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/core_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/evaluation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/regular_expression_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/string_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/token_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/tokenized_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/roxx/value_compare_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/security/signature_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/security/signature_verifier_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/aggregate_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/http_status_code_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/md5_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/numeric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/periodic_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 22:35:44.000000 rox-5.1.3/rox/core/utils/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/server/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/client/sdk_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/client/server_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/server/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/flags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/flags/flag_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/flags/normalize_flag_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/flags/rox_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/flags/server_entities_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox/server/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/logging/server_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/rox_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/rox_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 22:35:44.000000 rox-5.1.3/rox/server/rox_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:36:02.000000 rox-5.1.3/rox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-09 22:36:02.000000 rox-5.1.3/rox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-09 22:36:02.000000 rox-5.1.3/rox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:36:02.000000 rox-5.1.3/rox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 22:36:02.000000 rox-5.1.3/rox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 22:36:02.000000 rox-5.1.3/rox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:36:02.000000 rox-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 22:35:44.000000 rox-5.1.3/setup.py
```

### Comparing `rox-5.1.2/LICENSE` & `rox-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/PKG-INFO` & `rox-5.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox
-Version: 5.1.2
+Version: 5.1.3
 Summary: Rollout.io ROX Python SDK
 Home-page: https://support.rollout.io/docs/python-api
 Author: Rollout.io
 Author-email: support@rollout.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rox-5.1.2/README.md` & `rox-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/analytics-test/main.py` & `rox-5.1.3/analytics-test/main.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/e2e-server/server.py` & `rox-5.1.3/e2e-server/server.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/analytics/__init__.py` & `rox-5.1.3/rox/core/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/analytics/client.py` & `rox-5.1.3/rox/core/analytics/client.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/analytics/client_proxy.py` & `rox-5.1.3/rox/core/analytics/client_proxy.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/analytics/consumer.py` & `rox-5.1.3/rox/core/analytics/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # lower to leave space for extra data that will be added later, eg. "sentAt".
 BATCH_SIZE_LIMIT = 475000
 
 
 class Consumer(Thread):
     """Consumes the messages from the client's queue."""
     def __init__(self, device_properties, environment, queue, write_key, upload_size=100, host=None, on_error=None,
-                 upload_interval=0.5, gzip=False, retries=10):
+                 upload_interval=0.5, gzip=False, retries=9):
         """Create a consumer thread."""
         Thread.__init__(self)
         # Make consumer a daemon thread so that it doesn't block program exit
         self.daemon = True
         self.upload_size = upload_size
         self.upload_interval = upload_interval
         self.write_key = write_key
@@ -112,14 +112,15 @@
 
         return items
 
     def request(self, batch):
         """Attempt to upload the batch and retry before raising an error """
 
         def fatal_exception(exc):
+            Logging.get_logger().debug('error sending analytic data', exc)
             if isinstance(exc, APIError):
                 # retry on server errors and client errors with 429 status code (rate limited),
                 # don't retry on other client errors
                 return (400 <= exc.status < 500) and exc.status != 429
             else:
                 # retry on all other errors (eg. network)
                 return False
```

### Comparing `rox-5.1.2/rox/core/analytics/request.py` & `rox-5.1.3/rox/core/analytics/request.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/analytics/utils.py` & `rox-5.1.3/rox/core/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/client/buid.py` & `rox-5.1.3/rox/core/client/buid.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/client/device_properties.py` & `rox-5.1.3/rox/core/client/device_properties.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/client/dynamic_api.py` & `rox-5.1.3/rox/core/client/dynamic_api.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/client/internal_flags.py` & `rox-5.1.3/rox/core/client/internal_flags.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/configuration/configuration_fetched_invoker.py` & `rox-5.1.3/rox/core/configuration/configuration_fetched_invoker.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/configuration/configuration_parser.py` & `rox-5.1.3/rox/core/configuration/configuration_parser.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/consts/environment.py` & `rox-5.1.3/rox/core/consts/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 class Environment:
     @staticmethod
     def ROXY_INTERNAL_PATH():
         return 'device/request_configuration'
     
     def __init__(self, rox_options, api_type: ApiType):
+        self.api_type = api_type 
         if rox_options and rox_options.network_configuration_options:
             self.get_config_cdn_path = rox_options.network_configuration_options.get_config_cloud_endpoint
             self.get_config_api_path = rox_options.network_configuration_options.get_config_api_endpoint
             self.send_state_cdn_path = rox_options.network_configuration_options.send_state_cloud_endpoint
             self.send_state_api_path = rox_options.network_configuration_options.send_state_api_endpoint
             self.analytics_path = rox_options.network_configuration_options.analytics_endpoint
             self.push_notifications_path = rox_options.network_configuration_options.push_notification_endpoint
-            self.api_type = api_type 
         else:
             # backwards compatibility (relying on env var)
             rollout_mode = os.getenv('ROLLOUT_MODE', '')
             if rollout_mode == 'QA':
                 self.get_config_cdn_path = 'https://qa-conf.rollout.io'
                 self.get_config_api_path = 'https://qa-api.rollout.io/device/get_configuration'
                 self.send_state_cdn_path = 'https://qa-statestore.rollout.io'
```

### Comparing `rox-5.1.2/rox/core/consts/property_type.py` & `rox-5.1.3/rox/core/consts/property_type.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/core.py` & `rox-5.1.3/rox/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             
             is_api_key_valid = is_platform_api_key or is_rollout_api_key
             if is_api_key_valid is None:
                 raise ValueError('Illegal rollout apikey')
           
             if is_platform_api_key:
                 api_type = ApiType.PLATFORM
+                self.rox_options.disable_signature_verification = True
+                
         self.environment = Environment(self.rox_options, api_type)
         
         self.internal_flags = InternalFlags(self.experiment_repository, self.parser, rox_options)
         self.analytics_client = ClientProxy(device_properties, self.environment, device_properties.rollout_key)
         self.impression_invoker = ImpressionInvoker(self.internal_flags, self.custom_property_repository, device_properties, self.analytics_client, roxy_path is not None, self.user_unhandled_error_invoker)
         self.flag_setter = FlagSetter(self.flag_repository, self.parser, self.experiment_repository, self.impression_invoker)
         buid = BUID(sdk_settings, device_properties)
```

### Comparing `rox-5.1.2/rox/core/custom_properties/custom_property_type.py` & `rox-5.1.3/rox/core/custom_properties/custom_property_type.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/entities/flag.py` & `rox-5.1.3/rox/core/entities/flag.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/entities/flag_setter.py` & `rox-5.1.3/rox/core/entities/flag_setter.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/entities/rox_base.py` & `rox-5.1.3/rox/core/entities/rox_base.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/entities/rox_double.py` & `rox-5.1.3/rox/core/entities/rox_double.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/entities/rox_int.py` & `rox-5.1.3/rox/core/entities/rox_int.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/entities/rox_string.py` & `rox-5.1.3/rox/core/entities/rox_string.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/error_handling/userspace_unhandled_error_invoker.py` & `rox-5.1.3/rox/core/error_handling/userspace_unhandled_error_invoker.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/impression/impression_invoker.py` & `rox-5.1.3/rox/core/impression/impression_invoker.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/network/configuration_fetcher.py` & `rox-5.1.3/rox/core/network/configuration_fetcher.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/network/configuration_fetcher_base.py` & `rox-5.1.3/rox/core/network/configuration_fetcher_base.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/network/configuration_fetcher_roxy.py` & `rox-5.1.3/rox/core/network/configuration_fetcher_roxy.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/network/configuration_fetcher_self_managed.py` & `rox-5.1.3/rox/core/network/configuration_fetcher_self_managed.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/network/request.py` & `rox-5.1.3/rox/core/network/request.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/network/state_sender.py` & `rox-5.1.3/rox/core/network/state_sender.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/notifications/notification_listener.py` & `rox-5.1.3/rox/core/notifications/notification_listener.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/register/registerer.py` & `rox-5.1.3/rox/core/register/registerer.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/reporting/error_reporter.py` & `rox-5.1.3/rox/core/reporting/error_reporter.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/repositories/custom_property_repository.py` & `rox-5.1.3/rox/core/repositories/custom_property_repository.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/repositories/flag_repository.py` & `rox-5.1.3/rox/core/repositories/flag_repository.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/repositories/roxx/experiments_extensions.py` & `rox-5.1.3/rox/core/repositories/roxx/experiments_extensions.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/repositories/roxx/properties_extensions.py` & `rox-5.1.3/rox/core/repositories/roxx/properties_extensions.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/basic_operators.py` & `rox-5.1.3/rox/core/roxx/basic_operators.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/evaluation_result.py` & `rox-5.1.3/rox/core/roxx/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/parser.py` & `rox-5.1.3/rox/core/roxx/parser.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/regular_expression_extensions.py` & `rox-5.1.3/rox/core/roxx/regular_expression_extensions.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/string_tokenizer.py` & `rox-5.1.3/rox/core/roxx/string_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/token_type.py` & `rox-5.1.3/rox/core/roxx/token_type.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/tokenized_expression.py` & `rox-5.1.3/rox/core/roxx/tokenized_expression.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/roxx/value_compare_extensions.py` & `rox-5.1.3/rox/core/roxx/value_compare_extensions.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/security/signature_verifier.py` & `rox-5.1.3/rox/core/security/signature_verifier.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/utils/debounce.py` & `rox-5.1.3/rox/core/utils/debounce.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/core/utils/periodic_task.py` & `rox-5.1.3/rox/core/utils/periodic_task.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/server/flags/normalize_flag_type.py` & `rox-5.1.3/rox/server/flags/normalize_flag_type.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/server/flags/server_entities_provider.py` & `rox-5.1.3/rox/server/flags/server_entities_provider.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/server/logging/server_logger.py` & `rox-5.1.3/rox/server/logging/server_logger.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/server/rox_options.py` & `rox-5.1.3/rox/server/rox_options.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox/server/rox_server.py` & `rox-5.1.3/rox/server/rox_server.py`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/rox.egg-info/PKG-INFO` & `rox-5.1.3/rox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox
-Version: 5.1.2
+Version: 5.1.3
 Summary: Rollout.io ROX Python SDK
 Home-page: https://support.rollout.io/docs/python-api
 Author: Rollout.io
 Author-email: support@rollout.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rox-5.1.2/rox.egg-info/SOURCES.txt` & `rox-5.1.3/rox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rox-5.1.2/setup.py` & `rox-5.1.3/setup.py`

 * *Files identical despite different names*

