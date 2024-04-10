# Comparing `tmp/r2r-0.1.31.tar.gz` & `tmp/r2r-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.1.31.tar", max compression
+gzip compressed data, was "r2r-0.1.32.tar", max compression
```

## Comparing `r2r-0.1.31.tar` & `r2r-0.1.32.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1082 2024-04-05 21:53:39.847457 r2r-0.1.31/LICENSE.md
--rw-r--r--   0        0        0     6828 2024-04-05 21:53:39.847457 r2r-0.1.31/README.md
--rw-r--r--   0        0        0      680 2024-04-05 21:53:39.847457 r2r-0.1.31/config.json
--rw-r--r--   0        0        0     2252 2024-04-05 21:53:39.883458 r2r-0.1.31/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/__init__.py
--rw-r--r--   0        0        0       53 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/client/__init__.py
--rw-r--r--   0        0        0     5956 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/client/base.py
--rw-r--r--   0        0        0     1123 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/__init__.py
--rw-r--r--   0        0        0      110 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      781 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/abstractions/output.py
--rw-r--r--   0        0        0      249 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/adapters/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/adapters/advanced/reducto.py
--rw-r--r--   0        0        0     2797 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/adapters/base.py
--rw-r--r--   0        0        0     2407 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/embedding.py
--rw-r--r--   0        0        0     1334 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/eval.py
--rw-r--r--   0        0        0     2175 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/ingestion.py
--rw-r--r--   0        0        0     1515 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/pipeline.py
--rw-r--r--   0        0        0     6227 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/pipelines/rag.py
--rw-r--r--   0        0        0      935 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/embedding.py
--rw-r--r--   0        0        0     1015 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/eval.py
--rw-r--r--   0        0        0     1808 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/llm.py
--rw-r--r--   0        0        0    11873 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/logging.py
--rw-r--r--   0        0        0     1249 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/prompt.py
--rw-r--r--   0        0        0     3833 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/providers/vector_db.py
--rw-r--r--   0        0        0      256 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/base.py
--rw-r--r--   0        0        0       95 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66651 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      203 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     1676 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/modal/base.py
--rw-r--r--   0        0        0     3311 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/openai/base.py
--rw-r--r--   0        0        0     1923 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/embeddings/setence_transformer/base.py
--rw-r--r--   0        0        0      139 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/eval/deepeval/base.py
--rw-r--r--   0        0        0     2707 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/eval/parea/base.py
--rw-r--r--   0        0        0        0 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/__init__.py
--rw-r--r--   0        0        0     3244 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/run_basic_client.py
--rw-r--r--   0        0        0     4249 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/run_basic_client_old.py
--rw-r--r--   0        0        0     1625 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/clients/run_synthetic_query_client.py
--rw-r--r--   0        0        0      689 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/configs/local_llama_cpp.json
--rw-r--r--   0        0        0      687 2024-04-05 21:53:39.883458 r2r-0.1.31/r2r/examples/configs/local_ollama.json
--rw-r--r--   0        0        0   802904 2024-04-05 21:53:39.887458 r2r-0.1.31/r2r/examples/data/meditations.pdf
--rw-r--r--   0        0        0    14812 2024-04-05 21:53:39.887458 r2r-0.1.31/r2r/examples/data/test.pdf
--rw-r--r--   0        0        0  1307590 2024-04-05 21:53:39.891458 r2r-0.1.31/r2r/examples/data/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0     1223 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/basic_pipeline.py
--rw-r--r--   0        0        0      533 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/reducto_pipeline.py
--rw-r--r--   0        0        0     6746 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/synthetic_query_pipeline.py
--rw-r--r--   0        0        0      504 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/examples/servers/web_search_pipeline.py
--rw-r--r--   0        0        0      101 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1184 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3905 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/integrations/serper.py
--rw-r--r--   0        0        0      277 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3602 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/litellm/base.py
--rw-r--r--   0        0        0     4467 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/llama_cpp/base.py
--rw-r--r--   0        0        0        0 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3794 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/llms/openai/base.py
--rw-r--r--   0        0        0      217 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/__init__.py
--rw-r--r--   0        0        0    16236 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/app.py
--rw-r--r--   0        0        0     5108 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/factory.py
--rw-r--r--   0        0        0     3280 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/models.py
--rw-r--r--   0        0        0    10797 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/main/utils.py
--rw-r--r--   0        0        0      541 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/__init__.py
--rw-r--r--   0        0        0     5948 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/embedding.py
--rw-r--r--   0        0        0     1827 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/eval.py
--rw-r--r--   0        0        0     2978 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/ingestion.py
--rw-r--r--   0        0        0     1002 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/prompt_provider.py
--rw-r--r--   0        0        0     3079 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/basic/rag.py
--rw-r--r--   0        0        0     2392 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/pipelines/web_search/rag.py
--rw-r--r--   0        0        0     6035 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/tests/end_to_end.py
--rw-r--r--   0        0        0    14812 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/tests/test.pdf
--rw-r--r--   0        0        0      539 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5299 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9298 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/client.py
--rw-r--r--   0        0        0    35441 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vecs/exc.py
--rw-r--r--   0        0        0      166 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/local/base.py
--rw-r--r--   0        0        0     5607 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/pg_vector/base.py
--rw-r--r--   0        0        0     7125 2024-04-05 21:53:39.895459 r2r-0.1.31/r2r/vector_dbs/qdrant/base.py
--rw-r--r--   0        0        0     9297 1970-01-01 00:00:00.000000 r2r-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-10 05:26:32.861240 r2r-0.1.32/LICENSE.md
+-rw-r--r--   0        0        0     7112 2024-04-10 05:26:32.861240 r2r-0.1.32/README.md
+-rw-r--r--   0        0        0      680 2024-04-10 05:26:32.861240 r2r-0.1.32/config.json
+-rw-r--r--   0        0        0     2216 2024-04-10 05:26:32.893240 r2r-0.1.32/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/client/__init__.py
+-rw-r--r--   0        0        0     5956 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/client/base.py
+-rw-r--r--   0        0        0     1123 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      781 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/abstractions/output.py
+-rw-r--r--   0        0        0      249 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2928 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/adapters/advanced/reducto.py
+-rw-r--r--   0        0        0     2803 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/adapters/base.py
+-rw-r--r--   0        0        0     2407 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/embedding.py
+-rw-r--r--   0        0        0     1334 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/eval.py
+-rw-r--r--   0        0        0     2175 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/ingestion.py
+-rw-r--r--   0        0        0     1515 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/pipeline.py
+-rw-r--r--   0        0        0     6227 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/pipelines/rag.py
+-rw-r--r--   0        0        0      935 2024-04-10 05:26:32.893240 r2r-0.1.32/r2r/core/providers/embedding.py
+-rw-r--r--   0        0        0     1015 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/eval.py
+-rw-r--r--   0        0        0     1808 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/llm.py
+-rw-r--r--   0        0        0    11873 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/logging.py
+-rw-r--r--   0        0        0     1249 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/prompt.py
+-rw-r--r--   0        0        0     3833 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/providers/vector_db.py
+-rw-r--r--   0        0        0      256 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/base.py
+-rw-r--r--   0        0        0       95 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66651 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      203 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/modal/base.py
+-rw-r--r--   0        0        0     3311 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/openai/base.py
+-rw-r--r--   0        0        0     1923 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/embeddings/setence_transformer/base.py
+-rw-r--r--   0        0        0      139 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/eval/deepeval/base.py
+-rw-r--r--   0        0        0     2710 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/eval/parea/base.py
+-rw-r--r--   0        0        0        0 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/__init__.py
+-rw-r--r--   0        0        0     3244 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/run_basic_client.py
+-rw-r--r--   0        0        0     4249 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/run_basic_client_old.py
+-rw-r--r--   0        0        0     1625 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/clients/run_synthetic_query_client.py
+-rw-r--r--   0        0        0      689 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/configs/local_llama_cpp.json
+-rw-r--r--   0        0        0      687 2024-04-10 05:26:32.897240 r2r-0.1.32/r2r/examples/configs/local_ollama.json
+-rw-r--r--   0        0        0   802904 2024-04-10 05:26:32.901240 r2r-0.1.32/r2r/examples/data/meditations.pdf
+-rw-r--r--   0        0        0    14812 2024-04-10 05:26:32.901240 r2r-0.1.32/r2r/examples/data/test.pdf
+-rw-r--r--   0        0        0  1307590 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/data/the_republic.pdf
+-rw-r--r--   0        0        0        0 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/basic_pipeline.py
+-rw-r--r--   0        0        0      533 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/reducto_pipeline.py
+-rw-r--r--   0        0        0     6746 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/synthetic_query_pipeline.py
+-rw-r--r--   0        0        0      504 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/examples/servers/web_search_pipeline.py
+-rw-r--r--   0        0        0      101 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1184 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3905 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      277 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3602 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/litellm/base.py
+-rw-r--r--   0        0        0     4467 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/llama_cpp/base.py
+-rw-r--r--   0        0        0        0 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3794 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/llms/openai/base.py
+-rw-r--r--   0        0        0      217 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/__init__.py
+-rw-r--r--   0        0        0    16309 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/app.py
+-rw-r--r--   0        0        0     5108 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/factory.py
+-rw-r--r--   0        0        0     3280 2024-04-10 05:26:32.905240 r2r-0.1.32/r2r/main/models.py
+-rw-r--r--   0        0        0    10797 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/main/utils.py
+-rw-r--r--   0        0        0      541 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/__init__.py
+-rw-r--r--   0        0        0     5948 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/embedding.py
+-rw-r--r--   0        0        0     1830 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/eval.py
+-rw-r--r--   0        0        0     2978 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/ingestion.py
+-rw-r--r--   0        0        0     1002 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/prompt_provider.py
+-rw-r--r--   0        0        0     3079 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/basic/rag.py
+-rw-r--r--   0        0        0     2392 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/pipelines/web_search/rag.py
+-rw-r--r--   0        0        0     6035 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/tests/end_to_end.py
+-rw-r--r--   0        0        0    14812 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/tests/test.pdf
+-rw-r--r--   0        0        0      539 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3269 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5299 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9298 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/client.py
+-rw-r--r--   0        0        0    35441 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      166 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/local/base.py
+-rw-r--r--   0        0        0     5607 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/pg_vector/base.py
+-rw-r--r--   0        0        0     7125 2024-04-10 05:26:32.909240 r2r-0.1.32/r2r/vector_dbs/qdrant/base.py
+-rw-r--r--   0        0        0     9587 1970-01-01 00:00:00.000000 r2r-0.1.32/PKG-INFO
```

### Comparing `r2r-0.1.31/LICENSE.md` & `r2r-0.1.32/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/README.md` & `r2r-0.1.32/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 <img src="./docs/pages/r2r.png" alt="Sciphi Framework">
 <h3 align="center">
 Build, deploy, and optimize your RAG system.
 </h3>
 
 ## About
 
-R2R, short for RAG to Riches, provides the fastest and most efficient way to provide high quality RAG to end users. The framework is built around customizable pipelines and a feature-rich FastAPI implementation.
+R2R (RAG to Riches) offers a fast and efficient framework for serving high-quality Retrieval-Augmented Generation (RAG) to end users. The framework is designed with customizable pipelines and a feature-rich FastAPI implementation, enabling developers to quickly deploy and scale RAG-based applications.
+
 
 ## Why?
 
 R2R was conceived to bridge the gap between local LLM experimentation and scalable production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to React**. A JavaScript client for R2R deployments can be [found here](https://github.com/SciPhi-AI/r2r-js).
 
 ### Key Features
 
@@ -43,15 +44,15 @@
 
 [SciPhi Cloud](https://docs.sciphi.ai/)
 
 ## Quick Install:
 
 ```bash
 # use the `'r2r[all]'` to download all required deps
-pip install 'r2r[parsing,eval]'
+pip install 'r2r[eval]'
 
 # setup env 
 export OPENAI_API_KEY=sk-...
 # Set `LOCAL_DB_PATH` for local testing
 export LOCAL_DB_PATH=local.sqlite
 
 # OR do `vim .env.example && cp .env.example .env`
@@ -60,16 +61,19 @@
 ```
 
 ## Docker:
 
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
-# Place your secrets in `.env`
-docker run -d --name r2r_container -p 8000:8000 --env-file .env r2r
+# Choose from CONFIG_OPTION in {`default`, `local_ollama`}
+# For cloud deployment, select `default` and place your secrets in `.env`
+# For local deployment, select `local_ollama`
+docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest
+
 ```
 
 ## Basic Example
 
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
    ```bash
@@ -81,15 +85,15 @@
 
    ```bash
    # run the client
    python -m r2r.examples.clients.run_basic_client
    ```
 ### Running Basic Local RAG
 
-[Refer here](https://r2r-docs.sciphi.ai/tutorials/local-rag) for a tutorial on how to modify the commands above to use local providers.
+[Refer here](https://r2r-docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the commands above to use local providers.
 
 ## Synthetic Queries Example
 
 [`synthetic_query_pipeline.py`](r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to start a backend server equipped with an advanced pipeline. This pipeline is designed to create synthetic queries, enhancing the RAG system's learning and performance.
 
    ```bash
    # launch the server
```

#### html2text {}

```diff
@@ -1,50 +1,53 @@
 _[_D_o_c_s_]_[_D_i_s_c_o_r_d_]_[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
 [Sciphi Framework]
             ******** BBuuiilldd,, ddeeppllooyy,, aanndd ooppttiimmiizzee yyoouurr RRAAGG ssyysstteemm.. ********
-## About R2R, short for RAG to Riches, provides the fastest and most efficient
-way to provide high quality RAG to end users. The framework is built around
-customizable pipelines and a feature-rich FastAPI implementation. ## Why? R2R
-was conceived to bridge the gap between local LLM experimentation and scalable
-production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to
-React**. A JavaScript client for R2R deployments can be [found here](https://
-github.com/SciPhi-AI/r2r-js). ### Key Features - **ð Deploy**: Instantly
-launch production-ready RAG pipelines with streaming capabilities. - **ð§©
-Customize**: Tailor your pipeline with intuitive configuration files. - **ð
-Extend**: Enhance your pipeline with custom code integrations. - **âï¸
-Autoscale**: Scale your pipeline effortlessly in the cloud using [SciPhi]
-(https://app.sciphi.ai/). - **ð¤ OSS**: Benefit from a framework developed by
-the open-source community, designed to simplify RAG deployment. ## Demo(s)
-Using the cloud application to deploy the pre-built basic pipeline: https://
-www.loom.com/share/e3b934b554484787b005702ced650ac9 Note - the example above
-uses [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for
-deployment and observability. SciPhi is working to launch a self-hosted version
-of their cloud platform as R2R matures. ## Links [Join the Discord server]
-(https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart](https://r2r-
-docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud](https://
-docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to download
-all required deps pip install 'r2r[parsing,eval]' # setup env export
+## About R2R (RAG to Riches) offers a fast and efficient framework for serving
+high-quality Retrieval-Augmented Generation (RAG) to end users. The framework
+is designed with customizable pipelines and a feature-rich FastAPI
+implementation, enabling developers to quickly deploy and scale RAG-based
+applications. ## Why? R2R was conceived to bridge the gap between local LLM
+experimentation and scalable production solutions. **R2R is to LangChain/
+LlamaIndex what NextJS is to React**. A JavaScript client for R2R deployments
+can be [found here](https://github.com/SciPhi-AI/r2r-js). ### Key Features -
+**ð Deploy**: Instantly launch production-ready RAG pipelines with streaming
+capabilities. - **ð§© Customize**: Tailor your pipeline with intuitive
+configuration files. - **ð Extend**: Enhance your pipeline with custom code
+integrations. - **âï¸ Autoscale**: Scale your pipeline effortlessly in the
+cloud using [SciPhi](https://app.sciphi.ai/). - **ð¤ OSS**: Benefit from a
+framework developed by the open-source community, designed to simplify RAG
+deployment. ## Demo(s) Using the cloud application to deploy the pre-built
+basic pipeline: https://www.loom.com/share/e3b934b554484787b005702ced650ac9
+Note - the example above uses [SciPhi Cloud](https://app.sciphi.ai) to pair
+with the R2R framework for deployment and observability. SciPhi is working to
+launch a self-hosted version of their cloud platform as R2R matures. ## Links
+[Join the Discord server](https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart]
+(https://r2r-docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud]
+(https://docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to
+download all required deps pip install 'r2r[eval]' # setup env export
 OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
 LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
 INCLUDE secrets and modify config.json # if using cloud providers (e.g.
 pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
-latest # Place your secrets in `.env` docker run -d --name r2r_container -
-p 8000:8000 --env-file .env r2r ``` ## Basic Example [`basic_pipeline.py`](r2r/
-examples/servers/basic_pipeline.py): Execute this script to initiate the
-default **backend server**. It establishes a basic RAG pipeline that
-encompasses ingestion, embedding, and RAG processes, all accessible via
-FastAPI. ```bash # launch the server python -
+latest # Choose from CONFIG_OPTION in {`default`, `local_ollama`} # For cloud
+deployment, select `default` and place your secrets in `.env` # For local
+deployment, select `local_ollama` docker run -d --name r2r_container -p 8000:
+8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest ```
+## Basic Example [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py):
+Execute this script to initiate the default **backend server**. It establishes
+a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes,
+all accessible via FastAPI. ```bash # launch the server python -
 m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
 clients/run_basic_client.py): This **client script** should be executed
 subsequent to the server startup above. It facilitates the upload of text
 entries and PDFs to the server using the Python client and demonstrates the
 management of document and user-level vectors through its built-in features.
 ```bash # run the client python -m r2r.examples.clients.run_basic_client ```
 ### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/tutorials/
-local-rag) for a tutorial on how to modify the commands above to use local
+local_rag) for a tutorial on how to modify the commands above to use local
 providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/
 examples/servers/synthetic_query_pipeline.py): Execute this script to start a
 backend server equipped with an advanced pipeline. This pipeline is designed to
 create synthetic queries, enhancing the RAG system's learning and performance.
 ```bash # launch the server python -
 m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
```

### Comparing `r2r-0.1.31/config.json` & `r2r-0.1.32/config.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/pyproject.toml` & `r2r-0.1.32/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.1.31"
+version = "0.1.32"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
 # Python Versions
 python = ">=3.9,<3.13"
 
 # Required dependencies
+bs4= "^0.0.2"
 fastapi = "^0.109.2"
 fire = "^0.5.0"
 gunicorn = "^21.2.0"
 litellm = "^1.34.0"
 openai = "^1.11.1"
 pydantic = "^2.6.3"
+pypdf = "^4.2.0"
 python-dotenv = "^1.0.1"
 python-multipart = "^0.0.9"
 requests = "^2.31.0"
 types-requests = "^2.31.0"
 uvicorn = "^0.27.0.post1"
 vecs = "^0.4.0"
 
 
 # Optional dependencies
-bs4 = {version = "^0.0.2", optional = true}
-pypdf = {version = "^4.0.2", optional = true}
 tiktoken = {version = "^0.5.2", optional = true}
 datasets = {version = "^2.16.1", optional = true}
 qdrant_client = {version = "^1.7.0", optional = true}
 psycopg2-binary = {version = "^2.9.9", optional = true}
 numpy = {version = "^1.26.4", optional = true}
 sentry-sdk = {version = "^1.40.4", optional = true}
 deepeval = {version ="^0.20.88", optional = true}
@@ -44,25 +44,25 @@
 ionic-api-sdk = {version = "0.9.3", optional = true}
 boto3 = {version = "^1.34.71", optional = true}
 exa-py = {version = "^1.0.9", optional = true}
 llama-cpp-python = {version = "^0.2.57", optional = true}
 sentence-transformers = {version = "^2.6.1", optional = true}
 
 [tool.poetry.extras]
-parsing = ["bs4", "pypdf"]
 embedding = ["tiktoken"]
 streaming = ["datasets"]
 qdrant = ["qdrant_client"]
 postgres = ["psycopg2-binary"]
 monitoring = ["sentry-sdk"]
 deepeval = ["deepeval"]
 eval = ["parea-ai"]
 ionic = ["ionic-api-sdk"]
 reducto = ["boto3"]
 exa = ["exa-py"]
+sentence_transformers = ["sentence-transformers"]
 local_llm = ["llama-cpp-python", "sentence-transformers"]
 all = ["bs4", "pypdf", "tiktoken", "datasets", "qdrant_client", "psycopg2-binary", "sentry-sdk", "parea-ai", "boto3", "exa-py", "llama-cpp-python"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "6.1.0"
 isort = "5.12.0"
```

### Comparing `r2r-0.1.31/r2r/client/base.py` & `r2r-0.1.32/r2r/client/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/__init__.py` & `r2r-0.1.32/r2r/core/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/abstractions/output.py` & `r2r-0.1.32/r2r/core/abstractions/output.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/adapters/advanced/reducto.py` & `r2r-0.1.32/r2r/core/adapters/advanced/reducto.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/adapters/base.py` & `r2r-0.1.32/r2r/core/adapters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,9 +83,9 @@
         text = ""
         for page in pdf.pages:
             page_text = page.extract_text()
             if page_text is not None:
                 page_text = "".join(
                     filter(lambda x: x in string.printable, page_text)
                 )
-                text += page_text
+                text += page_text + " "
         return [text]
```

### Comparing `r2r-0.1.31/r2r/core/pipelines/embedding.py` & `r2r-0.1.32/r2r/core/pipelines/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/pipelines/eval.py` & `r2r-0.1.32/r2r/core/pipelines/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/pipelines/ingestion.py` & `r2r-0.1.32/r2r/core/pipelines/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/pipelines/pipeline.py` & `r2r-0.1.32/r2r/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/pipelines/rag.py` & `r2r-0.1.32/r2r/core/pipelines/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/providers/embedding.py` & `r2r-0.1.32/r2r/core/providers/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/providers/eval.py` & `r2r-0.1.32/r2r/core/providers/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/providers/llm.py` & `r2r-0.1.32/r2r/core/providers/llm.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/providers/logging.py` & `r2r-0.1.32/r2r/core/providers/logging.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/providers/prompt.py` & `r2r-0.1.32/r2r/core/providers/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/providers/vector_db.py` & `r2r-0.1.32/r2r/core/providers/vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/core/utils/splitter/text.py` & `r2r-0.1.32/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/embeddings/modal/base.py` & `r2r-0.1.32/r2r/embeddings/modal/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/embeddings/openai/base.py` & `r2r-0.1.32/r2r/embeddings/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/embeddings/setence_transformer/base.py` & `r2r-0.1.32/r2r/embeddings/setence_transformer/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/eval/deepeval/base.py` & `r2r-0.1.32/r2r/eval/deepeval/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/eval/parea/base.py` & `r2r-0.1.32/r2r/eval/parea/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     },
                     output=completion,
                 )
 
             self._create_log = create_log
         except ImportError:
             raise ImportError(
-                "Parea is not installed. Please install it using `pip install parea`."
+                "Parea is not installed. Please install it using `pip install parea-ai`."
             )
         if not os.getenv("OPENAI_API_KEY"):
             raise ValueError(
                 "Please set the `OPENAI_API_KEY` environment variable to run with Parea."
             )
 
     def _evaluate(
```

### Comparing `r2r-0.1.31/r2r/examples/clients/run_basic_client.py` & `r2r-0.1.32/r2r/examples/clients/run_basic_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/clients/run_basic_client_old.py` & `r2r-0.1.32/r2r/examples/clients/run_basic_client_old.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/clients/run_synthetic_query_client.py` & `r2r-0.1.32/r2r/examples/clients/run_synthetic_query_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/configs/local_llama_cpp.json` & `r2r-0.1.32/r2r/examples/configs/local_llama_cpp.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/configs/local_ollama.json` & `r2r-0.1.32/r2r/examples/configs/local_ollama.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/data/meditations.pdf` & `r2r-0.1.32/r2r/examples/data/meditations.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/data/test.pdf` & `r2r-0.1.32/r2r/examples/data/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/data/the_republic.pdf` & `r2r-0.1.32/r2r/examples/data/the_republic.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/servers/basic_pipeline.py` & `r2r-0.1.32/r2r/examples/servers/basic_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 
 OPTIONS = {
     "default": None,
     "local_ollama": os.path.join(configs_path, "local_ollama.json"),
     "local_llama_cpp": os.path.join(configs_path, "local_llama_cpp.json"),
 }
 
+
+def create_app(config_name: str = "default"):
+    config_path = OPTIONS[config_name]
+
+    app = E2EPipelineFactory.create_pipeline(
+        config=R2RConfig.load_config(config_path)
+    )
+    return app
+
+
+app = create_app()
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="R2R Pipeline")
     parser.add_argument(
         "--config",
         type=str,
         default="default",
         choices=OPTIONS.keys(),
         help="Configuration option for the pipeline",
     )
-    args = parser.parse_args()
-
-    config_path = OPTIONS[args.config]
-
-    # Creates a pipeline with the specified configuration
-    # This is the main entry point for the application
-    # The pipeline is built using the specified configuration file
-    # Read more about the configuration in the documentation [https://r2r-docs.sciphi.ai/core-features/factory]
-    app = E2EPipelineFactory.create_pipeline(
-        config=R2RConfig.load_config(config_path)
-    )
+    args, _ = parser.parse_known_args()
 
-    # Run the FastAPI application using Uvicorn
     uvicorn.run(app, host="0.0.0.0", port=8000)
```

### Comparing `r2r-0.1.31/r2r/examples/servers/reducto_pipeline.py` & `r2r-0.1.32/r2r/examples/servers/reducto_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/examples/servers/synthetic_query_pipeline.py` & `r2r-0.1.32/r2r/examples/servers/synthetic_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/integrations/exa.py` & `r2r-0.1.32/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/integrations/ionic.py` & `r2r-0.1.32/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/integrations/serper.py` & `r2r-0.1.32/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/llms/litellm/base.py` & `r2r-0.1.32/r2r/llms/litellm/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/llms/llama_cpp/base.py` & `r2r-0.1.32/r2r/llms/llama_cpp/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/llms/openai/base.py` & `r2r-0.1.32/r2r/llms/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/main/app.py` & `r2r-0.1.32/r2r/main/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,17 +223,18 @@
                 payload = {
                     "query": query.query,
                     "context": rag_completion.context or "",
                     "completion_text": completion_text or "",
                     "run_id": str(rag_pipeline.pipeline_run_info["run_id"]),
                     "settings": query.settings.rag_settings.dict(),
                 }
-                background_tasks.add_task(
-                    requests.post, f"{url}/eval", json=payload
-                )
+                if config.evals.get("frequency", 0.0) > 0.0:
+                    background_tasks.add_task(
+                        requests.post, f"{url}/eval", json=payload
+                    )
 
                 return rag_completion
 
             else:
 
                 async def _stream_rag_completion(
                     query: RAGQueryModel,
```

### Comparing `r2r-0.1.31/r2r/main/factory.py` & `r2r-0.1.32/r2r/main/factory.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/main/models.py` & `r2r-0.1.32/r2r/main/models.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/main/utils.py` & `r2r-0.1.32/r2r/main/utils.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/pipelines/__init__.py` & `r2r-0.1.32/r2r/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/pipelines/basic/embedding.py` & `r2r-0.1.32/r2r/pipelines/basic/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/pipelines/basic/eval.py` & `r2r-0.1.32/r2r/pipelines/basic/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             )
 
         elif provider == "parea":
             try:
                 from r2r.eval import PareaEvalProvider
             except ImportError:
                 raise ImportError(
-                    "Parea is not installed. Please install it using `pip install parea`."
+                    "Parea is not installed. Please install it using `pip install parea-ai`."
                 )
             self.eval_provider = PareaEvalProvider(
                 provider,
                 eval_config.get("sampling_fraction", 1.0),
             )
         else:
             self.eval_provider = None
```

### Comparing `r2r-0.1.31/r2r/pipelines/basic/ingestion.py` & `r2r-0.1.32/r2r/pipelines/basic/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/pipelines/basic/prompt_provider.py` & `r2r-0.1.32/r2r/pipelines/basic/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/pipelines/basic/rag.py` & `r2r-0.1.32/r2r/pipelines/basic/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/pipelines/web_search/rag.py` & `r2r-0.1.32/r2r/pipelines/web_search/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/tests/end_to_end.py` & `r2r-0.1.32/r2r/tests/end_to_end.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/tests/test.pdf` & `r2r-0.1.32/r2r/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/__init__.py` & `r2r-0.1.32/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/adapter/base.py` & `r2r-0.1.32/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/adapter/markdown.py` & `r2r-0.1.32/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/adapter/noop.py` & `r2r-0.1.32/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/adapter/text.py` & `r2r-0.1.32/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/client.py` & `r2r-0.1.32/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/collection.py` & `r2r-0.1.32/r2r/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vecs/exc.py` & `r2r-0.1.32/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vector_dbs/local/base.py` & `r2r-0.1.32/r2r/vector_dbs/local/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vector_dbs/pg_vector/base.py` & `r2r-0.1.32/r2r/vector_dbs/pg_vector/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/r2r/vector_dbs/qdrant/base.py` & `r2r-0.1.32/r2r/vector_dbs/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.31/PKG-INFO` & `r2r-0.1.32/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.1.31
+Version: 0.1.32
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,41 +16,41 @@
 Provides-Extra: deepeval
 Provides-Extra: embedding
 Provides-Extra: eval
 Provides-Extra: exa
 Provides-Extra: ionic
 Provides-Extra: local-llm
 Provides-Extra: monitoring
-Provides-Extra: parsing
 Provides-Extra: postgres
 Provides-Extra: qdrant
 Provides-Extra: reducto
+Provides-Extra: sentence-transformers
 Provides-Extra: streaming
 Requires-Dist: boto3 (>=1.34.71,<2.0.0) ; extra == "reducto" or extra == "all"
-Requires-Dist: bs4 (>=0.0.2,<0.0.3) ; extra == "parsing" or extra == "all"
+Requires-Dist: bs4 (>=0.0.2,<0.0.3) ; extra == "all"
 Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra == "streaming" or extra == "all"
 Requires-Dist: deepeval (>=0.20.88,<0.21.0) ; extra == "deepeval"
 Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or extra == "all"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0)
 Requires-Dist: ionic-api-sdk (==0.9.3) ; extra == "ionic"
 Requires-Dist: litellm (>=1.34.0,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra == "local-llm" or extra == "all"
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ; extra == "eval" or extra == "all"
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all"
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
-Requires-Dist: pypdf (>=4.0.2,<5.0.0) ; extra == "parsing" or extra == "all"
+Requires-Dist: pypdf (>=4.2.0,<5.0.0) ; extra == "all"
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: qdrant_client (>=1.7.0,<2.0.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra == "local-llm"
+Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra == "sentence-transformers" or extra == "local-llm"
 Requires-Dist: sentry-sdk (>=1.40.4,<2.0.0) ; extra == "monitoring" or extra == "all"
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra == "embedding" or extra == "all"
 Requires-Dist: types-requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0)
 Requires-Dist: vecs (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
@@ -65,15 +65,16 @@
 <img src="./docs/pages/r2r.png" alt="Sciphi Framework">
 <h3 align="center">
 Build, deploy, and optimize your RAG system.
 </h3>
 
 ## About
 
-R2R, short for RAG to Riches, provides the fastest and most efficient way to provide high quality RAG to end users. The framework is built around customizable pipelines and a feature-rich FastAPI implementation.
+R2R (RAG to Riches) offers a fast and efficient framework for serving high-quality Retrieval-Augmented Generation (RAG) to end users. The framework is designed with customizable pipelines and a feature-rich FastAPI implementation, enabling developers to quickly deploy and scale RAG-based applications.
+
 
 ## Why?
 
 R2R was conceived to bridge the gap between local LLM experimentation and scalable production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to React**. A JavaScript client for R2R deployments can be [found here](https://github.com/SciPhi-AI/r2r-js).
 
 ### Key Features
 
@@ -99,15 +100,15 @@
 
 [SciPhi Cloud](https://docs.sciphi.ai/)
 
 ## Quick Install:
 
 ```bash
 # use the `'r2r[all]'` to download all required deps
-pip install 'r2r[parsing,eval]'
+pip install 'r2r[eval]'
 
 # setup env 
 export OPENAI_API_KEY=sk-...
 # Set `LOCAL_DB_PATH` for local testing
 export LOCAL_DB_PATH=local.sqlite
 
 # OR do `vim .env.example && cp .env.example .env`
@@ -116,16 +117,19 @@
 ```
 
 ## Docker:
 
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
-# Place your secrets in `.env`
-docker run -d --name r2r_container -p 8000:8000 --env-file .env r2r
+# Choose from CONFIG_OPTION in {`default`, `local_ollama`}
+# For cloud deployment, select `default` and place your secrets in `.env`
+# For local deployment, select `local_ollama`
+docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest
+
 ```
 
 ## Basic Example
 
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
    ```bash
@@ -137,15 +141,15 @@
 
    ```bash
    # run the client
    python -m r2r.examples.clients.run_basic_client
    ```
 ### Running Basic Local RAG
 
-[Refer here](https://r2r-docs.sciphi.ai/tutorials/local-rag) for a tutorial on how to modify the commands above to use local providers.
+[Refer here](https://r2r-docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the commands above to use local providers.
 
 ## Synthetic Queries Example
 
 [`synthetic_query_pipeline.py`](r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to start a backend server equipped with an advanced pipeline. This pipeline is designed to create synthetic queries, enhancing the RAG system's learning and performance.
 
    ```bash
    # launch the server
```

#### html2text {}

```diff
@@ -1,83 +1,87 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.1.31 Summary: SciPhi R2R License:
+Metadata-Version: 2.1 Name: r2r Version: 0.1.32 Summary: SciPhi R2R License:
 MIT Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: deepeval Provides-Extra:
 embedding Provides-Extra: eval Provides-Extra: exa Provides-Extra: ionic
-Provides-Extra: local-llm Provides-Extra: monitoring Provides-Extra: parsing
-Provides-Extra: postgres Provides-Extra: qdrant Provides-Extra: reducto
-Provides-Extra: streaming Requires-Dist: boto3 (>=1.34.71,<2.0.0) ; extra ==
-"reducto" or extra == "all" Requires-Dist: bs4 (>=0.0.2,<0.0.3) ; extra ==
-"parsing" or extra == "all" Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra
-== "streaming" or extra == "all" Requires-Dist: deepeval (>=0.20.88,<0.21.0) ;
-extra == "deepeval" Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or
-extra == "all" Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist: fire
+Provides-Extra: local-llm Provides-Extra: monitoring Provides-Extra: postgres
+Provides-Extra: qdrant Provides-Extra: reducto Provides-Extra: sentence-
+transformers Provides-Extra: streaming Requires-Dist: boto3 (>=1.34.71,<2.0.0)
+; extra == "reducto" or extra == "all" Requires-Dist: bs4 (>=0.0.2,<0.0.3) ;
+extra == "all" Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra == "streaming"
+or extra == "all" Requires-Dist: deepeval (>=0.20.88,<0.21.0) ; extra ==
+"deepeval" Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or extra ==
+"all" Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist: fire
 (>=0.5.0,<0.6.0) Requires-Dist: gunicorn (>=21.2.0,<22.0.0) Requires-Dist:
 ionic-api-sdk (==0.9.3) ; extra == "ionic" Requires-Dist: litellm
 (>=1.34.0,<2.0.0) Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra ==
 "local-llm" or extra == "all" Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-
 Dist: openai (>=1.11.1,<2.0.0) Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ;
 extra == "eval" or extra == "all" Requires-Dist: psycopg2-binary
 (>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all" Requires-Dist:
-pydantic (>=2.6.3,<3.0.0) Requires-Dist: pypdf (>=4.0.2,<5.0.0) ; extra ==
-"parsing" or extra == "all" Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-Dist: qdrant_client
-(>=1.7.0,<2.0.0) ; extra == "qdrant" or extra == "all" Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra
-== "local-llm" Requires-Dist: sentry-sdk (>=1.40.4,<2.0.0) ; extra ==
-"monitoring" or extra == "all" Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra
-== "embedding" or extra == "all" Requires-Dist: types-requests
-(>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0) Requires-
-Dist: vecs (>=0.4.0,<0.5.0) Description-Content-Type: text/markdown
+pydantic (>=2.6.3,<3.0.0) Requires-Dist: pypdf (>=4.2.0,<5.0.0) ; extra ==
+"all" Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-
+multipart (>=0.0.9,<0.0.10) Requires-Dist: qdrant_client (>=1.7.0,<2.0.0) ;
+extra == "qdrant" or extra == "all" Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra == "sentence-
+transformers" or extra == "local-llm" Requires-Dist: sentry-sdk
+(>=1.40.4,<2.0.0) ; extra == "monitoring" or extra == "all" Requires-Dist:
+tiktoken (>=0.5.2,<0.6.0) ; extra == "embedding" or extra == "all" Requires-
+Dist: types-requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn
+(>=0.27.0.post1,<0.28.0) Requires-Dist: vecs (>=0.4.0,<0.5.0) Description-
+Content-Type: text/markdown
 _[_D_o_c_s_]_[_D_i_s_c_o_r_d_]_[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
 [Sciphi Framework]
             ******** BBuuiilldd,, ddeeppllooyy,, aanndd ooppttiimmiizzee yyoouurr RRAAGG ssyysstteemm.. ********
-## About R2R, short for RAG to Riches, provides the fastest and most efficient
-way to provide high quality RAG to end users. The framework is built around
-customizable pipelines and a feature-rich FastAPI implementation. ## Why? R2R
-was conceived to bridge the gap between local LLM experimentation and scalable
-production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to
-React**. A JavaScript client for R2R deployments can be [found here](https://
-github.com/SciPhi-AI/r2r-js). ### Key Features - **ð Deploy**: Instantly
-launch production-ready RAG pipelines with streaming capabilities. - **ð§©
-Customize**: Tailor your pipeline with intuitive configuration files. - **ð
-Extend**: Enhance your pipeline with custom code integrations. - **âï¸
-Autoscale**: Scale your pipeline effortlessly in the cloud using [SciPhi]
-(https://app.sciphi.ai/). - **ð¤ OSS**: Benefit from a framework developed by
-the open-source community, designed to simplify RAG deployment. ## Demo(s)
-Using the cloud application to deploy the pre-built basic pipeline: https://
-www.loom.com/share/e3b934b554484787b005702ced650ac9 Note - the example above
-uses [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for
-deployment and observability. SciPhi is working to launch a self-hosted version
-of their cloud platform as R2R matures. ## Links [Join the Discord server]
-(https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart](https://r2r-
-docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud](https://
-docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to download
-all required deps pip install 'r2r[parsing,eval]' # setup env export
+## About R2R (RAG to Riches) offers a fast and efficient framework for serving
+high-quality Retrieval-Augmented Generation (RAG) to end users. The framework
+is designed with customizable pipelines and a feature-rich FastAPI
+implementation, enabling developers to quickly deploy and scale RAG-based
+applications. ## Why? R2R was conceived to bridge the gap between local LLM
+experimentation and scalable production solutions. **R2R is to LangChain/
+LlamaIndex what NextJS is to React**. A JavaScript client for R2R deployments
+can be [found here](https://github.com/SciPhi-AI/r2r-js). ### Key Features -
+**ð Deploy**: Instantly launch production-ready RAG pipelines with streaming
+capabilities. - **ð§© Customize**: Tailor your pipeline with intuitive
+configuration files. - **ð Extend**: Enhance your pipeline with custom code
+integrations. - **âï¸ Autoscale**: Scale your pipeline effortlessly in the
+cloud using [SciPhi](https://app.sciphi.ai/). - **ð¤ OSS**: Benefit from a
+framework developed by the open-source community, designed to simplify RAG
+deployment. ## Demo(s) Using the cloud application to deploy the pre-built
+basic pipeline: https://www.loom.com/share/e3b934b554484787b005702ced650ac9
+Note - the example above uses [SciPhi Cloud](https://app.sciphi.ai) to pair
+with the R2R framework for deployment and observability. SciPhi is working to
+launch a self-hosted version of their cloud platform as R2R matures. ## Links
+[Join the Discord server](https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart]
+(https://r2r-docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud]
+(https://docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to
+download all required deps pip install 'r2r[eval]' # setup env export
 OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
 LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
 INCLUDE secrets and modify config.json # if using cloud providers (e.g.
 pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
-latest # Place your secrets in `.env` docker run -d --name r2r_container -
-p 8000:8000 --env-file .env r2r ``` ## Basic Example [`basic_pipeline.py`](r2r/
-examples/servers/basic_pipeline.py): Execute this script to initiate the
-default **backend server**. It establishes a basic RAG pipeline that
-encompasses ingestion, embedding, and RAG processes, all accessible via
-FastAPI. ```bash # launch the server python -
+latest # Choose from CONFIG_OPTION in {`default`, `local_ollama`} # For cloud
+deployment, select `default` and place your secrets in `.env` # For local
+deployment, select `local_ollama` docker run -d --name r2r_container -p 8000:
+8000 -e CONFIG_OPTION=local_ollama --env-file .env emrgntcmplxty/r2r:latest ```
+## Basic Example [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py):
+Execute this script to initiate the default **backend server**. It establishes
+a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes,
+all accessible via FastAPI. ```bash # launch the server python -
 m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
 clients/run_basic_client.py): This **client script** should be executed
 subsequent to the server startup above. It facilitates the upload of text
 entries and PDFs to the server using the Python client and demonstrates the
 management of document and user-level vectors through its built-in features.
 ```bash # run the client python -m r2r.examples.clients.run_basic_client ```
 ### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/tutorials/
-local-rag) for a tutorial on how to modify the commands above to use local
+local_rag) for a tutorial on how to modify the commands above to use local
 providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/
 examples/servers/synthetic_query_pipeline.py): Execute this script to start a
 backend server equipped with an advanced pipeline. This pipeline is designed to
 create synthetic queries, enhancing the RAG system's learning and performance.
 ```bash # launch the server python -
 m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
```

