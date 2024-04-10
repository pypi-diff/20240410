# Comparing `tmp/pymemgpt_nightly-0.3.8.dev20240408103946.tar.gz` & `tmp/pymemgpt_nightly-0.3.8.dev20240409104037.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemgpt_nightly-0.3.8.dev20240408103946.tar", max compression
+gzip compressed data, was "pymemgpt_nightly-0.3.8.dev20240409104037.tar", max compression
```

## Comparing `pymemgpt_nightly-0.3.8.dev20240408103946.tar` & `pymemgpt_nightly-0.3.8.dev20240409104037.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0    10760 2024-04-08 10:39:34.363279 pymemgpt_nightly-0.3.8.dev20240408103946/LICENSE
--rw-r--r--   0        0        0     8441 2024-04-08 10:39:34.363279 pymemgpt_nightly-0.3.8.dev20240408103946/README.md
--rw-r--r--   0        0        0      108 2024-04-08 10:39:46.055289 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/__init__.py
--rw-r--r--   0        0        0       29 2024-04-08 10:39:34.367280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/__main__.py
--rw-r--r--   0        0        0    55407 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent.py
--rw-r--r--   0        0        0    10728 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/chroma.py
--rw-r--r--   0        0        0    25552 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/db.py
--rw-r--r--   0        0        0     5288 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/lancedb.py
--rw-r--r--   0        0        0     6390 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/storage.py
--rw-r--r--   0        0        0      169 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/README.md
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/__init__.py
--rw-r--r--   0        0        0     7088 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/agent_autoreply.py
--rw-r--r--   0        0        0     6813 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/agent_docs.py
--rw-r--r--   0        0        0     7914 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/agent_groupchat.py
--rw-r--r--   0        0        0     7375 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
--rw-r--r--   0        0        0     9318 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/interface.py
--rw-r--r--   0        0        0    20931 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/memgpt_agent.py
--rw-r--r--   0        0        0     3644 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/benchmark/benchmark.py
--rw-r--r--   0        0        0      536 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/benchmark/constants.py
--rw-r--r--   0        0        0    34724 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/cli/cli.py
--rw-r--r--   0        0        0    40445 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/cli/cli_config.py
--rw-r--r--   0        0        0    10453 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/cli/cli_load.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/client/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/client/admin.py
--rw-r--r--   0        0        0    26592 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/client/client.py
--rw-r--r--   0        0        0    18729 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/config.py
--rw-r--r--   0        0        0      390 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/configs/memgpt_hosted.json
--rw-r--r--   0        0        0      373 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/configs/openai.json
--rw-r--r--   0        0        0     5364 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/constants.py
--rw-r--r--   0        0        0     4904 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/credentials.py
--rw-r--r--   0        0        0     9529 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/data_sources/connectors.py
--rw-r--r--   0        0        0    23711 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/data_types.py
--rw-r--r--   0        0        0     7601 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/embeddings.py
--rw-r--r--   0        0        0      820 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/errors.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/__init__.py
--rw-r--r--   0        0        0     7343 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/function_sets/base.py
--rw-r--r--   0        0        0     4629 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/function_sets/extras.py
--rw-r--r--   0        0        0     5626 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/functions.py
--rw-r--r--   0        0        0     5433 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/schema_generator.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/humans/__init__.py
--rw-r--r--   0        0        0       17 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/humans/examples/basic.txt
--rw-r--r--   0        0        0      305 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/humans/examples/cs_phd.txt
--rw-r--r--   0        0        0    12994 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/interface.py
--rw-r--r--   0        0        0    21252 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/llm_api_tools.py
--rw-r--r--   0        0        0      175 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/README.md
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/__init__.py
--rw-r--r--   0        0        0    13519 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/chat_completion_proxy.py
--rw-r--r--   0        0        0      912 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/constants.py
--rw-r--r--   0        0        0     2788 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/function_parser.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/__init__.py
--rw-r--r--   0        0        0    56322 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/gbnf_grammar_generator.py
--rw-r--r--   0        0        0      667 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/json.gbnf
--rw-r--r--   0        0        0     3255 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
--rw-r--r--   0        0        0     3562 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/groq/api.py
--rw-r--r--   0        0        0     7434 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/json_parser.py
--rw-r--r--   0        0        0     2586 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/koboldcpp/api.py
--rw-r--r--   0        0        0      557 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/koboldcpp/settings.py
--rw-r--r--   0        0        0     2492 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llamacpp/api.py
--rw-r--r--   0        0        0      548 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llamacpp/settings.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
--rw-r--r--   0        0        0    19913 2024-04-08 10:39:34.371280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
--rw-r--r--   0        0        0    21281 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
--rw-r--r--   0        0        0    19975 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
--rw-r--r--   0        0        0    10300 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
--rw-r--r--   0        0        0     6144 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
--rw-r--r--   0        0        0      419 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
--rw-r--r--   0        0        0    14956 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
--rw-r--r--   0        0        0     4630 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/lmstudio/api.py
--rw-r--r--   0        0        0      857 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/lmstudio/settings.py
--rw-r--r--   0        0        0     3660 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/ollama/api.py
--rw-r--r--   0        0        0      894 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/ollama/settings.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/__init__.py
--rw-r--r--   0        0        0     1222 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/deterministic_mirostat.py
--rw-r--r--   0        0        0     3058 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/settings.py
--rw-r--r--   0        0        0      719 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/simple.py
--rw-r--r--   0        0        0     4846 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/utils.py
--rw-r--r--   0        0        0     2612 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/vllm/api.py
--rw-r--r--   0        0        0     2658 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/api.py
--rw-r--r--   0        0        0     2354 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/legacy_api.py
--rw-r--r--   0        0        0      579 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/legacy_settings.py
--rw-r--r--   0        0        0      593 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/settings.py
--rw-r--r--   0        0        0     1211 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/log.py
--rw-r--r--   0        0        0    19851 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/main.py
--rw-r--r--   0        0        0    19653 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/memory.py
--rw-r--r--   0        0        0    29217 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/metadata.py
--rw-r--r--   0        0        0    31537 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/migrate.py
--rw-r--r--   0        0        0     2517 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/chat_completion_request.py
--rw-r--r--   0        0        0     1562 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/chat_completion_response.py
--rw-r--r--   0        0        0      356 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/embedding_response.py
--rw-r--r--   0        0        0     7977 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/openai.py
--rw-r--r--   0        0        0     7902 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/pydantic_models.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/openai_backcompat/__init__.py
--rw-r--r--   0        0        0    13692 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/openai_backcompat/openai_object.py
--rw-r--r--   0        0        0     5882 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/persistence_manager.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/anna_pa.txt
--rw-r--r--   0        0        0     1196 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/google_search_persona.txt
--rw-r--r--   0        0        0      431 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/memgpt_doc.txt
--rw-r--r--   0        0        0      164 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/memgpt_starter.txt
--rw-r--r--   0        0        0     1236 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sam.txt
--rw-r--r--   0        0        0     1171 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sam_pov.txt
--rw-r--r--   0        0        0     1053 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sam_simple_pov_gpt35.txt
--rw-r--r--   0        0        0     8192 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sqldb/test.db
--rw-r--r--   0        0        0      248 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/examples/memgpt_chat.yaml
--rw-r--r--   0        0        0      247 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/examples/memgpt_docs.yaml
--rw-r--r--   0        0        0      374 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/examples/memgpt_extras.yaml
--rw-r--r--   0        0        0     7575 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/presets.py
--rw-r--r--   0        0        0     2789 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/__init__.py
--rw-r--r--   0        0        0    12907 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/gpt_functions.py
--rw-r--r--   0        0        0     1139 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/gpt_summarize.py
--rw-r--r--   0        0        0     1045 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/gpt_system.py
--rw-r--r--   0        0        0     4758 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_base.txt
--rw-r--r--   0        0        0     5479 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_chat.txt
--rw-r--r--   0        0        0     1057 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_chat_compressed.txt
--rw-r--r--   0        0        0     4819 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_doc.txt
--rw-r--r--   0        0        0     5047 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_gpt35_extralong.txt
--rw-r--r--   0        0        0     2967 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
--rw-r--r--   0        0        0     4663 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_modified_chat.txt
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/__init__.py
--rw-r--r--   0        0        0       92 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/admin/__init__.py
--rw-r--r--   0        0        0     6130 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/admin/users.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/command.py
--rw-r--r--   0        0        0     6138 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/config.py
--rw-r--r--   0        0        0     5114 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/index.py
--rw-r--r--   0        0        0     7640 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/memory.py
--rw-r--r--   0        0        0     8583 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/message.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/auth/__init__.py
--rw-r--r--   0        0        0     1303 2024-04-08 10:39:34.375280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/auth/index.py
--rw-r--r--   0        0        0      775 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/auth_token.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/config/__init__.py
--rw-r--r--   0        0        0     1136 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/config/index.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/humans/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/humans/index.py
--rw-r--r--   0        0        0     5482 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/interface.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/models/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/models/index.py
--rw-r--r--   0        0        0    23956 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/openai_assistants/assistants.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/personas/__init__.py
--rw-r--r--   0        0        0     1795 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/personas/index.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/presets/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/presets/index.py
--rw-r--r--   0        0        0     9580 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/server.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/sources/__init__.py
--rw-r--r--   0        0        0     8218 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/sources/index.py
--rw-r--r--   0        0        0      914 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/static_files.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/tools/__init__.py
--rw-r--r--   0        0        0     2082 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/tools/index.py
--rw-r--r--   0        0        0    63383 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/server.py
--rw-r--r--   0        0        0    43424 2024-04-08 10:39:34.379279 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/assets/index-0c5d3001.css
--rw-r--r--   0        0        0   725155 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/assets/index-bf421135.js
--rw-r--r--   0        0        0    28783 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/favicon.ico
--rw-r--r--   0        0        0     1199 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/index.html
--rw-r--r--   0        0        0    85383 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/memgpt_logo_transparent.png
--rw-r--r--   0        0        0     1667 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/__init__.py
--rw-r--r--   0        0        0     4264 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/example_client.py
--rw-r--r--   0        0        0     4124 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/interface.py
--rw-r--r--   0        0        0     2257 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/protocol.py
--rw-r--r--   0        0        0     6122 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/server.py
--rw-r--r--   0        0        0     7281 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/system.py
--rw-r--r--   0        0        0    31128 2024-04-08 10:39:34.383280 pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/utils.py
--rw-r--r--   0        0        0     2285 2024-04-08 10:39:46.055289 pymemgpt_nightly-0.3.8.dev20240408103946/pyproject.toml
--rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.8.dev20240408103946/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-09 10:39:26.372159 pymemgpt_nightly-0.3.8.dev20240409104037/LICENSE
+-rw-r--r--   0        0        0     8441 2024-04-09 10:39:26.372159 pymemgpt_nightly-0.3.8.dev20240409104037/README.md
+-rw-r--r--   0        0        0      108 2024-04-09 10:40:37.497088 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/__main__.py
+-rw-r--r--   0        0        0    55439 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent.py
+-rw-r--r--   0        0        0    10728 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/chroma.py
+-rw-r--r--   0        0        0    25552 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/db.py
+-rw-r--r--   0        0        0     5288 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/lancedb.py
+-rw-r--r--   0        0        0     6390 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/storage.py
+-rw-r--r--   0        0        0      169 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/agent_autoreply.py
+-rw-r--r--   0        0        0     6813 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/agent_docs.py
+-rw-r--r--   0        0        0     7929 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/agent_groupchat.py
+-rw-r--r--   0        0        0     7375 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
+-rw-r--r--   0        0        0     9346 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/interface.py
+-rw-r--r--   0        0        0    20931 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/memgpt_agent.py
+-rw-r--r--   0        0        0     3644 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/benchmark/benchmark.py
+-rw-r--r--   0        0        0      536 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/benchmark/constants.py
+-rw-r--r--   0        0        0    34724 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/cli/cli.py
+-rw-r--r--   0        0        0    40445 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/cli/cli_config.py
+-rw-r--r--   0        0        0    10453 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/cli/cli_load.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/client/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/client/admin.py
+-rw-r--r--   0        0        0    26894 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/client/client.py
+-rw-r--r--   0        0        0    18729 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/config.py
+-rw-r--r--   0        0        0      390 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/configs/memgpt_hosted.json
+-rw-r--r--   0        0        0      373 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/configs/openai.json
+-rw-r--r--   0        0        0     5364 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/constants.py
+-rw-r--r--   0        0        0     4904 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/credentials.py
+-rw-r--r--   0        0        0     9529 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/data_sources/connectors.py
+-rw-r--r--   0        0        0    23711 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/data_types.py
+-rw-r--r--   0        0        0     7601 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/embeddings.py
+-rw-r--r--   0        0        0      820 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/errors.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/function_sets/base.py
+-rw-r--r--   0        0        0     4629 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/function_sets/extras.py
+-rw-r--r--   0        0        0     7403 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/functions.py
+-rw-r--r--   0        0        0     5433 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/schema_generator.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/humans/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/humans/examples/basic.txt
+-rw-r--r--   0        0        0      305 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/humans/examples/cs_phd.txt
+-rw-r--r--   0        0        0    12994 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/interface.py
+-rw-r--r--   0        0        0    21252 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/llm_api_tools.py
+-rw-r--r--   0        0        0      175 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/__init__.py
+-rw-r--r--   0        0        0    13519 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/chat_completion_proxy.py
+-rw-r--r--   0        0        0      912 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/constants.py
+-rw-r--r--   0        0        0     2788 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/function_parser.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.380159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/__init__.py
+-rw-r--r--   0        0        0    56322 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/gbnf_grammar_generator.py
+-rw-r--r--   0        0        0      667 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/json.gbnf
+-rw-r--r--   0        0        0     3255 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
+-rw-r--r--   0        0        0     3562 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/groq/api.py
+-rw-r--r--   0        0        0     7434 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/json_parser.py
+-rw-r--r--   0        0        0     2586 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/koboldcpp/api.py
+-rw-r--r--   0        0        0      557 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/koboldcpp/settings.py
+-rw-r--r--   0        0        0     2492 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llamacpp/api.py
+-rw-r--r--   0        0        0      548 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llamacpp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
+-rw-r--r--   0        0        0    19913 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
+-rw-r--r--   0        0        0    21281 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
+-rw-r--r--   0        0        0    19975 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
+-rw-r--r--   0        0        0    10300 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
+-rw-r--r--   0        0        0     6144 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
+-rw-r--r--   0        0        0      419 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
+-rw-r--r--   0        0        0    14956 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
+-rw-r--r--   0        0        0     4630 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/lmstudio/api.py
+-rw-r--r--   0        0        0      857 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/lmstudio/settings.py
+-rw-r--r--   0        0        0     3660 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/ollama/api.py
+-rw-r--r--   0        0        0      894 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/ollama/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/deterministic_mirostat.py
+-rw-r--r--   0        0        0     3058 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/settings.py
+-rw-r--r--   0        0        0      719 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/simple.py
+-rw-r--r--   0        0        0     4846 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/utils.py
+-rw-r--r--   0        0        0     2612 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/vllm/api.py
+-rw-r--r--   0        0        0     2658 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/api.py
+-rw-r--r--   0        0        0     2354 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/legacy_api.py
+-rw-r--r--   0        0        0      579 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/legacy_settings.py
+-rw-r--r--   0        0        0      593 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/settings.py
+-rw-r--r--   0        0        0     1211 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/log.py
+-rw-r--r--   0        0        0    19997 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/main.py
+-rw-r--r--   0        0        0    19653 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/memory.py
+-rw-r--r--   0        0        0    29420 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/metadata.py
+-rw-r--r--   0        0        0    31537 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/migrate.py
+-rw-r--r--   0        0        0     2517 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/chat_completion_request.py
+-rw-r--r--   0        0        0     1562 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/chat_completion_response.py
+-rw-r--r--   0        0        0      356 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/embedding_response.py
+-rw-r--r--   0        0        0     7977 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/openai.py
+-rw-r--r--   0        0        0     8957 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/pydantic_models.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/openai_backcompat/__init__.py
+-rw-r--r--   0        0        0    13692 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/openai_backcompat/openai_object.py
+-rw-r--r--   0        0        0     5882 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/persistence_manager.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/anna_pa.txt
+-rw-r--r--   0        0        0     1196 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/google_search_persona.txt
+-rw-r--r--   0        0        0      431 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/memgpt_doc.txt
+-rw-r--r--   0        0        0      164 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/memgpt_starter.txt
+-rw-r--r--   0        0        0     1236 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sam.txt
+-rw-r--r--   0        0        0     1171 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sam_pov.txt
+-rw-r--r--   0        0        0     1053 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sam_simple_pov_gpt35.txt
+-rw-r--r--   0        0        0     8192 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sqldb/test.db
+-rw-r--r--   0        0        0      248 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/examples/memgpt_chat.yaml
+-rw-r--r--   0        0        0      247 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/examples/memgpt_docs.yaml
+-rw-r--r--   0        0        0      374 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/examples/memgpt_extras.yaml
+-rw-r--r--   0        0        0     7575 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/presets.py
+-rw-r--r--   0        0        0     2789 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/utils.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/__init__.py
+-rw-r--r--   0        0        0    12907 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/gpt_functions.py
+-rw-r--r--   0        0        0     1139 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/gpt_summarize.py
+-rw-r--r--   0        0        0     1045 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/gpt_system.py
+-rw-r--r--   0        0        0     4758 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_base.txt
+-rw-r--r--   0        0        0     5479 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_chat.txt
+-rw-r--r--   0        0        0     1057 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_chat_compressed.txt
+-rw-r--r--   0        0        0     4819 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_doc.txt
+-rw-r--r--   0        0        0     5047 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_gpt35_extralong.txt
+-rw-r--r--   0        0        0     2967 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
+-rw-r--r--   0        0        0     4663 2024-04-09 10:39:26.384159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_modified_chat.txt
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/constants.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/admin/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/admin/users.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/command.py
+-rw-r--r--   0        0        0     6138 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/config.py
+-rw-r--r--   0        0        0     5114 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/index.py
+-rw-r--r--   0        0        0     7640 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/memory.py
+-rw-r--r--   0        0        0     8583 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/message.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/auth/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/auth/index.py
+-rw-r--r--   0        0        0      775 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/auth_token.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/config/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/config/index.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/humans/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/humans/index.py
+-rw-r--r--   0        0        0     5482 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/interface.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/models/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/models/index.py
+-rw-r--r--   0        0        0    23956 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/openai_assistants/assistants.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/personas/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/personas/index.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/presets/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/presets/index.py
+-rw-r--r--   0        0        0     9580 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/sources/__init__.py
+-rw-r--r--   0        0        0     8218 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/sources/index.py
+-rw-r--r--   0        0        0      914 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/tools/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/tools/index.py
+-rw-r--r--   0        0        0    63646 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/server.py
+-rw-r--r--   0        0        0    43424 2024-04-09 10:39:26.388159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/assets/index-0c5d3001.css
+-rw-r--r--   0        0        0   725155 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/assets/index-bf421135.js
+-rw-r--r--   0        0        0    28783 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/favicon.ico
+-rw-r--r--   0        0        0     1199 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/index.html
+-rw-r--r--   0        0        0    85383 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/memgpt_logo_transparent.png
+-rw-r--r--   0        0        0     1667 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/utils.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/example_client.py
+-rw-r--r--   0        0        0     4124 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/interface.py
+-rw-r--r--   0        0        0     2257 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/protocol.py
+-rw-r--r--   0        0        0     6122 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/server.py
+-rw-r--r--   0        0        0     7281 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/system.py
+-rw-r--r--   0        0        0    31128 2024-04-09 10:39:26.392159 pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/utils.py
+-rw-r--r--   0        0        0     2285 2024-04-09 10:40:37.497088 pymemgpt_nightly-0.3.8.dev20240409104037/pyproject.toml
+-rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.8.dev20240409104037/PKG-INFO
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/LICENSE` & `pymemgpt_nightly-0.3.8.dev20240409104037/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/README.md` & `pymemgpt_nightly-0.3.8.dev20240409104037/README.md`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         self.agent_state = init_agent_state
 
         # gpt-4, gpt-3.5-turbo, ...
         self.model = self.agent_state.llm_config.model
 
         # Store the system instructions (used to rebuild memory)
         if "system" not in self.agent_state.state:
-            raise ValueError(f"'system' not found in provided AgentState")
+            raise ValueError("'system' not found in provided AgentState")
         self.system = self.agent_state.state["system"]
 
         if "functions" not in self.agent_state.state:
             raise ValueError(f"'functions' not found in provided AgentState")
         # Store the functions schemas (this is passed as an argument to ChatCompletion)
         self.functions = self.agent_state.state["functions"]  # these are the schema
         # Link the actual python functions corresponding to the schemas
@@ -1097,11 +1097,11 @@
 
 def save_agent(agent: Agent, ms: MetadataStore):
     """Save agent to metadata store"""
 
     agent.update_state()
     agent_state = agent.agent_state
 
-    if ms.get_agent(agent_id=agent_state.id):
+    if ms.get_agent(agent_name=agent_state.name, user_id=agent_state.user_id):
         ms.update_agent(agent_state)
     else:
         ms.create_agent(agent_state)
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/chroma.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/chroma.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/db.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/db.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/lancedb.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/agent_store/storage.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/agent_store/storage.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/agent_autoreply.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/agent_autoreply.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/agent_docs.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/agent_docs.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/agent_groupchat.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/agent_groupchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
 
 # If USE_MEMGPT is False, then this example will be the same as the official AutoGen repo
 # (https://github.com/microsoft/autogen/blob/main/notebook/agentchat_groupchat.ipynb)
 # If USE_MEMGPT is True, then we swap out the "coder" agent with a MemGPT agent
 USE_MEMGPT = True
 
 # Set to True if you want to print MemGPT's inner workings.
-DEBUG = False
+# DEBUG = False
+DEBUG = True
 
 interface_kwargs = {
     "debug": DEBUG,
     "show_inner_thoughts": True,
     "show_function_outputs": DEBUG,
 }
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/examples/memgpt_coder_autogen.ipynb` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/examples/memgpt_coder_autogen.ipynb`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/interface.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,25 +62,25 @@
         self.show_function_outputs = show_function_outputs
         self.debug = debug
 
     def reset_message_list(self):
         """Clears the buffer. Call before every agent.step() when using MemGPT+AutoGen"""
         self.message_list = []
 
-    def internal_monologue(self, msg: str, msg_obj: Optional[Message]):
+    def internal_monologue(self, msg: str, msg_obj: Optional[Message] = None):
         # NOTE: never gets appended
         if self.debug:
             print(f"inner thoughts :: {msg}")
         if not self.show_inner_thoughts:
             return
         # ANSI escape code for italic is '\x1B[3m'
         message = f"\x1B[3m{Fore.LIGHTBLACK_EX}💭 {msg}{Style.RESET_ALL}" if self.fancy else f"[MemGPT agent's inner thoughts] {msg}"
         print(message)
 
-    def assistant_message(self, msg: str, msg_obj: Optional[Message]):
+    def assistant_message(self, msg: str, msg_obj: Optional[Message] = None):
         # NOTE: gets appended
         if self.debug:
             print(f"assistant :: {msg}")
         # message = f"{Fore.YELLOW}{Style.BRIGHT}🤖 {Fore.YELLOW}{msg}{Style.RESET_ALL}" if self.fancy else msg
         self.message_list.append(msg)
 
     def memory_message(self, msg: str):
@@ -96,15 +96,15 @@
         # NOTE: gets appended
         if self.debug:
             print(f"system :: {msg}")
         message = f"{Fore.MAGENTA}{Style.BRIGHT}🖥️ [system] {Fore.MAGENTA}{msg}{Style.RESET_ALL}" if self.fancy else f"[system] {msg}"
         print(message)
         self.message_list.append(msg)
 
-    def user_message(self, msg: str, msg_obj: Optional[Message], raw=False):
+    def user_message(self, msg: str, msg_obj: Optional[Message] = None, raw=False):
         if self.debug:
             print(f"user :: {msg}")
         if not self.show_user_message:
             return
 
         if isinstance(msg, str):
             if raw:
@@ -134,15 +134,15 @@
             message = f"{Fore.GREEN}{Style.BRIGHT}🖥️ {Fore.GREEN}{msg_json}{Style.RESET_ALL}" if self.fancy else f"[system] {msg}"
         else:
             message = f"{Fore.GREEN}{Style.BRIGHT}🧑 {Fore.GREEN}{msg_json}{Style.RESET_ALL}" if self.fancy else f"[user] {msg}"
 
         # TODO should we ever be appending this?
         self.message_list.append(message)
 
-    def function_message(self, msg: str, msg_obj: Optional[Message]):
+    def function_message(self, msg: str, msg_obj: Optional[Message] = None):
         if self.debug:
             print(f"function :: {msg}")
         if not self.show_function_outputs:
             return
 
         if isinstance(msg, dict):
             message = f"{Fore.RED}{Style.BRIGHT}⚡ [function] {Fore.RED}{msg}{Style.RESET_ALL}"
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/autogen/memgpt_agent.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/autogen/memgpt_agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/benchmark/benchmark.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/benchmark/constants.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/cli/cli.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/cli/cli_config.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/cli/cli_load.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/cli/cli_load.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/client/admin.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/client/admin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/client/client.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,17 @@
 
     # tools
 
     def list_tools(self):
         """List all tools."""
         raise NotImplementedError
 
-    def create_tool(self, name: str, source_code: str, source_type: str, tags: Optional[List[str]] = None):
+    def create_tool(
+        self, name: str, file_path: str, source_type: Optional[str] = "python", tags: Optional[List[str]] = None
+    ) -> CreateToolResponse:
         """Create a tool."""
         raise NotImplementedError
 
     # data sources
 
     def list_sources(self):
         """List loaded sources"""
@@ -417,25 +419,14 @@
         data = {"name": name, "text": persona}
         response = requests.post(f"{self.base_url}/api/personas", json=data, headers=self.headers)
         if response.status_code != 200:
             raise ValueError(f"Failed to create persona: {response.text}")
         print(response.json())
         return PersonaModel(**response.json())
 
-    # tools
-
-    def list_tools(self) -> ListToolsResponse:
-        response = requests.get(f"{self.base_url}/api/tools", headers=self.headers)
-        return ListToolsResponse(**response.json())
-
-    def create_tool(self, name: str, source_code: str, source_type: str, tags: Optional[List[str]] = None) -> CreateToolResponse:
-        data = {"name": name, "source_code": source_code, "source_type": source_type, "tags": tags}
-        response = requests.post(f"{self.base_url}/api/tools", json=data, headers=self.headers)
-        return CreateToolResponse(**response.json())
-
     # sources
 
     def list_sources(self):
         """List loaded sources"""
         response = requests.get(f"{self.base_url}/api/sources", headers=self.headers)
         response_json = response.json()
         return ListSourcesResponse(**response_json)
@@ -485,14 +476,31 @@
         response = requests.get(f"{self.base_url}/api/models", headers=self.headers)
         return ListModelsResponse(**response.json())
 
     def get_config(self) -> ConfigResponse:
         response = requests.get(f"{self.base_url}/api/config", headers=self.headers)
         return ConfigResponse(**response.json())
 
+    # tools
+
+    def create_tool(
+        self, name: str, file_path: str, source_type: Optional[str] = "python", tags: Optional[List[str]] = None
+    ) -> CreateToolResponse:
+        """Add a tool implemented in a file path"""
+        source_code = open(file_path, "r").read()
+        data = {"name": name, "source_code": source_code, "source_type": source_type, "tags": tags}
+        response = requests.post(f"{self.base_url}/api/tools", json=data, headers=self.headers)
+        if response.status_code != 200:
+            raise ValueError(f"Failed to create tool: {response.text}")
+        return CreateToolResponse(**response.json())
+
+    def list_tools(self) -> ListToolsResponse:
+        response = requests.get(f"{self.base_url}/api/tools", headers=self.headers)
+        return ListToolsResponse(**response.json())
+
 
 class LocalClient(AbstractClient):
     def __init__(
         self,
         auto_save: bool = False,
         user_id: Optional[str] = None,
         debug: bool = False,
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/config.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/constants.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/credentials.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/data_sources/connectors.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/data_sources/connectors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/data_types.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/data_types.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/embeddings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/embeddings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/errors.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/errors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/function_sets/base.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/function_sets/base.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/function_sets/extras.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/function_sets/extras.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/functions.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,55 @@
             }
 
     if len(function_dict) == 0:
         raise ValueError(f"No functions found in module {module}")
     return function_dict
 
 
+def validate_function(module_name, module_full_path):
+    try:
+        file = os.path.basename(module_full_path)
+        spec = importlib.util.spec_from_file_location(module_name, module_full_path)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+    except ModuleNotFoundError as e:
+        # Handle missing module imports
+        missing_package = str(e).split("'")[1]  # Extract the name of the missing package
+        print(f"{CLI_WARNING_PREFIX}skipped loading python file '{module_full_path}'!")
+        return (
+            False,
+            f"'{file}' imports '{missing_package}', but '{missing_package}' is not installed locally - install python package '{missing_package}' to link functions from '{file}' to MemGPT.",
+        )
+    except SyntaxError as e:
+        # Handle syntax errors in the module
+        return False, f"{CLI_WARNING_PREFIX}skipped loading python file '{file}' due to a syntax error: {e}"
+    except Exception as e:
+        # Handle other general exceptions
+        return False, f"{CLI_WARNING_PREFIX}skipped loading python file '{file}': {e}"
+
+    return True, None
+
+
+def write_function(module_name: str, function_name: str, function_code: str):
+    """Write a function to a file in the user functions directory"""
+    # Create the user functions directory if it doesn't exist
+    if not os.path.exists(USER_FUNCTIONS_DIR):
+        os.makedirs(USER_FUNCTIONS_DIR)
+
+    # Write the function to a file
+    file_path = os.path.join(USER_FUNCTIONS_DIR, f"{module_name}.py")
+    with open(file_path, "a") as f:
+        f.write(function_code)
+    succ, error = validate_function(module_name, file_path)
+
+    # raise error if function cannot be loaded
+    if not succ:
+        raise ValueError(error)
+
+
 def load_all_function_sets(merge: bool = True) -> dict:
     # functions/examples/*.py
     scripts_dir = os.path.dirname(os.path.abspath(__file__))  # Get the directory of the current script
     function_sets_dir = os.path.join(scripts_dir, "function_sets")  # Path to the function_sets directory
     # List all .py files in the directory (excluding __init__.py)
     example_module_files = [f for f in os.listdir(function_sets_dir) if f.endswith(".py") and f != "__init__.py"]
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/functions/schema_generator.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/functions/schema_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/interface.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/llm_api_tools.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/llm_api_tools.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/chat_completion_proxy.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/chat_completion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/constants.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/function_parser.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/function_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/gbnf_grammar_generator.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/gbnf_grammar_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/json.gbnf` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/groq/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/groq/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/json_parser.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/json_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/koboldcpp/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/koboldcpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/koboldcpp/settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/koboldcpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llamacpp/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llamacpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llamacpp/settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llamacpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/lmstudio/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/lmstudio/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/lmstudio/settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/lmstudio/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/ollama/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/ollama/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/ollama/settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/ollama/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/deterministic_mirostat.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/deterministic_mirostat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/settings/simple.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/settings/simple.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/utils.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/vllm/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/vllm/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/legacy_api.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/legacy_api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/legacy_settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/legacy_settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/local_llm/webui/settings.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/local_llm/webui/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/log.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/log.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/main.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import typer
 
 from rich.console import Console
 from memgpt.constants import FUNC_FAILED_HEARTBEAT_MESSAGE, JSON_ENSURE_ASCII, JSON_LOADS_STRICT, REQ_HEARTBEAT_MESSAGE
 
 console = Console()
 
+from memgpt.agent import save_agent
 from memgpt.agent_store.storage import StorageConnector, TableType
 from memgpt.interface import CLIInterface as interface  # for printing to terminal
 from memgpt.config import MemGPTConfig
 import memgpt.agent as agent
 import memgpt.system as system
 import memgpt.errors as errors
 from memgpt.cli.cli import run, version, server, open_folder, quickstart, migrate, delete_agent
@@ -188,15 +189,17 @@
                     if n_messages <= MIN_MESSAGES:
                         print(f"Agent only has {n_messages} messages in stack, none left to pop")
                     elif n_messages - pop_amount < MIN_MESSAGES:
                         print(f"Agent only has {n_messages} messages in stack, cannot pop more than {n_messages - MIN_MESSAGES}")
                     else:
                         print(f"Popping last {pop_amount} messages from stack")
                         for _ in range(min(pop_amount, len(memgpt_agent.messages))):
-                            memgpt_agent.messages.pop()
+                            memgpt_agent._messages.pop()
+                        # Persist the state
+                        save_agent(agent=memgpt_agent, ms=ms)
                     continue
 
                 elif user_input.lower() == "/retry":
                     # TODO this needs to also modify the persistence manager
                     print(f"Retrying for another answer")
                     while len(memgpt_agent.messages) > 0:
                         if memgpt_agent.messages[-1].get("role") == "user":
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/memory.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/metadata.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,15 @@
                 SourceModel.__table__,
                 AgentSourceMappingModel.__table__,
                 TokenModel.__table__,
                 PresetModel.__table__,
                 PresetSourceMapping.__table__,
                 HumanModel.__table__,
                 PersonaModel.__table__,
+                ToolModel.__table__,
             ],
         )
         self.session_maker = sessionmaker(bind=self.engine)
 
     @enforce_types
     def create_api_key(self, user_id: uuid.UUID, name: Optional[str] = None) -> Token:
         """Create an API key for a user"""
@@ -681,14 +682,20 @@
     @enforce_types
     def add_preset(self, preset: PresetModel):
         with self.session_maker() as session:
             session.add(preset)
             session.commit()
 
     @enforce_types
+    def add_tool(self, tool: ToolModel):
+        with self.session_maker() as session:
+            session.add(tool)
+            session.commit()
+
+    @enforce_types
     def get_human(self, name: str, user_id: uuid.UUID) -> Optional[HumanModel]:
         with self.session_maker() as session:
             results = session.query(HumanModel).filter(HumanModel.name == name).filter(HumanModel.user_id == user_id).all()
             if len(results) == 0:
                 return None
             assert len(results) == 1, f"Expected 1 result, got {len(results)}"
             return results[0]
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/migrate.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/migrate.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/chat_completion_request.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/chat_completion_response.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/openai.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/models/pydantic_models.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/models/pydantic_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,22 +40,42 @@
     persona: str = Field(default=get_persona_text(DEFAULT_PERSONA), description="The persona of the preset.")
     persona_name: Optional[str] = Field(None, description="The name of the persona of the preset.")
     human: str = Field(default=get_human_text(DEFAULT_HUMAN), description="The human of the preset.")
     human_name: Optional[str] = Field(None, description="The name of the human of the preset.")
     functions_schema: List[Dict] = Field(..., description="The functions schema of the preset.")
 
 
-class ToolModel(BaseModel):
+class ToolModel(SQLModel, table=True):
     # TODO move into database
     name: str = Field(..., description="The name of the function.")
-    json_schema: dict = Field(..., description="The JSON schema of the function.")
-    tags: List[str] = Field(..., description="Metadata tags.")
-    source_type: Optional[Literal["python"]] = Field(None, description="The type of the source code.")
+    id: uuid.UUID = Field(default_factory=uuid.uuid4, description="The unique identifier of the function.", primary_key=True)
+    tags: List[str] = Field(sa_column=Column(JSON), description="Metadata tags.")
+    source_type: Optional[str] = Field(None, description="The type of the source code.")
     source_code: Optional[str] = Field(..., description="The source code of the function.")
 
+    json_schema: Dict = Field(default_factory=dict, sa_column=Column(JSON), description="The JSON schema of the function.")
+
+    # Needed for Column(JSON)
+    class Config:
+        arbitrary_types_allowed = True
+
+
+class AgentToolMap(SQLModel, table=True):
+    # mapping between agents and tools
+    agent_id: uuid.UUID = Field(..., description="The unique identifier of the agent.")
+    tool_id: uuid.UUID = Field(..., description="The unique identifier of the tool.")
+    id: uuid.UUID = Field(default_factory=uuid.uuid4, description="The unique identifier of the agent-tool map.", primary_key=True)
+
+
+class PresetToolMap(SQLModel, table=True):
+    # mapping between presets and tools
+    preset_id: uuid.UUID = Field(..., description="The unique identifier of the preset.")
+    tool_id: uuid.UUID = Field(..., description="The unique identifier of the tool.")
+    id: uuid.UUID = Field(default_factory=uuid.uuid4, description="The unique identifier of the preset-tool map.", primary_key=True)
+
 
 class AgentStateModel(BaseModel):
     id: uuid.UUID = Field(..., description="The unique identifier of the agent.")
     name: str = Field(..., description="The name of the agent.")
     description: Optional[str] = Field(None, description="The description of the agent.")
     user_id: uuid.UUID = Field(..., description="The unique identifier of the user associated with the agent.")
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/openai_backcompat/openai_object.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/openai_backcompat/openai_object.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/persistence_manager.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/anna_pa.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/anna_pa.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/google_search_persona.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/google_search_persona.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sam.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sam.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sam_pov.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sam_pov.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sam_simple_pov_gpt35.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sam_simple_pov_gpt35.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/personas/examples/sqldb/test.db` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/personas/examples/sqldb/test.db`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/presets.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/presets.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/presets/utils.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/presets/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/gpt_functions.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/gpt_functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/gpt_summarize.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/gpt_summarize.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/gpt_system.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/gpt_system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_base.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_base.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_chat.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_chat_compressed.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_chat_compressed.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_doc.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_doc.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_gpt35_extralong.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_gpt35_extralong.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_intuitive_knowledge.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_intuitive_knowledge.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/prompts/system/memgpt_modified_chat.txt` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/prompts/system/memgpt_modified_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/admin/users.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/admin/users.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/command.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/command.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/config.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/memory.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/agents/message.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/agents/message.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/auth/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/auth/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/auth_token.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/auth_token.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/config/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/config/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/humans/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/humans/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/interface.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/models/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/models/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/openai_assistants/assistants.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/openai_assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/personas/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/personas/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/presets/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/presets/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/server.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/sources/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/sources/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/static_files.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/static_files.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/rest_api/tools/index.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/rest_api/tools/index.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,10 +47,20 @@
     async def create_tool(
         request: CreateToolRequest = Body(...),
         user_id: uuid.UUID = Depends(get_current_user_with_server),
     ):
         """
         Create a new tool (dummy route)
         """
+        from memgpt.functions.functions import write_function
+
+        # write function to ~/.memgt/functions directory
+        write_function(request.name, request.name, request.source_code)
+
+        print("adding tool", request.name, request.tags, request.source_code)
+        tool = ToolModel(name=request.name, json_schema={}, tags=request.tags, source_code=request.source_code)
+        server.ms.add_tool(tool)
+
+        # TODO: insert tool information into DB as ToolModel
         return CreateToolResponse(tool=ToolModel(name=request.name, json_schema={}, tags=[], source_code=request.source_code))
 
     return router
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/server.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     LLMConfig,
     EmbeddingConfig,
     Message,
     Token,
     Preset,
 )
 
-from memgpt.models.pydantic_models import SourceModel, PassageModel, DocumentModel, PresetModel
+from memgpt.models.pydantic_models import SourceModel, PassageModel, DocumentModel, PresetModel, ToolModel
 from memgpt.interface import AgentInterface  # abstract
 
 # TODO use custom interface
 from memgpt.interface import CLIInterface  # for printing to terminal
 from memgpt.metadata import MetadataStore
 
 logger = logging.getLogger(__name__)
@@ -1387,7 +1387,15 @@
                 num_passages=num_passages,
                 attached_agents=attached_agents,
             )
 
             sources_with_metadata.append(source)
 
         return sources_with_metadata
+
+    def create_tool(self, name: str, user_id: uuid.UUID) -> ToolModel:  # TODO: add other fields
+        """Create a new tool"""
+        pass
+
+    def delete_tool(self, tool_id: uuid.UUID, user_id: uuid.UUID):
+        """Delete a tool"""
+        pass
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/assets/index-0c5d3001.css` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/assets/index-0c5d3001.css`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/assets/index-bf421135.js` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/assets/index-bf421135.js`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/favicon.ico` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/index.html` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/index.html`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/static_files/memgpt_logo_transparent.png` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/static_files/memgpt_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/utils.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/example_client.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/example_client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/interface.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/protocol.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/protocol.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/server/ws_api/server.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/server/ws_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/system.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/memgpt/utils.py` & `pymemgpt_nightly-0.3.8.dev20240409104037/memgpt/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/pyproject.toml` & `pymemgpt_nightly-0.3.8.dev20240409104037/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymemgpt-nightly"
-version = "0.3.8.dev20240408103946"
+version = "0.3.8.dev20240409104037"
 packages = [
     {include = "memgpt"}
 ]
 description = "Teaching LLMs memory management for unbounded context"
 authors = [
     "MemGPT Team <hi@memgpt.ai>",
 ]
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240408103946/PKG-INFO` & `pymemgpt_nightly-0.3.8.dev20240409104037/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemgpt-nightly
-Version: 0.3.8.dev20240408103946
+Version: 0.3.8.dev20240409104037
 Summary: Teaching LLMs memory management for unbounded context
 License: Apache License
 Author: MemGPT Team
 Author-email: hi@memgpt.ai
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.8.dev20240408103946
+Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.8.dev20240409104037
 Summary: Teaching LLMs memory management for unbounded context License: Apache
 License Author: MemGPT Team Author-email: hi@memgpt.ai Requires-Python:
 >=3.10,<3.13 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: autogen Provides-Extra:
 dev Provides-Extra: local Provides-Extra: postgres Provides-Extra: server
```

