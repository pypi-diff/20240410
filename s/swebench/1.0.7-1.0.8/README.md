# Comparing `tmp/swebench-1.0.7.tar.gz` & `tmp/swebench-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.7.tar", last modified: Tue Apr  9 14:20:07 2024, max compression
+gzip compressed data, was "swebench-1.0.8.tar", last modified: Tue Apr  9 17:20:07 2024, max compression
```

## Comparing `swebench-1.0.7.tar` & `swebench-1.0.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.929087 swebench-1.0.7/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.7/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 14:20:07.929022 swebench-1.0.7/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.7/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.922089 swebench-1.0.7/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.7/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.922582 swebench-1.0.7/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.7/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.923797 swebench-1.0.7/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.7/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.7/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.7/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.7/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.7/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.7/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.7/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-09 14:20:07.929284 swebench-1.0.7/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.7/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.924026 swebench-1.0.7/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-09 14:20:01.000000 swebench-1.0.7/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.925701 swebench-1.0.7/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.926822 swebench-1.0.7/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    19019 2024-04-09 14:18:22.000000 swebench-1.0.7/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    31176 2024-04-07 22:22:31.000000 swebench-1.0.7/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.7/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.7/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.927950 swebench-1.0.7/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.7/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7097 2024-04-07 16:01:31.000000 swebench-1.0.7/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.7/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.928566 swebench-1.0.7/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.7/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:20:07.928769 swebench-1.0.7/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 14:20:07.000000 swebench-1.0.7/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-09 14:20:07.000000 swebench-1.0.7/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-09 14:20:07.000000 swebench-1.0.7/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-09 14:20:07.000000 swebench-1.0.7/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-09 14:20:07.000000 swebench-1.0.7/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.814625 swebench-1.0.8/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.8/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 17:20:07.814557 swebench-1.0.8/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.8/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.804450 swebench-1.0.8/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.805310 swebench-1.0.8/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.807673 swebench-1.0.8/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.8/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.8/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.8/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-09 17:20:07.814837 swebench-1.0.8/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.8/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.808002 swebench-1.0.8/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-09 17:19:55.000000 swebench-1.0.8/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.810023 swebench-1.0.8/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.811535 swebench-1.0.8/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    19019 2024-04-09 14:18:22.000000 swebench-1.0.8/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    31165 2024-04-09 15:28:28.000000 swebench-1.0.8/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.8/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.8/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.813228 swebench-1.0.8/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.8/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.0.8/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.8/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.814125 swebench-1.0.8/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.814326 swebench-1.0.8/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.7/LICENSE` & `swebench-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/PKG-INFO` & `swebench-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.7
+Version: 1.0.8
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.7 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.8 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.7/README.md` & `swebench-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/llamao/distributed_attention.py` & `swebench-1.0.8/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.8/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.8/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/make_datasets/create_instance.py` & `swebench-1.0.8/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.8/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.8/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.8/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/make_datasets/utils.py` & `swebench-1.0.8/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/run_api.py` & `swebench-1.0.8/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/run_live.py` & `swebench-1.0.8/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/inference/run_llama.py` & `swebench-1.0.8/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/setup.py` & `swebench-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/__init__.py` & `swebench-1.0.8/swebench/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.7/swebench/collect/build_dataset.py` & `swebench-1.0.8/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/collect/build_dataset_ft.py` & `swebench-1.0.8/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.8/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/collect/get_top_pypi.py` & `swebench-1.0.8/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/collect/print_pulls.py` & `swebench-1.0.8/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/collect/utils.py` & `swebench-1.0.8/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/harness/constants.py` & `swebench-1.0.8/swebench/harness/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/harness/context_manager.py` & `swebench-1.0.8/swebench/harness/context_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def __call__(self, cmd, raise_error=True, **kwargs):
         try:
             if isinstance(cmd, list):
                 self.logger.write(f"Command: {' '.join(cmd)}", level=DEBUG)
             else:
                 self.logger.write(f"Command: {cmd}", level=DEBUG)
             combined_args = {**self.subprocess_args, **kwargs}
-            self.logger.write(f"Subprocess args:\n{json.dumps(combined_args, indent=4)}", level=DEBUG)
+            self.logger.write(f"Subprocess args: {json.dumps(combined_args)}", level=DEBUG)
             output = subprocess.run(cmd, **combined_args)
             self.logger.write(f"Std. Output:\n{output.stdout}", level=DEBUG)
             if output.stderr:
                 self.logger.write(f"Std. Error:\n{output.stderr}", level=DEBUG)
             return output
         except subprocess.CalledProcessError as e:
             if raise_error and self.logger is not None:
```

### Comparing `swebench-1.0.7/swebench/harness/engine_evaluation.py` & `swebench-1.0.8/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/harness/engine_validation.py` & `swebench-1.0.8/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/harness/run_evaluation.py` & `swebench-1.0.8/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/harness/utils.py` & `swebench-1.0.8/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/metrics/constants.py` & `swebench-1.0.8/swebench/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/metrics/conversion.py` & `swebench-1.0.8/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/metrics/getters.py` & `swebench-1.0.8/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/metrics/log_parsers.py` & `swebench-1.0.8/swebench/metrics/log_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
             test_case = line.split()
             if len(test_case) <= 1:
                 continue
             has_option = option_pattern.search(test_case[1])
             if has_option:
                 main, option = has_option.groups()
                 if option.startswith('/') and not option.startswith('//') and '*' not in option:
-                    option = option.split('/')[-1]
-                test_name = f'{main}[/{option}]'
+                    option = "/" + option.split('/')[-1]
+                test_name = f'{main}[{option}]'
             else:
                 test_name = test_case[1]
             test_status_map[test_name] = test_case[0]
     return test_status_map
 
 
 def parse_log_django(log: str) -> dict:
```

### Comparing `swebench-1.0.7/swebench/metrics/metrics.py` & `swebench-1.0.8/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/metrics/monitor.py` & `swebench-1.0.8/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/metrics/report.py` & `swebench-1.0.8/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/versioning/constants.py` & `swebench-1.0.8/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/versioning/get_versions.py` & `swebench-1.0.8/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench/versioning/utils.py` & `swebench-1.0.8/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.7/swebench.egg-info/PKG-INFO` & `swebench-1.0.8/swebench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.7
+Version: 1.0.8
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.7 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.8 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.7/swebench.egg-info/SOURCES.txt` & `swebench-1.0.8/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

