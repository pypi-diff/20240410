# Comparing `tmp/lionagi-0.0.316.tar.gz` & `tmp/lionagi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lionagi-0.0.316.tar", last modified: Sat Mar 30 22:32:44 2024, max compression
+gzip compressed data, was "lionagi-0.1.0.tar", last modified: Wed Apr 10 04:41:42 2024, max compression
```

## Comparing `lionagi-0.0.316.tar` & `lionagi-0.1.0.tar`

### file list

```diff
@@ -1,160 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.114936 lionagi-0.0.316/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-30 22:32:20.000000 lionagi-0.0.316/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-03-30 22:32:44.114936 lionagi-0.0.316/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-03-30 22:32:20.000000 lionagi-0.0.316/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-30 22:32:20.000000 lionagi-0.0.316/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.090935 lionagi-0.0.316/lionagi/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.090935 lionagi-0.0.316/lionagi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.090935 lionagi-0.0.316/lionagi/core/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/agent/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.094936 lionagi-0.0.316/lionagi/core/branch/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.094936 lionagi-0.0.316/lionagi/core/branch/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/base_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/branch_flow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/executable_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/branch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.094936 lionagi-0.0.316/lionagi/core/direct/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/cot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/react.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/direct/vote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.094936 lionagi-0.0.316/lionagi/core/flow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.094936 lionagi-0.0.316/lionagi/core/flow/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/base/baseflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.098935 lionagi-0.0.316/lionagi/core/flow/monoflow/
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/monoflow/ReAct.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/monoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/monoflow/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/monoflow/chat_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/monoflow/followup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.098935 lionagi-0.0.316/lionagi/core/flow/polyflow/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/polyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/flow/polyflow/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.098935 lionagi-0.0.316/lionagi/core/mail/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/mail/mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/mail/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.098935 lionagi-0.0.316/lionagi/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/messages/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.098935 lionagi-0.0.316/lionagi/core/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/prompt/action_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/prompt/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/prompt/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/prompt/scored_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.098935 lionagi-0.0.316/lionagi/core/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/action_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/base_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    15702 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/data_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    32197 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/schema/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/core/session/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37975 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/core/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/tool/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/core/tool/tool_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/integrations/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/integrations/bridge/langchain_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/langchain_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/langchain_/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/langchain_/langchain_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/node_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/textnode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/integrations/bridge/pydantic_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/pydantic_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.102935 lionagi-0.0.316/lionagi/integrations/chunker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/chunker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/chunker/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.106936 lionagi-0.0.316/lionagi/integrations/config/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/config/mlx_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/config/oai_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/config/ollama_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/config/openrouter_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.106936 lionagi-0.0.316/lionagi/integrations/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/loader/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/loader/load_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.106936 lionagi-0.0.316/lionagi/integrations/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/litellm.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/mistralai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/mlx_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/integrations/provider/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.110936 lionagi-0.0.316/lionagi/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34556 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    23520 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/ln_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/libs/sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.110936 lionagi-0.0.316/lionagi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.110936 lionagi-0.0.316/lionagi/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18629 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_base_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_chat_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_session_base_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_core/test_tool_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.110936 lionagi-0.0.316/lionagi/tests/test_integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.110936 lionagi-0.0.316/lionagi/tests/test_libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/tests/test_libs/test_sys_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-30 22:32:20.000000 lionagi-0.0.316/lionagi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 22:32:44.110936 lionagi-0.0.316/lionagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-03-30 22:32:44.000000 lionagi-0.0.316/lionagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-30 22:32:44.000000 lionagi-0.0.316/lionagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 22:32:44.000000 lionagi-0.0.316/lionagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-30 22:32:44.000000 lionagi-0.0.316/lionagi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-30 22:32:44.000000 lionagi-0.0.316/lionagi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-30 22:32:20.000000 lionagi-0.0.316/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 22:32:44.114936 lionagi-0.0.316/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-30 22:32:20.000000 lionagi-0.0.316/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.672225 lionagi-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-10 04:41:26.000000 lionagi-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-10 04:41:42.672225 lionagi-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-10 04:41:26.000000 lionagi-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-10 04:41:26.000000 lionagi-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.648225 lionagi-0.1.0/lionagi/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.648225 lionagi-0.1.0/lionagi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.648225 lionagi-0.1.0/lionagi/core/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/agent/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/branch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/executable_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/flow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/direct/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/cot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/react.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/base_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/branch_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/instruction_map_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/structure_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/baseflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/mono_chat_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/flow/monoflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/ReAct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/chat_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/followup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/flow/polyflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/polyflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/polyflow/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/form/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/action_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/scored_form.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/mail/mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/mail/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/messages/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38110 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/tool/tool_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/langchain_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/node_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/textnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/pydantic_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/pydantic_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/chunker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/chunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/chunker/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.664225 lionagi-0.1.0/lionagi/integrations/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/mlx_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/oai_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/ollama_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/openrouter_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.664225 lionagi-0.1.0/lionagi/integrations/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/loader/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/loader/load_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.664225 lionagi-0.1.0/lionagi/integrations/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/litellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/mistralai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/mlx_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17351 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_base_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_chat_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_session_base_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_tool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-10 04:41:26.000000 lionagi-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 04:41:42.672225 lionagi-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-10 04:41:26.000000 lionagi-0.1.0/setup.py
```

### Comparing `lionagi-0.0.316/LICENSE` & `lionagi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/PKG-INFO` & `lionagi-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionagi
-Version: 0.0.316
+Version: 0.1.0
 Summary: Towards automated general intelligence.
 Author: HaiyangLi
 Author-email: Haiyang Li <ocean@lionagi.ai>
 License: MIT License
         
         Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
```

### Comparing `lionagi-0.0.316/README.md` & `lionagi-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/core/branch/base_branch.py` & `lionagi-0.1.0/lionagi/core/branch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from abc import ABC
 from typing import Any
 
-from lionagi.libs.sys_util import PATH_TYPE
+from pathlib import Path
 from lionagi.libs import convert, dataframe, SysUtil
 
-from ..schema.base_node import BaseRelatableNode
-from ..schema.data_logger import DataLogger, DLog
-from ..messages.schema import (
+from lionagi.core.generic import BaseNode, DataLogger, DLog
+from lionagi.core.messages.schema import (
     BranchColumns,
     System,
     Response,
     Instruction,
     BaseMessage,
 )
-from .util import MessageUtil
+from lionagi.core.branch.util import MessageUtil
 
 
-class BaseBranch(BaseRelatableNode, ABC):
+class BaseBranch(BaseNode, ABC):
     """
     Base class for managing branches of conversation, incorporating messages
     and logging functionality.
 
     Attributes:
             messages (dataframe.ln_DataFrame): Holds the messages in the branch.
             datalogger (DataLogger): Logs data related to the branch's operation.
-            persist_path (PATH_TYPE): Filesystem path for data persistence.
+            persist_path (str | Path): Filesystem path for data persistence.
     """
 
     _columns: list[str] = BranchColumns.COLUMNS.value
 
     def __init__(
         self,
         messages: dataframe.ln_DataFrame | None = None,
         datalogger: DataLogger | None = None,
-        persist_path: PATH_TYPE | None = None,
+        persist_path: str | Path | None = None,
         name=None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         if isinstance(messages, dataframe.ln_DataFrame):
             if MessageUtil.validate_messages(messages):
                 self.messages = messages
@@ -93,14 +92,15 @@
                     _msg.recipient = self.name
                 if recipient is not None and self.name is None:
                     _msg.recipient = recipient
             if "response" in _msg.content.keys():
                 if self.name is not None:
                     _msg.sender = self.name
 
+        setattr(_msg, "node_id", _msg.id_)
         _msg.content = _msg.msg_content
         self.messages.loc[len(self.messages)] = _msg.to_pd_series()
 
     def _to_chatcompletion_message(
         self, with_sender: bool = False
     ) -> list[dict[str, Any]]:
         """
@@ -328,15 +328,15 @@
     def _from_json(cls, filename: str, read_kwargs=None, **kwargs) -> "BaseBranch":
         read_kwargs = {} if read_kwargs is None else read_kwargs
         messages = dataframe.read_json(filename, **read_kwargs)
         return cls(messages=messages, **kwargs)
 
     def to_csv_file(
         self,
-        filename: PATH_TYPE = "messages.csv",
+        filename: str | Path = "messages.csv",
         dir_exist_ok: bool = True,
         timestamp: bool = True,
         time_prefix: bool = False,
         verbose: bool = True,
         clear: bool = True,
         **kwargs,
     ) -> None:
@@ -371,15 +371,15 @@
             if clear:
                 self.clear_messages()
         except Exception as e:
             raise ValueError(f"Error in saving to csv: {e}") from e
 
     def to_json_file(
         self,
-        filename: PATH_TYPE = "messages.json",
+        filename: str | Path = "messages.json",
         dir_exist_ok: bool = True,
         timestamp: bool = True,
         time_prefix: bool = False,
         verbose: bool = True,
         clear: bool = True,
         **kwargs,
     ) -> None:
@@ -416,15 +416,15 @@
             if clear:
                 self.clear_messages()
         except Exception as e:
             raise ValueError(f"Error in saving to json: {e}") from e
 
     def log_to_csv(
         self,
-        filename: PATH_TYPE = "log.csv",
+        filename: str | Path = "log.csv",
         dir_exist_ok: bool = True,
         timestamp: bool = True,
         time_prefix: bool = False,
         verbose: bool = True,
         clear: bool = True,
         flatten_=True,
         sep="[^_^]",
@@ -452,15 +452,15 @@
             flatten_=flatten_,
             sep=sep,
             **kwargs,
         )
 
     def log_to_json(
         self,
-        filename: PATH_TYPE = "log.json",
+        filename: str | Path = "log.json",
         dir_exist_ok: bool = True,
         timestamp: bool = True,
         time_prefix: bool = False,
         verbose: bool = True,
         clear: bool = True,
         flatten_=True,
         sep="[^_^]",
@@ -632,23 +632,22 @@
             sender=sender,
             start_time=start_time,
             end_time=end_time,
             content_keywords=content_keywords,
             case_sensitive=case_sensitive,
         )
 
-    # noinspection PyTestUnpassedFixture
     def _info(self, use_sender: bool = False) -> dict[str, int]:
         """
         Helper method to generate summaries of messages either by role or sender.
 
         Args:
                 use_sender: If True, summary is categorized by sender. Otherwise, by role.
 
         Returns:
                 A dictionary summarizing the count of messages either by role or sender.
         """
 
         messages = self.messages["sender"] if use_sender else self.messages["role"]
         result = messages.value_counts().to_dict()
         result["total"] = len(self.messages)
-        return result
+        return result
```

### Comparing `lionagi-0.0.316/lionagi/core/branch/branch.py` & `lionagi-0.1.0/lionagi/core/branch/branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 This module contains the Branch class, which represents a branch in a conversation tree.
 """
 
 from collections import deque
 from typing import Any, Union, TypeVar, Callable
+from pathlib import Path
 
-from lionagi.libs.sys_util import PATH_TYPE
 from lionagi.libs import StatusTracker, BaseService, convert, dataframe
 
-from ..schema import TOOL_TYPE, Tool, DataLogger
-from ..tool import ToolManager, func_to_tool
-
-from ..messages import System
-from ..mail import BaseMail
-
-from .util import MessageUtil
-from .base_branch import BaseBranch
-from .branch_flow_mixin import BranchFlowMixin
+from lionagi.core.generic import DataLogger
+from lionagi.core.tool import ToolManager, func_to_tool, Tool, TOOL_TYPE
+from lionagi.core.messages.schema import System
+from lionagi.core.mail.schema import BaseMail
+
+from lionagi.core.branch.util import MessageUtil
+from lionagi.core.branch.base import BaseBranch
+from lionagi.core.branch.flow_mixin import BranchFlowMixin
 
 from dotenv import load_dotenv
 
 load_dotenv()
 
 T = TypeVar("T", bound=Tool)
 
@@ -91,15 +90,15 @@
         system: dict | list | System | None = None,
         messages: dataframe.ln_DataFrame | None = None,
         service: BaseService | None = None,
         sender: str | None = None,
         llmconfig: dict[str, str | int | dict] | None = None,
         tools: list[Callable | Tool] | None = None,
         datalogger: None | DataLogger = None,
-        persist_path: PATH_TYPE | None = None,  # instruction_sets=None,
+        persist_path: str | Path | None = None,  # instruction_sets=None,
         tool_manager: ToolManager | None = None,
         **kwargs,
     ):
         """
         Initializes the Branch instance.
 
         Args:
@@ -107,15 +106,15 @@
             system (dict | list | System): The system message for the branch (optional).
             messages (dataframe.ln_DataFrame): The messages in the branch (optional).
             service (BaseService): The service associated with the branch (optional).
             sender (str): The sender of the branch (optional, default: "system").
             llmconfig (dict[str, str | int | dict]): The configuration for the language model (optional).
             tools (list[Callable | Tool]): The tools to register in the branch (optional).
             datalogger (DataLogger): The data logger for the branch (optional).
-            persist_path (PATH_TYPE): The path to persist the branch data (optional).
+            persist_path (str | Path): The path to persist the branch data (optional).
             tool_manager (ToolManager): The tool manager for the branch (optional).
             **kwargs: Additional keyword arguments.
 
         Raises:
             TypeError: If there is an error in registering the tools.
         """
 
@@ -161,30 +160,30 @@
         cls,
         filepath,
         name: str | None = None,
         service: BaseService | None = None,
         llmconfig: dict[str, str | int | dict] | None = None,
         tools: TOOL_TYPE | None = None,
         datalogger: None | DataLogger = None,
-        persist_path: PATH_TYPE | None = None,  # instruction_sets=None,
+        persist_path: str | Path | None = None,  # instruction_sets=None,
         tool_manager: ToolManager | None = None,
         read_kwargs=None,
         **kwargs,
     ) -> "Branch":
         """
         Creates a Branch instance from a CSV file.
 
         Args:
             filepath: The path to the CSV file.
             name (str): The name of the branch (optional).
             service (BaseService): The service associated with the branch (optional).
             llmconfig (dict[str, str | int | dict]): The configuration for the language model (optional).
             tools (TOOL_TYPE): The tools to register in the branch (optional).
             datalogger (DataLogger): The data logger for the branch (optional).
-            persist_path (PATH_TYPE): The path to persist the branch data (optional).
+            persist_path (str | Path): The path to persist the branch data (optional).
             tool_manager (ToolManager): The tool manager for the branch (optional).
             read_kwargs: Additional keyword arguments for reading the CSV file (optional).
             **kwargs: Additional keyword arguments.
 
         Returns:
             Branch: The created Branch instance.
         """
@@ -207,30 +206,30 @@
         cls,
         filepath,
         name: str | None = None,
         service: BaseService | None = None,
         llmconfig: dict[str, str | int | dict] | None = None,
         tools: TOOL_TYPE | None = None,
         datalogger: None | DataLogger = None,
-        persist_path: PATH_TYPE | None = None,  # instruction_sets=None,
+        persist_path: str | Path | None = None,  # instruction_sets=None,
         tool_manager: ToolManager | None = None,
         read_kwargs=None,
         **kwargs,
     ) -> "Branch":
         """
         Creates a Branch instance from a JSON string file.
 
         Args:
             filepath: The path to the JSON string file.
             name (str): The name of the branch (optional).
             service (BaseService): The service associated with the branch (optional).
             llmconfig (dict[str, str | int | dict]): The configuration for the language model (optional).
             tools (TOOL_TYPE): The tools to register in the branch (optional).
             datalogger (DataLogger): The data logger for the branch (optional).
-            persist_path (PATH_TYPE): The path to persist the branch data (optional).
+            persist_path (str | Path): The path to persist the branch data (optional).
             tool_manager (ToolManager): The tool manager for the branch (optional).
             read_kwargs: Additional keyword arguments for reading the JSON string file (optional).
             **kwargs: Additional keyword arguments.
 
         Returns:
             Branch: The created Branch instance.
         """
@@ -344,27 +343,30 @@
             if verbose:
                 print("tools successfully deleted")
             return True
         if verbose:
             print("tools deletion failed")
         return False
 
-    def send(self, recipient: str, category: str, package: Any) -> None:
+    def send(self, recipient_id: str, category: str, package: Any) -> None:
         """
         Sends a mail to a recipient.
 
         Args:
             recipient (str): The recipient of the mail.
             category (str): The category of the mail.
             package (Any): The package to send in the mail.
         """
-        mail_ = BaseMail(
-            sender=self.sender, recipient=recipient, category=category, package=package
+        mail = BaseMail(
+            sender_id=self.id_,
+            recipient_id=recipient_id,
+            category=category,
+            package=package,
         )
-        self.pending_outs.append(mail_)
+        self.pending_outs.append(mail)
 
     def receive(
         self,
         sender: str,
         messages: bool = True,
         tools: bool = True,
         service: bool = True,
@@ -464,8 +466,8 @@
             if convert.to_dict(content)["action_response"].keys() >= {
                 "function",
                 "arguments",
                 "output",
             }:
                 return True
         except Exception:
-            return False
+            return False
```

### Comparing `lionagi-0.0.316/lionagi/core/branch/branch_flow_mixin.py` & `lionagi-0.1.0/lionagi/core/branch/flow_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 from typing import Any, Optional, Union, TypeVar
 
-from ..schema import TOOL_TYPE, Tool
-from ..messages import Instruction, System
-from ..flow.monoflow import MonoChat, MonoFollowup, MonoReAct
+from lionagi.core.tool import Tool, TOOL_TYPE
+from lionagi.core.messages.schema import Instruction, System
+from lionagi.core.flow.monoflow import MonoChat, MonoFollowup, MonoReAct
 
 T = TypeVar("T", bound=Tool)
 
 
 class BranchFlowMixin(ABC):
 
     async def chat(
@@ -16,28 +16,28 @@
         context: Optional[Any] = None,
         sender: Optional[str] = None,
         system: Optional[Union[System, str, dict[str, Any]]] = None,
         tools: TOOL_TYPE = False,
         out: bool = True,
         invoke: bool = True,
         output_fields=None,
-        prompt_template=None,
+        form=None,
         **kwargs,
     ) -> Any:
         flow = MonoChat(self)
         return await flow.chat(
             instruction=instruction,
             context=context,
             sender=sender,
             system=system,
             tools=tools,
             out=out,
             invoke=invoke,
             output_fields=output_fields,
-            prompt_template=prompt_template,
+            form=form,
             **kwargs,
         )
 
     async def ReAct(
         self,
         instruction: Instruction | str | dict[str, dict | str],
         context=None,
@@ -89,8 +89,8 @@
             tools=tools,
             max_followup=max_followup,
             auto=auto,
             followup_prompt=followup_prompt,
             output_prompt=output_prompt,
             out=out,
             **kwargs,
-        )
+        )
```

### Comparing `lionagi-0.0.316/lionagi/core/branch/util.py` & `lionagi-0.1.0/lionagi/core/branch/util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -316,8 +316,8 @@
                         answers.append(nested.nget(content, ["assistant_response"]))
             elif i.role == "user":
                 with contextlib.suppress(Exception):
                     answers.append(nested.nget(content, ["instruction"]))
             else:
                 with contextlib.suppress(Exception):
                     answers.append(nested.nget(content, ["system_info"]))
-        return "\n".join(answers)
+        return "\n".join(answers)
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/plan.py` & `lionagi-0.1.0/lionagi/core/direct/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # plan.py
 
 from lionagi.libs import func_call, ParseUtil
 from lionagi.integrations.bridge.pydantic_.pydantic_bridge import Field
-from ..prompt.scored_template import ScoredTemplate
-from ..branch import Branch
+from lionagi.core.form.scored_form import ScoredForm
+from lionagi.core.branch.branch import Branch
 
 
-class PlanTemplate(ScoredTemplate):
+class PlanTemplate(ScoredForm):
     template_name: str = "default_plan"
     sentence: str | list | dict = Field(
         default_factory=str,
         description="the given sentence(s) or context to generate a plan for",
     )
-    plan: dict | str= Field(
-        default_factory=dict, description="the generated step by step plan, return as a dictionary following {step_n: {plan: ..., reason: ...}} format")
+    plan: dict | str = Field(
+        default_factory=dict,
+        description="the generated step by step plan, return as a dictionary following {step_n: {plan: ..., reason: ...}} format",
+    )
     signature: str = "sentence -> plan"
 
     def __init__(
         self,
         sentence=None,
         instruction=None,
         confidence_score=False,
@@ -85,23 +87,23 @@
         instruction=instruction,
         confidence_score=confidence_score,
         reason=reason,
     )
 
     await func_call.rcall(
         branch.chat,
-        prompt_template=_template,
+        form=_template,
         retries=retries,
         delay=delay,
         backoff_factor=backoff_factor,
         default=default_value,
         timeout=timeout,
         **kwargs,
     )
-    
+
     _template.plan = ParseUtil.fuzzy_parse_json(_template.plan)
 
     return (_template, branch) if return_branch else _template
 
 
 async def plan(
     sentence,
@@ -155,8 +157,8 @@
             **kwargs,
         )
 
     if num_instances == 1:
         return await _inner()
 
     elif num_instances > 1:
-        return await func_call.alcall(range(num_instances), _inner)
+        return await func_call.alcall(range(num_instances), _inner)
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/predict.py` & `lionagi-0.1.0/lionagi/core/direct/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 using a language model. It includes fields for the input sentence, number of sentences to predict, predicted answer,
 confidence score, and reason for the prediction.
 """
 
 from lionagi.libs import func_call
 from lionagi.integrations.bridge.pydantic_.pydantic_bridge import Field
 
-from ..prompt.scored_template import ScoredTemplate
-from ..branch import Branch
+from lionagi.core.form.scored_form import ScoredForm
+from lionagi.core.branch.branch import Branch
 
 
-class PredictTemplate(ScoredTemplate):
+class PredictTemplate(ScoredForm):
     """
     A class for predicting the next sentence(s) based on a given sentence.
 
     Attributes:
         template_name (str): The name of the predict template (default: "default_predict_template").
         sentence (str | list | dict): The given sentence(s) to predict.
         num_sentences (int): The number of sentences to predict.
@@ -64,15 +64,15 @@
             num_sentences (Optional[int]): The number of sentences to predict.
             confidence_score (bool): Whether to include the confidence score in the output (default: False).
             reason (bool): Whether to include the reason for the prediction in the output (default: False).
             **kwargs: Additional keyword arguments.
         """
         super().__init__(**kwargs)
 
-        self.sentence = sentence or ''
+        self.sentence = sentence or ""
         self.num_sentences = num_sentences
         self.task = f"follow instruction to predict the next {self.num_sentences} sentence(s). Instruction: {instruction}."
 
         if reason:
             self.output_fields.append("reason")
 
         if confidence_score:
@@ -150,15 +150,15 @@
         num_sentences=num_sentences,
         confidence_score=confidence_score,
         reason=reason,
     )
 
     await func_call.rcall(
         branch.chat,
-        prompt_template=predict_template,
+        form=predict_template,
         retries=retries,
         delay=delay,
         backoff_factor=backoff_factor,
         default=default_value,
         timeout=timeout,
         **kwargs,
     )
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/react.py` & `lionagi-0.1.0/lionagi/core/direct/react.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from lionagi.libs import func_call, convert, AsyncUtil
+from lionagi.libs import func_call, AsyncUtil
 
 from lionagi.integrations.bridge.pydantic_.pydantic_bridge import Field
-from ..prompt.action_template import ActionedTemplate
-from ..branch import Branch
-from .utils import _process_tools
+from lionagi.core.form.action_form import ActionForm
+from lionagi.core.branch.branch import Branch
+from lionagi.core.direct.utils import _process_tools
 
 
-class ReactTemplate(ActionedTemplate):
+class ReactTemplate(ActionForm):
     template_name: str = "default_react"
-    sentence: str | list | dict | None= Field(
+    sentence: str | list | dict | None = Field(
         default_factory=str,
         description="the given sentence(s) to reason and take actions on",
     )
 
     def __init__(
         self,
         sentence=None,
@@ -57,15 +57,15 @@
     if "temperature" not in kwargs:
         kwargs["temperature"] = 0.1
 
     instruction = instruction or ""
 
     if branch and tools:
         _process_tools(tools, branch)
-        
+
     branch = branch or Branch(
         name=branch_name,
         system=system,
         messages=messages,
         service=service,
         sender=sender,
         llmconfig=llmconfig,
@@ -79,15 +79,15 @@
         sentence=sentence,
         instruction=instruction,
         confidence_score=confidence_score,
     )
 
     await func_call.rcall(
         branch.chat,
-        prompt_template=_template,
+        form=_template,
         retries=retries,
         delay=delay,
         backoff_factor=backoff_factor,
         default=default_value,
         timeout=timeout,
         **kwargs,
     )
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/score.py` & `lionagi-0.1.0/lionagi/core/direct/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 The module also includes functions for scoring a single instance or multiple instances of the context using the
 ScoreTemplate class and a language model.
 """
 
 from pydantic import Field
 import numpy as np
 from lionagi.libs import func_call, convert
-from ..prompt.scored_template import ScoredTemplate
-from ..branch import Branch
+from lionagi.core.form.scored_form import ScoredForm
+from lionagi.core.branch.branch import Branch
 
 
-class ScoreTemplate(ScoredTemplate):
+class ScoreTemplate(ScoredForm):
     """
     A class for scoring a given context using a language model.
 
     Attributes:
         template_name (str): The name of the score template (default: "default_score").
         sentence (str | list | dict): The given context to score.
         answer (float): The numeric score for the context.
@@ -165,15 +165,15 @@
         num_digit=num_digit,
         confidence_score=confidence_score,
         reason=reason,
     )
 
     await func_call.rcall(
         branch.chat,
-        prompt_template=_template,
+        form=_template,
         retries=retries,
         delay=delay,
         backoff_factor=backoff_factor,
         default=default_value,
         timeout=timeout,
         **kwargs,
     )
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/select.py` & `lionagi-0.1.0/lionagi/core/direct/select.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 and a language model.
 """
 
 from enum import Enum
 from pydantic import Field
 
 from lionagi.libs import func_call, StringMatch
-from ..prompt.scored_template import ScoredTemplate
-from ..branch import Branch
+from lionagi.core.form.scored_form import ScoredForm
+from lionagi.core.branch.branch import Branch
 
 
-class SelectTemplate(ScoredTemplate):
+class SelectTemplate(ScoredForm):
     """
     A class for selecting an item from given choices based on a given context.
 
     Attributes:
         template_name (str): The name of the select template (default: "default_select").
         sentence (str | list | dict): The given context.
         answer (Enum | str): The selected item from the given choices.
@@ -149,15 +149,15 @@
         instruction=instruction,
         confidence_score=confidence_score,
         reason=reason,
     )
 
     await func_call.rcall(
         branch.chat,
-        prompt_template=_template,
+        form=_template,
         retries=retries,
         delay=delay,
         backoff_factor=backoff_factor,
         default=default_value,
         timeout=timeout,
         **kwargs,
     )
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/utils.py` & `lionagi-0.1.0/lionagi/core/direct/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable
-from ..tool import func_to_tool
-from ..schema import Tool
+from lionagi.core.tool import func_to_tool, Tool
+
 # import contextlib
 # from lionagi.libs import ParseUtil, StringMatch, convert, func_call
 
 
 # def _parse_out(out_):
 #     if isinstance(out_, str):
 #         try:
@@ -95,13 +95,16 @@
         _process_tool(tool_obj, branch)
     else:
         for i in tool_obj:
             _process_tool(i, branch)
 
 
 def _process_tool(tool_obj, branch):
-    if isinstance(tool_obj, Tool) and tool_obj.schema_["function"]["name"] not in branch.tool_manager.registry:
+    if (
+        isinstance(tool_obj, Tool)
+        and tool_obj.schema_["function"]["name"] not in branch.tool_manager.registry
+    ):
         branch.register_tools(tool_obj)
     if isinstance(tool_obj, Callable):
         tool = func_to_tool(tool_obj)[0]
         if tool.schema_["function"]["name"] not in branch.tool_manager.registry:
-            branch.register_tools(tool)
+            branch.register_tools(tool)
```

### Comparing `lionagi-0.0.316/lionagi/core/direct/vote.py` & `lionagi-0.1.0/lionagi/core/direct/vote.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 The vote function generates multiple outputs using a specified directive function (default: predict), scores each output
 using the score function, and returns the top-ranked output(s) based on the scores. It allows for customization of the
 number of generations, number of outputs to return, number of scorers, score range, and scorer instruction.
 """
 
 from lionagi.libs import func_call
 import numpy as np
-from .predict import predict
-from .score import score
+from lionagi.core.direct.predict import predict
+from lionagi.core.direct.score import score
 
 
 async def vote(
     sentence,
     directive=predict,
     num_generations=5,
     num_output=1,
```

### Comparing `lionagi-0.0.316/lionagi/core/flow/monoflow/ReAct.py` & `lionagi-0.1.0/lionagi/core/flow/monoflow/ReAct.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 This module contains the MonoReAct class for performing reasoning and action tasks with an LLM.
 
 The MonoReAct class allows for conducting a series of reasoning and action steps with an LLM, with the ability to
 process instructions, system messages, and invoke tools during the conversation. It extends the MonoChat class.
 """
 
 from typing import Callable
-from .chat import MonoChat
-from lionagi.core.schema import Tool
-from lionagi.core.messages import Instruction
+from lionagi.core.flow.monoflow.chat import MonoChat
+from lionagi.core.tool import Tool
+from lionagi.core.messages.schema import Instruction
 
 
 class MonoReAct(MonoChat):
     """
     A class for performing reasoning and action tasks with an LLM, processing instructions and system messages,
     and optionally invoking tools.
 
@@ -231,8 +231,8 @@
 
             _prompt = self._get_prompt(
                 prompt=output_prompt,
                 default=self.OUTPUT_PROMPT,
                 instruction=instruction,
             )
             _out = await self.chat(_prompt, sender=sender, **kwargs)
-            return _out if out else None
+            return _out if out else None
```

### Comparing `lionagi-0.0.316/lionagi/core/flow/monoflow/chat.py` & `lionagi-0.1.0/lionagi/core/flow/monoflow/chat.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The MonoChat class allows for processing instructions and system messages, and optionally invoking tools
 during the chat conversation. It extends the BaseMonoFlow and MonoChatMixin classes.
 """
 
 from typing import Any
 
-from lionagi.core.flow.base.baseflow import BaseMonoFlow
+from lionagi.core.flow.baseflow import BaseMonoFlow
 from lionagi.core.flow.monoflow.chat_mixin import MonoChatMixin
 
 
 class MonoChat(BaseMonoFlow, MonoChatMixin):
     """
     A class for performing a chat conversation with an LLM, processing instructions and system messages,
     and optionally invoking tools.
@@ -20,15 +20,15 @@
         branch: The Branch instance to perform chat operations.
 
     Methods:
         __init__(self, branch) -> None:
             Initializes the MonoChat instance.
 
         async chat(self, instruction=None, context=None, sender=None, system=None, tools=False,
-                   out=True, invoke=True, output_fields=None, prompt_template=None, **kwargs) -> Any:
+                   out=True, invoke=True, output_fields=None, form=None, **kwargs) -> Any:
             Performs a chat conversation with an LLM, processing instructions and system messages,
             and optionally invoking tools.
     """
 
     def __init__(self, branch) -> None:
         """
         Initializes the MonoChat instance.
@@ -44,15 +44,15 @@
         context=None,
         sender=None,
         system=None,
         tools=False,
         out: bool = True,
         invoke: bool = True,
         output_fields=None,
-        prompt_template=None,
+        form=None,
         **kwargs,
     ) -> Any:
         """
         Performs a chat conversation with an LLM, processing instructions and system messages,
         and optionally invoking tools.
 
         Args:
@@ -60,36 +60,36 @@
             context (Optional[Any]): Additional context for the chat.
             sender (Optional[str]): The sender of the chat message.
             system (Optional[Union[System, str, Dict[str, Any]]]): System message to be processed.
             tools (Union[bool, Tool, List[Tool], str, List[str]]): Specifies tools to be invoked.
             out (bool): If True, outputs the chat response.
             invoke (bool): If True, invokes tools as part of the chat.
             output_fields (Optional[Any]): The output fields for the chat.
-            prompt_template (Optional[Any]): The prompt template for the chat.
+            form (Optional[Any]): The prompt template for the chat.
             **kwargs: Arbitrary keyword arguments for chat completion.
 
         Returns:
             Any: The result of the chat conversation.
 
         Examples:
             >>> await MonoChat.chat(branch, "Ask about user preferences")
         """
 
         config = self._create_chat_config(
             instruction=instruction,
             context=context,
             sender=sender,
             system=system,
-            prompt_template=prompt_template,
+            form=form,
             tools=tools,
             output_fields=output_fields,
             **kwargs,
         )
 
         await self._call_chatcompletion(**config)
 
         return await self._output(
             invoke=invoke,
             out=out,
             output_fields=output_fields,
-            prompt_template=prompt_template,
+            form=form,
         )
```

### Comparing `lionagi-0.0.316/lionagi/core/flow/monoflow/chat_mixin.py` & `lionagi-0.1.0/lionagi/core/flow/monoflow/chat_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 """
 This module contains mixins for configuring and invoking chatbots.
 """
 
 from abc import ABC
 from typing import Any
 
+import re
+from lionagi.libs import nested, func_call, convert, StringMatch, ParseUtil
+from lionagi.core.tool.tool import TOOL_TYPE
 from lionagi.core.messages.schema import Instruction
-from lionagi.core.schema.base_node import TOOL_TYPE
-from lionagi.libs import (
-    ln_nested as nested,
-    ln_func_call as func_call,
-    ln_convert as convert,
-)
-from lionagi.libs.ln_parse import ParseUtil, StringMatch
 
 
 class MonoChatConfigMixin(ABC):
     """
     Mixin class for configuring chatbots.
 
     Methods:
         _create_chat_config(self, instruction=None, context=None, sender=None, system=None,
-                            output_fields=None, prompt_template=None, tools=False, **kwargs) -> Any:
-            Creates a chat configuration based on the provided parameters.
+        output_fields=None, form=None, tools=False, **kwargs) -> Any:
+        Creates a chat configuration based on the provided parameters.
     """
 
     def _create_chat_config(
         self,
         instruction: Instruction | str | dict[str, Any] = None,
         context: Any | None = None,
         sender: str | None = None,
         system: str | dict[str, Any] | None = None,
         output_fields=None,
-        prompt_template=None,
+        form=None,
         tools: TOOL_TYPE = False,
         **kwargs,
     ) -> Any:
         """
         Creates a chat configuration based on the provided parameters.
 
         Args:
             instruction (Instruction | str | dict[str, Any]): The instruction for the chatbot (optional).
             context (Any): The context for the chatbot (optional).
             sender (str): The sender of the message (optional).
             system (str | dict[str, Any]): The system message for the chatbot (optional).
             output_fields: The output fields for the chatbot (optional).
-            prompt_template: The prompt template for the chatbot (optional).
+            form: The prompt template for the chatbot (optional).
             tools (TOOL_TYPE): The tools for the chatbot (default: False).
             **kwargs: Additional keyword arguments for the chat configuration.
 
         Returns:
             Any: The chat configuration.
         """
         if system:
             self.branch.change_first_system_message(system)
 
-        if not prompt_template:
+        if not form:
             self.branch.add_message(
                 instruction=instruction,
                 context=context,
                 sender=sender,
                 output_fields=output_fields,
             )
         else:
-            instruct_ = Instruction.from_prompt_template(prompt_template)
+            instruct_ = Instruction.from_form(form)
             self.branch.add_message(instruction=instruct_)
 
         if "tool_parsed" in kwargs:
             kwargs.pop("tool_parsed")
             tool_kwarg = {"tools": tools}
             kwargs = tool_kwarg | kwargs
         elif tools and self.branch.has_tools:
@@ -81,16 +77,16 @@
 
 
 class MonoChatInvokeMixin(ABC):
     """
     Mixin class for invoking chatbots.
 
     Methods:
-        async _output(self, invoke, out, output_fields, func_calls_=None, prompt_template=None,
-                      return_template=True):
+        async _output(self, invoke, out, output_fields, func_calls_=None, form=None,
+                    return_template=True):
             Processes the output of the chatbot.
 
         _return_response(content_, output_fields) -> Any:
             Returns the response from the chatbot.
 
         async _invoke_tools(self, content_=None, func_calls_=None):
             Invokes the tools associated with the chatbot.
@@ -104,41 +100,42 @@
 
     async def _output(
         self,
         invoke,
         out,
         output_fields,
         func_calls_=None,
-        prompt_template=None,
+        form=None,
         return_template=True,
     ):
         """
         Processes the output of the chatbot.
 
         Args:
             invoke: Flag indicating whether to invoke the tools.
             out: Flag indicating whether to return the output.
             output_fields: The output fields for the chatbot.
             func_calls_: The function calls for invoking the tools (optional).
-            prompt_template: The prompt template for the chatbot (optional).
+            form: The prompt template for the chatbot (optional).
             return_template (bool): Flag indicating whether to return the prompt template (default: True).
         """
 
         content_ = self.branch.last_message_content
 
         if invoke:
             try:
                 await self._invoke_tools(content_, func_calls_=func_calls_)
             except Exception:
                 pass
 
         response_ = self._return_response(content_, output_fields)
-        if prompt_template:
-            prompt_template._process_response(response_)
-            return prompt_template if return_template else prompt_template.out
+
+        if form:
+            form._process_response(response_)
+            return form if return_template else form.outputs
 
         if out:
             return response_
 
     @staticmethod
     def _return_response(content_, output_fields):
         """
@@ -155,32 +152,25 @@
 
         if len(content_.items()) == 1 and len(nested.get_flattened_keys(content_)) == 1:
             key = nested.get_flattened_keys(content_)[0]
             out_ = content_[key]
 
         if output_fields:
             try:
-                if isinstance(out_, dict):
-                    out_ = convert.to_str(out_.values())
-
-                if isinstance(out_, str):
-                    try:
-                        out_ = ParseUtil.md_to_json(out_)
-                    except Exception:
-                        out_ = ParseUtil.md_to_json(out_.replace("'", '"'))
-
-                out_ = StringMatch.correct_keys(output_fields=output_fields, out_=out_)
+                return StringMatch.force_validate_dict(
+                    out_, keys=list(output_fields.keys())
+                )
             except Exception:
                 pass
 
         if isinstance(out_, str):
             try:
-                out_ = ParseUtil.md_to_json(out_)
-                out_ = StringMatch.correct_keys(output_fields=output_fields, out_=out_)
-                return out_
+                match = re.search(r"```json\n({.*?})\n```", out_, re.DOTALL)
+                if match:
+                    out_ = ParseUtil.fuzzy_parse_json(match.group(1))
             except Exception:
                 pass
 
         return out_
 
     async def _invoke_tools(self, content_=None, func_calls_=None):
         """
@@ -256,8 +246,8 @@
 
 
 class MonoChatMixin(MonoChatConfigMixin, MonoChatInvokeMixin, ABC):
     """
     Mixin class that combines MonoChatConfigMixin and MonoChatInvokeMixin.
     """
 
-    pass
+    pass
```

### Comparing `lionagi-0.0.316/lionagi/core/flow/monoflow/followup.py` & `lionagi-0.1.0/lionagi/core/flow/monoflow/followup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 This module contains the MonoFollowup class for performing followup chats with an LLM.
 
 The MonoFollowup class allows for conducting a series of followup chats with an LLM, with the ability to
 process instructions, system messages, and invoke tools during the conversation. It extends the MonoChat class.
 """
 
 from typing import Callable
-from lionagi.core.messages import Instruction
-from lionagi.core.schema import Tool
-from .chat import MonoChat
+from lionagi.core.messages.schema import Instruction
+from lionagi.core.tool.tool import Tool
+from lionagi.core.flow.monoflow.chat import MonoChat
 
 
 class MonoFollowup(MonoChat):
     """
     A class for performing followup chats with an LLM, processing instructions and system messages,
     and optionally invoking tools.
 
@@ -207,8 +207,8 @@
 
             _prompt = self._get_prompt(
                 prompt=output_prompt,
                 default=self.OUTPUT_PROMPT,
                 instruction=instruction,
             )
             _out = await self.chat(_prompt, sender=sender, **kwargs)
-            return _out if out else None
+            return _out if out else None
```

### Comparing `lionagi-0.0.316/lionagi/core/flow/polyflow/chat.py` & `lionagi-0.1.0/lionagi/core/flow/polyflow/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 The PolyChat class allows for conducting parallel chat conversations with multiple branches, each processing
 instructions and context independently. It provides methods for parallel chat execution and manages the
 created branches within the session.
 """
 
 from typing import Any
 
-from lionagi.libs import ln_convert as convert
-from lionagi.libs.ln_async import AsyncUtil
-
+from lionagi.libs import convert, AsyncUtil
 from lionagi.core.messages.schema import Instruction
 from lionagi.core.branch.branch import Branch
-
-from lionagi.core.flow.base.baseflow import BasePolyFlow
+from lionagi.core.flow.baseflow import BasePolyFlow
 
 
 class PolyChat(BasePolyFlow):
     """
     A class for performing parallel chat conversations with multiple branches.
 
     Methods:
-        __init__(self, session) -> None:
+        __init__(self, session: Any) -> None:
             Initializes the PolyChat instance.
 
-        async parallel_chat(self, instruction, num_instances=1, context=None, sender=None, branch_system=None,
-                             messages=None, tools=False, out=True, invoke=True, output_fields=None,
-                             persist_path=None, branch_config=None, explode=False, **kwargs) -> Any:
+        async parallel_chat(self, instruction: Union[Instruction, str], num_instances: int = 1,
+                             context: Optional[Any] = None, sender: Optional[str] = None,
+                             branch_system: Optional[Any] = None, messages: Optional[Any] = None,
+                             tools: bool = False, out: bool = True, invoke: bool = True,
+                             output_fields: Optional[Any] = None, persist_path: Optional[str] = None,
+                             branch_config: Optional[dict] = None, explode: bool = False, **kwargs) -> Any:
             Performs parallel chat conversations with multiple branches.
 
-        async _parallel_chat(self, instruction, num_instances=1, context=None, sender=None, messages=None,
-                              tools=False, out=True, invoke=True, output_fields=None, persist_path=None,
-                              branch_config={}, explode=False, include_mapping=True, default_key="response",
+        async _parallel_chat(self, instruction: Union[Instruction, str], num_instances: int = 1,
+                              context: Optional[Any] = None, sender: Optional[str] = None,
+                              messages: Optional[Any] = None, tools: bool = False, out: bool = True,
+                              invoke: bool = True, output_fields: Optional[Any] = None,
+                              persist_path: Optional[str] = None, branch_config: dict = {},
+                              explode: bool = False, include_mapping: bool = True, default_key: str = "response",
                               **kwargs) -> Any:
             Internal method for performing parallel chat conversations with multiple branches.
     """
 
     def __init__(self, session) -> None:
         """
         Initializes the PolyChat instance.
```

### Comparing `lionagi-0.0.316/lionagi/core/mail/mail_manager.py` & `lionagi-0.1.0/lionagi/core/mail/mail_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import deque
 from lionagi.libs import AsyncUtil
-from ..schema import BaseNode
-from .schema import BaseMail
+from lionagi.core.generic import Node
+from lionagi.core.mail.schema import BaseMail, MailCategory
 
 
 class MailManager:
     """
     Manages the sending, receiving, and storage of mail items between various sources.
 
     This class acts as a central hub for managing mail transactions within a system. It allows for the addition
@@ -30,26 +30,28 @@
                     self.sources[v.id_] = v
                     self.mails[v.id_] = {}
         elif isinstance(sources, list):
             for v in sources:
                 if v.id_ not in self.sources:
                     self.sources[v.id_] = v
                     self.mails[v.id_] = {}
+        else:
+            raise ValueError("Failed to add source, please input list or dict.")
 
     @staticmethod
     def create_mail(sender_id, recipient_id, category, package):
         return BaseMail(sender_id, recipient_id, category, package)
 
-    def add_source(self, sources: list[BaseNode]):
-        for source in sources:
-            if source.id_ in self.sources:
-                # raise ValueError(f"Source {source.id_} exists, please input a different name.")
-                continue
-            self.sources[source.id_] = source
-            self.mails[source.id_] = {}
+    # def add_source(self, sources: list[Node]):
+    #     for source in sources:
+    #         if source.id_ in self.sources:
+    #             # raise ValueError(f"Source {source.id_} exists, please input a different name.")
+    #             continue
+    #         self.sources[source.id_] = source
+    #         self.mails[source.id_] = {}
 
     def delete_source(self, source_id):
         if source_id not in self.sources:
             raise ValueError(f"Source {source_id} does not exist.")
         # if self.mails[source_id]:
         #     raise ValueError(f"None empty pending mails in source {source_id}")
         self.sources.pop(source_id)
@@ -61,15 +63,15 @@
         while self.sources[sender_id].pending_outs:
             mail_ = self.sources[sender_id].pending_outs.popleft()
             if mail_.recipient_id not in self.sources:
                 raise ValueError(
                     f"Recipient source {mail_.recipient_id} does not exist"
                 )
             if mail_.sender_id not in self.mails[mail_.recipient_id]:
-                self.mails[mail_.recipient_id] = {mail_.sender_id: deque()}
+                self.mails[mail_.recipient_id].update({mail_.sender_id: deque()})
             self.mails[mail_.recipient_id][mail_.sender_id].append(mail_)
 
     def send(self, recipient_id):
         if recipient_id not in self.sources:
             raise ValueError(f"Recipient source {recipient_id} does not exist.")
         if not self.mails[recipient_id]:
             return
```

### Comparing `lionagi-0.0.316/lionagi/core/mail/schema.py` & `lionagi-0.1.0/lionagi/core/mail/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import deque
 from enum import Enum
 
-from lionagi.core.schema.base_node import BaseRelatableNode
+from lionagi.core.generic import Node
 
 
 class MailCategory(str, Enum):
     MESSAGES = "messages"
     TOOL = "tool"
     SERVICE = "service"
     MODEL = "model"
@@ -35,22 +35,29 @@
             raise ValueError(
                 f"Invalid request title. Valid titles are "
                 f"{list(MailCategory)}, Error: {e}"
             ) from e
         self.package = package
 
 
-class StartMail(BaseRelatableNode):
+class StartMail(Node):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.pending_outs = deque()
 
     def trigger(self, context, structure_id, executable_id):
         start_mail_content = {"context": context, "structure_id": structure_id}
         start_mail = BaseMail(
             sender_id=self.id_,
             recipient_id=executable_id,
             category="start",
             package=start_mail_content,
         )
         self.pending_outs.append(start_mail)
+
+
+class MailTransfer(Node):
+    def __init__(self):
+        super().__init__()
+        self.pending_ins = {}
+        self.pending_outs = deque()
```

### Comparing `lionagi-0.0.316/lionagi/core/prompt/action_template.py` & `lionagi-0.1.0/lionagi/core/form/action_form.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any
 from lionagi.integrations.bridge.pydantic_.pydantic_bridge import Field
 
-from .scored_template import ScoredTemplate
+from lionagi.core.form.scored_form import ScoredForm
 
 
 class ActionRequest: ...
 
 
-class ActionedTemplate(ScoredTemplate):
+class ActionForm(ScoredForm):
 
     action_needed: bool | None = Field(
         False, description="true if actions are needed else false"
     )
 
     actions: list[dict | ActionRequest | Any] | None = Field(
         default_factory=list,
```

### Comparing `lionagi-0.0.316/lionagi/core/prompt/field_validator.py` & `lionagi-0.1.0/lionagi/core/form/field_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,24 @@
 including numeric, boolean, string, and enum. It also provides a dictionary `validation_funcs` that
 maps data types to their corresponding validation functions.
 """
 
 from lionagi.libs import convert, StringMatch, ParseUtil
 
 
-def _has_action_keys(dict_):
-    return list(dict_.keys()) >= ["function", "arguments"]
+def check_dict_field(x, keys: list[str] | dict, fix_=True, **kwargs):
+    if isinstance(x, dict):
+        return x
+    if fix_:
+        try:
+            x = convert.to_str(x)
+            return StringMatch.force_validate_dict(x, keys=keys, **kwargs)
+        except Exception as e:
+            raise ValueError("Invalid dict field type.") from e
+    raise ValueError(f"Default value for DICT must be a dict, got {type(x).__name__}")
 
 
 def check_action_field(x, fix_=True, **kwargs):
     if (
         isinstance(x, list)
         and convert.is_same_dtype(x, dict)
         and all(_has_action_keys(y) for y in x)
@@ -23,34 +31,14 @@
     try:
         x = _fix_action_field(x, fix_)
         return x
     except Exception as e:
         raise ValueError("Invalid action field type.") from e
 
 
-def _fix_action_field(x, discard_=True):
-    corrected = []
-    if isinstance(x, str):
-        x = ParseUtil.fuzzy_parse_json(x)
-
-    try:
-        x = convert.to_list(x)
-
-        for i in x:
-            i = convert.to_dict(i)
-            if _has_action_keys(i):
-                corrected.append(i)
-            elif not discard_:
-                raise ValueError(f"Invalid action field: {i}")
-    except Exception as e:
-        raise ValueError(f"Invalid action field: {e}") from e
-
-    return corrected
-
-
 def check_number_field(x, fix_=True, **kwargs):
     """
     Checks if the given value is a valid numeric field.
 
     Args:
         x: The value to check.
         fix_ (bool): Flag indicating whether to attempt fixing the value if it's invalid (default: True).
@@ -167,14 +155,38 @@
         raise ValueError(
             f"Default value for ENUM must be one of the {choices}, got {x}"
         )
 
     return x
 
 
+def _has_action_keys(dict_):
+    return list(dict_.keys()) >= ["function", "arguments"]
+
+
+def _fix_action_field(x, discard_=True):
+    corrected = []
+    if isinstance(x, str):
+        x = ParseUtil.fuzzy_parse_json(x)
+
+    try:
+        x = convert.to_list(x)
+
+        for i in x:
+            i = convert.to_dict(i)
+            if _has_action_keys(i):
+                corrected.append(i)
+            elif not discard_:
+                raise ValueError(f"Invalid action field: {i}")
+    except Exception as e:
+        raise ValueError(f"Invalid action field: {e}") from e
+
+    return corrected
+
+
 def _fix_number_field(x, *args, **kwargs):
     """
     Attempts to fix an invalid numeric field value.
 
     Args:
         x: The value to fix.
         *args: Additional positional arguments for fixing the value.
@@ -205,25 +217,21 @@
     Returns:
         The fixed boolean value.
 
     Raises:
         ValueError: If the value cannot be converted into a valid boolean value.
     """
     try:
-        x = convert.to_str(x)
-        if (
-            convert.strip_lower(x) in ["true", "1", "correct", "yes"]
-            or convert.to_num(x) == 1
-        ):
+        x = convert.strip_lower(convert.to_str(x))
+        if x in ["true", "1", "correct", "yes"]:
             return True
-        elif (
-            convert.strip_lower(x) in ["false", "0", "incorrect", "no", "none", "n/a"]
-            or convert.to_num(x) == 0
-        ):
+
+        elif x in ["false", "0", "incorrect", "no", "none", "n/a"]:
             return False
+
         raise ValueError(f"Failed to convert {x} into a boolean value")
     except Exception as e:
         raise ValueError(f"Failed to convert {x} into a boolean value") from e
 
 
 def _fix_str_field(x):
     """
@@ -271,8 +279,9 @@
 
 validation_funcs = {
     "number": check_number_field,
     "bool": check_bool_field,
     "str": check_str_field,
     "enum": check_enum_field,
     "action": check_action_field,
+    "dict": check_dict_field,
 }
```

### Comparing `lionagi-0.0.316/lionagi/core/schema/__init__.py` & `lionagi-0.1.0/lionagi/core/generic/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-from .base_node import BaseNode, BaseRelatableNode, Tool, TOOL_TYPE
-from .data_node import DataNode
-from .data_logger import DLog, DataLogger
-from .structure import Relationship, Graph, Structure
-from .action_node import ActionNode, ActionSelection
+from .component import BaseComponent, BaseNode
 from .condition import Condition
+from .data_logger import DataLogger, DLog
+from .signal import Signal, Start
+from .mail import Mail, Package
+from .mailbox import MailBox
+from .edge import Edge
+from .relation import Relations
+from .transfer import Transfer
+from .work import Work, Worker
+from .node import Node
+from .structure import BaseStructure
+from .action import ActionNode, ActionSelection
+
 
 __all__ = [
+    "BaseComponent",
     "BaseNode",
-    "BaseRelatableNode",
-    "Tool",
-    "DataNode",
-    "DLog",
-    "DataLogger",
-    "Relationship",
-    "Graph",
-    "Structure",
+    "BaseStructure",
+    "BaseWork",
+    "Condition",
+    "Edge",
+    "Mail",
+    "MailBox",
+    "Start",
+    "Package",
+    "Relations",
+    "Signal",
+    "Transfer",
+    "Node",
+    "Work",
+    "Worker",
     "ActionNode",
-    "TOOL_TYPE",
     "ActionSelection",
-    "Condition",
+    "DataLogger",
+    "DLog",
 ]
```

### Comparing `lionagi-0.0.316/lionagi/core/schema/base_mixin.py` & `lionagi-0.1.0/lionagi/core/generic/component.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,230 @@
+"""This module provides base components used in lionagi"""
+
 from abc import ABC
 from functools import singledispatchmethod
-from typing import Any, TypeVar, Type, Callable
+from typing import Any, TypeVar
 
-import pandas as pd
-from pydantic import BaseModel, ValidationError
+from pydantic import AliasChoices, BaseModel, Field, ValidationError
+from pandas import DataFrame, Series
 
-from lionagi.libs import nested, convert, ParseUtil, SysUtil
+from lionagi.libs import SysUtil, func_call, convert, ParseUtil, nested
 
-T = TypeVar("T")  # Generic type for return type of from_obj method
 
+T = TypeVar("T")
 
-class BaseToObjectMixin(ABC, BaseModel):
 
-    def to_json_str(self, *args, **kwargs) -> str:
+class BaseComponent(BaseModel, ABC):
+    """
+    Base class for creating component models.
+
+    Attributes:
+        id_ (str): A 32-char unique hash identifier for the node.
+        timestamp (str): The timestamp of when the node was created.
+    """
+
+    id_: str = Field(
+        title="ID",
+        default_factory=SysUtil.create_id,
+        validation_alias=AliasChoices("node_id", "ID", "id"),
+        description="A 32-char unique hash identifier for the node.",
+    )
+
+    timestamp: str = Field(
+        default_factory=lambda: SysUtil.get_timestamp(sep=None),
+        description="The timestamp of when the node was created.",
+    )
+
+    class Config:
+        """Model configuration settings."""
+
+        extra = "allow"
+        arbitrary_types_allowed = True
+        populate_by_name = True
+        validate_assignment = True
+        validate_return = True
+        str_strip_whitespace = True
+
+    @classmethod
+    def class_name(cls) -> str:
         """
-        Serializes the model instance into a JSON string.
+        Retrieve the name of the class.
 
-        This method utilizes the model's `model_dump_json` method, typically available in Pydantic
-        models or models with similar serialization mechanisms, to convert the instance into a JSON
-        string. It supports passing arbitrary arguments to the underlying `model_dump_json` method.
+        Returns:
+            str: The name of the class.
+        """
+        return cls.__name__
+
+    @property
+    def _field_annotations(self) -> dict:
+        """
+        Return the annotations for each field in the model.
+
+        Returns:
+            dict: A dictionary mapping field names to their annotations.
+        """
+        return self._get_field_annotation(list(self.model_fields.keys()))
+
+    def _get_field_attr(self, k: str, attr: str, default=False) -> Any:
+        """
+        Get the value of a field attribute.
 
         Args:
-                *args: Variable-length argument list to be passed to `model_dump_json`.
-                **kwargs: Arbitrary keyword arguments, with `by_alias=True` set by default to use
-                                  model field aliases in the output JSON, if any.
+            k (str): The field name.
+            attr (str): The attribute name.
+            default (Any): Default value to return if the attribute is not
+                found.
 
         Returns:
-                str: A JSON string representation of the model instance.
+            Any: The value of the field attribute, or the default value if not
+                found.
+
+        Raises:
+            ValueError: If the field does not have the specified attribute.
         """
-        return self.model_dump_json(*args, by_alias=True, **kwargs)
+        try:
+            if not self._field_has_attr(k, attr):
+                raise ValueError(f"field {k} has no attribute {attr}")
+            field = self.model_fields[k]
+            a = getattr(field, attr)
+            if not a:
+                try:
+                    a = field.json_schema_extra[attr]
+                    return a
+                except Exception:
+                    return None
+            return a
+        except Exception as e:
+            if default is not False:
+                return default
+            raise e
 
-    def to_dict(self, *args, **kwargs) -> dict[str, Any]:
+    @singledispatchmethod
+    def _get_field_annotation(self, field_name: str) -> Any:
+        """
+        Get the annotation for a field.
+
+        Args:
+            field_name (str): The name of the field.
+
+        Raises:
+            TypeError: If the field_name is of an unsupported type.
         """
-        Converts the model instance into a dictionary.
+        raise TypeError(f"Unsupported type {type(field_name)}")
 
-        Leveraging the model's `model_dump` method, this function produces a dictionary representation
-        of the model. The dictionary keys correspond to the model's field names, with an option to use
-        aliases instead of the original field names.
+    @_get_field_annotation.register(str)
+    def _(self, field_name) -> dict[str, Any]:
+        """
+        Get the annotation for a field as a dictionary.
 
         Args:
-                *args: Variable-length argument list for the `model_dump` method.
-                **kwargs: Arbitrary keyword arguments. By default, `by_alias=True` is applied, indicating
-                                  that field aliases should be used as keys in the resulting dictionary.
+            field_name (str): The name of the field.
 
         Returns:
-                dict[str, Any]: The dictionary representation of the model instance.
+            dict[str, Any]: A dictionary mapping the field name to its
+                annotation.
         """
-        return self.model_dump(*args, by_alias=True, **kwargs)
+        dict_ = {field_name: self.model_fields[field_name].annotation}
+        for k, v in dict_.items():
+            if "|" in str(v):
+                v = str(v)
+                v = v.split("|")
+                dict_[k] = func_call.lcall(v, convert.strip_lower)
+            else:
+                dict_[k] = [v.__name__]
+        return dict_
 
-    def to_xml(self) -> str:
+    @_get_field_annotation.register(list)
+    def _(self, field_name) -> dict[str, Any]:
         """
-        Serializes the model instance into an XML string.
+        Get the annotations for multiple fields as a dictionary.
 
-        This method converts the model instance into an XML format. It first transforms the instance
-        into a dictionary and then recursively constructs an XML tree representing the model's data.
-        The root element of the XML tree is named after the class of the model instance.
+        Args:
+            field_name (list): A list or tuple of field names.
 
         Returns:
-                str: An XML string representation of the model instance.
+            dict[str, Any]: A dictionary mapping field names to their
+                annotations.
         """
+        dict_ = {}
+        for i in field_name:
+            dict_.update(self._get_field_annotation(i))
+        return dict_
+
+
+    @_get_field_annotation.register(tuple)
+    def _(self, field_name) -> dict[str, Any]:
+        """
+        Get the annotations for multiple fields as a dictionary.
+
+        Args:
+            field_name (tuple): A list or tuple of field names.
 
+        Returns:
+            dict[str, Any]: A dictionary mapping field names to their
+                annotations.
+        """
+        dict_ = {}
+        for i in field_name:
+            dict_.update(self._get_field_annotation(i))
+        return dict_
+
+
+    def _field_has_attr(self, k: str, attr: str) -> bool:
+        """
+        Check if a field has a specific attribute.
+
+        Args:
+            k (str): The field name.
+            attr (str): The attribute name.
+
+        Returns:
+            bool: True if the field has the attribute, False otherwise.
+        """
+        field = self.model_fields.get(k, None)
+        if field is None:
+            raise ValueError(f"Field {k} not found in model fields.")
+
+        a = attr in str(field)
+        if not a:
+            try:
+                a = (
+                    self.model_fields[k].json_schema_extra[attr] is not None
+                    and attr in self.model_fields[k].json_schema_extra
+                )
+                return a if isinstance(a, bool) else False
+            except Exception:
+                return False
+        return a
+
+    def to_json_str(self, *args, **kwargs) -> str:
+        """
+        Convert the component to a JSON string.
+
+        Returns:
+            str: The JSON string representation of the component.
+        """
+        return self.model_dump_json(*args, by_alias=True, **kwargs)
+
+    def to_dict(self, *args, **kwargs) -> dict[str, Any]:
+        """
+        Convert the component to a dictionary.
+
+        Returns:
+            dict[str, Any]: The dictionary representation of the component.
+        """
+        return self.model_dump(*args, by_alias=True, **kwargs)
+
+    def to_xml(self) -> str:
+        """
+        Convert the component to an XML string.
+
+        Returns:
+            str: The XML string representation of the component.
+        """
         import xml.etree.ElementTree as ET
 
         root = ET.Element(self.__class__.__name__)
 
         def convert(dict_obj, parent):
             for key, val in dict_obj.items():
                 if isinstance(val, dict):
@@ -72,225 +233,225 @@
                 else:
                     element = ET.SubElement(parent, key)
                     element.text = str(val)
 
         convert(self.to_dict(), root)
         return ET.tostring(root, encoding="unicode")
 
-    def to_pd_series(self, *args, pd_kwargs: dict | None = None, **kwargs) -> pd.Series:
+    def to_pd_series(self, *args, pd_kwargs: dict | None = None, **kwargs) -> Series:
         """
-        Converts the model instance into a pandas Series.
-
-        This method first transforms the model instance into a dictionary and then constructs a pandas
-        Series from it. The Series' index corresponds to the model's field names, with an option to
-        customize the Series creation through `pd_kwargs`.
-
-        Args:
-                *args: Variable-length argument list for the `to_dict` method.
-                pd_kwargs (dict | None): Optional dictionary of keyword arguments to pass to the pandas
-                                                                 Series constructor. Defaults to None, in which case an empty
-                                                                 dictionary is used.
-                **kwargs: Arbitrary keyword arguments for the `to_dict` method, influencing the dictionary
-                                  representation used for Series creation.
+        Convert the node to a Pandas Series.
 
         Returns:
-                pd.Series: A pandas Series representation of the model instance.
+            Series: The Pandas Series representation of the node.
         """
         pd_kwargs = {} if pd_kwargs is None else pd_kwargs
         dict_ = self.to_dict(*args, **kwargs)
-        return pd.Series(dict_, **pd_kwargs)
+        return Series(dict_, **pd_kwargs)
 
 
-class BaseFromObjectMixin(ABC, BaseModel):
+class BaseNode(BaseComponent):
+    """
+    Base class for creating node models.
+
+    Attributes:
+        content (Any | None): The optional content of the node.
+        metadata (dict[str, Any]): Additional metadata for the node.
+    """
+
+    content: Any | None = Field(
+        default=None,
+        validation_alias=AliasChoices("text", "page_content", "chunk_content", "data"),
+        description="The optional content of the node.",
+    )
+
+    metadata: dict[str, Any] = Field(
+        default_factory=dict,
+        alias="meta",
+        description="Additional metadata for the node.",
+    )
 
     @singledispatchmethod
     @classmethod
-    def from_obj(cls: Type[T], obj: Any, *args, **kwargs) -> T:
+    def from_obj(cls, obj: Any, *args, **kwargs) -> T:
+        """
+        Create a node instance from an object.
+
+        Args:
+            obj (Any): The object to create the node from.
+
+        Raises:
+            NotImplementedError: If the object type is not supported.
+        """
         raise NotImplementedError(f"Unsupported type: {type(obj)}")
 
     @from_obj.register(dict)
     @classmethod
-    def _from_dict(cls, obj: dict, *args, **kwargs) -> T:
+    def _from_dict(cls, obj, *args, **kwargs) -> T:
+        """
+        Create a node instance from a dictionary.
+
+        Args:
+            obj (dict): The dictionary to create the node from.
+
+        Returns:
+            T: The created node instance.
+        """
         return cls.model_validate(obj, *args, **kwargs)
 
     @from_obj.register(str)
     @classmethod
-    def _from_str(cls, obj: str, *args, fuzzy_parse=False, **kwargs) -> T:
+    def _from_str(cls, obj, *args, fuzzy_parse=False, **kwargs) -> T:
+        """
+        Create a node instance from a JSON string.
+
+        Args:
+            obj (str): The JSON string to create the node from.
+            fuzzy_parse (bool): Whether to perform fuzzy parsing.
+
+        Returns:
+            T: The created node instance.
+        """
         obj = ParseUtil.fuzzy_parse_json(obj) if fuzzy_parse else convert.to_dict(obj)
         try:
             return cls.from_obj(obj, *args, **kwargs)
         except ValidationError as e:
             raise ValueError(f"Invalid JSON for deserialization: {e}") from e
 
     @from_obj.register(list)
     @classmethod
-    def _from_list(cls, obj: list[Any], *args, **kwargs) -> list[T]:
+    def _from_list(cls, obj, *args, **kwargs) -> list[T]:
+        """
+        Create a list of node instances from a list of objects.
+
+        Args:
+            obj (list): The list of objects to create nodes from.
+
+        Returns:
+            list[T]: The list of created node instances.
+        """
         return [cls.from_obj(item, *args, **kwargs) for item in obj]
 
-    @from_obj.register(pd.Series)
+    @from_obj.register(Series)
     @classmethod
-    def _from_pd_series(cls, obj: pd.Series, *args, pd_kwargs=None, **kwargs) -> T:
+    def _from_pd_series(cls, obj, *args, pd_kwargs=None, **kwargs) -> T:
+        """
+        Create a node instance from a Pandas Series.
+
+        Args:
+            obj (Series): The Pandas Series to create the node from.
+
+        Returns:
+            T: The created node instance.
+        """
         if pd_kwargs is None:
             pd_kwargs = {}
         return cls.from_obj(obj.to_dict(**pd_kwargs), *args, **kwargs)
 
-    @from_obj.register(pd.DataFrame)
+    @from_obj.register(DataFrame)
     @classmethod
-    def _from_pd_dataframe(
-        cls, obj: pd.DataFrame, *args, pd_kwargs=None, **kwargs
-    ) -> list[T]:
+    def _from_pd_dataframe(cls, obj, *args, pd_kwargs=None, **kwargs) -> list[T]:
+        """
+        Create a list of node instances from a Pandas DataFrame.
+
+        Args:
+            obj (DataFrame): The Pandas DataFrame to create nodes from.
+
+        Returns:
+            list[T]: The list of created node instances.
+        """
         if pd_kwargs is None:
             pd_kwargs = {}
         return [
             cls.from_obj(row, *args, **pd_kwargs, **kwargs) for _, row in obj.iterrows()
         ]
 
     @from_obj.register(BaseModel)
     @classmethod
-    def _from_base_model(cls, obj: BaseModel, pydantic_kwargs=None, **kwargs) -> T:
-        if pydantic_kwargs is None:
-            pydantic_kwargs = {"by_alias": True}
-        config_ = {**obj.model_dump(**pydantic_kwargs), **kwargs}
-        return cls.from_obj(**config_)
-
-
-class BaseMetaManageMixin(ABC, BaseModel):
-
-    def meta_keys(self, flattened: bool = False, **kwargs) -> list[str]:
+    def _from_base_model(cls, obj, pydantic_kwargs=None, **kwargs) -> T:
         """
-        Retrieves a list of metadata keys.
+        Create a node instance from a Pydantic BaseModel.
 
         Args:
-                flattened (bool): If True, returns keys from a flattened metadata structure.
-                **kwargs: Additional keyword arguments passed to the flattening function.
+            obj (BaseModel): The Pydantic BaseModel to create the node from.
 
         Returns:
-                list[str]: List of metadata keys.
-        """
-        if flattened:
-            return nested.get_flattened_keys(self.metadata, **kwargs)
-        return list(self.metadata.keys())
-
-    def meta_has_key(self, key: str, flattened: bool = False, **kwargs) -> bool:
+            T: The created node instance.
         """
-        Checks if a specified key exists in the metadata.
+        if pydantic_kwargs is None:
+            pydantic_kwargs = {"by_alias": True}
 
-        Args:
-                key (str): The key to check.
-                flattened (bool): If True, checks within a flattened metadata structure.
-                **kwargs: Additional keyword arguments for flattening.
+        config_ = {}
+        try:
+            config_ = obj.model_dump(**pydantic_kwargs)
+        except:
+            config_ = obj.dict(**pydantic_kwargs)
 
-        Returns:
-                bool: True if key exists, False otherwise.
-        """
-        if flattened:
-            return key in nested.get_flattened_keys(self.metadata, **kwargs)
-        return key in self.metadata
+        return cls.from_obj(config_ | kwargs)
 
     def meta_get(
         self, key: str, indices: list[str | int] = None, default: Any = None
     ) -> Any:
         """
-        Retrieves the value associated with a given key from the metadata.
+        Get a value from the metadata dictionary.
 
         Args:
-                key (str): The key for the desired value.
-                indices: Optional indices for nested retrieval.
-                default (Any): The default value to return if the key is not found.
+            key (str): The key to retrieve the value for.
+            indices (list[str | int]): Optional list of indices for nested
+                retrieval.
+            default (Any): The default value to return if the key is not found.
 
         Returns:
-                Any: The value associated with the key or the default value.
+            Any: The retrieved value or the default value if not found.
         """
         if indices:
-            return nested.nget(self.metadata, key, indices, default)
+            return nested.nget(self.metadata, indices, default)
         return self.metadata.get(key, default)
 
     def meta_change_key(self, old_key: str, new_key: str) -> bool:
         """
-        Renames a key in the metadata.
+        Change a key in the metadata dictionary.
 
         Args:
-                old_key (str): The current key name.
-                new_key (str): The new key name.
+            old_key (str): The old key to be changed.
+            new_key (str): The new key to replace the old key.
 
         Returns:
-                bool: True if the key was changed, False otherwise.
+            bool: True if the key was changed successfully, False otherwise.
         """
         if old_key in self.metadata:
             SysUtil.change_dict_key(self.metadata, old_key, new_key)
             return True
         return False
 
     def meta_insert(self, indices: str | list, value: Any, **kwargs) -> bool:
         """
-        Inserts a value into the metadata at specified indices.
+        Insert a value into the metadata dictionary at the specified indices.
 
         Args:
-                indices (str | list): The indices where the value should be inserted.
-                value (Any): The value to insert.
-                **kwargs: Additional keyword arguments.
+            indices (str | list): The indices to insert the value at.
+            value (Any): The value to be inserted.
+            **kwargs: Additional keyword arguments for the `nested.ninsert`
+                function.
 
         Returns:
-                bool: True if the insertion was successful, False otherwise.
+            bool: True if the value was inserted successfully, False otherwise.
         """
         return nested.ninsert(self.metadata, indices, value, **kwargs)
 
-    # ToDo: do a nested pop
-    def meta_pop(self, key: str, default: Any = None) -> Any:
-        """
-        Removes a key from the metadata and returns its value.
-
-        Args:
-                key (str): The key to remove.
-                default (Any): The default value to return if the key is not found.
-
-        Returns:
-                Any: The value of the removed key or the default value.
-        """
-        return self.metadata.pop(key, default)
-
     def meta_merge(
         self, additional_metadata: dict[str, Any], overwrite: bool = False, **kwargs
     ) -> None:
         """
-        Merges additional metadata into the existing metadata.
+        Merge additional metadata into the existing metadata dictionary.
 
         Args:
-                additional_metadata (dict[str, Any]): The metadata to merge in.
-                overwrite (bool): If True, existing keys will be overwritten by those in additional_metadata.
-                **kwargs: Additional keyword arguments for the merge.
-
-        Returns:
-                None
+            additional_metadata (dict[str, Any]): The additional metadata to be
+                merged.
+            overwrite (bool): Whether to overwrite existing keys with the new
+                values.
+            **kwargs: Additional keyword arguments for the `nested.nmerge`
+                function.
         """
-        nested.nmerge(
+        self.metadata = nested.nmerge(
             [self.metadata, additional_metadata], overwrite=overwrite, **kwargs
         )
-
-        for key, value in additional_metadata.items():
-            if overwrite or key not in self.metadata:
-                self.metadata[key] = value
-
-    def meta_clear(self) -> None:
-        """
-        Clears all metadata.
-
-        Returns:
-                None
-        """
-        self.metadata.clear()
-
-    def meta_filter(self, condition: Callable[[Any, Any], bool]) -> dict[str, Any]:
-        """
-        Filters the metadata based on a condition.
-
-        Args:
-                condition (Callable[[Any, Any], bool]): The condition function to apply.
-
-        Returns:
-                dict[str, Any]: The filtered metadata.
-        """
-        return nested.nfilter(self.metadata, condition)
-
-
-class BaseComponentMixin(BaseFromObjectMixin, BaseToObjectMixin, BaseMetaManageMixin):
-    pass
```

### Comparing `lionagi-0.0.316/lionagi/core/session/session.py` & `lionagi-0.1.0/lionagi/core/session/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections import deque
 from typing import Tuple
 
-from lionagi.libs.sys_util import PATH_TYPE
+from pathlib import Path
 from lionagi.libs import BaseService, convert, dataframe
 
-from lionagi.core.schema import TOOL_TYPE, Tool, DataLogger
-from lionagi.core.tool import ToolManager
-from lionagi.core.mail import MailManager
-from lionagi.core.messages import System, Instruction
-from lionagi.core.branch import Branch
+from lionagi.core.generic import DataLogger
+from lionagi.core.tool import ToolManager, Tool, TOOL_TYPE
+from lionagi.core.mail.mail_manager import MailManager
+from lionagi.core.messages.schema import System, Instruction
+from lionagi.core.branch.branch import Branch
 from lionagi.core.flow.polyflow import PolyChat
 
 
 class Session:
     """
     Represents a session for managing conversations and branches.
 
@@ -37,15 +37,15 @@
         default_branch: Branch | None = None,
         default_branch_name: str | None = None,
         tools: TOOL_TYPE | None = None,
         # instruction_sets: Optional[List[Instruction]] = None,
         tool_manager: ToolManager | None = None,
         messages: dataframe.ln_DataFrame | None = None,
         datalogger: None | DataLogger = None,
-        persist_path: PATH_TYPE | None = None,
+        persist_path: Path | str | None = None,
     ):
         """Initialize a new session with optional configuration for managing conversations.
 
         Args:
                 system (Optional[Union[str, System]]): The system message.
                 sender (str | None): the default sender name for default branch
                 llmconfig (dict[str, Any] | None): Configuration for language learning models.
@@ -222,15 +222,15 @@
 
     def register_tools(self, tools):
         self.default_branch.register_tools(tools)
 
     @classmethod
     def from_csv(
         cls,
-        filepath: PATH_TYPE,
+        filepath: Path | str,
         system: dict | list | System | None = None,
         sender: str | None = None,
         llmconfig: dict[str, str | int | dict] | None = None,
         service: BaseService = None,
         default_branch_name: str = "main",
         tools: TOOL_TYPE = False,  # instruction_sets=None,
         tool_manager=None,
@@ -268,15 +268,15 @@
             messages=df,
             **kwargs,
         )
 
     @classmethod
     def from_json(
         cls,
-        filepath: PATH_TYPE,
+        filepath: Path | str,
         system: dict | list | System | None = None,
         sender: str | None = None,
         llmconfig: dict[str, str | int | dict] | None = None,
         service: BaseService = None,
         default_branch_name: str = "main",
         tools: TOOL_TYPE = False,  # instruction_sets=None,
         tool_manager=None,
@@ -848,16 +848,16 @@
             if from_ == self.default_branch:
                 self.default_branch_name = to_name
                 self.default_branch = to_branch
             self.delete_branch(from_, verbose=False)
 
     def take_branch(self, branch):
         self.branches[branch.branch_name] = branch
-        self.mail_manager.sources[branch.branch_name] = branch
-        self.mail_manager.mails[branch.branch_name] = {}
+        self.mail_manager.sources[branch.id_] = branch
+        self.mail_manager.mails[branch.id_] = {}
 
     def collect(self, from_: str | Branch | list[str | Branch] | None = None):
         """
         Collects requests from specified branches or from all branches if none are specified.
 
         This method is intended to aggregate data or requests from one or more branches for processing or analysis.
 
@@ -868,24 +868,25 @@
 
         Examples:
                 >>> session.collect("branch_name")
                 >>> session.collect([branch_instance_1, "branch_name_2"])
                 >>> session.collect()  # Collects from all branches
         """
         if from_ is None:
-            for branch in self.branches.keys():
-                self.mail_manager.collect(branch)
+            for branch in self.branches.values():
+                self.mail_manager.collect(branch.id_)
         else:
             if not isinstance(from_, list):
-                from_ = convert.to_list(from_)
+                from_ = [from_]
             for branch in from_:
-                if isinstance(branch, Branch):
-                    branch = branch.name
                 if isinstance(branch, str):
-                    self.mail_manager.collect(branch)
+                    branch = self.branches[branch]
+                    self.mail_manager.collect(branch.id_)
+                elif isinstance(branch, Branch):
+                    self.mail_manager.collect(branch.id_)
 
     def send(self, to_: str | Branch | list[str | Branch] | None = None):
         """
         Sends requests or data to specified branches or to all branches if none are specified.
 
         This method facilitates the distribution of data or requests to one or more branches, potentially for further tool or processing.
 
@@ -896,24 +897,25 @@
 
         Examples:
                 >>> session.send("target_branch")
                 >>> session.send([branch_instance_1, "target_branch_2"])
                 >>> session.send()  # Sends to all branches
         """
         if to_ is None:
-            for branch in self.branches.keys():
-                self.mail_manager.send(branch)
+            for branch in self.branches.values():
+                self.mail_manager.send(branch.id_)
         else:
             if not isinstance(to_, list):
                 to_ = [to_]
             for branch in to_:
-                if isinstance(branch, Branch):
-                    branch = branch.name
                 if isinstance(branch, str):
-                    self.mail_manager.send(branch)
+                    branch = self.branches[branch]
+                    self.mail_manager.send(branch.id_)
+                if isinstance(branch, Branch):
+                    self.mail_manager.send(branch.id_)
 
     def collect_send_all(self, receive_all=False):
         """
         Collects and sends requests across all branches, optionally invoking a receive operation on each branch.
 
         This method is a convenience function for performing a full cycle of collect and send operations across all branches,
         useful in scenarios where data or requests need to be aggregated and then distributed uniformly.
@@ -976,8 +978,8 @@
         )
 
         self.default_branch = branch
         self.default_branch_name = default_branch_name or "main"
         if system:
             self.default_branch.add_message(system=system, sender=sender)
 
-        self.llmconfig = self.default_branch.llmconfig
+        self.llmconfig = self.default_branch.llmconfig
```

### Comparing `lionagi-0.0.316/lionagi/core/tool/tool_manager.py` & `lionagi-0.1.0/lionagi/core/tool/tool_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from typing import Tuple, Any, TypeVar, Callable
-
 import asyncio
 
+from typing import Tuple, Any, TypeVar, Callable
 from lionagi.libs import func_call, convert, ParseUtil
-from lionagi.core.schema import Tool, TOOL_TYPE
+
+from lionagi.core.tool.tool import Tool, TOOL_TYPE
 
 T = TypeVar("T", bound=Tool)
 
 
 class ToolManager:
     """
     A manager class for handling the registration and invocation of tools that are subclasses of Tool.
 
     This class maintains a registry of tool instances, allowing for dynamic invocation based on
     tool name and provided arguments. It supports both synchronous and asynchronous tool function
     calls.
 
     Attributes:
-            registry (dict[str, Tool]): A dictionary to hold registered tools, keyed by their names.
+        registry (dict[str, Tool]): A dictionary to hold registered tools, keyed by their names.
     """
 
     registry: dict = {}
 
     def name_existed(self, name: str) -> bool:
         """
         Checks if a tool name already exists in the registry.
 
         Args:
-                name (str): The name of the tool to check.
+            name (str): The name of the tool to check.
 
         Returns:
-                bool: True if the name exists, False otherwise.
+            bool: True if the name exists, False otherwise.
         """
         return name in self.registry
 
     @property
     def has_tools(self):
         return self.registry != {}
 
     def _register_tool(self, tool: Tool | Callable) -> None:
         """
         Registers a tool in the registry. Raises a TypeError if the object is not an instance of Tool.
 
         Args:
-                tool (Tool): The tool instance to register.
+            tool (Tool): The tool instance to register.
 
         Raises:
-                TypeError: If the provided object is not an instance of Tool.
+            TypeError: If the provided object is not an instance of Tool.
         """
         if isinstance(tool, Callable):
             tool = func_to_tool(tool)[0]
         if not isinstance(tool, Tool):
             raise TypeError("Please register a Tool object.")
         name = tool.schema_["function"]["name"]
         self.registry.update({name: tool})
 
     async def invoke(self, func_calls: Tuple[str, dict[str, Any]]) -> Any:
         """
         Invokes a registered tool's function with the given arguments. Supports both coroutine and regular functions.
 
         Args:
-                func_call (Tuple[str, Dict[str, Any]]): A tuple containing the function name and a dictionary of keyword arguments.
+            func_call (Tuple[str, Dict[str, Any]]): A tuple containing the function name and a dictionary of keyword arguments.
 
         Returns:
-                Any: The result of the function call.
+            Any: The result of the function call.
 
         Raises:
-                ValueError: If the function name is not registered or if there's an error during function invocation.
+            ValueError: If the function name is not registered or if there's an error during function invocation.
         """
         name, kwargs = func_calls
         if not self.name_existed(name):
             raise ValueError(f"Function {name} is not registered.")
         tool = self.registry[name]
         func = tool.func
         parser = tool.parser
@@ -89,21 +89,21 @@
 
     @staticmethod
     def get_function_call(response: dict) -> Tuple[str, dict]:
         """
         Extracts a function call and arguments from a response dictionary.
 
         Args:
-                response (dict): The response dictionary containing the function call information.
+            response (dict): The response dictionary containing the function call information.
 
         Returns:
-                Tuple[str, dict]: A tuple containing the function name and a dictionary of arguments.
+            Tuple[str, dict]: A tuple containing the function name and a dictionary of arguments.
 
         Raises:
-                ValueError: If the response does not contain valid function call information.
+            ValueError: If the response does not contain valid function call information.
         """
         try:
             func = response["action"][7:]
             args = convert.to_dict(response["arguments"])
             return func, args
         except Exception:
             try:
@@ -114,51 +114,51 @@
                 raise ValueError("response is not a valid function call")
 
     def register_tools(self, tools: list[Tool]) -> None:
         """
         Registers multiple tools in the registry.
 
         Args:
-                tools (list[Tool]): A list of tool instances to register.
+            tools (list[Tool]): A list of tool instances to register.
         """
         func_call.lcall(tools, self._register_tool)
 
     def to_tool_schema_list(self) -> list[dict[str, Any]]:
         """
         Generates a list of schemas for all registered tools.
 
         Returns:
-                list[dict[str, Any]]: A list of tool schemas.
+            list[dict[str, Any]]: A list of tool schemas.
 
         """
         return [tool.schema_ for tool in self.registry.values()]
 
     def parse_tool(self, tools: TOOL_TYPE, **kwargs) -> dict:
         """
         Parses tool information and generates a dictionary for tool invocation.
 
         Args:
-                tools: Tool information which can be a single Tool instance, a list of Tool instances, a tool name, or a list of tool names.
-                **kwargs: Additional keyword arguments.
+            tools: Tool information which can be a single Tool instance, a list of Tool instances, a tool name, or a list of tool names.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-                dict: A dictionary containing tool schema information and any additional keyword arguments.
+            dict: A dictionary containing tool schema information and any additional keyword arguments.
 
         Raises:
-                ValueError: If a tool name is provided that is not registered.
+            ValueError: If a tool name is provided that is not registered.
         """
 
         def tool_check(tool):
             if isinstance(tool, dict):
                 return tool
             elif isinstance(tool, Tool):
                 return tool.schema_
             elif isinstance(tool, str):
                 if self.name_existed(tool):
-                    tool = self.registry[tool]
+                    tool: Tool = self.registry[tool]
                     return tool.schema_
                 else:
                     raise ValueError(f"Function {tool} is not registered.")
 
         if isinstance(tools, bool):
             tool_kwarg = {"tools": self.to_tool_schema_list()}
             kwargs = tool_kwarg | kwargs
@@ -186,74 +186,74 @@
 
     The function to be transformed can be any Callable that adheres to the
     specified docstring conventions. The resulting Tool object encapsulates the
     original function, allowing it to be utilized within environments that require
     objects with structured metadata.
 
     Args:
-            func_ (Callable): The function to be transformed into a Tool object. This
-                                              function should have a docstring that follows the
-                                              specified docstring style for accurate schema generation.
-            parser (Optional[Any]): An optional parser object associated with the Tool.
-                                                            This parameter is currently not utilized in the
-                                                            transformation process but is included for future
-                                                            compatibility and extension purposes.
-            docstring_style (str): The format of the docstring to be parsed, indicating
-                                                       the convention used in the function's docstring.
-                                                       Supports 'google' for Google-style docstrings and
-                                                       'reST' for reStructuredText-style docstrings. The
-                                                       chosen style affects how the docstring is parsed and
-                                                       how the schema is generated.
+        func_ (Callable): The function to be transformed into a Tool object. This
+            function should have a docstring that follows the
+            specified docstring style for accurate schema generation.
+        parser (Optional[Any]): An optional parser object associated with the Tool.
+                  This parameter is currently not utilized in the
+                  transformation process but is included for future
+                  compatibility and extension purposes.
+        docstring_style (str): The format of the docstring to be parsed, indicating
+                 the convention used in the function's docstring.
+                 Supports 'google' for Google-style docstrings and
+                 'reST' for reStructuredText-style docstrings. The
+                 chosen style affects how the docstring is parsed and
+                 how the schema is generated.
 
     Returns:
-            Tool: An object representing the original function wrapped as a Tool, along
-                      with its generated schema. This Tool object can be used in systems that
-                      require detailed metadata about functions, facilitating tasks such as
-                      automatic documentation generation, user interface creation, or
-                      integration with other software tools.
+        Tool: An object representing the original function wrapped as a Tool, along
+            with its generated schema. This Tool object can be used in systems that
+            require detailed metadata about functions, facilitating tasks such as
+            automatic documentation generation, user interface creation, or
+            integration with other software tools.
 
     Examples:
-            >>> def example_function_google(param1: int, param2: str) -> bool:
-            ...     '''
-            ...     An example function using Google style docstrings.
-            ...
-            ...     Args:
-            ...         param1 (int): The first parameter, demonstrating an integer input_.
-            ...         param2 (str): The second parameter, demonstrating a string input_.
-            ...
-            ...     Returns:
-            ...         bool: A boolean value, illustrating the return type.
-            ...     '''
-            ...     return True
-            ...
-            >>> tool_google = func_to_tool(example_function_google, docstring_style='google')
-            >>> print(isinstance(tool_google, Tool))
-            True
-
-            >>> def example_function_reST(param1: int, param2: str) -> bool:
-            ...     '''
-            ...     An example function using reStructuredText (reST) style docstrings.
-            ...
-            ...     :param param1: The first parameter, demonstrating an integer input_.
-            ...     :type param1: int
-            ...     :param param2: The second parameter, demonstrating a string input_.
-            ...     :type param2: str
-            ...     :returns: A boolean value, illustrating the return type.
-            ...     :rtype: bool
-            ...     '''
-            ...     return True
-            ...
-            >>> tool_reST = func_to_tool(example_function_reST, docstring_style='reST')
-            >>> print(isinstance(tool_reST, Tool))
-            True
+        >>> def example_function_google(param1: int, param2: str) -> bool:
+        ...     '''
+        ...     An example function using Google style docstrings.
+        ...
+        ...     Args:
+        ...         param1 (int): The first parameter, demonstrating an integer input_.
+        ...         param2 (str): The second parameter, demonstrating a string input_.
+        ...
+        ...     Returns:
+        ...         bool: A boolean value, illustrating the return type.
+        ...     '''
+        ...     return True
+        ...
+        >>> tool_google = func_to_tool(example_function_google, docstring_style='google')
+        >>> print(isinstance(tool_google, Tool))
+        True
+
+        >>> def example_function_reST(param1: int, param2: str) -> bool:
+        ...     '''
+        ...     An example function using reStructuredText (reST) style docstrings.
+        ...
+        ...     :param param1: The first parameter, demonstrating an integer input_.
+        ...     :type param1: int
+        ...     :param param2: The second parameter, demonstrating a string input_.
+        ...     :type param2: str
+        ...     :returns: A boolean value, illustrating the return type.
+        ...     :rtype: bool
+        ...     '''
+        ...     return True
+        ...
+        >>> tool_reST = func_to_tool(example_function_reST, docstring_style='reST')
+        >>> print(isinstance(tool_reST, Tool))
+        True
 
     Note:
-            The transformation process relies heavily on the accuracy and completeness of
-            the function's docstring. Functions with incomplete or incorrectly formatted
-            docstrings may result in incomplete or inaccurate Tool schemas.
+        The transformation process relies heavily on the accuracy and completeness of
+        the function's docstring. Functions with incomplete or incorrectly formatted
+        docstrings may result in incomplete or inaccurate Tool schemas.
     """
 
     fs = []
     funcs = convert.to_list(func_, flatten=True, dropna=True)
     parsers = convert.to_list(parser, flatten=True, dropna=True)
 
     if parser:
```

### Comparing `lionagi-0.0.316/lionagi/integrations/bridge/langchain_/documents.py` & `lionagi-0.1.0/lionagi/integrations/bridge/langchain_/documents.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/bridge/langchain_/langchain_bridge.py` & `lionagi-0.1.0/lionagi/integrations/bridge/langchain_/langchain_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py` & `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/node_parser.py` & `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/node_parser.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/reader.py` & `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/reader.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/bridge/llamaindex_/textnode.py` & `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/textnode.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/chunker/chunk.py` & `lionagi-0.1.0/lionagi/integrations/chunker/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import Union, Callable
 
 from lionagi.libs import func_call
-from lionagi.core.schema import DataNode
+from lionagi.core.generic import Node
 from ..bridge.langchain_.langchain_bridge import LangchainBridge
 from ..bridge.llamaindex_.llama_index_bridge import LlamaIndexBridge
 
 
 from ..loader.load_util import ChunkerType, file_to_chunks, _datanode_parser
 
 
 def datanodes_convert(documents, chunker_type):
 
     for i in range(len(documents)):
-        if type(documents[i]) == DataNode:
+        if type(documents[i]) == Node:
             if chunker_type == ChunkerType.LLAMAINDEX:
                 documents[i] = documents[i].to_llama_index()
             elif chunker_type == ChunkerType.LANGCHAIN:
                 documents[i] = documents[i].to_langchain()
     return documents
 
 
 def text_chunker(documents, args, kwargs):
 
     def chunk_node(node):
         chunks = file_to_chunks(node.to_dict(), *args, **kwargs)
         func_call.lcall(chunks, lambda chunk: chunk.pop("node_id"))
-        return [DataNode.from_obj({**chunk}) for chunk in chunks]
+        return [Node.from_obj({**chunk}) for chunk in chunks]
 
     return [chunk_node(doc) for doc in documents]
 
 
 def chunk(
     documents,
     chunker,
@@ -102,15 +102,15 @@
         nodes = splitter.split(documents, **chunking_kwargs)
     except Exception as e:
         raise ValueError(
             f"Self defined chunker {chunker} is not valid. Error: {e}"
         ) from e
 
     if isinstance(to_datanode, bool) and to_datanode is True:
-        raise ValueError("Please define a valid parser to DataNode.")
+        raise ValueError("Please define a valid parser to Node.")
     elif isinstance(to_datanode, Callable):
         nodes = _datanode_parser(nodes, to_datanode)
     return nodes
 
 
 def _llama_index_chunker(
     documents,
@@ -123,15 +123,15 @@
     if documents_convert_func:
         documents = documents_convert_func(documents, "llama_index")
     nodes = LlamaIndexBridge.llama_index_parse_node(
         documents, chunker, chunker_args, chunker_kwargs
     )
 
     if isinstance(to_datanode, bool) and to_datanode is True:
-        nodes = [DataNode.from_llama_index(i) for i in nodes]
+        nodes = [Node.from_llama_index(i) for i in nodes]
     elif isinstance(to_datanode, Callable):
         nodes = _datanode_parser(nodes, to_datanode)
     return nodes
 
 
 def _langchain_chunker(
     documents,
@@ -144,17 +144,17 @@
     if documents_convert_func:
         documents = documents_convert_func(documents, "langchain")
     nodes = LangchainBridge.langchain_text_splitter(
         documents, chunker, chunker_args, chunker_kwargs
     )
     if isinstance(to_datanode, bool) and to_datanode is True:
         if isinstance(documents, str):
-            nodes = [DataNode(content=i) for i in nodes]
+            nodes = [Node(content=i) for i in nodes]
         else:
-            nodes = [DataNode.from_langchain(i) for i in nodes]
+            nodes = [Node.from_langchain(i) for i in nodes]
     elif isinstance(to_datanode, Callable):
         nodes = _datanode_parser(nodes, to_datanode)
     return nodes
 
 
 def _plain_chunker(documents, chunker, chunker_args, chunker_kwargs):
     try:
```

### Comparing `lionagi-0.0.316/lionagi/integrations/config/oai_configs.py` & `lionagi-0.1.0/lionagi/integrations/config/oai_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,42 +75,42 @@
     "config": oai_audio_speech_llmconfig,
 }
 
 # Audio ----------- create transcription
 oai_audio_transcriptions_llmconfig = {
     "model": "whisper-1",
     "language": None,
-    "prompt": None,
+    "format_prompt": None,
     "response_format": "json",
     "temperature": 0,
 }
 oai_audio_transcriptions_schema = {
     "required": ["model", "voice"],
     "optional": [
         "response_format",
         "language",
-        "prompt",
+        "format_prompt",
         "response_format",
         "temperature",
     ],
     "input_": "file",
     "config": oai_audio_transcriptions_llmconfig,
 }
 
 # Audio ------------    translations
 oai_audio_translations_llmconfig = {
     "model": "whisper-1",
-    "prompt": None,
+    "format_prompt": None,
     "response_format": "json",
     "temperature": 0,
 }
 
 oai_audio_translations_schema = {
     "required": ["model"],
-    "optional": ["response_format", "speed", "prompt", "temperature"],
+    "optional": ["response_format", "speed", "format_prompt", "temperature"],
     "input_": "file",
     "config": oai_audio_translations_llmconfig,
 }
 
 # images
```

### Comparing `lionagi-0.0.316/lionagi/integrations/config/openrouter_configs.py` & `lionagi-0.1.0/lionagi/integrations/config/openrouter_configs.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/loader/load.py` & `lionagi-0.1.0/lionagi/integrations/loader/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Callable
 
-from lionagi.core.schema import DataNode
+from lionagi.core.generic import Node
 from ..bridge.langchain_.langchain_bridge import LangchainBridge
 from ..bridge.llamaindex_.llama_index_bridge import LlamaIndexBridge
 
 from .load_util import dir_to_nodes, ReaderType, _datanode_parser
 
 
 def text_reader(args, kwargs):
     """
-    Reads text files from a directory and converts them to DataNode instances.
+    Reads text files from a directory and converts them to Node instances.
 
     Args:
         args: Positional arguments for the dir_to_nodes function.
         kwargs: Keyword arguments for the dir_to_nodes function.
 
     Returns:
-        A list of DataNode instances.
+        A list of Node instances.
 
     Example usage:
         >>> args = ['path/to/text/files']
         >>> kwargs = {'file_extension': 'txt'}
         >>> nodes = text_reader(args, kwargs)
     """
     return dir_to_nodes(*args, **kwargs)
@@ -92,15 +92,15 @@
             f"Reader {reader} is currently not supported. Error: {e}"
         ) from e
 
 
 def _langchain_reader(reader, reader_args, reader_kwargs, to_datanode: bool | Callable):
     nodes = LangchainBridge.langchain_loader(reader, reader_args, reader_kwargs)
     if isinstance(to_datanode, bool) and to_datanode is True:
-        nodes = [DataNode.from_langchain(i) for i in nodes]
+        nodes = [Node.from_langchain(i) for i in nodes]
 
     elif isinstance(to_datanode, Callable):
         nodes = _datanode_parser(nodes, to_datanode)
     return nodes
 
 
 def _llama_index_reader(
@@ -111,15 +111,15 @@
     load_kwargs,
     to_datanode: bool | Callable,
 ):
     nodes = LlamaIndexBridge.llama_index_read_data(
         reader, reader_args, reader_kwargs, load_args, load_kwargs
     )
     if isinstance(to_datanode, bool) and to_datanode is True:
-        nodes = [DataNode.from_llama_index(i) for i in nodes]
+        nodes = [Node.from_llama_index(i) for i in nodes]
     elif isinstance(to_datanode, Callable):
         nodes = _datanode_parser(nodes, to_datanode)
     return nodes
 
 
 def _self_defined_reader(
     reader,
@@ -134,15 +134,15 @@
         nodes = loader.load(*load_args, **load_kwargs)
     except Exception as e:
         raise ValueError(
             f"Self defined reader {reader} is not valid. Error: {e}"
         ) from e
 
     if isinstance(to_datanode, bool) and to_datanode is True:
-        raise ValueError("Please define a valid parser to DataNode.")
+        raise ValueError("Please define a valid parser to Node.")
     elif isinstance(to_datanode, Callable):
         nodes = _datanode_parser(nodes, to_datanode)
     return nodes
 
 
 read_funcs = {
     ReaderType.PLAIN: _plain_reader,
```

### Comparing `lionagi-0.0.316/lionagi/integrations/loader/load_util.py` & `lionagi-0.1.0/lionagi/integrations/loader/load_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # use utils and schema
 import math
 from enum import Enum
 from pathlib import Path
 from typing import List, Union, Dict, Any, Tuple
 
 from lionagi.libs import convert, func_call
-from lionagi.core.schema import DataNode
+from lionagi.core.generic import Node
 
 
 class ReaderType(str, Enum):
     PLAIN = "plain"
     LANGCHAIN = "langchain"
     LLAMAINDEX = "llama_index"
     SELFDEFINED = "self_defined"
@@ -58,39 +58,39 @@
 
 def dir_to_nodes(
     dir: str,
     ext: Union[List[str], str],
     recursive: bool = False,
     flatten: bool = True,
     clean_text: bool = True,
-) -> List[DataNode]:
+) -> List[Node]:
     """
-    Converts directory contents into DataNode objects based on specified file extensions.
+    Converts directory contents into Node objects based on specified file extensions.
 
-    This function first retrieves a list of file paths from the specified directory, matching the given file extension. It then reads the content of these files, optionally cleaning the text, and converts each file's content into a DataNode object.
+    This function first retrieves a list of file paths from the specified directory, matching the given file extension. It then reads the content of these files, optionally cleaning the text, and converts each file's content into a Node object.
 
     Parameters:
         dir (str): The directory path from which to read files.
         ext: The file extension(s) to include. Can be a single string or a list/tuple of strings.
         recursive (bool, optional): If True, the function searches for files recursively in subdirectories. Defaults to False.
         flatten (bool, optional): If True, flattens the directory structure in the returned paths. Defaults to True.
         clean_text (bool, optional): If True, cleans the text read from files. Defaults to True.
 
     Returns:
-        list: A list of DataNode objects created from the files in the specified directory.
+        list: A list of Node objects created from the files in the specified directory.
 
     Example:
         nodes = dir_to_nodes("/path/to/dir", ".txt", recursive=True)
         # This would read all .txt files in /path/to/dir and its subdirectories,
-        # converting them into DataNode objects.
+        # converting them into Node objects.
     """
 
     path_list = dir_to_path(dir, ext, recursive, flatten)
     files_info = func_call.lcall(path_list, read_text, clean=clean_text)
-    return func_call.lcall(files_info, lambda x: DataNode(content=x[0], metadata=x[1]))
+    return func_call.lcall(files_info, lambda x: Node(content=x[0], metadata=x[1]))
 
 
 def chunk_text(
     input: str, chunk_size: int, overlap: float, threshold: int
 ) -> List[Union[str, None]]:
     """
     Chunks the input text into smaller parts, with optional overlap and threshold for final chunk.
@@ -259,8 +259,8 @@
 
 
 def _datanode_parser(nodes, parser):
 
     try:
         return parser(nodes)
     except Exception as e:
-        raise ValueError(f"DataNode parser {parser} failed. Error:{e}") from e
+        raise ValueError(f"Node parser {parser} failed. Error:{e}") from e
```

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/litellm.py` & `lionagi-0.1.0/lionagi/integrations/provider/litellm.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/mlx_service.py` & `lionagi-0.1.0/lionagi/integrations/provider/mlx_service.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/oai.py` & `lionagi-0.1.0/lionagi/integrations/provider/oai.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/ollama.py` & `lionagi-0.1.0/lionagi/integrations/provider/ollama.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/openrouter.py` & `lionagi-0.1.0/lionagi/integrations/provider/openrouter.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/services.py` & `lionagi-0.1.0/lionagi/integrations/provider/services.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/integrations/provider/transformers.py` & `lionagi-0.1.0/lionagi/integrations/provider/transformers.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/__init__.py` & `lionagi-0.1.0/lionagi/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/ln_api.py` & `lionagi-0.1.0/lionagi/libs/ln_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,24 +373,24 @@
                             num_tokens -= (
                                 1
                                 # role is always required and always 1 token
                             )
                 num_tokens += 2  # every reply is primed with <im_start>assistant
                 return num_tokens + completion_tokens
             else:
-                prompt = payload["prompt"]
-                if isinstance(prompt, str):  # single prompt
+                prompt = payload["format_prompt"]
+                if isinstance(prompt, str):  # single format_prompt
                     prompt_tokens = len(encoding.encode(prompt))
                     return prompt_tokens + completion_tokens
                 elif isinstance(prompt, list):  # multiple prompts
                     prompt_tokens = sum(len(encoding.encode(p)) for p in prompt)
                     return prompt_tokens + completion_tokens * len(prompt)
                 else:
                     raise TypeError(
-                        'Expecting either string or list of strings for "prompt" field in completion request'
+                        'Expecting either string or list of strings for "format_prompt" field in completion request'
                     )
         elif api_endpoint == "embeddings":
             input = payload["input"]
             if isinstance(input, str):  # single input
                 return len(encoding.encode(input))
             elif isinstance(input, list):  # multiple inputs
                 return sum(len(encoding.encode(i)) for i in input)
```

### Comparing `lionagi-0.0.316/lionagi/libs/ln_async.py` & `lionagi-0.1.0/lionagi/libs/ln_async.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/ln_convert.py` & `lionagi-0.1.0/lionagi/libs/ln_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/ln_dataframe.py` & `lionagi-0.1.0/lionagi/libs/ln_dataframe.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/ln_func_call.py` & `lionagi-0.1.0/lionagi/libs/ln_func_call.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/ln_nested.py` & `lionagi-0.1.0/lionagi/libs/ln_nested.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/libs/ln_parse.py` & `lionagi-0.1.0/lionagi/libs/ln_parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from collections.abc import Callable
 import re
 import inspect
 import itertools
-from collections.abc import Callable
+import contextlib
+from functools import singledispatchmethod
 from typing import Any
 import numpy as np
 import lionagi.libs.ln_convert as convert
 
+
 md_json_char_map = {"\n": "\\n", "\r": "\\r", "\t": "\\t", '"': '\\"'}
 
 
 class ParseUtil:
 
     @staticmethod
     def fuzzy_parse_json(str_to_parse: str, *, strict: bool = False):
@@ -586,22 +589,23 @@
                 d[i - 1][j] + 1,  # deletion
                 d[i][j - 1] + 1,  # insertion
                 d[i - 1][j - 1] + cost,
             )  # substitution
         return d[m][n]
 
     @staticmethod
-    def correct_keys(output_fields, out_, score_func=None):
+    def correct_dict_keys(keys: dict | list[str], dict_, score_func=None):
         if score_func is None:
             score_func = StringMatch.jaro_winkler_similarity
-        fields_set = set(output_fields.keys())
+
+        fields_set = set(keys if isinstance(keys, list) else keys.keys())
         corrected_out = {}
         used_keys = set()
 
-        for k, v in out_.items():
+        for k, v in dict_.items():
             if k in fields_set:
                 corrected_out[k] = v
                 fields_set.remove(k)  # Remove the matched key
                 used_keys.add(k)
             else:
                 # Calculate Jaro-Winkler similarity scores for each potential match
                 scores = np.array([score_func(k, field) for field in fields_set])
@@ -610,16 +614,16 @@
                 # Select the best match based on the highest score
                 best_match = list(fields_set)[max_score_index]
 
                 corrected_out[best_match] = v
                 fields_set.remove(best_match)  # Remove the matched key
                 used_keys.add(best_match)
 
-        if len(used_keys) < len(out_):
-            for k, v in out_.items():
+        if len(used_keys) < len(dict_):
+            for k, v in dict_.items():
                 if k not in used_keys:
                     corrected_out[k] = v
 
         return corrected_out
 
     @staticmethod
     def choose_most_similar(word, correct_words_list, score_func=None):
@@ -633,7 +637,40 @@
                 score_func(convert.to_str(word), correct_word)
                 for correct_word in correct_words_list
             ]
         )
         # Find the index of the highest score
         max_score_index = np.argmax(scores)
         return correct_words_list[max_score_index]
+
+    @staticmethod
+    def force_validate_dict(x, keys: dict | list[str]) -> dict:
+        out_ = x
+
+        if isinstance(out_, str):
+            # first try to parse it straight as a fuzzy json
+            try:
+                out_ = ParseUtil.fuzzy_parse_json(out_)
+            except Exception:
+                try:
+                    # if failed we try to extract the json block and parse it
+                    out_ = ParseUtil.md_to_json(out_)
+                except Exception:
+                    # if still failed we try to extract the json block using re and parse it again
+                    match = re.search(r"```json\n({.*?})\n```", out_, re.DOTALL)
+                    if match:
+                        out_ = match.group(1)
+                        try:
+                            out_ = ParseUtil.fuzzy_parse_json(out_)
+                        except:
+                            try:
+                                out_ = ParseUtil.fuzzy_parse_json(
+                                    out_.replace("'", '"')
+                                )
+                            except:
+                                pass
+
+        if isinstance(out_, dict):
+            try:
+                return StringMatch.correct_dict_keys(keys, out_)
+            except Exception as e:
+                raise ValueError(f"Failed to force_validate_dict for input: {x}") from e
```

### Comparing `lionagi-0.0.316/lionagi/libs/sys_util.py` & `lionagi-0.1.0/lionagi/libs/sys_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 """
 MIT License
 
 Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Permission is hereby granted, free of charge, to any person 
+obtaining a copy of this software and associated documentation 
+files (the "Software"), to deal in the Software without 
+restriction, including without limitation the rights to use, 
+copy, modify, merge, publish, distribute, sublicense, and/or 
+sell copies of the Software, and to permit persons to whom 
+the Software is furnished to do so, subject to the following 
+conditions:
+
+The above copyright notice and this permission notice shall be 
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, 
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES 
+OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND 
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS 
+BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN 
+ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+SOFTWARE.
 """
 
 import copy
 import importlib
 import logging
 import os
 import platform
@@ -359,14 +374,15 @@
     def create_path(
         directory: Path | str,
         filename: str,
         timestamp: bool = True,
         dir_exist_ok: bool = True,
         time_prefix: bool = False,
         custom_timestamp_format: str | None = None,
+        random_hash_digits=0,
     ) -> Path:
         """
         Creates a path with an optional timestamp in the specified directory.
 
         Args:
                 directory (Union[Path, str]): The directory where the file will be located.
                 filename (str): The filename. Must include a valid extension.
@@ -396,15 +412,21 @@
             timestamp_str = datetime.now().strftime(timestamp_format)
             filename = (
                 f"{timestamp_str}_{name}" if time_prefix else f"{name}_{timestamp_str}"
             )
         else:
             filename = name
 
-        full_filename = f"{filename}{ext}"
+        random_hash = (
+            "-" + SysUtil.create_id(random_hash_digits)
+            if random_hash_digits > 0
+            else ""
+        )
+
+        full_filename = f"{filename}{random_hash}{ext}"
         full_path = directory / full_filename
         full_path.parent.mkdir(parents=True, exist_ok=dir_exist_ok)
 
         return full_path
 
     @staticmethod
     def list_files(dir_path: Path | str, extension: str = None) -> list[Path]:
```

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_base_branch.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_base_branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # from lionagi.core.branch.base_branch import BaseBranch
 # from lionagi.core.branch.util import MessageUtil
 # from lionagi.core.messages.schema import System
 # from lionagi.core.schema import DataLogger
 
-
 # import unittest
 # from unittest.mock import patch, MagicMock
 # import pandas as pd
 # from datetime import datetime
 # import json
```

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_branch.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # import unittest
 # from unittest.mock import patch, MagicMock
 # import pandas as pd
 # import json
 # from collections import deque
 
 
+
 # class TestBranch(unittest.TestCase):
 #     def setUp(self):
 #         # Assuming no need for actual files or external services for initialization
 #         self.test_messages = [
 #             {
 #                 "node_id": "1",
 #                 "timestamp": "2021-01-01 00:00:00",
@@ -80,14 +81,15 @@
 #         # Initially, no tools are registered
 #         self.assertFalse(self.branch.has_tools)
 
 #         # Mock tool registration
 #         self.branch.register_tools(self.tool)
 #         self.assertTrue(self.branch.has_tools)
 
+
 #     # @patch("lionagi.core.branch.BaseBranch._from_csv")
 #     # def test_from_csv(self, mock_from_csv):
 #     #     """Test creating a Branch instance from a CSV file."""
 #     #     filepath = "path/to/your/csvfile.csv"
 #     #     Branch.from_csv(filepath=filepath, branch_name="TestBranchFromCSV")
 #     #     mock_from_csv.assert_called_once_with(
 #     #         filepath=filepath,
@@ -114,14 +116,15 @@
 #     #         llmconfig=None,
 #     #         tools=None,
 #     #         datalogger=None,
 #     #         persist_path=None,
 #     #         tool_manager=None,
 #     #     )
 
+
 #     def test_messages_describe(self):
 #         """Test the messages_describe method for accuracy."""
 #         # Assuming self.branch has been set up with some messages
 #         description = self.branch.messages_describe()
 #         self.assertIn("total_messages", description)
 #         self.assertIn("summary_by_role", description)
 #         self.assertIn("summary_by_sender", description)
```

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_chat_flow.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_chat_flow.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_mail_manager.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_mail_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_prompts.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_prompts.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_session.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_session.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_session_base_util.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_session_base_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # from lionagi.core.branch.util import MessageUtil
 # from lionagi.core.messages.schema import System, Instruction, Response
 
+
 # import unittest
 # import pandas as pd
 # import json
 # from datetime import datetime
 
 
 # class TestCreateMessage(unittest.TestCase):
```

### Comparing `lionagi-0.0.316/lionagi/tests/test_core/test_tool_manager.py` & `lionagi-0.1.0/lionagi/tests/test_core/test_tool_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_libs/test_api.py` & `lionagi-0.1.0/lionagi/tests/libs/test_api.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_libs/test_convert.py` & `lionagi-0.1.0/lionagi/tests/libs/test_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_libs/test_func_call.py` & `lionagi-0.1.0/lionagi/tests/libs/test_func_call.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_libs/test_nested.py` & `lionagi-0.1.0/lionagi/tests/libs/test_nested.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_libs/test_parse.py` & `lionagi-0.1.0/lionagi/tests/libs/test_parse.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi/tests/test_libs/test_sys_util.py` & `lionagi-0.1.0/lionagi/tests/libs/test_sys_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/lionagi.egg-info/PKG-INFO` & `lionagi-0.1.0/lionagi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionagi
-Version: 0.0.316
+Version: 0.1.0
 Summary: Towards automated general intelligence.
 Author: HaiyangLi
 Author-email: Haiyang Li <ocean@lionagi.ai>
 License: MIT License
         
         Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
```

### Comparing `lionagi-0.0.316/lionagi.egg-info/SOURCES.txt` & `lionagi-0.1.0/lionagi.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,63 +10,76 @@
 lionagi.egg-info/dependency_links.txt
 lionagi.egg-info/requires.txt
 lionagi.egg-info/top_level.txt
 lionagi/core/__init__.py
 lionagi/core/agent/__init__.py
 lionagi/core/agent/base_agent.py
 lionagi/core/branch/__init__.py
-lionagi/core/branch/base_branch.py
+lionagi/core/branch/base.py
 lionagi/core/branch/branch.py
-lionagi/core/branch/branch_flow_mixin.py
 lionagi/core/branch/executable_branch.py
+lionagi/core/branch/flow_mixin.py
 lionagi/core/branch/util.py
-lionagi/core/branch/base/__init__.py
 lionagi/core/direct/__init__.py
 lionagi/core/direct/cot.py
 lionagi/core/direct/plan.py
 lionagi/core/direct/predict.py
 lionagi/core/direct/react.py
 lionagi/core/direct/score.py
 lionagi/core/direct/select.py
 lionagi/core/direct/sentiment.py
 lionagi/core/direct/utils.py
 lionagi/core/direct/vote.py
+lionagi/core/execute/__init__.py
+lionagi/core/execute/base_executor.py
+lionagi/core/execute/branch_executor.py
+lionagi/core/execute/instruction_map_executor.py
+lionagi/core/execute/structure_executor.py
 lionagi/core/flow/__init__.py
-lionagi/core/flow/base/__init__.py
-lionagi/core/flow/base/baseflow.py
+lionagi/core/flow/baseflow.py
+lionagi/core/flow/mono_chat_mixin.py
 lionagi/core/flow/monoflow/ReAct.py
 lionagi/core/flow/monoflow/__init__.py
 lionagi/core/flow/monoflow/chat.py
 lionagi/core/flow/monoflow/chat_mixin.py
 lionagi/core/flow/monoflow/followup.py
 lionagi/core/flow/polyflow/__init__.py
 lionagi/core/flow/polyflow/chat.py
+lionagi/core/form/__init__.py
+lionagi/core/form/action_form.py
+lionagi/core/form/field_validator.py
+lionagi/core/form/form.py
+lionagi/core/form/mixin.py
+lionagi/core/form/scored_form.py
+lionagi/core/generic/__init__.py
+lionagi/core/generic/action.py
+lionagi/core/generic/component.py
+lionagi/core/generic/condition.py
+lionagi/core/generic/data_logger.py
+lionagi/core/generic/edge.py
+lionagi/core/generic/mail.py
+lionagi/core/generic/mailbox.py
+lionagi/core/generic/node.py
+lionagi/core/generic/relation.py
+lionagi/core/generic/signal.py
+lionagi/core/generic/structure.py
+lionagi/core/generic/transfer.py
+lionagi/core/generic/work.py
+lionagi/core/graph/__init__.py
+lionagi/core/graph/graph.py
+lionagi/core/graph/tree.py
 lionagi/core/mail/__init__.py
 lionagi/core/mail/mail_manager.py
 lionagi/core/mail/schema.py
 lionagi/core/messages/__init__.py
 lionagi/core/messages/schema.py
-lionagi/core/prompt/__init__.py
-lionagi/core/prompt/action_template.py
-lionagi/core/prompt/field_validator.py
-lionagi/core/prompt/prompt_template.py
-lionagi/core/prompt/scored_template.py
-lionagi/core/schema/__init__.py
-lionagi/core/schema/action_node.py
-lionagi/core/schema/base_mixin.py
-lionagi/core/schema/base_node.py
-lionagi/core/schema/condition.py
-lionagi/core/schema/data_logger.py
-lionagi/core/schema/data_node.py
-lionagi/core/schema/prompt_template.py
-lionagi/core/schema/structure.py
 lionagi/core/session/__init__.py
 lionagi/core/session/session.py
 lionagi/core/tool/__init__.py
-lionagi/core/tool/manual.py
+lionagi/core/tool/tool.py
 lionagi/core/tool/tool_manager.py
 lionagi/integrations/__init__.py
 lionagi/integrations/bridge/__init__.py
 lionagi/integrations/bridge/langchain_/__init__.py
 lionagi/integrations/bridge/langchain_/documents.py
 lionagi/integrations/bridge/langchain_/langchain_bridge.py
 lionagi/integrations/bridge/llamaindex_/__init__.py
@@ -100,27 +113,29 @@
 lionagi/libs/ln_api.py
 lionagi/libs/ln_async.py
 lionagi/libs/ln_convert.py
 lionagi/libs/ln_dataframe.py
 lionagi/libs/ln_func_call.py
 lionagi/libs/ln_nested.py
 lionagi/libs/ln_parse.py
+lionagi/libs/ln_validate.py
 lionagi/libs/sys_util.py
 lionagi/tests/__init__.py
+lionagi/tests/integrations/__init__.py
+lionagi/tests/libs/__init__.py
+lionagi/tests/libs/test_api.py
+lionagi/tests/libs/test_async.py
+lionagi/tests/libs/test_convert.py
+lionagi/tests/libs/test_field_validators.py
+lionagi/tests/libs/test_func_call.py
+lionagi/tests/libs/test_nested.py
+lionagi/tests/libs/test_parse.py
+lionagi/tests/libs/test_sys_util.py
 lionagi/tests/test_core/__init__.py
 lionagi/tests/test_core/test_base_branch.py
 lionagi/tests/test_core/test_branch.py
 lionagi/tests/test_core/test_chat_flow.py
 lionagi/tests/test_core/test_mail_manager.py
 lionagi/tests/test_core/test_prompts.py
 lionagi/tests/test_core/test_session.py
 lionagi/tests/test_core/test_session_base_util.py
-lionagi/tests/test_core/test_tool_manager.py
-lionagi/tests/test_integrations/__init__.py
-lionagi/tests/test_libs/__init__.py
-lionagi/tests/test_libs/test_api.py
-lionagi/tests/test_libs/test_async.py
-lionagi/tests/test_libs/test_convert.py
-lionagi/tests/test_libs/test_func_call.py
-lionagi/tests/test_libs/test_nested.py
-lionagi/tests/test_libs/test_parse.py
-lionagi/tests/test_libs/test_sys_util.py
+lionagi/tests/test_core/test_tool_manager.py
```

### Comparing `lionagi-0.0.316/pyproject.toml` & `lionagi-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lionagi-0.0.316/setup.py` & `lionagi-0.1.0/setup.py`

 * *Files identical despite different names*

