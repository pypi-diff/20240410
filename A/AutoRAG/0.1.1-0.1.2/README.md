# Comparing `tmp/AutoRAG-0.1.1.tar.gz` & `tmp/AutoRAG-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoRAG-0.1.1.tar", last modified: Fri Apr  5 15:04:14 2024, max compression
+gzip compressed data, was "AutoRAG-0.1.2.tar", last modified: Wed Apr 10 04:46:25 2024, max compression
```

## Comparing `AutoRAG-0.1.1.tar` & `AutoRAG-0.1.2.tar`

### file list

```diff
@@ -1,440 +1,456 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.864409 AutoRAG-0.1.1/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.720327 AutoRAG-0.1.1/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 AutoRAG-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.721033 AutoRAG-0.1.1/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 AutoRAG-0.1.1/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 AutoRAG-0.1.1/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.863450 AutoRAG-0.1.1/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    29326 2024-04-05 15:04:14.000000 AutoRAG-0.1.1/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    16300 2024-04-05 15:04:14.000000 AutoRAG-0.1.1/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-05 15:04:14.000000 AutoRAG-0.1.1/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-05 15:04:14.000000 AutoRAG-0.1.1/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      462 2024-04-05 15:04:14.000000 AutoRAG-0.1.1/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-05 15:04:14.000000 AutoRAG-0.1.1/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 AutoRAG-0.1.1/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    29326 2024-04-05 15:04:14.864089 AutoRAG-0.1.1/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    14436 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.726056 AutoRAG-0.1.1/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-05 14:55:22.000000 AutoRAG-0.1.1/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 AutoRAG-0.1.1/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4333 2024-03-29 05:05:10.000000 AutoRAG-0.1.1/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.726511 AutoRAG-0.1.1/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 AutoRAG-0.1.1/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.727708 AutoRAG-0.1.1/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 AutoRAG-0.1.1/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 AutoRAG-0.1.1/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 AutoRAG-0.1.1/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.729642 AutoRAG-0.1.1/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-25 11:47:15.000000 AutoRAG-0.1.1/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2754 2024-03-25 11:47:15.000000 AutoRAG-0.1.1/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7107 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.730052 AutoRAG-0.1.1/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1050 2024-03-22 04:01:20.000000 AutoRAG-0.1.1/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.731848 AutoRAG-0.1.1/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 AutoRAG-0.1.1/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.733897 AutoRAG-0.1.1/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 AutoRAG-0.1.1/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.735224 AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    11906 2024-04-05 14:53:42.000000 AutoRAG-0.1.1/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 AutoRAG-0.1.1/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 AutoRAG-0.1.1/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    16846 2024-03-30 16:07:43.000000 AutoRAG-0.1.1/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.735417 AutoRAG-0.1.1/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.736789 AutoRAG-0.1.1/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 AutoRAG-0.1.1/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 AutoRAG-0.1.1/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 AutoRAG-0.1.1/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 AutoRAG-0.1.1/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 AutoRAG-0.1.1/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.738419 AutoRAG-0.1.1/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)       88 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2433 2024-03-06 19:11:31.000000 AutoRAG-0.1.1/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 AutoRAG-0.1.1/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 AutoRAG-0.1.1/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.742039 AutoRAG-0.1.1/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      217 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1664 2024-04-05 03:16:26.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6838 2024-03-06 19:44:35.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4105 2024-02-15 17:29:06.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.743193 AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4452 2024-03-06 19:44:35.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 AutoRAG-0.1.1/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.744621 AutoRAG-0.1.1/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       29 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1058 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 AutoRAG-0.1.1/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.746211 AutoRAG-0.1.1/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 AutoRAG-0.1.1/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 AutoRAG-0.1.1/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 AutoRAG-0.1.1/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 AutoRAG-0.1.1/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.748644 AutoRAG-0.1.1/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      155 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6415 2024-03-08 17:59:53.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10751 2024-02-15 17:27:26.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 AutoRAG-0.1.1/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.749884 AutoRAG-0.1.1/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2649 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.750787 AutoRAG-0.1.1/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 AutoRAG-0.1.1/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9447 2024-03-31 05:37:30.000000 AutoRAG-0.1.1/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-02-18 10:18:03.000000 AutoRAG-0.1.1/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.751860 AutoRAG-0.1.1/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 AutoRAG-0.1.1/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 AutoRAG-0.1.1/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      110 2024-03-30 16:07:43.000000 AutoRAG-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.754523 AutoRAG-0.1.1/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.764533 AutoRAG-0.1.1/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 AutoRAG-0.1.1/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.768805 AutoRAG-0.1.1/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 AutoRAG-0.1.1/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.775386 AutoRAG-0.1.1/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      763 2024-03-26 06:03:31.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1091 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1917 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      764 2024-01-31 10:39:33.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1299 2024-02-03 13:50:08.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      401 2024-01-17 15:59:52.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 AutoRAG-0.1.1/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 AutoRAG-0.1.1/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-03-30 16:07:43.000000 AutoRAG-0.1.1/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.775946 AutoRAG-0.1.1/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 AutoRAG-0.1.1/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.776561 AutoRAG-0.1.1/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4056 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 AutoRAG-0.1.1/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6083 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.776797 AutoRAG-0.1.1/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.777620 AutoRAG-0.1.1/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 AutoRAG-0.1.1/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 AutoRAG-0.1.1/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2846 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.778229 AutoRAG-0.1.1/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3036 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.780386 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2225 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.780866 AutoRAG-0.1.1/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2665 2024-03-31 11:01:41.000000 AutoRAG-0.1.1/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.781696 AutoRAG-0.1.1/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.783112 AutoRAG-0.1.1/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2073 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.784457 AutoRAG-0.1.1/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 AutoRAG-0.1.1/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 AutoRAG-0.1.1/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.784720 AutoRAG-0.1.1/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 AutoRAG-0.1.1/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 AutoRAG-0.1.1/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)      965 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.786804 AutoRAG-0.1.1/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 AutoRAG-0.1.1/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 AutoRAG-0.1.1/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 AutoRAG-0.1.1/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3114 2024-04-05 14:53:46.000000 AutoRAG-0.1.1/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 AutoRAG-0.1.1/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 AutoRAG-0.1.1/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.787055 AutoRAG-0.1.1/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 AutoRAG-0.1.1/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.787370 AutoRAG-0.1.1/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 AutoRAG-0.1.1/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.788421 AutoRAG-0.1.1/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 AutoRAG-0.1.1/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.788771 AutoRAG-0.1.1/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 AutoRAG-0.1.1/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-05 15:04:14.864471 AutoRAG-0.1.1/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.789780 AutoRAG-0.1.1/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.791967 AutoRAG-0.1.1/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.713945 AutoRAG-0.1.1/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.792837 AutoRAG-0.1.1/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 AutoRAG-0.1.1/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 AutoRAG-0.1.1/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 AutoRAG-0.1.1/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.793665 AutoRAG-0.1.1/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1415 2024-03-25 11:47:15.000000 AutoRAG-0.1.1/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2720 2024-03-25 07:44:05.000000 AutoRAG-0.1.1/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1931 2024-03-22 03:52:09.000000 AutoRAG-0.1.1/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.794694 AutoRAG-0.1.1/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.795484 AutoRAG-0.1.1/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 AutoRAG-0.1.1/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1375 2024-03-28 05:50:53.000000 AutoRAG-0.1.1/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 AutoRAG-0.1.1/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3191 2024-02-23 12:23:14.000000 AutoRAG-0.1.1/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.714655 AutoRAG-0.1.1/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.796746 AutoRAG-0.1.1/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 AutoRAG-0.1.1/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 AutoRAG-0.1.1/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 AutoRAG-0.1.1/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 AutoRAG-0.1.1/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.797849 AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2525 2024-02-22 16:08:56.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.800762 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3337 2024-02-22 16:33:58.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.801282 AutoRAG-0.1.1/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1767 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7998 2024-03-31 10:29:05.000000 AutoRAG-0.1.1/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.803836 AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.806610 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3608 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4997 2024-02-14 10:09:21.000000 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.807362 AutoRAG-0.1.1/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 AutoRAG-0.1.1/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6871 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    13837 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 AutoRAG-0.1.1/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.807974 AutoRAG-0.1.1/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 AutoRAG-0.1.1/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9058 2024-03-25 07:44:05.000000 AutoRAG-0.1.1/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 AutoRAG-0.1.1/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 AutoRAG-0.1.1/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.811932 AutoRAG-0.1.1/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 AutoRAG-0.1.1/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.715105 AutoRAG-0.1.1/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.813050 AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-03-31 10:20:41.000000 AutoRAG-0.1.1/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 AutoRAG-0.1.1/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.814350 AutoRAG-0.1.1/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 AutoRAG-0.1.1/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.815363 AutoRAG-0.1.1/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.816556 AutoRAG-0.1.1/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.816941 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.822651 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.824275 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.824570 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.827154 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.827571 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.828793 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.831372 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.833694 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 AutoRAG-0.1.1/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.834064 AutoRAG-0.1.1/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.834371 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.836043 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.716776 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.836396 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.839142 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.841067 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.841452 AutoRAG-0.1.1/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.717083 AutoRAG-0.1.1/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.841790 AutoRAG-0.1.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.842105 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.843677 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.844130 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.845471 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.847369 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.849730 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.850119 AutoRAG-0.1.1/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 AutoRAG-0.1.1/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.851044 AutoRAG-0.1.1/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.851329 AutoRAG-0.1.1/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 AutoRAG-0.1.1/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.851643 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.860529 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 AutoRAG-0.1.1/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 AutoRAG-0.1.1/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.718565 AutoRAG-0.1.1/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.861501 AutoRAG-0.1.1/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 AutoRAG-0.1.1/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 AutoRAG-0.1.1/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-05 15:04:14.862056 AutoRAG-0.1.1/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 AutoRAG-0.1.1/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      653 2024-02-15 10:23:20.000000 AutoRAG-0.1.1/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 AutoRAG-0.1.1/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.222951 AutoRAG-0.1.2/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.066325 AutoRAG-0.1.2/.github/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 AutoRAG-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.066797 AutoRAG-0.1.2/.github/workflows/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 AutoRAG-0.1.2/.github/workflows/sphinx.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      862 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 AutoRAG-0.1.2/.gitignore
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.222156 AutoRAG-0.1.2/AutoRAG.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33191 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    17176 2024-04-10 04:46:25.000000 AutoRAG-0.1.2/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      506 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 AutoRAG-0.1.2/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33191 2024-04-10 04:46:25.222672 AutoRAG-0.1.2/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18212 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.069927 AutoRAG-0.1.2/autorag/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-10 04:41:48.000000 AutoRAG-0.1.2/autorag/VERSION
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 AutoRAG-0.1.2/autorag/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4333 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/autorag/cli.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.070195 AutoRAG-0.1.2/autorag/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 AutoRAG-0.1.2/autorag/data/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.070793 AutoRAG-0.1.2/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 AutoRAG-0.1.2/autorag/data/corpus/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 AutoRAG-0.1.2/autorag/data/corpus/langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 AutoRAG-0.1.2/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.072358 AutoRAG-0.1.2/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2754 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/autorag/data/qacreation/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7107 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.072747 AutoRAG-0.1.2/autorag/data/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/data/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1050 2024-03-22 04:01:20.000000 AutoRAG-0.1.2/autorag/data/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/autorag/deploy.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.084665 AutoRAG-0.1.2/autorag/evaluate/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/autorag/evaluate/generation.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.086067 AutoRAG-0.1.2/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.087055 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11906 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 AutoRAG-0.1.2/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 AutoRAG-0.1.2/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/metric/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/autorag/evaluate/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    16846 2024-03-30 16:07:43.000000 AutoRAG-0.1.2/autorag/evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/node_line.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.087185 AutoRAG-0.1.2/autorag/nodes/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.088240 AutoRAG-0.1.2/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 AutoRAG-0.1.2/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 AutoRAG-0.1.2/autorag/nodes/generator/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 AutoRAG-0.1.2/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 AutoRAG-0.1.2/autorag/nodes/generator/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 AutoRAG-0.1.2/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.089279 AutoRAG-0.1.2/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       88 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2433 2024-03-06 19:11:31.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.095164 AutoRAG-0.1.2/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      403 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1664 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3625 2024-04-08 12:04:54.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3534 2024-04-10 04:41:53.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6838 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4105 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3889 2024-04-08 08:26:20.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.096018 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4452 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.097502 AutoRAG-0.1.2/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.098976 AutoRAG-0.1.2/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.100657 AutoRAG-0.1.2/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      155 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6415 2024-03-08 17:59:53.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    10751 2024-02-15 17:27:26.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.101238 AutoRAG-0.1.2/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/schema/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/schema/module.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/schema/node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3102 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/autorag/support.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.101723 AutoRAG-0.1.2/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/utils/preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9447 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/autorag/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/autorag/web.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-02-18 10:18:03.000000 AutoRAG-0.1.2/dev_requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.102306 AutoRAG-0.1.2/docs/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 AutoRAG-0.1.2/docs/Makefile
+-rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 AutoRAG-0.1.2/docs/make.bat
+-rw-r--r--   0 jeffrey    (501) staff       (20)      110 2024-03-30 16:07:43.000000 AutoRAG-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.104117 AutoRAG-0.1.2/docs/source/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.112793 AutoRAG-0.1.2/docs/source/_static/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/data_creation.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/data_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_lines.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 AutoRAG-0.1.2/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/project_folders.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.117002 AutoRAG-0.1.2/docs/source/_static/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 AutoRAG-0.1.2/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/trial_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/trial_json.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/trial_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/docs/source/_static/web_interface.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.124928 AutoRAG-0.1.2/docs/source/api_spec/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      763 2024-03-26 06:03:31.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1091 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2772 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1299 2024-02-03 13:50:08.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      401 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/modules.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-03-30 16:07:43.000000 AutoRAG-0.1.2/docs/source/conf.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.125380 AutoRAG-0.1.2/docs/source/data_creation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/docs/source/data_creation/data_format.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.125872 AutoRAG-0.1.2/docs/source/deploy/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/docs/source/deploy/web.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4056 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/docs/source/index.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 AutoRAG-0.1.2/docs/source/install.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6083 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/docs/source/local_model.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.126091 AutoRAG-0.1.2/docs/source/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.126803 AutoRAG-0.1.2/docs/source/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 AutoRAG-0.1.2/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5062 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/index.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.127235 AutoRAG-0.1.2/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3036 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.129717 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      647 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2324 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.130600 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.131184 AutoRAG-0.1.2/docs/source/nodes/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.132161 AutoRAG-0.1.2/docs/source/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2073 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.133116 AutoRAG-0.1.2/docs/source/optimization/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 AutoRAG-0.1.2/docs/source/optimization/custom_config.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 AutoRAG-0.1.2/docs/source/optimization/optimization.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.133288 AutoRAG-0.1.2/docs/source/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/docs/source/troubleshooting.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/docs/source/tutorial.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/pyproject.toml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1101 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.142612 AutoRAG-0.1.2/sample_config/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 AutoRAG-0.1.2/sample_config/compact_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/sample_config/compact_openai.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/sample_config/config_korean.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/sample_config/extracted_sample.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3569 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/sample_config/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 AutoRAG-0.1.2/sample_config/simple_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/sample_config/simple_openai.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.142819 AutoRAG-0.1.2/sample_dataset/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 AutoRAG-0.1.2/sample_dataset/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.143049 AutoRAG-0.1.2/sample_dataset/eli5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 AutoRAG-0.1.2/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.143231 AutoRAG-0.1.2/sample_dataset/msmarco/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 AutoRAG-0.1.2/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.143516 AutoRAG-0.1.2/sample_dataset/triviaqa/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 AutoRAG-0.1.2/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-10 04:46:25.223009 AutoRAG-0.1.2/setup.cfg
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.144370 AutoRAG-0.1.2/tests/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.145906 AutoRAG-0.1.2/tests/autorag/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.059939 AutoRAG-0.1.2/tests/autorag/data/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.146627 AutoRAG-0.1.2/tests/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 AutoRAG-0.1.2/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 AutoRAG-0.1.2/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.147380 AutoRAG-0.1.2/tests/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1415 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2720 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1931 2024-03-22 03:52:09.000000 AutoRAG-0.1.2/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.148350 AutoRAG-0.1.2/tests/autorag/evaluate/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.149076 AutoRAG-0.1.2/tests/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1375 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3191 2024-02-23 12:23:14.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.060708 AutoRAG-0.1.2/tests/autorag/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.149985 AutoRAG-0.1.2/tests/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.150786 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2525 2024-02-22 16:08:56.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.153723 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-08 12:04:54.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1078 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1524 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3337 2024-02-22 16:33:58.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1120 2024-04-08 08:26:20.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.154364 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7998 2024-03-31 10:29:05.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.160750 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.162355 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3608 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4997 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.162845 AutoRAG-0.1.2/tests/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/tests/autorag/test_cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6871 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/test_deploy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13837 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/autorag/test_evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/test_strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/test_support.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/tests/autorag/test_web.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.163305 AutoRAG-0.1.2/tests/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9058 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/utils/test_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/conftest.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/delete_tests.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 AutoRAG-0.1.2/tests/mock.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.165665 AutoRAG-0.1.2/tests/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 AutoRAG-0.1.2/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.061171 AutoRAG-0.1.2/tests/resources/data_creation/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.166517 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-03-31 10:20:41.000000 AutoRAG-0.1.2/tests/resources/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 AutoRAG-0.1.2/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.167168 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 AutoRAG-0.1.2/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.167971 AutoRAG-0.1.2/tests/resources/result_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.168441 AutoRAG-0.1.2/tests/resources/result_project/0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.168652 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.171322 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.172466 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.172699 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.173942 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.174081 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.184479 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.186012 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.187546 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 AutoRAG-0.1.2/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.187774 AutoRAG-0.1.2/tests/resources/result_project/1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.188181 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.190061 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.062922 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.190219 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.191240 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.192651 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.192886 AutoRAG-0.1.2/tests/resources/result_project/2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.063164 AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.193200 AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.193498 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.195168 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.205860 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.206481 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.209149 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.210946 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.211176 AutoRAG-0.1.2/tests/resources/result_project/3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.212176 AutoRAG-0.1.2/tests/resources/result_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.212504 AutoRAG-0.1.2/tests/resources/result_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.212813 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.219789 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/trial.json
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.064433 AutoRAG-0.1.2/tests/resources/sample_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.220648 AutoRAG-0.1.2/tests/resources/sample_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 AutoRAG-0.1.2/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 AutoRAG-0.1.2/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.221243 AutoRAG-0.1.2/tests/resources/sample_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 AutoRAG-0.1.2/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 jeffrey    (501) staff       (20)      653 2024-02-15 10:23:20.000000 AutoRAG-0.1.2/tests/resources/simple.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 AutoRAG-0.1.2/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `AutoRAG-0.1.1/.github/workflows/sphinx.yml` & `AutoRAG-0.1.2/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/.github/workflows/test.yml` & `AutoRAG-0.1.2/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   pull_request:
     branches:
       - main
 
 env:
   OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
   COHERE_API_KEY: ${{ secrets.COHERE_API_KEY }}
+  JINAAI_API_KEY: ${{ secrets.JINAAI_API_KEY }}
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Upgrade pip
```

### Comparing `AutoRAG-0.1.1/.gitignore` & `AutoRAG-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/AutoRAG.egg-info/PKG-INFO` & `AutoRAG-0.1.2/AutoRAG.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -239,15 +239,18 @@
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: torch
 Requires-Dist: sentencepiece
 Requires-Dist: guidance
 Requires-Dist: cohere>=5.0.0a9
 Requires-Dist: tokenlog>=0.0.2
+Requires-Dist: aiohttp
 Requires-Dist: bert_score
+Requires-Dist: sentence-transformers
+Requires-Dist: FlagEmbedding
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
@@ -489,22 +492,22 @@
             model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
             temperature: [ 0.5, 1.0, 1.5 ]
 
 ```
 
 # ❗Supporting Nodes & modules
 
-|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                    Modules                                                                                                                                                                                                                                                                                    |
-|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                        [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                        |
-|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                 |
-|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html) |
-| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                   [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)                                                                                                                                                                                                                                   |
-|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                 [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                 |
-|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                              [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                              |
+|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                                                                                                                                                                                                                                                                    [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                                                                                                                                                                                                                                                            [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                                                                                                                                                                                                                                                             |
+|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html)<br/>[Jina Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/jina_reranker.html)<br/>[Sentence Transformer Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/setence_transformer_reranker.html)<br/>[Colbert Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/colbert.html)<br/>[Flag Embedding Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/flag_embedding_reranker.html) |
+| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                                                                                                                                                                                                  [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)<br/>[Long Context Reorder](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/long_context_reorder.html)                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                             [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                                                                                                                                                                                                                                                                          [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
```

### Comparing `AutoRAG-0.1.1/AutoRAG.egg-info/SOURCES.txt` & `AutoRAG-0.1.2/AutoRAG.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,32 @@
 autorag/nodes/passagecompressor/base.py
 autorag/nodes/passagecompressor/pass_compressor.py
 autorag/nodes/passagecompressor/run.py
 autorag/nodes/passagecompressor/tree_summarize.py
 autorag/nodes/passagereranker/__init__.py
 autorag/nodes/passagereranker/base.py
 autorag/nodes/passagereranker/cohere.py
+autorag/nodes/passagereranker/colbert.py
+autorag/nodes/passagereranker/flag_embedding.py
+autorag/nodes/passagereranker/jina.py
 autorag/nodes/passagereranker/koreranker.py
 autorag/nodes/passagereranker/monot5.py
 autorag/nodes/passagereranker/pass_reranker.py
 autorag/nodes/passagereranker/rankgpt.py
 autorag/nodes/passagereranker/run.py
+autorag/nodes/passagereranker/sentence_transformer.py
 autorag/nodes/passagereranker/upr.py
 autorag/nodes/passagereranker/tart/__init__.py
 autorag/nodes/passagereranker/tart/modeling_enc_t5.py
 autorag/nodes/passagereranker/tart/tart.py
 autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
 autorag/nodes/promptmaker/__init__.py
 autorag/nodes/promptmaker/base.py
 autorag/nodes/promptmaker/fstring.py
+autorag/nodes/promptmaker/long_context_reorder.py
 autorag/nodes/promptmaker/run.py
 autorag/nodes/queryexpansion/__init__.py
 autorag/nodes/queryexpansion/base.py
 autorag/nodes/queryexpansion/hyde.py
 autorag/nodes/queryexpansion/pass_query_expansion.py
 autorag/nodes/queryexpansion/query_decompose.py
 autorag/nodes/queryexpansion/run.py
@@ -150,21 +155,26 @@
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
 docs/source/nodes/generator/vllm.md
 docs/source/nodes/passage_compressor/passage_compressor.md
 docs/source/nodes/passage_compressor/tree_summarize.md
 docs/source/nodes/passage_reranker/cohere.md
+docs/source/nodes/passage_reranker/colbert.md
+docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+docs/source/nodes/passage_reranker/jina_reranker.md
 docs/source/nodes/passage_reranker/koreranker.md
 docs/source/nodes/passage_reranker/monot5.md
 docs/source/nodes/passage_reranker/passage_reranker.md
 docs/source/nodes/passage_reranker/rankgpt.md
+docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
 docs/source/nodes/passage_reranker/tart.md
 docs/source/nodes/passage_reranker/upr.md
 docs/source/nodes/prompt_maker/fstring.md
+docs/source/nodes/prompt_maker/long_context_reorder.md
 docs/source/nodes/prompt_maker/prompt_maker.md
 docs/source/nodes/query_expansion/hyde.md
 docs/source/nodes/query_expansion/query_decompose.md
 docs/source/nodes/query_expansion/query_expansion.md
 docs/source/nodes/retrieval/bm25.md
 docs/source/nodes/retrieval/hybrid_cc.md
 docs/source/nodes/retrieval/hybrid_rrf.md
@@ -212,23 +222,29 @@
 tests/autorag/nodes/generator/test_llama_index_llm.py
 tests/autorag/nodes/generator/test_run_generator_node.py
 tests/autorag/nodes/generator/test_vllm.py
 tests/autorag/nodes/passagecompressor/test_pass_compressor.py
 tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
 tests/autorag/nodes/passagecompressor/test_tree_summarize.py
 tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+tests/autorag/nodes/passagereranker/test_flag_embedding.py
+tests/autorag/nodes/passagereranker/test_jina_reranker.py
 tests/autorag/nodes/passagereranker/test_koreranker.py
 tests/autorag/nodes/passagereranker/test_monot5.py
 tests/autorag/nodes/passagereranker/test_pass_reranker.py
 tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
 tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
 tests/autorag/nodes/passagereranker/test_rankgpt.py
+tests/autorag/nodes/passagereranker/test_sentence_transformer.py
 tests/autorag/nodes/passagereranker/test_tart.py
 tests/autorag/nodes/passagereranker/test_upr.py
 tests/autorag/nodes/promptmaker/test_fstring.py
+tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
 tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
 tests/autorag/nodes/queryexpansion/test_hyde.py
 tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
 tests/autorag/nodes/queryexpansion/test_query_decompose.py
 tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
 tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
 tests/autorag/nodes/retrieval/test_bm25.py
```

### Comparing `AutoRAG-0.1.1/LICENSE` & `AutoRAG-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/PKG-INFO` & `AutoRAG-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -239,15 +239,18 @@
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: torch
 Requires-Dist: sentencepiece
 Requires-Dist: guidance
 Requires-Dist: cohere>=5.0.0a9
 Requires-Dist: tokenlog>=0.0.2
+Requires-Dist: aiohttp
 Requires-Dist: bert_score
+Requires-Dist: sentence-transformers
+Requires-Dist: FlagEmbedding
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
@@ -489,22 +492,22 @@
             model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
             temperature: [ 0.5, 1.0, 1.5 ]
 
 ```
 
 # ❗Supporting Nodes & modules
 
-|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                    Modules                                                                                                                                                                                                                                                                                    |
-|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                        [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                        |
-|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                 |
-|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html) |
-| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                   [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)                                                                                                                                                                                                                                   |
-|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                 [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                 |
-|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                              [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                              |
+|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                                                                                                                                                                                                                                                                    [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                                                                                                                                                                                                                                                            [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                                                                                                                                                                                                                                                             |
+|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html)<br/>[Jina Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/jina_reranker.html)<br/>[Sentence Transformer Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/setence_transformer_reranker.html)<br/>[Colbert Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/colbert.html)<br/>[Flag Embedding Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/flag_embedding_reranker.html) |
+| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                                                                                                                                                                                                  [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)<br/>[Long Context Reorder](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/long_context_reorder.html)                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                             [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                                                                                                                                                                                                                                                                          [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
```

### Comparing `AutoRAG-0.1.1/README.md` & `AutoRAG-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -233,22 +233,22 @@
             model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
             temperature: [ 0.5, 1.0, 1.5 ]
 
 ```
 
 # ❗Supporting Nodes & modules
 
-|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                    Modules                                                                                                                                                                                                                                                                                    |
-|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                        [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                        |
-|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                 |
-|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html) |
-| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                   [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)                                                                                                                                                                                                                                   |
-|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                 [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                 |
-|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                              [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                              |
+|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                                                                                                                                                                                                                                                                    [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                                                                                                                                                                                                                                                            [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                                                                                                                                                                                                                                                             |
+|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html)<br/>[Jina Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/jina_reranker.html)<br/>[Sentence Transformer Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/setence_transformer_reranker.html)<br/>[Colbert Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/colbert.html)<br/>[Flag Embedding Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/flag_embedding_reranker.html) |
+| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                                                                                                                                                                                                  [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)<br/>[Long Context Reorder](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/long_context_reorder.html)                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                             [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                                                                                                                                                                                                                                                                          [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
```

### Comparing `AutoRAG-0.1.1/autorag/__init__.py` & `AutoRAG-0.1.2/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/cli.py` & `AutoRAG-0.1.2/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/corpus/langchain.py` & `AutoRAG-0.1.2/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/corpus/llama_index.py` & `AutoRAG-0.1.2/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/qacreation/base.py` & `AutoRAG-0.1.2/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/qacreation/llama_index.py` & `AutoRAG-0.1.2/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/qacreation/llama_index_default_prompt.txt` & `AutoRAG-0.1.2/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/qacreation/simple.py` & `AutoRAG-0.1.2/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/data/utils/util.py` & `AutoRAG-0.1.2/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/deploy.py` & `AutoRAG-0.1.2/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/generation.py` & `AutoRAG-0.1.2/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/generation.py` & `AutoRAG-0.1.2/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/retrieval.py` & `AutoRAG-0.1.2/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/metric/retrieval_contents.py` & `AutoRAG-0.1.2/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/retrieval.py` & `AutoRAG-0.1.2/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/retrieval_contents.py` & `AutoRAG-0.1.2/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluate/util.py` & `AutoRAG-0.1.2/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/evaluator.py` & `AutoRAG-0.1.2/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/node_line.py` & `AutoRAG-0.1.2/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/generator/base.py` & `AutoRAG-0.1.2/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/generator/llama_index_llm.py` & `AutoRAG-0.1.2/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/generator/run.py` & `AutoRAG-0.1.2/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/generator/vllm.py` & `AutoRAG-0.1.2/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagecompressor/base.py` & `AutoRAG-0.1.2/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagecompressor/run.py` & `AutoRAG-0.1.2/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagecompressor/tree_summarize.py` & `AutoRAG-0.1.2/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/base.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/cohere.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/koreranker.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/monot5.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/pass_reranker.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/rankgpt.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/run.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/tart.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/passagereranker/upr.py` & `AutoRAG-0.1.2/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/promptmaker/base.py` & `AutoRAG-0.1.2/autorag/nodes/promptmaker/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,15 @@
         assert "retrieved_contents" in previous_result.columns, "previous_result must have retrieved_contents column."
         query = previous_result["query"].tolist()
         retrieved_contents = previous_result["retrieved_contents"].tolist()
         prompt = kwargs.pop("prompt")
 
         if func.__name__ == 'fstring':
             return func(prompt, query, retrieved_contents)
+        elif func.__name__ == 'long_context_reorder':
+            assert "retrieve_scores" in previous_result.columns, "previous_result must have retrieve_scores column."
+            retrieve_scores = previous_result["retrieve_scores"].tolist()
+            return func(prompt, query, retrieved_contents, retrieve_scores)
         else:
             raise NotImplementedError(f"Module {func.__name__} is not implemented or not supported.")
 
     return wrapper
```

### Comparing `AutoRAG-0.1.1/autorag/nodes/promptmaker/fstring.py` & `AutoRAG-0.1.2/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/promptmaker/run.py` & `AutoRAG-0.1.2/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/queryexpansion/base.py` & `AutoRAG-0.1.2/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/queryexpansion/hyde.py` & `AutoRAG-0.1.2/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/queryexpansion/query_decompose.py` & `AutoRAG-0.1.2/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/queryexpansion/run.py` & `AutoRAG-0.1.2/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/retrieval/base.py` & `AutoRAG-0.1.2/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/retrieval/bm25.py` & `AutoRAG-0.1.2/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/retrieval/hybrid_cc.py` & `AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/retrieval/hybrid_rrf.py` & `AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/retrieval/run.py` & `AutoRAG-0.1.2/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/nodes/retrieval/vectordb.py` & `AutoRAG-0.1.2/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/schema/module.py` & `AutoRAG-0.1.2/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/schema/node.py` & `AutoRAG-0.1.2/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/strategy.py` & `AutoRAG-0.1.2/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/support.py` & `AutoRAG-0.1.2/autorag/support.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,19 +27,24 @@
         'monot5': ('autorag.nodes.passagereranker', 'monot5'),
         'tart': ('autorag.nodes.passagereranker', 'tart'),
         'upr': ('autorag.nodes.passagereranker', 'upr'),
         'koreranker': ('autorag.nodes.passagereranker', 'koreranker'),
         'pass_reranker': ('autorag.nodes.passagereranker', 'pass_reranker'),
         'cohere_reranker': ('autorag.nodes.passagereranker', 'cohere_reranker'),
         'rankgpt': ('autorag.nodes.passagereranker', 'rankgpt'),
+        'jina_reranker': ('autorag.nodes.passagereranker', 'jina_reranker'),
+        'colbert_reranker': ('autorag.nodes.passagereranker', 'colbert_reranker'),
+        'sentence_transformer_reranker': ('autorag.nodes.passagereranker', 'sentence_transformer_reranker'),
+        'flag_embedding_reranker': ('autorag.nodes.passagereranker', 'flag_embedding_reranker'),
         # passage_compressor
         'tree_summarize': ('autorag.nodes.passagecompressor', 'tree_summarize'),
         'pass_compressor': ('autorag.nodes.passagecompressor', 'pass_compressor'),
         # prompt_maker
         'fstring': ('autorag.nodes.promptmaker', 'fstring'),
+        'long_context_reorder': ('autorag.nodes.promptmaker', 'long_context_reorder'),
         # generator
         'llama_index_llm': ('autorag.nodes.generator', 'llama_index_llm'),
         'vllm': ('autorag.nodes.generator', 'vllm'),
     }
     return dynamically_find_function(module_name, support_modules)
```

### Comparing `AutoRAG-0.1.1/autorag/utils/preprocess.py` & `AutoRAG-0.1.2/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/utils/util.py` & `AutoRAG-0.1.2/autorag/utils/util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/autorag/web.py` & `AutoRAG-0.1.2/autorag/web.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/Makefile` & `AutoRAG-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/make.bat` & `AutoRAG-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/data_creation.png` & `AutoRAG-0.1.2/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/data_folder.png` & `AutoRAG-0.1.2/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/node_folder.png` & `AutoRAG-0.1.2/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/node_line_folder.png` & `AutoRAG-0.1.2/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/node_line_summary.png` & `AutoRAG-0.1.2/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/node_lines.png` & `AutoRAG-0.1.2/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/node_summary.png` & `AutoRAG-0.1.2/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/project_folder_example.png` & `AutoRAG-0.1.2/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/project_folders.png` & `AutoRAG-0.1.2/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/resources_folder.png` & `AutoRAG-0.1.2/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/roadmap/RAG_paradigms.png` & `AutoRAG-0.1.2/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/roadmap/advanced_RAG.png` & `AutoRAG-0.1.2/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/roadmap/cycle.png` & `AutoRAG-0.1.2/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/roadmap/merger.png` & `AutoRAG-0.1.2/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/roadmap/node_line_modular.png` & `AutoRAG-0.1.2/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/roadmap/policy.png` & `AutoRAG-0.1.2/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/samsung_sundae.jpeg` & `AutoRAG-0.1.2/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/trial_folder.png` & `AutoRAG-0.1.2/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/trial_json.png` & `AutoRAG-0.1.2/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/trial_summary.png` & `AutoRAG-0.1.2/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/_static/web_interface.png` & `AutoRAG-0.1.2/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.data.corpus.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.data.qacreation.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.evaluate.metric.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.evaluate.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.generator.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,38 @@
 -------------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.cohere
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagereranker.colbert module
+--------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.colbert
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.flag\_embedding module
+----------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.flag_embedding
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+autorag.nodes.passagereranker.jina module
+-----------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.jina
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagereranker.koreranker module
 -----------------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.koreranker
    :members:
    :undoc-members:
    :show-inheritance:
@@ -64,14 +88,22 @@
 ----------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.run
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagereranker.sentence\_transformer module
+----------------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.sentence_transformer
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagereranker.upr module
 ----------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.upr
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 ----------------------------------------
 
 .. automodule:: autorag.nodes.promptmaker.fstring
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.promptmaker.long\_context\_reorder module
+-------------------------------------------------------
+
+.. automodule:: autorag.nodes.promptmaker.long_context_reorder
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.promptmaker.run module
 ------------------------------------
 
 .. automodule:: autorag.nodes.promptmaker.run
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.nodes.retrieval.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/api_spec/autorag.rst` & `AutoRAG-0.1.2/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/conf.py` & `AutoRAG-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/data_creation/data_format.md` & `AutoRAG-0.1.2/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/data_creation/tutorial.md` & `AutoRAG-0.1.2/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/deploy/api_endpoint.md` & `AutoRAG-0.1.2/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/deploy/web.md` & `AutoRAG-0.1.2/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/index.rst` & `AutoRAG-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/install.md` & `AutoRAG-0.1.2/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/local_model.md` & `AutoRAG-0.1.2/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/generator/generator.md` & `AutoRAG-0.1.2/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/generator/llama_index_llm.md` & `AutoRAG-0.1.2/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/generator/vllm.md` & `AutoRAG-0.1.2/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/index.md` & `AutoRAG-0.1.2/docs/source/nodes/index.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available List
 
-|                              Nodes                               |                                                                                                                                          Modules                                                                                                                                          |
-|:----------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|     [Query_Expansion](./query_expansion/query_expansion.md)      |                                                                                  pass_query_expansion<br/>[Query_Decompose](./query_expansion/query_decompose.md)<br/>[HyDE](./query_expansion/hyde.md)                                                                                   |
-|              [Retrieval](./retrieval/retrieval.md)               |                                                                 [BM25](./retrieval/bm25.md)<br/>[Vectordb](./retrieval/vectordb.md)<br/>[Hybrid_RRF](./retrieval/hybrid_rrf.md)<br/>[Hybrid_CC](./retrieval/hybrid_cc.md)                                                                 |
-|    [Passage_Reranker](./passage_reranker/passage_reranker.md)    | pass_reranker<br/>[UPR](./passage_reranker/upr.md)<br/>[Tart](./passage_reranker/tart.md)<br/>[MonoT5](./passage_reranker/monot5.md)<br/>[Ko-reranker](./passage_reranker/koreranker.md)<br/>[Cohere Reranker](./passage_reranker/cohere.md)<br/>[RankGPT](./passage_reranker/rankgpt.md) |
-| [Passage_Compressor](./passage_compressor/passage_compressor.md) |                                                                                                       pass_compressor<br/>[Tree Summarize](./passage_compressor/tree_summarize.md)                                                                                                        |
-|          [Prompt Maker](./prompt_maker/prompt_maker.md)          |                                                                                                                           [fstring](./prompt_maker/fstring.md)                                                                                                                            |
-|              [Generator](./generator/generator.md)               |                                                                                                     [llama_index llm](./generator/llama_index_llm.md)<br/>[vllm](./generator/vllm.md)                                                                                                     |
+|                              Nodes                               |                                                                                                                                                                                                                                                                                    Modules                                                                                                                                                                                                                                                                                     |
+|:----------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+|     [Query_Expansion](./query_expansion/query_expansion.md)      |                                                                                                                                                                                                                             pass_query_expansion<br/>[Query_Decompose](./query_expansion/query_decompose.md)<br/>[HyDE](./query_expansion/hyde.md)                                                                                                                                                                                                                             |
+|              [Retrieval](./retrieval/retrieval.md)               |                                                                                                                                                                                                           [BM25](./retrieval/bm25.md)<br/>[Vectordb](./retrieval/vectordb.md)<br/>[Hybrid_RRF](./retrieval/hybrid_rrf.md)<br/>[Hybrid_CC](./retrieval/hybrid_cc.md)                                                                                                                                                                                                            |
+|    [Passage_Reranker](./passage_reranker/passage_reranker.md)    | pass_reranker<br/>[UPR](./passage_reranker/upr.md)<br/>[Tart](./passage_reranker/tart.md)<br/>[MonoT5](./passage_reranker/monot5.md)<br/>[Ko-reranker](./passage_reranker/koreranker.md)<br/>[Cohere Reranker](./passage_reranker/cohere.md)<br/>[RankGPT](./passage_reranker/rankgpt.md)<br/>[Jina Reranker](./passage_reranker/jina_reranker.md)<br/>[Sentence Transformer Reranker](./passage_reranker/sentence_transformer_reranker.md)<br/>[Colbert Reranker](./passage_reranker/colbert.md)<br/>[Flag Embedding Reranker](./passage_reranker/flag_embedding_reranker.md) |
+| [Passage_Compressor](./passage_compressor/passage_compressor.md) |                                                                                                                                                                                                             pass_compressor<br/>[Tree Summarize](./passage_compressor/tree_summarize.md)<br/>[Long Context Reoreder](./passage_compressor/long_context_reorder.md)                                                                                                                                                                                                             |
+|          [Prompt Maker](./prompt_maker/prompt_maker.md)          |                                                                                                                                                                                                                                                                      [fstring](./prompt_maker/fstring.md)                                                                                                                                                                                                                                                                      |
+|              [Generator](./generator/generator.md)               |                                                                                                                                                                                                                                               [llama_index llm](./generator/llama_index_llm.md)<br/>[vllm](./generator/vllm.md)                                                                                                                                                                                                                                                |
```

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_compressor/passage_compressor.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_compressor/tree_summarize.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_reranker/cohere.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_reranker/monot5.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_reranker/passage_reranker.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,8 +50,13 @@
 maxdepth: 1
 ---
 upr.md
 tart.md
 monot5.md
 koreranker.md
 cohere.md
+rankgpt.md
+jina_reranker.md
+colbert.md
+sentence_transformer_reranker.md
+flag_embedding_reranker.md
 ```
```

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_reranker/rankgpt.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_reranker/tart.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/passage_reranker/upr.md` & `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/prompt_maker/fstring.md` & `AutoRAG-0.1.2/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/prompt_maker/prompt_maker.md` & `AutoRAG-0.1.2/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files 10% similar despite different names*

```diff
@@ -56,8 +56,9 @@
 #### Supported Modules
 
 ```{toctree}
 ---
 maxdepth: 1
 ---
 fstring.md
+long_context_reorder.md
 ```
```

### Comparing `AutoRAG-0.1.1/docs/source/nodes/query_expansion/hyde.md` & `AutoRAG-0.1.2/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/query_expansion/query_decompose.md` & `AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/query_expansion/query_expansion.md` & `AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/retrieval/bm25.md` & `AutoRAG-0.1.2/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/retrieval/hybrid_cc.md` & `AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/retrieval/hybrid_rrf.md` & `AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/retrieval/retrieval.md` & `AutoRAG-0.1.2/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/nodes/retrieval/vectordb.md` & `AutoRAG-0.1.2/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/optimization/custom_config.md` & `AutoRAG-0.1.2/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/optimization/folder_structure.md` & `AutoRAG-0.1.2/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/optimization/optimization.md` & `AutoRAG-0.1.2/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/optimization/sample_full_config.yaml` & `AutoRAG-0.1.2/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/roadmap/modular_rag.md` & `AutoRAG-0.1.2/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/structure.md` & `AutoRAG-0.1.2/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/troubleshooting.md` & `AutoRAG-0.1.2/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/docs/source/tutorial.md` & `AutoRAG-0.1.2/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/pyproject.toml` & `AutoRAG-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/requirements.txt` & `AutoRAG-0.1.2/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 fastapi  # for api server
 uvicorn  # for api server
 torch  # for monot5 reranker
 sentencepiece  # for monot5 reranker
 guidance # for qa data creation
 cohere>=5.0.0a9 # for cohere services
 tokenlog>=0.0.2 # for token logging
+aiohttp # for async http requests
 bert_score # for bert score
+sentence-transformers # for sentence transformer reranker
+FlagEmbedding # for flag embedding reranker
 
 ### LlamaIndex ###
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 # Embeddings
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
```

### Comparing `AutoRAG-0.1.1/sample_config/compact_local.yaml` & `AutoRAG-0.1.2/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_config/compact_openai.yaml` & `AutoRAG-0.1.2/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_config/config_korean.yaml` & `AutoRAG-0.1.2/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_config/extracted_sample.yaml` & `AutoRAG-0.1.2/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_config/full.yaml` & `AutoRAG-0.1.2/tests/resources/result_project/0/config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
         speed_threshold: 10
         top_k: 10
         retrieval_modules:
           - module_type: bm25
           - module_type: vectordb
             embedding_model: openai
       modules:
-        - module_type: pass_query_expansion
         - module_type: query_decompose
           llm: openai
           temperature: [0.2, 1.0]
         - module_type: hyde
           llm: openai
           max_token: 64
 - node_line_name: retrieve_node_line  # Arbitrary node line name
@@ -25,71 +24,46 @@
         metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
         speed_threshold: 10
       top_k: 10
       modules:
         - module_type: bm25
         - module_type: vectordb
           embedding_model: openai
-        - module_type: hybrid_rrf
-          target_modules: ('bm25', 'vectordb')
-          rrf_k: [3, 5, 10]
-        - module_type: hybrid_cc
-          target_modules: ('bm25', 'vectordb')
-          weights:
-            - (0.5, 0.5)
-            - (0.3, 0.7)
-            - (0.7, 0.3)
     - node_type: passage_reranker
       strategy:
         metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
         speed_threshold: 10
       top_k: 5
       modules:
-        - module_type: pass_reranker
         - module_type: tart
         - module_type: monot5
-        - module_type: upr
-        - module_type: cohere_reranker
     - node_type: passage_compressor
       strategy:
         metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
         speed_threshold: 10
       modules:
-        - module_type: pass_compressor
         - module_type: tree_summarize
           llm: openai
           model: gpt-3.5-turbo-16k
 - node_line_name: post_retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: prompt_maker
       strategy:
-        metrics:
-          - metric_name: bleu
-          - metric_name: meteor
-          - metric_name: rouge
-          - metric_name: sem_score
-            embedding_model: openai
-          - metric_name: g_eval
+        metrics: [bleu, meteor, rouge]
         speed_threshold: 10
         generator_modules:
           - module_type: llama_index_llm
             llm: openai
             model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
       modules:
         - module_type: fstring
           prompt: ["Tell me something about the question: {query} \n\n {retrieved_contents}",
                    "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?"]
     - node_type: generator
       strategy:
-        metrics:
-          - metric_name: bleu
-          - metric_name: meteor
-          - metric_name: rouge
-          - metric_name: sem_score
-            embedding_model: openai
-          - metric_name: g_eval
+        metrics: [bleu, meteor, rouge]
         speed_threshold: 10
       modules:
         - module_type: llama_index_llm
           llm: [openai]
           model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
           temperature: [0.5, 1.0, 1.5]
```

### Comparing `AutoRAG-0.1.1/sample_config/simple_local.yaml` & `AutoRAG-0.1.2/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_config/simple_openai.yaml` & `AutoRAG-0.1.2/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_dataset/README.md` & `AutoRAG-0.1.2/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_dataset/eli5/load_eli5_dataset.py` & `AutoRAG-0.1.2/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_dataset/msmarco/load_msmarco_dataset.py` & `AutoRAG-0.1.2/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `AutoRAG-0.1.2/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/data/corpus/test_base.py` & `AutoRAG-0.1.2/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/data/corpus/test_langchain.py` & `AutoRAG-0.1.2/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/data/corpus/test_llama_index_corpus.py` & `AutoRAG-0.1.2/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/data/qacreation/test_base_qacreation.py` & `AutoRAG-0.1.2/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `AutoRAG-0.1.2/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/data/qacreation/test_simple.py` & `AutoRAG-0.1.2/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/metric/test_generation_metric.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/test_evaluate_util.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/test_generation_evaluate.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/evaluate/test_retrieval_evaluate.py` & `AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/generator/test_generator_base.py` & `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/generator/test_llama_index_llm.py` & `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/generator/test_run_generator_node.py` & `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/generator/test_vllm.py` & `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_koreranker.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_monot5.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_tart.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/passagereranker/test_upr.py` & `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/promptmaker/test_fstring.py` & `AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-import pandas as pd
-
 from autorag.nodes.promptmaker import fstring
-
-prompt = "Answer this question: {query} \n\n {retrieved_contents}"
-queries = ["What is the capital of Japan?", "What is the capital of China?"]
-retrieved_contents = [
-    ["Tokyo is the capital of Japan.", "Tokyo, the capital of Japan, is a huge metropolitan city."],
-    ["Beijing is the capital of China.", "Beijing, the capital of China, is a huge metropolitan city."]]
+from tests.autorag.nodes.promptmaker.test_prompt_maker_base import prompt, queries, retrieved_contents, previous_result
 
 
 def test_fstring():
     fstring_original = fstring.__wrapped__
     result_prompts = fstring_original(prompt, queries, retrieved_contents)
     assert len(result_prompts) == 2
     assert isinstance(result_prompts, list)
     assert result_prompts[0] == "Answer this question: What is the capital of Japan? \n\n Tokyo is the capital of Japan.\n\nTokyo, the capital of Japan, is a huge metropolitan city."
     assert result_prompts[1] == "Answer this question: What is the capital of China? \n\n Beijing is the capital of China.\n\nBeijing, the capital of China, is a huge metropolitan city."
 
 
 def test_fstring_node():
-    previous_result = pd.DataFrame({
-        "query": queries,
-        "retrieved_contents": retrieved_contents
-    })
     result = fstring(project_dir="pseudo_project_dir",
                      previous_result=previous_result,
                      prompt=prompt)
     assert len(result) == 2
     assert result.columns == ["prompts"]
     assert result['prompts'][0] == "Answer this question: What is the capital of Japan? \n\n Tokyo is the capital of Japan.\n\nTokyo, the capital of Japan, is a huge metropolitan city."
     assert result['prompts'][1] == "Answer this question: What is the capital of China? \n\n Beijing is the capital of China.\n\nBeijing, the capital of China, is a huge metropolitan city."
```

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_hyde.py` & `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_bm25.py` & `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/nodes/retrieval/test_vectordb.py` & `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/schema/test_module_schema.py` & `AutoRAG-0.1.2/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/schema/test_node_schema.py` & `AutoRAG-0.1.2/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/test_cli.py` & `AutoRAG-0.1.2/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/test_deploy.py` & `AutoRAG-0.1.2/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/test_evaluator.py` & `AutoRAG-0.1.2/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/test_strategy.py` & `AutoRAG-0.1.2/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/test_web.py` & `AutoRAG-0.1.2/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/utils/test_preprocess.py` & `AutoRAG-0.1.2/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/autorag/utils/test_util.py` & `AutoRAG-0.1.2/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/delete_tests.py` & `AutoRAG-0.1.2/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/mock.py` & `AutoRAG-0.1.2/tests/mock.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/README.md` & `AutoRAG-0.1.2/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/corpus_data_sample.parquet` & `AutoRAG-0.1.2/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/sample1.txt` & `AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/sample2.txt` & `AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/data_creation/raw_dir/sample3.txt` & `AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/full.yaml` & `AutoRAG-0.1.2/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/qa_data_sample.parquet` & `AutoRAG-0.1.2/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/qa_test_data_sample.parquet` & `AutoRAG-0.1.2/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/config.yaml` & `AutoRAG-0.1.2/tests/resources/result_project/1/config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 node_lines:
-- node_line_name: pre_retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: query_expansion
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
+  - node_line_name: pre_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: query_expansion
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+          top_k: 10
+          retrieval_modules:
+            - module_type: bm25
+            - module_type: vectordb
+              embedding_model: openai
+        modules:
+          - module_type: query_decompose
+            llm: openai
+            temperature: [ 0.2, 1.0 ]
+          - module_type: hyde
+            llm: openai
+            max_token: 64
+  - node_line_name: retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: retrieval
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
         top_k: 10
-        retrieval_modules:
+        modules:
           - module_type: bm25
           - module_type: vectordb
             embedding_model: openai
-      modules:
-        - module_type: query_decompose
-          llm: openai
-          temperature: [0.2, 1.0]
-        - module_type: hyde
-          llm: openai
-          max_token: 64
-- node_line_name: retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: retrieval
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
-      top_k: 10
-      modules:
-        - module_type: bm25
-        - module_type: vectordb
-          embedding_model: openai
-    - node_type: passage_reranker
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
-      top_k: 5
-      modules:
-        - module_type: tart
-        - module_type: monot5
-    - node_type: passage_compressor
-      strategy:
-        metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
-        speed_threshold: 10
-      modules:
-        - module_type: tree_summarize
-          llm: openai
-          model: gpt-3.5-turbo-16k
-- node_line_name: post_retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: prompt_maker
-      strategy:
-        metrics: [bleu, meteor, rouge]
-        speed_threshold: 10
-        generator_modules:
-          - module_type: llama_index_llm
+      - node_type: passage_reranker
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+        top_k: 5
+        modules:
+          - module_type: tart
+          - module_type: monot5
+      - node_type: passage_compressor
+        strategy:
+          metrics: [ retrieval_token_f1, retrieval_token_recall, retrieval_token_precision ]
+          speed_threshold: 10
+        modules:
+          - module_type: tree_summarize
             llm: openai
-            model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
-      modules:
-        - module_type: fstring
-          prompt: ["Tell me something about the question: {query} \n\n {retrieved_contents}",
-                   "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?"]
-    - node_type: generator
-      strategy:
-        metrics: [bleu, meteor, rouge]
-        speed_threshold: 10
-      modules:
-        - module_type: llama_index_llm
-          llm: [openai]
-          model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
-          temperature: [0.5, 1.0, 1.5]
+            model: gpt-3.5-turbo-16k
+  - node_line_name: post_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: prompt_maker
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+          generator_modules:
+            - module_type: llama_index_llm
+              llm: openai
+              model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
+        modules:
+          - module_type: fstring
+            prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
+                      "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
+      - node_type: generator
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+        modules:
+          - module_type: llama_index_llm
+            llm: [ openai ]
+            model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
+            temperature: [ 0.5, 1.0, 1.5 ]
```

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/0/summary.csv` & `AutoRAG-0.1.2/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/config.yaml` & `AutoRAG-0.1.2/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/config.yaml` & `AutoRAG-0.1.2/sample_config/full.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,103 @@
 node_lines:
-  - node_line_name: pre_retrieve_node_line  # Arbitrary node line name
-    nodes:
-      - node_type: query_expansion
-        strategy:
-          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
-          speed_threshold: 10
-          top_k: 10
-          retrieval_modules:
-            - module_type: bm25
-            - module_type: vectordb
-              embedding_model: openai
-        modules:
-          - module_type: query_decompose
-            llm: openai
-            temperature: [ 0.2, 1.0 ]
-          - module_type: hyde
-            llm: openai
-            max_token: 64
-  - node_line_name: retrieve_node_line  # Arbitrary node line name
-    nodes:
-      - node_type: retrieval
-        strategy:
-          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
-          speed_threshold: 10
+- node_line_name: pre_retrieve_node_line  # Arbitrary node line name
+  nodes:
+    - node_type: query_expansion
+      strategy:
+        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
+        speed_threshold: 10
         top_k: 10
-        modules:
+        retrieval_modules:
           - module_type: bm25
           - module_type: vectordb
             embedding_model: openai
-      - node_type: passage_reranker
-        strategy:
-          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
-          speed_threshold: 10
-        top_k: 5
-        modules:
-          - module_type: tart
-          - module_type: monot5
-      - node_type: passage_compressor
-        strategy:
-          metrics: [ retrieval_token_f1, retrieval_token_recall, retrieval_token_precision ]
-          speed_threshold: 10
-        modules:
-          - module_type: tree_summarize
-            llm: openai
-            model: gpt-3.5-turbo-16k
-  - node_line_name: post_retrieve_node_line  # Arbitrary node line name
-    nodes:
-      - node_type: prompt_maker
-        strategy:
-          metrics: [ bleu, meteor, rouge ]
-          speed_threshold: 10
-          generator_modules:
-            - module_type: llama_index_llm
-              llm: openai
-              model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
-        modules:
-          - module_type: fstring
-            prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
-                      "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
-      - node_type: generator
-        strategy:
-          metrics: [ bleu, meteor, rouge ]
-          speed_threshold: 10
-        modules:
+      modules:
+        - module_type: pass_query_expansion
+        - module_type: query_decompose
+          llm: openai
+          temperature: [0.2, 1.0]
+        - module_type: hyde
+          llm: openai
+          max_token: 64
+- node_line_name: retrieve_node_line  # Arbitrary node line name
+  nodes:
+    - node_type: retrieval
+      strategy:
+        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
+        speed_threshold: 10
+      top_k: 10
+      modules:
+        - module_type: bm25
+        - module_type: vectordb
+          embedding_model: openai
+        - module_type: hybrid_rrf
+          target_modules: ('bm25', 'vectordb')
+          rrf_k: [3, 5, 10]
+        - module_type: hybrid_cc
+          target_modules: ('bm25', 'vectordb')
+          weights:
+            - (0.5, 0.5)
+            - (0.3, 0.7)
+            - (0.7, 0.3)
+    - node_type: passage_reranker
+      strategy:
+        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
+        speed_threshold: 10
+      top_k: 5
+      modules:
+        - module_type: pass_reranker
+        - module_type: tart
+        - module_type: monot5
+        - module_type: upr
+        - module_type: cohere_reranker
+        - module_type: rankgpt
+        - module_type: jina_reranker
+        - module_type: colbert_reranker
+        - module_type: sentence_transformer_reranker
+        - module_type: flag_embedding_reranker
+    - node_type: passage_compressor
+      strategy:
+        metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
+        speed_threshold: 10
+      modules:
+        - module_type: pass_compressor
+        - module_type: tree_summarize
+          llm: openai
+          model: gpt-3.5-turbo-16k
+- node_line_name: post_retrieve_node_line  # Arbitrary node line name
+  nodes:
+    - node_type: prompt_maker
+      strategy:
+        metrics:
+          - metric_name: bleu
+          - metric_name: meteor
+          - metric_name: rouge
+          - metric_name: sem_score
+            embedding_model: openai
+          - metric_name: g_eval
+        speed_threshold: 10
+        generator_modules:
           - module_type: llama_index_llm
-            llm: [ openai ]
-            model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
-            temperature: [ 0.5, 1.0, 1.5 ]
+            llm: openai
+            model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
+      modules:
+        - module_type: fstring
+          prompt: ["Tell me something about the question: {query} \n\n {retrieved_contents}",
+                   "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?"]
+        - module_type: long_context_reorder
+          prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
+                    "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
+    - node_type: generator
+      strategy:
+        metrics:
+          - metric_name: bleu
+          - metric_name: meteor
+          - metric_name: rouge
+          - metric_name: sem_score
+            embedding_model: openai
+          - metric_name: g_eval
+        speed_threshold: 10
+      modules:
+        - module_type: llama_index_llm
+          llm: [openai]
+          model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
+          temperature: [0.5, 1.0, 1.5]
```

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/3/config.yaml` & `AutoRAG-0.1.2/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/best.yaml` & `AutoRAG-0.1.2/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/data/corpus.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/data/qa.parquet` & `AutoRAG-0.1.2/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/resources/bm25.pkl` & `AutoRAG-0.1.2/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/sample_contents_nqa.csv` & `AutoRAG-0.1.2/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/sample_project/data/corpus.parquet` & `AutoRAG-0.1.2/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/sample_project/data/qa.parquet` & `AutoRAG-0.1.2/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/sample_project/resources/bm25.pkl` & `AutoRAG-0.1.2/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/simple.yaml` & `AutoRAG-0.1.2/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.1/tests/resources/test_bm25_retrieval.pkl` & `AutoRAG-0.1.2/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

