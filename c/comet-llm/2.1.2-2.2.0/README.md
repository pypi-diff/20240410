# Comparing `tmp/comet_llm-2.1.2.tar.gz` & `tmp/comet_llm-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-2.1.2.tar", last modified: Tue Mar 26 14:12:47 2024, max compression
+gzip compressed data, was "comet_llm-2.2.0.tar", last modified: Wed Apr 10 09:56:17 2024, max compression
```

## Comparing `comet_llm-2.1.2.tar` & `comet_llm-2.2.0.tar`

### file list

```diff
@@ -1,102 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-26 14:12:39.000000 comet_llm-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-26 14:12:47.413566 comet_llm-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-03-26 14:12:39.000000 comet_llm-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 14:12:47.413566 comet_llm-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-26 14:12:39.000000 comet_llm-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.397566 comet_llm-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.405566 comet_llm-2.1.2/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.405566 comet_llm-2.1.2/src/comet_llm/api_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/api_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/api_objects/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/api_objects/llm_trace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.405566 comet_llm-2.1.2/src/comet_llm/autologgers/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.405566 comet_llm-2.1.2/src/comet_llm/autologgers/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/openai/chat_completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/openai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/openai/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/openai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/autologgers/openai/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/backend_error_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.409566 comet_llm-2.1.2/src/comet_llm/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/span.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/thread_context_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/chains/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/datetimes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.409566 comet_llm-2.1.2/src/comet_llm/dummy_api/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/dummy_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/dummy_api/dummy_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.409566 comet_llm-2.1.2/src/comet_llm/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/exceptions/filter_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.409566 comet_llm-2.1.2/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/experiment_api/failed_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/experiment_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.409566 comet_llm-2.1.2/src/comet_llm/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/src/comet_llm/import_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/callable_extenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/callback_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/module_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/import_hooks/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/llm_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/logging_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/src/comet_llm/message_processing/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/offline_message_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/online_message_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/src/comet_llm/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/prompts/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/prompts/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/prompts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/query_dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-26 14:12:39.000000 comet_llm-2.1.2/src/comet_llm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-26 14:12:47.000000 comet_llm-2.1.2/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-26 14:12:47.000000 comet_llm-2.1.2/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:12:47.000000 comet_llm-2.1.2/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:12:47.000000 comet_llm-2.1.2/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-26 14:12:47.000000 comet_llm-2.1.2/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 14:12:47.000000 comet_llm-2.1.2/src/comet_llm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:12:47.413566 comet_llm-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-26 14:12:39.000000 comet_llm-2.1.2/tests/testlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 09:56:12.000000 comet_llm-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-10 09:56:17.632742 comet_llm-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-10 09:56:12.000000 comet_llm-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:56:17.632742 comet_llm-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-10 09:56:12.000000 comet_llm-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.616741 comet_llm-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.620741 comet_llm-2.2.0/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.624741 comet_llm-2.2.0/src/comet_llm/api_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api_key/base64_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api_key/comet_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.624741 comet_llm-2.2.0/src/comet_llm/api_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api_objects/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/api_objects/llm_trace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.624741 comet_llm-2.2.0/src/comet_llm/autologgers/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.624741 comet_llm-2.2.0/src/comet_llm/autologgers/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/openai/chat_completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/openai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/openai/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/openai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/autologgers/openai/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/backend_error_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.624741 comet_llm-2.2.0/src/comet_llm/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/thread_context_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/chains/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/datetimes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.628741 comet_llm-2.2.0/src/comet_llm/dummy_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/dummy_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/dummy_api/dummy_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.628741 comet_llm-2.2.0/src/comet_llm/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/exceptions/filter_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.628741 comet_llm-2.2.0/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/experiment_api/failed_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/experiment_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.628741 comet_llm-2.2.0/src/comet_llm/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.628741 comet_llm-2.2.0/src/comet_llm/import_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/callable_extenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/callback_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/module_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/import_hooks/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/llm_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/logging_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/src/comet_llm/message_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/offline_message_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/online_message_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/src/comet_llm/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/prompts/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/prompts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/prompts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/query_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-10 09:56:12.000000 comet_llm-2.2.0/src/comet_llm/url_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-10 09:56:17.000000 comet_llm-2.2.0/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-10 09:56:17.000000 comet_llm-2.2.0/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:56:17.000000 comet_llm-2.2.0/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:56:17.000000 comet_llm-2.2.0/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 09:56:17.000000 comet_llm-2.2.0/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:56:17.000000 comet_llm-2.2.0/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:56:17.632742 comet_llm-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 09:56:12.000000 comet_llm-2.2.0/tests/testlib.py
```

### Comparing `comet_llm-2.1.2/LICENSE` & `comet_llm-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/PKG-INFO` & `comet_llm-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 2.1.2
+Version: 2.2.0
 Summary: Comet logger for LLM
 Home-page: https://www.comet.com
 Author: Comet ML Inc.
 Author-email: mail@comet.com
 License: MIT
 Project-URL: Source code, https://github.com/comet-ml/comet-llm
 Keywords: comet_llm
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: comet_ml>=3.35.5
+Requires-Dist: comet_ml>=3.37.1
 Requires-Dist: dataclasses; python_version < "3.7.0"
 Requires-Dist: flatten-dict
 Requires-Dist: requests
 Requires-Dist: types-requests
 
 <p align="center">
     <img alt="cometLLM" src="https://github.com/comet-ml/comet-llm/raw/main/logo.svg">
```

### Comparing `comet_llm-2.1.2/README.md` & `comet_llm-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/setup.py` & `comet_llm-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # *******************************************************
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 requirements = [
-    "comet_ml>=3.35.5",
+    "comet_ml>=3.37.1",
     "dataclasses; python_version<'3.7.0'",
     "flatten-dict",
     "requests",
     "types-requests",
 ]
 project_urls = {"Source code": "https://github.com/comet-ml/comet-llm"}
 this_directory = Path(__file__).parent
@@ -55,11 +55,11 @@
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.com",
     project_urls=project_urls,
-    version="2.1.2",
+    version="2.2.0",
     zip_safe=False,
     license="MIT",
 )
```

### Comparing `comet_llm-2.1.2/src/comet_llm/__init__.py` & `comet_llm-2.2.0/src/comet_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/api.py` & `comet_llm-2.2.0/src/comet_llm/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/api_objects/__init__.py` & `comet_llm-2.2.0/src/comet_llm/api_key/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/api_objects/api.py` & `comet_llm-2.2.0/src/comet_llm/api_objects/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/api_objects/llm_trace_api.py` & `comet_llm-2.2.0/src/comet_llm/api_objects/llm_trace_api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/app.py` & `comet_llm-2.2.0/src/comet_llm/app.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/__init__.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/api.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/openai/__init__.py` & `comet_llm-2.2.0/src/comet_llm/api_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/openai/chat_completion_parsers.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/openai/chat_completion_parsers.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/openai/context.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/openai/context.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/openai/hooks.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/openai/hooks.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/openai/metadata.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/openai/metadata.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/autologgers/openai/patcher.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/openai/patcher.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/backend_error_codes.py` & `comet_llm-2.2.0/src/comet_llm/backend_error_codes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/__init__.py` & `comet_llm-2.2.0/src/comet_llm/autologgers/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/api.py` & `comet_llm-2.2.0/src/comet_llm/chains/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/chain.py` & `comet_llm-2.2.0/src/comet_llm/chains/chain.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/context.py` & `comet_llm-2.2.0/src/comet_llm/chains/context.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/deepmerge.py` & `comet_llm-2.2.0/src/comet_llm/chains/deepmerge.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/span.py` & `comet_llm-2.2.0/src/comet_llm/chains/span.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/state.py` & `comet_llm-2.2.0/src/comet_llm/chains/state.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/thread_context_registry.py` & `comet_llm-2.2.0/src/comet_llm/chains/thread_context_registry.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/chains/version.py` & `comet_llm-2.2.0/src/comet_llm/chains/version.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/constants.py` & `comet_llm-2.2.0/src/comet_llm/constants.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/convert.py` & `comet_llm-2.2.0/src/comet_llm/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/datetimes.py` & `comet_llm-2.2.0/src/comet_llm/datetimes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/dummy_api/__init__.py` & `comet_llm-2.2.0/src/comet_llm/dummy_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/dummy_api/dummy_class.py` & `comet_llm-2.2.0/src/comet_llm/dummy_api/dummy_class.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/exceptions/__init__.py` & `comet_llm-2.2.0/src/comet_llm/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/exceptions/exceptions.py` & `comet_llm-2.2.0/src/comet_llm/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/exceptions/filter_decorator.py` & `comet_llm-2.2.0/src/comet_llm/exceptions/filter_decorator.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/experiment_api/__init__.py` & `comet_llm-2.2.0/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-2.2.0/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-2.2.0/src/comet_llm/experiment_api/experiment_api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/experiment_api/failed_response_handler.py` & `comet_llm-2.2.0/src/comet_llm/experiment_api/failed_response_handler.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-2.2.0/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/experiment_info.py` & `comet_llm-2.2.0/src/comet_llm/experiment_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,31 +18,39 @@
 from . import config, exceptions
 
 DEFAULT_PROJECT_NAME = "llm-general"
 
 
 @dataclasses.dataclass
 class ExperimentInfo:
+    # If you have a better name for this class and module, you are welcome to suggest
     api_key: Optional[str]
     workspace: Optional[str]
     project_name: Optional[str]
 
 
 def get(
     api_key: Optional[str] = None,
     workspace: Optional[str] = None,
     project_name: Optional[str] = None,
     api_key_not_found_message: Optional[str] = None,
 ) -> ExperimentInfo:
+    """
+    Use this function when you work with an API
+    that accepts api_key, project or workspace.
+    """
     api_key = api_key if api_key else config.api_key()
 
     if api_key is None and api_key_not_found_message is not None:
         raise exceptions.CometLLMException(
             api_key_not_found_message, log_message_once=True
         )
 
+    if api_key is not None:
+        config.setup_comet_url(api_key)
+
     workspace = workspace if workspace else config.workspace()
     project_name = project_name if project_name else config.project_name()
 
     project_name = project_name if project_name else DEFAULT_PROJECT_NAME
 
     return ExperimentInfo(api_key, workspace, project_name)
```

### Comparing `comet_llm-2.1.2/src/comet_llm/handlers/__init__.py` & `comet_llm-2.2.0/src/comet_llm/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/__init__.py` & `comet_llm-2.2.0/src/comet_llm/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/callable_extenders.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/callable_extenders.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/callback_runners.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/callback_runners.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/finder.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/finder.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/module_extension.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/module_extension.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/module_loader.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/module_loader.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/patcher.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/patcher.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/registry.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/registry.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/types.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/validate.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/validate.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/import_hooks/wrapper.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/llm_result.py` & `comet_llm-2.2.0/src/comet_llm/llm_result.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/logging.py` & `comet_llm-2.2.0/src/comet_llm/logging.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/logging_messages.py` & `comet_llm-2.2.0/src/comet_llm/logging_messages.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,7 +32,17 @@
 METADATA_KEY_COLLISION_DURING_DEEPMERGE = (
     "Chain or prompt metadata value for the sub-key '%s' was overwritten from '%s' to '%s' during the deep merge",
 )
 
 INVALID_TIMESTAMP = "Invalid timestamp: %s. Timestamp must be in seconds if specified."
 
 GLOBAL_CHAIN_NOT_INITIALIZED = "Global chain is not initialized for this thread. Initialize it with `comet_llm.start_chain(...)` if you wish to use %s"
+
+PARSE_API_KEY_EMPTY_KEY = "Can not parse empty Comet API key"
+
+PARSE_API_KEY_EMPTY_EXPECTED_ATTRIBUTES = (
+    "Expected attributes not found in the Comet API key: %r"
+)
+
+PARSE_API_KEY_TOO_MANY_PARTS = "Too many parts (%d) found in the Comet API key: %r"
+
+BASE_URL_MISMATCH_CONFIG_API_KEY = "Comet URL conflict detected between config (%r) and API Key (%r). SDK will use config URL. Resolve by either removing config URL or set it to the same value."
```

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/__init__.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/api.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/messages.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/messages.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/offline_message_processor.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/offline_message_processor.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/__init__.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/chain.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/chain.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/offline_senders/prompt.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/offline_senders/prompt.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/online_message_processor.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/online_message_processor.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/__init__.py` & `comet_llm-2.2.0/src/comet_llm/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/chain.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/chain.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/message_processing/online_senders/prompt.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/prompt.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/prompts/__init__.py` & `comet_llm-2.2.0/src/comet_llm/message_processing/online_senders/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/prompts/api.py` & `comet_llm-2.2.0/src/comet_llm/prompts/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/prompts/convert.py` & `comet_llm-2.2.0/src/comet_llm/prompts/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/prompts/preprocess.py` & `comet_llm-2.2.0/src/comet_llm/prompts/preprocess.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/query_dsl.py` & `comet_llm-2.2.0/src/comet_llm/query_dsl.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/summary.py` & `comet_llm-2.2.0/src/comet_llm/summary.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm/types.py` & `comet_llm-2.2.0/src/comet_llm/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.1.2/src/comet_llm.egg-info/PKG-INFO` & `comet_llm-2.2.0/src/comet_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 2.1.2
+Version: 2.2.0
 Summary: Comet logger for LLM
 Home-page: https://www.comet.com
 Author: Comet ML Inc.
 Author-email: mail@comet.com
 License: MIT
 Project-URL: Source code, https://github.com/comet-ml/comet-llm
 Keywords: comet_llm
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: comet_ml>=3.35.5
+Requires-Dist: comet_ml>=3.37.1
 Requires-Dist: dataclasses; python_version < "3.7.0"
 Requires-Dist: flatten-dict
 Requires-Dist: requests
 Requires-Dist: types-requests
 
 <p align="center">
     <img alt="cometLLM" src="https://github.com/comet-ml/comet-llm/raw/main/logo.svg">
```

### Comparing `comet_llm-2.1.2/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-2.2.0/src/comet_llm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 README.md
 setup.py
 src/comet_llm/__init__.py
 src/comet_llm/api.py
 src/comet_llm/app.py
 src/comet_llm/backend_error_codes.py
 src/comet_llm/config.py
+src/comet_llm/config_helper.py
 src/comet_llm/constants.py
 src/comet_llm/convert.py
 src/comet_llm/datetimes.py
 src/comet_llm/experiment_info.py
 src/comet_llm/llm_result.py
 src/comet_llm/logging.py
 src/comet_llm/logging_messages.py
 src/comet_llm/query_dsl.py
 src/comet_llm/summary.py
 src/comet_llm/types.py
+src/comet_llm/url_helpers.py
 src/comet_llm.egg-info/PKG-INFO
 src/comet_llm.egg-info/SOURCES.txt
 src/comet_llm.egg-info/dependency_links.txt
 src/comet_llm.egg-info/not-zip-safe
 src/comet_llm.egg-info/requires.txt
 src/comet_llm.egg-info/top_level.txt
+src/comet_llm/api_key/__init__.py
+src/comet_llm/api_key/base64_helper.py
+src/comet_llm/api_key/comet_api_key.py
 src/comet_llm/api_objects/__init__.py
 src/comet_llm/api_objects/api.py
 src/comet_llm/api_objects/llm_trace_api.py
 src/comet_llm/autologgers/__init__.py
 src/comet_llm/autologgers/api.py
 src/comet_llm/autologgers/openai/__init__.py
 src/comet_llm/autologgers/openai/chat_completion_parsers.py
```

