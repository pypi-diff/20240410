# Comparing `tmp/r2r-0.1.32.tar.gz` & `tmp/r2r-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.1.32.tar", max compression
+gzip compressed data, was "r2r-0.1.33.tar", max compression
```

## Comparing `r2r-0.1.32.tar` & `r2r-0.1.33.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1082 2024-04-10 05:26:32.861240 r2r-0.1.32/LICENSE.md
--rw-r--r--   0        0        0     7112 2024-04-10 05:26:32.861240 r2r-0.1.32/README.md
--rw-r--r--   0        0        0      680 2024-04-10 05:26:32.861240 r2r-0.1.32/config.json
--rw-r--r--   0        0        0     2216 2024-04-10 05:26:32.893240 r2r-0.1.32/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/__init__.py
--rw-r--r--   0        0        0       53 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/client/__init__.py
--rw-r--r--   0        0        0     5956 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/client/base.py
--rw-r--r--   0        0        0     1123 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/__init__.py
--rw-r--r--   0        0        0      110 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      781 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/abstractions/output.py
--rw-r--r--   0        0        0      249 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/adapters/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/adapters/advanced/reducto.py
--rw-r--r--   0        0        0     2803 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/adapters/base.py
--rw-r--r--   0        0        0     2407 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/embedding.py
--rw-r--r--   0        0        0     1334 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/eval.py
--rw-r--r--   0        0        0     2175 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/ingestion.py
--rw-r--r--   0        0        0     1515 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/pipeline.py
--rw-r--r--   0        0        0     6227 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/rag.py
--rw-r--r--   0        0        0      935 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/providers/embedding.py
--rw-r--r--   0        0        0     1015 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/eval.py
--rw-r--r--   0        0        0     1808 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/llm.py
--rw-r--r--   0        0        0    11873 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/logging.py
--rw-r--r--   0        0        0     1249 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/prompt.py
--rw-r--r--   0        0        0     3833 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/vector_db.py
--rw-r--r--   0        0        0      256 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/base.py
--rw-r--r--   0        0        0       95 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66651 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      203 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     1676 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/modal/base.py
--rw-r--r--   0        0        0     3311 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/openai/base.py
--rw-r--r--   0        0        0     1923 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/setence_transformer/base.py
--rw-r--r--   0        0        0      139 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/eval/deepeval/base.py
--rw-r--r--   0        0        0     2710 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/eval/parea/base.py
--rw-r--r--   0        0        0        0 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/__init__.py
--rw-r--r--   0        0        0     3244 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/run_basic_client.py
--rw-r--r--   0        0        0     4249 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/run_basic_client_old.py
--rw-r--r--   0        0        0     1625 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/run_synthetic_query_client.py
--rw-r--r--   0        0        0      689 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/configs/local_llama_cpp.json
--rw-r--r--   0        0        0      687 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/configs/local_ollama.json
--rw-r--r--   0        0        0   802904 2024-04-10 05:26:32.901240 r2r-0.1.32/r2r/examples/data/meditations.pdf
--rw-r--r--   0        0        0    14812 2024-04-10 05:26:32.901240 r2r-0.1.32/r2r/examples/data/test.pdf
--rw-r--r--   0        0        0  1307590 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/data/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0      975 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/basic_pipeline.py
--rw-r--r--   0        0        0      533 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/reducto_pipeline.py
--rw-r--r--   0        0        0     6746 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/synthetic_query_pipeline.py
--rw-r--r--   0        0        0      504 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/web_search_pipeline.py
--rw-r--r--   0        0        0      101 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1184 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3905 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/serper.py
--rw-r--r--   0        0        0      277 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3602 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/litellm/base.py
--rw-r--r--   0        0        0     4467 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/llama_cpp/base.py
--rw-r--r--   0        0        0        0 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3794 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/openai/base.py
--rw-r--r--   0        0        0      217 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/__init__.py
--rw-r--r--   0        0        0    16309 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/app.py
--rw-r--r--   0        0        0     5108 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/factory.py
--rw-r--r--   0        0        0     3280 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/models.py
--rw-r--r--   0        0        0    10797 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/main/utils.py
--rw-r--r--   0        0        0      541 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/__init__.py
--rw-r--r--   0        0        0     5948 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/embedding.py
--rw-r--r--   0        0        0     1830 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/eval.py
--rw-r--r--   0        0        0     2978 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/ingestion.py
--rw-r--r--   0        0        0     1002 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/prompt_provider.py
--rw-r--r--   0        0        0     3079 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/rag.py
--rw-r--r--   0        0        0     2392 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/web_search/rag.py
--rw-r--r--   0        0        0     6035 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/tests/end_to_end.py
--rw-r--r--   0        0        0    14812 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/tests/test.pdf
--rw-r--r--   0        0        0      539 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5299 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9298 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/client.py
--rw-r--r--   0        0        0    35441 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/exc.py
--rw-r--r--   0        0        0      166 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/local/base.py
--rw-r--r--   0        0        0     5607 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/pg_vector/base.py
--rw-r--r--   0        0        0     7125 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/qdrant/base.py
--rw-r--r--   0        0        0     9587 1970-01-01 00:00:00.000000 r2r-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-10 06:00:09.599917 r2r-0.1.33/LICENSE.md
+-rw-r--r--   0        0        0     7175 2024-04-10 06:00:09.599917 r2r-0.1.33/README.md
+-rw-r--r--   0        0        0      680 2024-04-10 06:00:09.599917 r2r-0.1.33/config.json
+-rw-r--r--   0        0        0     2217 2024-04-10 06:00:09.631916 r2r-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/client/__init__.py
+-rw-r--r--   0        0        0     5956 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/client/base.py
+-rw-r--r--   0        0        0     1123 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      781 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/abstractions/output.py
+-rw-r--r--   0        0        0      249 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2928 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/adapters/advanced/reducto.py
+-rw-r--r--   0        0        0     2803 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/adapters/base.py
+-rw-r--r--   0        0        0     2407 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/pipelines/embedding.py
+-rw-r--r--   0        0        0     1334 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/pipelines/eval.py
+-rw-r--r--   0        0        0     2175 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/pipelines/ingestion.py
+-rw-r--r--   0        0        0     1515 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/pipelines/pipeline.py
+-rw-r--r--   0        0        0     6227 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/pipelines/rag.py
+-rw-r--r--   0        0        0      935 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/providers/embedding.py
+-rw-r--r--   0        0        0     1015 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/providers/eval.py
+-rw-r--r--   0        0        0     1808 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/providers/llm.py
+-rw-r--r--   0        0        0    11873 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/providers/logging.py
+-rw-r--r--   0        0        0     1249 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/providers/prompt.py
+-rw-r--r--   0        0        0     3833 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/providers/vector_db.py
+-rw-r--r--   0        0        0      256 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/utils/base.py
+-rw-r--r--   0        0        0       95 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66651 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      203 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/embeddings/modal/base.py
+-rw-r--r--   0        0        0     3311 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/embeddings/openai/base.py
+-rw-r--r--   0        0        0     1923 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/embeddings/setence_transformer/base.py
+-rw-r--r--   0        0        0      139 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/eval/deepeval/base.py
+-rw-r--r--   0        0        0     2710 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/eval/parea/base.py
+-rw-r--r--   0        0        0        0 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/clients/__init__.py
+-rw-r--r--   0        0        0     3244 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/clients/run_basic_client.py
+-rw-r--r--   0        0        0     4249 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/clients/run_basic_client_old.py
+-rw-r--r--   0        0        0     1625 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/clients/run_synthetic_query_client.py
+-rw-r--r--   0        0        0      689 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/configs/local_llama_cpp.json
+-rw-r--r--   0        0        0      687 2024-04-10 06:00:09.635916 r2r-0.1.33/r2r/examples/configs/local_ollama.json
+-rw-r--r--   0        0        0   802904 2024-04-10 06:00:09.639916 r2r-0.1.33/r2r/examples/data/meditations.pdf
+-rw-r--r--   0        0        0    14812 2024-04-10 06:00:09.639916 r2r-0.1.33/r2r/examples/data/test.pdf
+-rw-r--r--   0        0        0  1307590 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/examples/data/the_republic.pdf
+-rw-r--r--   0        0        0        0 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/examples/servers/basic_pipeline.py
+-rw-r--r--   0        0        0      533 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/examples/servers/reducto_pipeline.py
+-rw-r--r--   0        0        0     6746 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/examples/servers/synthetic_query_pipeline.py
+-rw-r--r--   0        0        0      504 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/examples/servers/web_search_pipeline.py
+-rw-r--r--   0        0        0      101 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1184 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3905 2024-04-10 06:00:09.643916 r2r-0.1.33/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      277 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3602 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/llms/litellm/base.py
+-rw-r--r--   0        0        0     4467 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/llms/llama_cpp/base.py
+-rw-r--r--   0        0        0        0 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3794 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/llms/openai/base.py
+-rw-r--r--   0        0        0      217 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/main/__init__.py
+-rw-r--r--   0        0        0    16309 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/main/app.py
+-rw-r--r--   0        0        0     5108 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/main/factory.py
+-rw-r--r--   0        0        0     3280 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/main/models.py
+-rw-r--r--   0        0        0    10797 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/main/utils.py
+-rw-r--r--   0        0        0      541 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/__init__.py
+-rw-r--r--   0        0        0     5948 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/basic/embedding.py
+-rw-r--r--   0        0        0     1830 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/basic/eval.py
+-rw-r--r--   0        0        0     2978 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/basic/ingestion.py
+-rw-r--r--   0        0        0     1002 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/basic/prompt_provider.py
+-rw-r--r--   0        0        0     3079 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/basic/rag.py
+-rw-r--r--   0        0        0     2392 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/pipelines/web_search/rag.py
+-rw-r--r--   0        0        0     6035 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/tests/end_to_end.py
+-rw-r--r--   0        0        0    14812 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/tests/test.pdf
+-rw-r--r--   0        0        0      539 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3269 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5299 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9298 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/client.py
+-rw-r--r--   0        0        0    35441 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      166 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vector_dbs/local/base.py
+-rw-r--r--   0        0        0     5607 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vector_dbs/pg_vector/base.py
+-rw-r--r--   0        0        0     7125 2024-04-10 06:00:09.647916 r2r-0.1.33/r2r/vector_dbs/qdrant/base.py
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 r2r-0.1.33/PKG-INFO
```

### Comparing `r2r-0.1.32/LICENSE.md` & `r2r-0.1.33/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/README.md` & `r2r-0.1.33/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
 # Choose from CONFIG_OPTION in {`default`, `local_ollama`}
 # For cloud deployment, select `default` and place your secrets in `.env`
 # For local deployment, select `local_ollama`
-docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest
+docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama
 
 ```
 
 ## Basic Example
 
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
@@ -81,15 +81,16 @@
    python -m r2r.examples.servers.basic_pipeline
    ```
 
 [`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
    # run the client
-   python -m r2r.examples.clients.run_basic_client
+   python -m r2r.examples.clients.run_basic_client ingest
+   python -m r2r.examples.clients.run_basic_client search --query="What is the meaning of life?"
    ```
 ### Running Basic Local RAG
 
 [Refer here](https://r2r-docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the commands above to use local providers.
 
 ## Synthetic Queries Example
```

#### html2text {}

```diff
@@ -27,33 +27,34 @@
 OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
 LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
 INCLUDE secrets and modify config.json # if using cloud providers (e.g.
 pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
 latest # Choose from CONFIG_OPTION in {`default`, `local_ollama`} # For cloud
 deployment, select `default` and place your secrets in `.env` # For local
 deployment, select `local_ollama` docker run -d --name r2r_container -p 8000:
-8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest ```
-## Basic Example [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py):
-Execute this script to initiate the default **backend server**. It establishes
-a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes,
-all accessible via FastAPI. ```bash # launch the server python -
+8000 -e CONFIG_OPTION=local_ollama ``` ## Basic Example [`basic_pipeline.py`]
+(r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the
+default **backend server**. It establishes a basic RAG pipeline that
+encompasses ingestion, embedding, and RAG processes, all accessible via
+FastAPI. ```bash # launch the server python -
 m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
 clients/run_basic_client.py): This **client script** should be executed
 subsequent to the server startup above. It facilitates the upload of text
 entries and PDFs to the server using the Python client and demonstrates the
 management of document and user-level vectors through its built-in features.
-```bash # run the client python -m r2r.examples.clients.run_basic_client ```
-### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/tutorials/
-local_rag) for a tutorial on how to modify the commands above to use local
-providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/
-examples/servers/synthetic_query_pipeline.py): Execute this script to start a
-backend server equipped with an advanced pipeline. This pipeline is designed to
-create synthetic queries, enhancing the RAG system's learning and performance.
-```bash # launch the server python -
-m r2r.examples.servers.synthetic_query_pipeline ```
+```bash # run the client python -m r2r.examples.clients.run_basic_client ingest
+python -m r2r.examples.clients.run_basic_client search --query="What is the
+meaning of life?" ``` ### Running Basic Local RAG [Refer here](https://r2r-
+docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the
+commands above to use local providers. ## Synthetic Queries Example
+[`synthetic_query_pipeline.py`](r2r/examples/servers/
+synthetic_query_pipeline.py): Execute this script to start a backend server
+equipped with an advanced pipeline. This pipeline is designed to create
+synthetic queries, enhancing the RAG system's learning and performance. ```bash
+# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
 run_synthetic_query_client.py): Use this client script after the synthetic
 query pipeline is running. It's tailored for use with the synthetic query
 pipeline, demonstrating the improved features of the RAG system. ```bash # run
 the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
 Extra Examples [`reducto_pipeline.py`](r2r/examples/servers/
 reducto_pipeline.py): Launch this script to activate a backend server that
```

### Comparing `r2r-0.1.32/config.json` & `r2r-0.1.33/config.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/pyproject.toml` & `r2r-0.1.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.1.32"
+version = "0.1.33"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
 # Python Versions
 python = ">=3.9,<3.13"
 
 # Required dependencies
-bs4= "^0.0.2"
+bs4 = "^0.0.2"
 fastapi = "^0.109.2"
 fire = "^0.5.0"
 gunicorn = "^21.2.0"
 litellm = "^1.34.0"
 openai = "^1.11.1"
 pydantic = "^2.6.3"
 pypdf = "^4.2.0"
```

### Comparing `r2r-0.1.32/r2r/client/base.py` & `r2r-0.1.33/r2r/client/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/__init__.py` & `r2r-0.1.33/r2r/core/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/abstractions/output.py` & `r2r-0.1.33/r2r/core/abstractions/output.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/adapters/advanced/reducto.py` & `r2r-0.1.33/r2r/core/adapters/advanced/reducto.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/adapters/base.py` & `r2r-0.1.33/r2r/core/adapters/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/pipelines/embedding.py` & `r2r-0.1.33/r2r/core/pipelines/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/pipelines/eval.py` & `r2r-0.1.33/r2r/core/pipelines/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/pipelines/ingestion.py` & `r2r-0.1.33/r2r/core/pipelines/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/pipelines/pipeline.py` & `r2r-0.1.33/r2r/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/pipelines/rag.py` & `r2r-0.1.33/r2r/core/pipelines/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/providers/embedding.py` & `r2r-0.1.33/r2r/core/providers/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/providers/eval.py` & `r2r-0.1.33/r2r/core/providers/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/providers/llm.py` & `r2r-0.1.33/r2r/core/providers/llm.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/providers/logging.py` & `r2r-0.1.33/r2r/core/providers/logging.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/providers/prompt.py` & `r2r-0.1.33/r2r/core/providers/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/providers/vector_db.py` & `r2r-0.1.33/r2r/core/providers/vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/core/utils/splitter/text.py` & `r2r-0.1.33/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/embeddings/modal/base.py` & `r2r-0.1.33/r2r/embeddings/modal/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/embeddings/openai/base.py` & `r2r-0.1.33/r2r/embeddings/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/embeddings/setence_transformer/base.py` & `r2r-0.1.33/r2r/embeddings/setence_transformer/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/eval/deepeval/base.py` & `r2r-0.1.33/r2r/eval/deepeval/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/eval/parea/base.py` & `r2r-0.1.33/r2r/eval/parea/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/clients/run_basic_client.py` & `r2r-0.1.33/r2r/examples/clients/run_basic_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/clients/run_basic_client_old.py` & `r2r-0.1.33/r2r/examples/clients/run_basic_client_old.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/clients/run_synthetic_query_client.py` & `r2r-0.1.33/r2r/examples/clients/run_synthetic_query_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/configs/local_llama_cpp.json` & `r2r-0.1.33/r2r/examples/configs/local_llama_cpp.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/configs/local_ollama.json` & `r2r-0.1.33/r2r/examples/configs/local_ollama.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/data/meditations.pdf` & `r2r-0.1.33/r2r/examples/data/meditations.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/data/test.pdf` & `r2r-0.1.33/r2r/examples/data/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/data/the_republic.pdf` & `r2r-0.1.33/r2r/examples/data/the_republic.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/servers/basic_pipeline.py` & `r2r-0.1.33/r2r/examples/servers/basic_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/servers/reducto_pipeline.py` & `r2r-0.1.33/r2r/examples/servers/reducto_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/examples/servers/synthetic_query_pipeline.py` & `r2r-0.1.33/r2r/examples/servers/synthetic_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/integrations/exa.py` & `r2r-0.1.33/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/integrations/ionic.py` & `r2r-0.1.33/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/integrations/serper.py` & `r2r-0.1.33/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/llms/litellm/base.py` & `r2r-0.1.33/r2r/llms/litellm/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/llms/llama_cpp/base.py` & `r2r-0.1.33/r2r/llms/llama_cpp/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/llms/openai/base.py` & `r2r-0.1.33/r2r/llms/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/main/app.py` & `r2r-0.1.33/r2r/main/app.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/main/factory.py` & `r2r-0.1.33/r2r/main/factory.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/main/models.py` & `r2r-0.1.33/r2r/main/models.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/main/utils.py` & `r2r-0.1.33/r2r/main/utils.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/__init__.py` & `r2r-0.1.33/r2r/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/basic/embedding.py` & `r2r-0.1.33/r2r/pipelines/basic/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/basic/eval.py` & `r2r-0.1.33/r2r/pipelines/basic/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/basic/ingestion.py` & `r2r-0.1.33/r2r/pipelines/basic/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/basic/prompt_provider.py` & `r2r-0.1.33/r2r/pipelines/basic/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/basic/rag.py` & `r2r-0.1.33/r2r/pipelines/basic/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/pipelines/web_search/rag.py` & `r2r-0.1.33/r2r/pipelines/web_search/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/tests/end_to_end.py` & `r2r-0.1.33/r2r/tests/end_to_end.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/tests/test.pdf` & `r2r-0.1.33/r2r/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/__init__.py` & `r2r-0.1.33/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/adapter/base.py` & `r2r-0.1.33/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/adapter/markdown.py` & `r2r-0.1.33/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/adapter/noop.py` & `r2r-0.1.33/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/adapter/text.py` & `r2r-0.1.33/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/client.py` & `r2r-0.1.33/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/collection.py` & `r2r-0.1.33/r2r/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vecs/exc.py` & `r2r-0.1.33/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vector_dbs/local/base.py` & `r2r-0.1.33/r2r/vector_dbs/local/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vector_dbs/pg_vector/base.py` & `r2r-0.1.33/r2r/vector_dbs/pg_vector/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/r2r/vector_dbs/qdrant/base.py` & `r2r-0.1.33/r2r/vector_dbs/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.32/PKG-INFO` & `r2r-0.1.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.1.32
+Version: 0.1.33
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -120,15 +120,15 @@
 
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
 # Choose from CONFIG_OPTION in {`default`, `local_ollama`}
 # For cloud deployment, select `default` and place your secrets in `.env`
 # For local deployment, select `local_ollama`
-docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest
+docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama
 
 ```
 
 ## Basic Example
 
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
@@ -137,15 +137,16 @@
    python -m r2r.examples.servers.basic_pipeline
    ```
 
 [`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
    # run the client
-   python -m r2r.examples.clients.run_basic_client
+   python -m r2r.examples.clients.run_basic_client ingest
+   python -m r2r.examples.clients.run_basic_client search --query="What is the meaning of life?"
    ```
 ### Running Basic Local RAG
 
 [Refer here](https://r2r-docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the commands above to use local providers.
 
 ## Synthetic Queries Example
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.1.32 Summary: SciPhi R2R License:
+Metadata-Version: 2.1 Name: r2r Version: 0.1.33 Summary: SciPhi R2R License:
 MIT Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: deepeval Provides-Extra:
 embedding Provides-Extra: eval Provides-Extra: exa Provides-Extra: ionic
@@ -61,33 +61,34 @@
 OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
 LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
 INCLUDE secrets and modify config.json # if using cloud providers (e.g.
 pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
 latest # Choose from CONFIG_OPTION in {`default`, `local_ollama`} # For cloud
 deployment, select `default` and place your secrets in `.env` # For local
 deployment, select `local_ollama` docker run -d --name r2r_container -p 8000:
-8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest ```
-## Basic Example [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py):
-Execute this script to initiate the default **backend server**. It establishes
-a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes,
-all accessible via FastAPI. ```bash # launch the server python -
+8000 -e CONFIG_OPTION=local_ollama ``` ## Basic Example [`basic_pipeline.py`]
+(r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the
+default **backend server**. It establishes a basic RAG pipeline that
+encompasses ingestion, embedding, and RAG processes, all accessible via
+FastAPI. ```bash # launch the server python -
 m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
 clients/run_basic_client.py): This **client script** should be executed
 subsequent to the server startup above. It facilitates the upload of text
 entries and PDFs to the server using the Python client and demonstrates the
 management of document and user-level vectors through its built-in features.
-```bash # run the client python -m r2r.examples.clients.run_basic_client ```
-### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/tutorials/
-local_rag) for a tutorial on how to modify the commands above to use local
-providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/
-examples/servers/synthetic_query_pipeline.py): Execute this script to start a
-backend server equipped with an advanced pipeline. This pipeline is designed to
-create synthetic queries, enhancing the RAG system's learning and performance.
-```bash # launch the server python -
-m r2r.examples.servers.synthetic_query_pipeline ```
+```bash # run the client python -m r2r.examples.clients.run_basic_client ingest
+python -m r2r.examples.clients.run_basic_client search --query="What is the
+meaning of life?" ``` ### Running Basic Local RAG [Refer here](https://r2r-
+docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the
+commands above to use local providers. ## Synthetic Queries Example
+[`synthetic_query_pipeline.py`](r2r/examples/servers/
+synthetic_query_pipeline.py): Execute this script to start a backend server
+equipped with an advanced pipeline. This pipeline is designed to create
+synthetic queries, enhancing the RAG system's learning and performance. ```bash
+# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
 run_synthetic_query_client.py): Use this client script after the synthetic
 query pipeline is running. It's tailored for use with the synthetic query
 pipeline, demonstrating the improved features of the RAG system. ```bash # run
 the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
 Extra Examples [`reducto_pipeline.py`](r2r/examples/servers/
 reducto_pipeline.py): Launch this script to activate a backend server that
```

